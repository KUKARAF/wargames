---
category: "[[Clippings]]"
author: 
title: "Natas Level 3 → Level 4"
source: https://overthewire.org/wargames/natas/natas4.html
clipped: 2023-08-12
published: 
topics: 
tags: [clippings]
---

```
Username: natas4
URL:      http://natas4.natas.labs.overthewire.org

user:natas3
Password:G6ctbMJ5Nb4cbFwhpMPSvxGHhQ7I6W8Q
```

# solutions
Not even google will find it this time? Interesting! 
![[Screenshot from 2023-08-12 17-26-58.png]]


Google crawls or doesn't crawl a website based on the [robots.txt](https://developers.google.com/search/docs/crawling-indexing/robots/intro) file. this file is public and google obeys everything described in it like: google please do not access those sensitive files. We have no such limitations though. 

Indeed when we load [/robots.txt](http://natas3.natas.labs.overthewire.org/robots.txt) we find: 

```
User-agent: *
Disallow: /s3cr3t/  
```

This leads us to [users.txt](natas3.natas.labs.overthewire.org/s3cr3t/users.txt) and ultimately to the password:
`natas4:tKOcJIbzM4lTs8hbCmzn5Zr4434fGZQm`


