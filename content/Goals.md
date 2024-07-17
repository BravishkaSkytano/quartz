---
obsidianUIMode: preview
cssclasses:
  - cards
---
## Yearly

```dataviewjs
let goals = dv.pages('"00-09 System/05 Goals/05.01 Yearly"');
dv.table(["Goal", "Target", "Progress", "Deadline"],
goals.map(goal => [
`<div style="position: relative; overflow: hidden; width: 100%; height: 200px;"> <img src="${goal.banner}" alt="Banner" style="object-fit: cover; object-position: center; width: 100%; height: 100%;"> <div style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></div>
</div>`, `<span style="font-size: 1.1em;">${goal.file.link}</span>`,
goal.deadline,
`<progress value="${goal.progress}" max="${goal.target}"></progress><br>${Math.round((goal.progress / goal.target) * 100)}% completed` ]) );
dv.container.classList.add("cards-align-top");
```

## Quarterly

```dataviewjs
let goals = dv.pages('"00-09 System/05 Goals/05.02 Quarterly"');
dv.table(["Goal", "Target", "Progress", "Deadline"],
goals.map(goal => [
`<div style="position: relative; overflow: hidden; width: 100%; height: 200px;"> <img src="${goal.banner}" alt="Banner" style="object-fit: cover; object-position: center; width: 100%; height: 100%;"> <div style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></div>
</div>`, `<span style="font-size: 1.1em;">${goal.file.link}</span>`,
goal.deadline,
`<progress value="${goal.progress}" max="${goal.target}"></progress><br>${Math.round((goal.progress / goal.target) * 100)}% completed` ]) );
dv.container.classList.add("cards-align-top");
```