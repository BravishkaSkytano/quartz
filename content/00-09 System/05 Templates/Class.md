<%"---"%>
id: <% tp.date.now("YYYYMMDDHHss") %>
date: <% tp.date.now("YYYY-MM-DD") %>
cssclasses:
  - dashboard
<%"---"%>

<%"```toggl"%>
SUMMARY 
FROM <% tp.file.cursor(1) %> TO <% tp.file.cursor(2) %>
INCLUDE PROJECTS "<% tp.file.title %>"
<%"```"%>

## Description

<% tp.file.cursor(3) %>

## Syllabus

<%"- [ ]"%> <% tp.file.cursor(4) %>

