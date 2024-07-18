<%"---"%>
id: <% tp.date.now("YYYYMMDDHHmm") %>
title: <% tp.date.now("[Week] WW of YYYY") %>
obsidianUIMode: preview
tags:
- 📥/🌲 
<%"---"%>

[[<% tp.date.now("YY.[W]WW", -7) %>|⬅ <% tp.date.now("[Week] WW", -7) %>]] | [[<% tp.date.now("YY.[W]WW", 7) %>|<% tp.date.now("[Week] WW", 7) %> ➡]]

## Goals

> [!milestone] Goals for this Quarter
> ![[<% tp.date.now("YYYY-[Q]Q") %>#^goals-link]]

- 

^goals-link

## Memos

- [[<% tp.date.weekday("YYYY-MM-DD", 0) %>|Monday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 0) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 1) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 1) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 2) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 2) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 3) %>|Thursday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 3) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 4) %>|Friday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 4) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 5) %>|Saturday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 5) %>#^memo-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 6) %>|Sunday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 6) %>#^memo-link]]

^memo-link

## Work Log

- [[<% tp.date.weekday("YYYY-MM-DD", 0) %>|Monday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 0) %>#^work-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 1) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 1) %>#^work-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 2) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 2) %>#^work-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 3) %>|Thursday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 3) %>#^work-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 4) %>|Friday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 4) %>#^work-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 5) %>|Saturday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 5) %>#^work-link]]
- [[<% tp.date.weekday("YYYY-MM-DD", 6) %>|Sunday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 6) %>#^work-link]] 

^work-link

```meta-bind
INPUT[list(title(Wins This Week)):list]
```
