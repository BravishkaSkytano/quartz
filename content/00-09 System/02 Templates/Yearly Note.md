<%"---"%>
id: <% tp.date.now("YYYYMMDDHHmm") %>
title: <% tp.date.now("YYYY") %>
obsidianUIMode: preview
banner: https://preview.redd.it/arqa352ph7x61.jpg?width=960&crop=smart&auto=webp&s=84f9245d607b029667d5bfc4abf36547fc6213de
cssclasses:
  - cards
tags:
  - 📥/🌲 
<%"---"%>

[[<% tp.date.now("YYYY", "P-1Y") %>|↶ <% tp.date.now("YYYY", "P-1Y") %>]] ⁝ [[<% tp.date.now("YYYY", "P1Y") %>|<% tp.date.now("YYYY", "P1Y") %> ↷]]

## Goals

- Goal 1: *Read ## Books*
- Goal 2: *Goal 2*

^goals-link

## Books Read This Year

<%"```dataview"%>
LIST WITHOUT ID
"So far in <% tp.date.now("YYYY") %>, I've read " + length(rows) + " books."
FROM "60-69 Bookshelf"
WHERE contains(string(readdates.finished), "<% tp.date.now("YYYY") %>")
GROUP BY dateformat(finished, "yyyy")
<%"```"%>

### Favorites

<%"```dataview"%>
LIST WITHOUT ID
title + " (" + author + ")"
FROM "60-69 Bookshelf"
WHERE rating=5 AND contains(string(readdates.finished), "<% tp.date.now("YYYY") %>")
<%"```"%>

### All Books

<%"```dataviewjs"%>
function renderReadDates(readdates) {
	let str = '';
	str += new Date(readdates.started).toLocaleDateString('en-us', { month:"short", day:"numeric"});
	str += ' - ';
	str += new Date(readdates.finished).toLocaleDateString('en-us', { month:"short", day:"numeric"});
	return str;
}

function fullBookList(dvarr, year) {
	const retArr = [];

    // Get only books read during the specified year
    // But if a book was reread during the year, list it twice
	dvarr.map(b => {
		if(b.readdates) {
			b.readdates.map(d => {
				if(new Date(d.finished).getFullYear() === year) {
					const book = Object.assign({}, b);
					book.readdates = d;
					retArr.push(book);
				}
				return d;
			});
		}
		return b;
	});

    // Sort by date finished
	retArr.sort((a,b) => {
		let ret = 0;
		if(a.readdates.finished.toString() > b.readdates.finished.toString()) {
			ret = 1;
		} else if(a.readdates.finished.toString() < b.readdates.finished.toString()) {
			ret = -1;
		}
		return ret;
	});
	
	return retArr;
}

// Function definitions finished, kick it off here and set your year:

const year = <% tp.date.now("YYYY") %>;
const pages = dv.pages('"60-69 Bookshelf"');
const expandedPages = dv.array(fullBookList(pages, year));

dv.table(
	["cover", "title", "author", "series", "read", "rating"],
	expandedPages.map(b => [
		"![" + b.cover + "|80](" + b.cover + ")",
		b.title,
		b.author,
		b.series,
		renderReadDates(b.readdates),
		"⭐".repeat(b.rating)
	])
);
<%"```"%>
