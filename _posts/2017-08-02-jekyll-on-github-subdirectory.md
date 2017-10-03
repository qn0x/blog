---
title: Using Jekyll on Github, Served under a Subdirectory
updated: 2017-08-02 18:30
categories:
    - hosting
tag: hosting
---

For a long time I've wanted to write blogs but never got around to doing it.
About half a year ago I discovered Jekyll.
Back then I struggled to get the configurations right, getting stuck with different dependencies, using different themes, but most of all, I wanted to host my blog on Github under a subdirectory with a custom URL.
I've searched both Github's and Jekyll's documentations for any kind of hint but never found one.
Now, after letting it stew for a while I found a very simple solution:  

1. Initialize a new repository either on Github or on your machine  
2. Paste your Jekyll content in the repository root directory  
3. Edit your `.gitignore` so the directory with the generated pages is excluded from version control (e.g. `./_site`)  
4. Edit your `_config.yml` as follows:
  * `baseurl: "/blog"` - the subdirectory you want to host your blog in, must end WITHOUT a slash
  * `url: "http://qn0x.xyz"` - your custom domain
5. Checkout a new branch `"gh-pages"`
6. Commit and push to this branch on Github  
7. On the Github website, go to you repository settings and set `Options -> Github Pages -> Source to "gh-pages branch"`
8. All done!  

Hope this helps anyone wanting to do the same thing :)
