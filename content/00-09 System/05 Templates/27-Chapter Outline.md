<%"---"%>
id: <% tp.date.now("YYYYMMDDHHss") %>
date: <% tp.date.now("YYYY-MM-DD") %>
tags:
<%"---"%>

> [!multi-column]
> 
> > [!map] Parents
> > 
> 
> > [!map] Siblings
> > 

> [!info] Summary
> <% tp.file.cursor(1) %>

## Outline

### Act 1 - Setup

#### Block 1 - Introducing the main characters

###### 1. INTRODUCTION - Intro to set up their ordinary world

<% tp.file.cursor(2) %>

###### 2. INCIDENT - Inciting incident to start of the story

<% tp.file.cursor(3) %>

###### 3. FALL OUT - Immediate reaction to the incident

<% tp.file.cursor(4) %>

#### Block 2 - Life gets disrupted

###### 4. REACTION - MC reacts & reflects on long-term impacts

<% tp.file.cursor(5) %>

###### 5. ACTION - MC takes action

<% tp.file.cursor(6) %>

###### 6. CONSEQUENCE - Immediate consequences of MC’s actions

<% tp.file.cursor(7) %>

#### Block 3 - Time to change

###### 7. PRESSURE - MC’s Life has changed, creating pressure & stress

<% tp.file.cursor(8) %>

###### 8. PLOT TWIST - The first pinch or plot twist occurs

<% tp.file.cursor(9) %>

###### 9. PUSH → - Due to the plot twist, the MC is pushed into the new world

<% tp.file.cursor(10) %>

### Act 2 - Conflict

#### Block 4 - Settle into new world

###### 10. NEW WORLD - Intro to the new world. What’s changed? MC’s feelings?

<% tp.file.cursor(11) %>

###### 11. FUN & GAMES - MC takes a break, has a little fun

<% tp.file.cursor(12) %>

###### 12. JUXTAPOSITION - Comparison between the past world and the present one

<% tp.file.cursor(13) %>

#### Block 5 - Main conflict

###### 13. BUILD UP - Midpoint is approaching!

<% tp.file.cursor(14) %>

###### 14. MIDPOINT - The main midpoint conflict

<% tp.file.cursor(15) %>

###### 15. REVERSAL - Immediate reaction or consequence of the midpoint

<% tp.file.cursor(16) %>

#### Block 6 - Find the end-goal

###### 16. CONSEQUENCE - MC reflects on long-term impacts of midpoint

<% tp.file.cursor(17) %>

###### 17. TRIALS - MC takes action, but due to the enormity of the task, stuff go wrong

<% tp.file.cursor(18) %>

###### 18. DEDICATED - Despite setbacks, MC decides to succeed no matter what

<% tp.file.cursor(19) %>

### Act 3 - Resolution

#### Block 7 - Darkest moment

###### 19. CALM BEFORE THE STORM - Stuff seem to calm down, but the tension is still there

<% tp.file.cursor(20) %>

###### 20. PLOT TWIST - MC experiences something completely unexpected

<% tp.file.cursor(21) %>

###### 21. DARKEST MOMENT - Success seems impossible

<% tp.file.cursor(22) %>

#### Block 8 - Motivated

###### 22. POWER WITHIN - MC remembers their desire to succeed & finds their inner power

<% tp.file.cursor(23) %>

###### 23. ACTION/RALLY - MC takes action, plot lines begin to converge

<% tp.file.cursor(24) %>

###### 24. CONVERGE - The final battle is approaching!

<% tp.file.cursor(25) %>

#### Block 9 - Finale

###### 25. BATTLE - The finale! MC has one last battle

<% tp.file.cursor(26) %>

###### 26. CLIMAX - MC takes action to resolve the problem from the midpoint

<% tp.file.cursor(27) %>

###### 27. RESOLUTION - Immediate reaction to MC’s decision

<% tp.file.cursor(28) %>

## Scenes

> [!map] Children
> ```dataview
> LIST
> FROM "<% tp.file.path(true) %>"
> WHERE file.name != "<% await tp.file.title %>"
> ```
