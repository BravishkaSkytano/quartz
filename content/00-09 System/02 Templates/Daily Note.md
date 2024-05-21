<%"---"%>
id: <% tp.date.now("YYYYMMDDHHss") %>
banner_icon: 🗝️
<%"---"%>

## [[<% tp.date.yesterday("YYYY.MM.DD") %>|⬅]] <% tp.date.now("dddd 💠 MMMM Do 💠 YYYY") %> [[<% tp.date.tomorrow("YYYY.MM.DD") %>|➡]]

> [!INFO]- Metadata
> - Created:: <% tp.date.now("YYYY-MM-DD @ HH:mm") %>
> - Updated:: <% tp.date.now("YYYY-MM-DD @ HH:mm") %>
> - ID:: <% tp.date.now('YYYYMMDDHHmm') %>
> - Week:: [[<% tp.date.now("YY.[W]WW") %>]]

<% tp.web.daily_quote() %>

### Memos
- …

^memo-link

### Work Log
- …

^work-link

### Trackers

#### Statistics

- Feeling:: 
- Learned Word:: 
- Money Spent:: 
- Panic:: 
- Prayer:: 
- Steps:: 

#### Habits

- Anki:: 
- Exercise:: 
- Martial Arts:: 
- Reading:: 
- Shower:: 
- Writing:: 

### Tasks

<%"```toggl"%>
LIST <% tp.date.now("YYYY-MM-DD") %>
GROUP BY PROJECT
SORT DESC
<%"```"%>

#### Not Done

<%"```tasks"%>
happens <% tp.date.now("YYYY-MM-DD") %>
short mode
<%"```"%>

#### New Today
- [ ]
