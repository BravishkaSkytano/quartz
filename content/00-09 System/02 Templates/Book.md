<%"---"%>
id: <% tp.date.now("YYYYMMDDHHss") %>
date: <% tp.date.now("YYYY-MM-DD") %>
modified: 
share: true
tags:
- type/book
title: "{{title}}"
subtitle: "{{subtitle}}"
author: {{author}}
cover: <%=book.coverUrl ? `https://books.google.com/books/publisher/content/images/frontcover/${[...book.coverUrl.split("&")[0].matchAll(/id.?(.*)/g)][0][1]}?fife=w600-h900&source=gbs_api` : ''%>
series: 
seriesnumber: 
rating: 
readdates:
- started: 
  finished: 
shelf: toread
publisher: {{publisher}}
publish: {{publishDate}}
total: {{totalPage}}
isbn: {{isbn10}} {{isbn13}}
<%"---"%>

![cover|150]({{coverUrl}})


Author(s): <%=book.authors.map(author => `[[${author}]]`).join(', ')%>
Series: 

## Description

{{description}}

## Notes

