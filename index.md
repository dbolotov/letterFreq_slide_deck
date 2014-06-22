---
title       : letterFreq
subtitle    : Developing Data Products
author      : D Bolotov
job         : 
framework   : io2012    # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.jS  # {highlight.js, prettify, highlight}
hitheme     : googlecode          # zenburn tomorrow
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Slide 2

Ever read some text and wondered what the distribution of characters looks like?

---

## Slide 3

hey there

---

## Demo




```r
str <- "I am a test string with numeric (1234) and other non-alpha characters. (^_^)y "

sanitize(str)
```

```
##       a       c       d       e       g       h       i       l       m 
## 0.13462 0.05769 0.01923 0.07692 0.01923 0.07692 0.07692 0.01923 0.03846 
##       n       o       p       r       s       t       u       w       y 
## 0.09615 0.03846 0.01923 0.09615 0.05769 0.11538 0.01923 0.01923 0.01923
```

---

## Slide 5

Link to shinyapp

The end.




