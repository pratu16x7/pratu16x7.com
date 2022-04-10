---
title: "Autotagging Urls"
subtitle: ""
date: 2019-04-13T12:00:00+05:30
color: "sepia"
draft: false
summary: "**The Problem**: Given a set of URLs of programming learning resources, categorize them based  one or more definative characteristics: language, type of site, stage of learning etc."
---

## The Problem 

*"Given a set of URLs of programming learning resources, categorize them based  one or more definative characteristics: language, type of site, stage of learning etc."*



To see how they look, here's a small sampling of links:

```py
urls = [
    "https://medium.com/@pratu16x7",
    "https://signalvnoise.com/posts/3250-clarity-over-brevity-in-variable-and-method-names",
    "http://flask.pocoo.org/","http://docs.python-requests.org/en/master/",
    "http://docs.python-guide.org/en/latest",
    "http://www.writethedocs.org/guide/writing/beginners-guide-to-docs/#what-to-write",
    "https://getbootstrap.com/docs/4.1/content/reboot/",
    "https://vuejs.org/v2/guide/",
    "https://yarnpkg.com/en/docs",
    "http://blissfuljs.com/docs.html",
    "https://www.kennethreitz.org/documentation-is-king/",
    "https://signalvnoise.com/posts/454-why-most-copywriting-on-the-web-sucks",
    "https://jgthms.com/web-design-in-4-minutes/",
    "https://vuejs.org/v2/guide/components.html",
    "https://vuejs.org/v2/guide/",
    "https://vuejs.org/v2/api/#vm-mount",
    "https://news.ycombinator.com/item?id=11164013",
    "https://docs.gitbook.com/",
    "https://docsify.js.org/#/",
    "https://docsify.js.org/#/plugins?id=list-of-plugins",
    "https://vuepress.vuejs.org/guide/#how-it-works",
    "https://vuepress.vuejs.org/guide/#why-not",
    "https://frappe.io/charts",
    "https://www.youtube.com/watch?v=ahXIMUkSXX0",
    "https://gist.github.com/kenneth-reitz/973705",
    
    "Stack overflow 3",
    ""
]
```

 

## Making the program aware 

Before parsing any data, it makes sense to define certain features  that the program is looking for in the links. Let's look at three forms  of categorisation, or *tags*:

#### Which technology? 

Programmining languages or software tools, widely used. Let's get the top 50 of them over from [StackOverflow's most popular tags](https://data.stackexchange.com/stackoverflow/query/172362/get-all-tags) which are primarily technology focussed.

```shell
>>> ['javascript', 'java', 'c#', 'php', 'android', 'python', 'jquery', 'html', 'c++', 'ios', 'css', 'mysql', 'sql', 'asp.net', 'ruby-on-rails', 'c', 'arrays', 'objective-c', 'r', '.net', 'node.js', 'json', 'angularjs', 'sql-server', 'swift', 'iphone', 'regex', 'ruby', 'ajax', 'django', 'excel', 'xml', 'asp.net-mvc', 'linux', 'angular', 'database', 'python-3.x', 'spring', 'wpf', 'wordpress', 'vba', 'string', 'reactjs', 'xcode', 'windows', 'vb.net', 'html5', 'eclipse', 'multithreading', 'laravel']
```

These can now be used for fuzzing matching content later on to decide what technology a link belongs to.



#### What stage of learning?

This is somewhat tricky and will depend on the kind of  course/training, but we can come up with a basic scale that can apply to  most:

-  **[Level 0]**: Pre requisites and skills
-  **[Level 1]**: Basic tech, Hello world project 
-  **[Level 2]**: Roadblocks to Intermediate
-  **[Level 3]**: Advanced concepts
-  **[Level 4]**: Case studies / Main Project

Now that we know what tags we have to categorize by, let's take a closer look at our data.



 

## Parsing the data 

### Stage 1: The URL strings 

The URLs on their own can also . Not all links will present useful  information, but many will. It makes sense to perform all the parsing  that we'd do for the link page data on the link URL itself, to see if we  can get down some of the categorisations.

The most we can infer is the tech if referred in the URL. And if the  domain matches one of the links in our knowledge base of links in  diffferent resource types

Assigning an internal domain tag will also be useful for specific API handling (discussed later in stage 3).

### Stage 2: The link page data 

While somewhat expensive for a large number of links,

### Stage 3: Specific handling based on domain 

Why is this worth investing in? Because as we have seen, most links  will be from official docs, forums like stackexchange and code hosting  services, most of which have well maintained developer APIs. By writing  modules to handle just 3-4 of these services, we can acquire highly  accurate data than page parsing for possibly 30-50% of the links.

### Stage 4: NLP (Optional) 

In order to derive information from the bare scratch, using TF-IDF can lead to interesting results.

