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

Ever read something and wondered what the distribution of (English) characters looks like?

Whether that wall of text contains 153 a's, or 154?

Whether your phone texts contain too many consonants?

What the most common English letters are?


---

## letterFreq!

Wonder no more.

LetterFreq!, a handy little app built in [Rstudio](http://www.rstudio.com/) and [Shiny](http://shiny.rstudio.com/), will take care of your letter-counting needs.

The app eats any text, dirty or clean, and shows you the relative and absolute frequencies of the English letters contained therein.

Optionally, the app will also plot the letter distribution from some English literature classics, or the main entries in the Oxford English dictionary.


Let's see a demo of the histogram capabilities.

---

## letterFreq!



Let's define a test string, get frequency counts for it, and plot them.

```r
str <- "I am a string with numeric (123) and other non-alpha (%$^#&!)characters. 
        I live in this presentation and wonder what the rest of the world is like."
sanitize(str) #clean the string and get absolute frequency counts
```

```
##  a  c  d  e  f  g  h  i  k  l  m  n  o  p  r  s  t  u  v  w 
## 10  3  4 11  1  1  8 11  1  4  2 10  6  2  9  6 11  1  1  4
```
This could use a few z's.


```r
str <- "I am a string with numeric (123) and other non-alpha (%$^#&!)characters. 
        I live in this presentation and wonder what the rest of the world is like. ZzZZzzZ."
sanitize(str)
```

```
##  a  c  d  e  f  g  h  i  k  l  m  n  o  p  r  s  t  u  v  w  z 
## 10  3  4 11  1  1  8 11  1  4  2 10  6  2  9  6 11  1  1  4  7
```

---

## letterFreq!

Let's define a test string, get frequency counts for it, and plot them.

```r
fplot(str) #plot relative and absolute counts starting from the raw string
```

<img src="assets/fig/unnamed-chunk-4.png" title="plot of chunk unnamed-chunk-4" alt="plot of chunk unnamed-chunk-4" style="display: block; margin: auto;" />

Hmm. No j, but eleven i's? And not even one b? Fascinating.

Enter your own text, check other distributions, and see it in action here: [letterFreq!](https://dontpanic.shinyapps.io/letterFreq/)





