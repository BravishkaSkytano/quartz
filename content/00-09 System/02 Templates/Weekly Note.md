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

```meta-bind
INPUT[list(title(Wins This Week)):list]
```

## Memos

- [[<% tp.date.weekday("YYYY-MM-DD", 0) %>|Sunday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 0) %>#Memos]]
- [[<% tp.date.weekday("YYYY-MM-DD", 1) %>|Monday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 1) %>#Memos]]
- [[<% tp.date.weekday("YYYY-MM-DD", 2) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 2) %>#Memos]]
- [[<% tp.date.weekday("YYYY-MM-DD", 3) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 3) %>#Memos]]
- [[<% tp.date.weekday("YYYY-MM-DD", 4) %>|Thursday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 4) %>#Memos]]
- [[<% tp.date.weekday("YYYY-MM-DD", 5) %>|Friday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 5) %>#Memos]]
- [[<% tp.date.weekday("YYYY-MM-DD", 6) %>|Saturday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 6) %>#Memos]]

Memos

## Work Log

- [[<% tp.date.weekday("YYYY-MM-DD", 0) %>|Sunday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 0) %>#Work Log]]
- [[<% tp.date.weekday("YYYY-MM-DD", 1) %>|Monday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 1) %>#Work Log]]
- [[<% tp.date.weekday("YYYY-MM-DD", 2) %>|Tuesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 2) %>#Work Log]]
- [[<% tp.date.weekday("YYYY-MM-DD", 3) %>|Wednesday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 3) %>#Work Log]]
- [[<% tp.date.weekday("YYYY-MM-DD", 4) %>|Thursday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 4) %>#Work Log]]
- [[<% tp.date.weekday("YYYY-MM-DD", 5) %>|Friday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 5) %>#Work Log]]
- [[<% tp.date.weekday("YYYY-MM-DD", 6) %>|Saturday]]
	![[<% tp.date.weekday("YYYY-MM-DD", 6) %>#Work Log]] 
