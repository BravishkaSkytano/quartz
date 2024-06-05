---
title: 51 Bookshelf
id: 202405161031
date: 2024-05-16
modified: 2024-05-22
tags:
  - moc
  - source/books
draft: false
---

## Currently Reading

- [[Introduction to Philosophy by Norman L Geisler and Paul D Feinberg]] ![progress-bar](https://progress-bar.dev/10)
- A Villianess for the Tyrant
    - Started: 
    - [Novel](https://tapas.io/series/a-villainess-for-the-tyrant-novel)
    - [Comic](https://tapas.io/series/a-villainess-for-the-tyrant)
- [Raising My Fiancée with Money](https://tapas.io/series/raising-my-fiance-with-money)
    - Started:
- Revolutionary Princess Eve
    - Started:
    - [Comic](https://tapas.io/series/revolutionary-princess-eve)
    - [Novel](https://tapas.io/series/revolutionary-princess-eve-novel)
- [The Vampire’s Consort](https://tapas.io/series/the-vampires-consort-novel/info), ch 15 of 177
    - Started:
- [Going Rogue in the Apocalypse](https://tapas.io/series/going-rogue-in-the-apocalypse/info), ch 17 of 105
    - Started
- [Winter Wolf](https://tapas.io/series/winter-wolf)
    - Started
- https://tapas.io/series/the-bird-empress
- https://tapas.io/series/my-k-pop-secret-novel
- https://tapas.io/series/daisy-how-to-become-the-dukes-fiancee-novel
- https://tapas.io/series/I-Made-a-Deal-with-the-Devil-Novel
- https://tapas.io/series/positively-yours

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
