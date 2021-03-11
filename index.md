---
lesson-example: "https://carpentries.github.io/lesson-example/"
layout: default
title: "Building websites in GitHub"
---

[//]: # ({{ site.title }})

{{ site.description }}

# Project lead

{% assign lead = site.team_members | where:"role", "project lead" | first %}

The project is lead by {{ lead.name }}. 
[See our full team](about.md#funders).


[See our full team](about#funders).

## This is Robert's personal website btw ;)

In this website I will showcase my professional portfolio.
And here is a loremipsum. :)

Here's an [example lesson:]({{ page.lesson-example }})

[More about me/ my research](about.md)

[//]: # (This may be the most platform independent comment)

## Blog posts

{% for post in site.posts | sort: "author" %}
- {{ post.date | date_to_string }}: {{ post.title }} by *{{ post.author }}*
{% endfor %}

