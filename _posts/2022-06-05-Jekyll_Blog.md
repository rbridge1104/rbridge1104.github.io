---
title: 
date: 2022-06-05 01:36
categories: [homelab, programming]
tags: [ programming, homelab]
---

# How This Was made

First off I would like to start by saying this site looks way better than I thought it would.  For that I would like to thank Techno Tim for his Youtube video [Meet Jekyll](https://www.youtube.com/watch?v=F8iOU1ci19Q). In additon the [chirpy-starter](https://github.com/cotes2020/chirpy-starter) repo by [cotes2020](https://github.com/cotes2020) is amazing. 
## Why Jekyll
When I started doing research on doing my own blog all my research started pointing to either using Medium or hosting my own Wordpress.  These both seemed like good options.

The problem with medium was that I was also trying to host this on my site not utilize another platform.  That way I could learn some of the back end of maintaing and deploying a website.

The other primary option was Wordpress.  Although many people use this option it semmed overly complex for what I was wanting to do. I also would have to find a place to host it.  

Jekyll seemed like the ideal fit.  First I could use github pages to host the site which is free.  The deployment and build were also easy and simple but had the features I wanted.  I also could add complexity later on if I chose.  Below are some of the lessons I learned while deploying it for the first time.

## Lessons Learned

### Lesson 1 Base URL
 Some of the things that I learned, not sure if I missed documentation or not was that on the _config.yml file you need to comment out the base url
```yml

# Change the following value to '/PROJECT_NAME' ONLY IF your site type is GitHub Pages Project sites
# and doesn't have a custom domain.
# baseurl: ""
```
When that line was active the entire site was not visible on my github pages.  I think this my be usefull if you use a custom URL but I haven't gotten that far yet.

### Lesson 2 File Name
This one is totally my fault.  When I named my first blog post I wasn't paying attention to the demo so I named it
```bash
 Hello_World_in_7_languages.md
```
So when I deployed the website nothing showed up.  For some reason you have to add the date to the file name, I think it is for indexing purposes. For example
``` bash
 2020-06-05-Hello_World_in_7_languages.md

```
This allowed the post to populate.

I hope you find this post usefull or at least I will next time I try and do this.  