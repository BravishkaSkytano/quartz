<%"---"%>
id: <% tp.date.now("YYYYMMDDHHmm") %>
title: <% tp.date.now("dddd, MMMM Do, YYYY") %>
banner_icon: 🗝️
<%"---"%>

[[<% tp.date.yesterday("YYYY.MM.DD") %>|⬅ <% tp.date.yesterday("MMMM Do") %>]] | [[<% tp.date.tomorrow("YYYY.MM.DD") %>| <% tp.date.tomorrow("MMMM Do") %> ➡]]

<% tp.web.daily_quote() %>

```meta-bind
INPUT[progressBar(title(Proudness), minValue(0), maxValue(10)):proudness]
```

## Memos

- 

^memo-link

## Work Log

- 

^work-link

## Trackers

> [!milestone] Goals for this Week
> ![[<% tp.date.now("YYYY-[W]ww") %>#^goals-link]]

> [!orbit] Habit Tracker
> Writing: `INPUT[toggle:writing]` Stretch: `INPUT[toggle:stretch]` Reading: `INPUT[toggle:reading]`

## Tasks

### Not Done Yet

<%"```tasks"%>
happens <% tp.date.now("YYYY-MM-DD") %>
short mode
<%"```"%>

### New Additions

- 
