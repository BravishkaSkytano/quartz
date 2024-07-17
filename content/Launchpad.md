---
obsidianUIMode: preview
cssclasses:
  - dashboard
  - wide
  - cards
---

`BUTTON[daily-note]` 💠 `BUTTON[weekly-note]` 💠 `BUTTON[light-mode, dark-mode]` 💠 `BUTTON[tasks]`

![[Tasks Calendar]]

---
```meta-bind-button
style: default
label: Open Daily Note
hidden: true
id: daily-note
actions:
  - type: command
    command: periodic-notes:open-daily-note

```
```meta-bind-button
style: default
hidden: true
label: Open Weekly Note
id: weekly-note
actions:
  - type: command
    command: periodic-notes:open-weekly-note
```
```meta-bind-button
style: default
label: View Tasks
hidden: true
id: tasks
actions:
  - type: command
    command: card-board:open-card-board-plugin-0
```
```meta-bind-button
style: default
label: Light Mode
id: light-mode
hidden: true
actions:
  - type: command
    command: theme:use-light
```
```meta-bind-button
style: default
label: Dark Mode
id: dark-mode
hidden: true
actions:
  - type: command
    command: theme:use-dark
```
