<%"---"%>
id: <% tp.date.now("YYYYMMDDHHss") %>
obsidianUIMode: preview
banner: https://preview.redd.it/arqa352ph7x61.jpg?width=960&crop=smart&auto=webp&s=84f9245d607b029667d5bfc4abf36547fc6213de
cssclasses:
  - three-column-list
<%"---"%>

[[<% tp.date.now("YY.MM MMMM", "P-1M") %>|↶ <% tp.date.now("MMMM YYYY", "P-1M") %>]] ⁝ [[<% tp.date.now("YY.MM MMMM", "P1M") %>|<% tp.date.now("MMMM YYYY", "P1M") %> ↷]]

## Toggl

<%"```toggl"%>
SUMMARY FROM <% moment(tp.date.now("YYYY-MM-DD")).startOf("month").format("YYYY-MM-DD") %> TO <% moment(tp.date.now("YYYY-MM-DD")).endOf("month").format("YYYY-MM-DD") %>
TITLE "<% tp.date.now("YYYY") %>"
<%"```"%>

## Books Read

<%"```dataview"%>
LIST WITHOUT ID
title + " (" + author + ")"
FROM "60-69 Bookshelf"
WHERE contains(string(readdates.finished), "<% tp.date.now("YYYY-MM") %>")
<%"```"%>

---

<%"%%"%> Waypoint <%"%%"%>
