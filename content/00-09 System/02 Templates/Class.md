<%"---"%>
id: <% tp.date.now("YYYYMMDDHHmm") %>
title: <% tp.system.prompt("Title:") %>
date: <% tp.date.now("YYYY-MM-DD") %>
modified: 
tags:
- 📥/🌲 
<%"---"%>


## Description

<% tp.file.cursor(1) %>

## Learning Objectives

1. <% tp.file.cursor(2) %>

## Assignments

<%"- [ ]"%> <% tp.file.cursor(3) %>

