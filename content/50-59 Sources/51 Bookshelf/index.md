---
title: 51 Bookshelf
id: 202405161031
date: 2024-05-16
modified: 2024-05-20
tags:
  - moc
  - source/books
draft: true
---

## Currently Reading

- [[Introduction to Philosophy by Norman L Geisler and Paul D Feinberg]]

%%
```dataview
TABLE WITHOUT ID
"![cover|80](" + cover + ")" AS "Cover",
title AS "Title",
author AS "Author(s)", series + " #" + seriesnumber as "Series"
FROM "50-59 Sources/51 Bookshelf/books"
WHERE shelf="reading"
SORT title ASC
```
%%

## Stopped Reading

%%
```dataview
TABLE WITHOUT ID
"![cover|80](" + cover + ")" AS "Cover",
title AS "Title",
author AS "Author(s)", series + " #" + seriesnumber as "Series"
FROM "50-59 Sources/51 Bookshelf/books"
WHERE shelf="stopped"
SORT title ASC
```
%%

## To Be Read

%%
```dataview
TABLE WITHOUT ID
"![cover|80](" + cover + ")" AS "Cover",
title AS "Title",
author AS "Author(s)", series + " #" + seriesnumber as "Series"
FROM "50-59 Sources/51 Bookshelf/books"
WHERE shelf="toread"
SORT title ASC
```
%%
