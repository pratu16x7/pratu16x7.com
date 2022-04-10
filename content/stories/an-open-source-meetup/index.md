---
title: "An Open Source Meetup"
subtitle: ""
date: 2017-04-10T12:00:00+05:30
color: "green"
draft: false
thumbnail: "thumbnail.jpg"
---

We were all at the LUG (Linux Users Group) meet-up this weekend, with an  assorted group of programmers, contributors, professors and students  coming together to talk on all things open source. Here are some of the highlights.

<!--more-->

## The Yocto Project

What is the best way to deploy Linux on custom hardware? Joe Steeve gave us the straightforward way to setup, say, a kiosk (like an ATM  machine) with a distro. We could probably configure the .bash_profile  for a startup sequence to open up a browser and disable some keys.  Straightforward, but unscalable and an overkill. Embedded distros can  come in handy for specific applications, but even with so many out  there, it is unlikely you’ll find the perfect one for your needs.

Right up, Joe introduced us to the [Yocto project](https://www.yoctoproject.org), that gives you tools to build your own customized Linux distribution  (Yep). At its most basic, you can download the sources, setup the  environment and the configuration files, and run the build with BitBake. For even deeper customization for a functionality, you can write  recipes for the build that run tasks and add packages to the generated  image. I always thought that to make a custom OS, the only way was to  assemble it from scratch. The Yocto project achieves the same flexibilty in a way that is a lot less painful.

## An Intro to Regex

(aka A Regex Ninja’s Musings*)

It is said that the power of regular expressions compensates for their  readability. To obviate the latter, we had a comprehensive dive into  their syntax and working with R. K. Rajeev. For string and pattern  matching cases, the grammar is pretty compact. The idea of capturing  groups looked powerful for transforming strings, because it allowed to  pass information about the previous state of the string. It meant that  replacing could be dynamic depending on this state. Also was escaping  characters seems to be the norm, but inconsistent across  implementations. We learned enough to explore more for any application  that needed it.

## Education: Technology not Tools

We are all aware with a problem in the approach of teaching  technology-based courses in colleges. Ignoring the underlying goal and  with the focus on the software that is used with instructions specific  to it, means that as students, not everyone is aware of alternatives.  However, we do have people working to make a change. Two of the  attendees who were maths professors have filed a petition to make the  course syllabus vendor-free. The computer staff at [DBIT](http://www.dbit.in) have migrated every college lab onto Ubuntu to foster the use of more open tools. Our company [Frappé Technologies](https://frappe.io/about) along with DBIT organises an open source [hackathon](https://mumbaihackathon.in) every year with no restrictions on the way to build a project. It has the goal of ultimately —

## Evangelising and using Open source

Pumped with the ongoing contributions from various user groups, there are  plenty of opportunities to get everyone involved. It would pay-off well  to have such meet-ups at colleges with active student groups, making  fantastic hubs. At this one itself, Joe geared up student attendees on  remixing a typical final year robotics project by setting up a  BeagleBone with a Yocto built image. They could even report and write  patches for any cross-compilation issues along the way. Also, Regex was a great way to see some of their Theoretical Computer Science concepts in action.

[Rushabh Mehta](https://medium.com/u/cec2918eee75?source=post_page-----f4c801c56e2e--------------------------------) suggested a way to take evangelising a step further; the meets could  develop projects to solve a real world problem. While being an effective way to make an impact, it would mean people with different expertise  could come together to figure out solutions.

![The Folk](the_folk.jpg)

## Wrapping up

Plenty of discussions, and views on what we could do to connect even more  groups. Not to mention the breadth of everyone’s experiences when  turning to open source (Rajeev’s anecdotes since the dawn of the Unix  movement in India made Sourceforge look new). It was enlightening to  have the flame wars off the forums for a change (Unity vs. Gnome shell,  Vim vs. Emacs; we were out of time, or [perhaps …](https://xkcd.com/378/)). We look forward to more of these in future.

**courtesy R. K. Rajeev.*