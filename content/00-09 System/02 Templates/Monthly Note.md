<%"---"%>
id: <% tp.date.now("YYYYMMDDHHmm") %>
title: <% tp.date.now("YYYY MMMM") %>
obsidianUIMode: preview
banner: https://preview.redd.it/arqa352ph7x61.jpg?width=960&crop=smart&auto=webp&s=84f9245d607b029667d5bfc4abf36547fc6213de
tags:
- 📥/🌲 
<%"---"%>

[[<% tp.date.now("YY.MM MMMM", "P-1M") %>|⬅ <% tp.date.now("MMMM YYYY", "P-1M") %>]] | [[<% tp.date.now("YY.MM MMMM", "P1M") %>|<% tp.date.now("MMMM YYYY", "P1M") %> ➡]]

## Goals

![[<% tp.date.now("YYYY-[Q]Q") %>#^goals-link]]

## Memos

- [[<%tp.date.now("YYYY-[W]ww")%>|Week 1]]
	[[<%tp.date.now("YYYY-[W]ww")%>#^memo-link]]
- [[<%tp.date.now("YYYY-[W]ww", 7)%>|Week 2]]
	[[<%tp.date.now("YYYY-[W]ww", 7)%>#^memo-link]]
- [[<%tp.date.now("YYYY-[W]ww", 14)%>|Week 3]]
	[[<%tp.date.now("YYYY-[W]ww", 14)%>#^memo-link]]
- [[<%tp.date.now("YYYY-[W]ww", 21)%>|Week 4]]
	[[<%tp.date.now("YYYY-[W]ww", 21)%>#^memo-link]]
- [[<%tp.date.now("YYYY-[W]ww", 28)%>|Week 5]]
	[[<%tp.date.now("YYYY-[W]ww", 28)%>#^memo-link]]

^memo-link

## Work Log

- [[<%tp.date.now("YYYY-[W]ww")%>|Week 1]]
	[[<%tp.date.now("YYYY-[W]ww")%>#^work-link]]
- [[<%tp.date.now("YYYY-[W]ww", 7)%>|Week 2]]
	[[<%tp.date.now("YYYY-[W]ww", 7)%>#^work-link]]
- [[<%tp.date.now("YYYY-[W]ww", 14)%>|Week 3]]
	[[<%tp.date.now("YYYY-[W]ww", 14)%>#^work-link]]
- [[<%tp.date.now("YYYY-[W]ww", 21)%>|Week 4]]
	[[<%tp.date.now("YYYY-[W]ww", 21)%>#^work-link]]
- [[<%tp.date.now("YYYY-[W]ww", 28)%>|Week 5]]
	[[<%tp.date.now("YYYY-[W]ww", 28)%>#^work-link]]

^work-link

## Books Read This Month

<%"```dataview"%>
LIST WITHOUT ID
title + " (" + author + ")"
FROM "60-69 Bookshelf"
WHERE contains(string(readdates.finished), "<% tp.date.now("YYYY-MM") %>")
<%"```"%>
