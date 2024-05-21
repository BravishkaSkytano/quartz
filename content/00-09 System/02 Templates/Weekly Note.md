
## <% tp.date.now("YYYY [Week] WW") %>

[[<% tp.date.now("YY.[W]WW", -7) %>|↶ <% tp.date.now("[Week] WW", -7) %>]] | [[<% tp.date.now("YY.[W]WW", 7) %>|<% tp.date.now("[Week] WW", 7) %> ↷]]

> [!METADATA]-
> Created:: [[<% tp.date.now('YYYY-MM-DD') %>]] <% tp.date.now('HH:mm') %>
> Updated:: <% tp.date.now('YYYY-MM-DD HH:mm') %>
> ID:: <% tp.date.now('YYYYMMDDHHmmss') %>

### Memos

- [[<% tp.date.weekday("YYYY.MM.DD", 0) %>|Monday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 0) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 1) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 1) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 2) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 2) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 3) %>|Thursday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 3) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 4) %>|Friday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 4) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 5) %>|Saturday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 5) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 6) %>|Sunday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 6) %>#^memo-link]]

### Work Log
- [[<% tp.date.weekday("YYYY.MM.DD", 0) %>|Monday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 0) %>#^work-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 1) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 1) %>#^work-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 2) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 2) %>#^work-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 3) %>|Thursday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 3) %>#^work-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 4) %>|Friday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 4) %>#^work-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 5) %>|Saturday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 5) %>#^work-link]]
- [[<% tp.date.weekday("YYYY.MM.DD", 6) %>|Sunday]]
	![[<% tp.date.weekday("YYYY.MM.DD", 6) %>#^work-link]] 

### Overview

#### Week Statistics

<%"```dataviewjs"%>
const daysPath = dv.current().file.folder;

const attributes = {
	'panic': {
		label: 'Panic',
		average: 10,
	},
	'money-spent': {
		label: 'Money Spent',
		backgroundColor: 'rgba(85, 174, 229, 0.2)',
		borderColor: 'rgba(85, 174, 229, 1)',
		average: 20,
	},
	'prayer': {
		label: 'Prayer',
		backgroundColor: 'rgba(255, 211, 101, 0.2)',
		borderColor: 'rgba(255, 211, 101, 1)',
		average: 5,
	},
	'steps': {
		label: 'Steps',
		backgroundColor: 'rgba(141, 82, 188, 0.2)',
		borderColor: 'rgba(141, 82, 188, 1)',
		average: 10000,
	},
};

const date = "<% tp.date.now('YYYY-MM-DD') %>";

customJS.DvCharts.renderWeeklyChart({
	dv,
	context: this,
	daysPath: '00-09 System/03 Journal/<% tp.date.now("YYYY") %>/<%tp.date.now("YY.MM MMMM")%>',
	attributes,
	type: 'average',
	date
})
<%"```"%>

<%"```dataview"%>
TABLE WITHOUT ID
	link(file.name) as "Day",
	feeling AS "💭",
	money-spent AS "💸",
	panic AS "🌪️",
	prayer AS "🙏",
	steps AS "👣"
FROM "00-09 System/03 Journal"
WHERE week = [[<% tp.date.now("YY.[W]WW") %>]]
SORT file.name ASC
<%"```"%>

#### Habits

<%"```dataview"%>
TABLE WITHOUT ID
	file.link AS "Day",
	anki AS "📇",
	exercise AS "🏋️",
	martial-arts AS "🥋",
	reading AS "👓",
	shower AS "🚿",
	writing AS "✍"
FROM "00-09 System/03 Journal"
WHERE week = [[<% tp.date.now("YY.[W]WW") %>]]
SORT file.name ASC
<%"```"%>

#### Learned Words

<%"```dataviewjs"%>
dv.table(
	["Learned Word", "Meaning"],
	dv.pages('"00-09 System/03 Journal"')
	.filter(p => p["Learned Word"] && p.week.path == "<% tp.date.now("YY.[W]WW") %>")
	.sort(p => dv.date(p.file.name), 'asc')
	.flatMap(p =>
		Array.from(
			{
				length: Math.floor(
					p["Learned Word"].length / 2
				)
			},
			(_, i) => [
				`${'**'}${p["Learned Word"][i * 2]}${'**'}`,
				p["Learned Word"][(i * 2) +1]
			]
		)
	)
)
<%"```"%>

#### Toggl

<%"```toggl"%>
SUMMARY FROM <% tp.date.weekday("YYYY-MM-DD", 0) %> TO <% tp.date.weekday("YYYY-MM-DD", 6) %>
<%"```"%>
