---
title       : letterFreq!
subtitle    : A presentation for Developing Data Products course
author      : D Bolotov
job         : 
framework   : io2012   # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js # {highlight.js, prettify, highlight}
hitheme     : tomorrow_edited         # zenburn tomorrow
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## letterFreq!

Ever read some text and wondered what the distribution of characters looks like?

Whether that wall of text contains 23 a's, or 24?

What the most common English letters are?


---

## letterFreq!

hey there

---

## letterFreq!



Let's define a test string, get frequency counts for it, and plot them.

```r
str <- "I am a string with numeric (123) and other non-alpha (%$^#&!)characters."
sanitize(str) 
```

```
## a c d e g h i l m n o p r s t u w 
## 7 3 1 3 1 4 4 1 2 5 2 1 5 2 4 1 1
```



---

## letterFreq!

Let's define a test string, get frequency counts for it, and plot them.

```r
fplot(str)
```

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3.png) 

Enter your own text, check other distributions, and see it in action here: [letterFreq!](https://dontpanic.shinyapps.io/letterFreq/)





