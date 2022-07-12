---
title: "Clean Code - Introduction"
date: 2022-07-12T18:11:19+02:00
draft: false
author: "Ganeshdip"
description: "An introduction to clean coding"
tags: ["clean code", "programming", "design"]
series: ["Clean Code"]
ShowToc: true
TocOpen: true
---

What is mean by clean code? Let's find out. Inspired by the book `Clean Code` by `Robert C. Martin (Uncle Bob)`. 

<!--more-->

# Code
The code is a part of our daily lives now. It's running on smartphones, smartwatches, and TVs. Almost everywhere. And there is always a need for enhancement or new features which results in the addition/update of the existing code base. 

So the code will always be there with us. 

# Bad code 
As a programmer, we always come across bad code.  But identifying the bad code doesn't make us the good programmer. Programming is an art. One can tell the difference between a good painting and a bad painting. But it will not make someone a good painter. Painting is an art that needs to be acquired through practice. The same applies to coding. 

We need to practice it to become good programmers and have a `code sense`.

# Cost of owning the bad code
Bad code is hard to read and hard to change. it always creates doubt in the mind of the programmer that it may start breaking the unknown part of the code. It slows down development. Redesigning the whole system into clean code is even more costly. 

It becomes a building with broken windows that nobody cares about. 

# Clean code
Clean code is simple to read and change. It does what the reader is expecting. In short, it is focused and minimal. It is written by someone who cares about it. 

Following is an example of real world problem - 
```go
func makeCupOfTea(kettle, water, teaBag) cupOfTea {
    hotWater := boilWater(kettle, water)
    cupWithHotWater := pourWater(hotWater,cup)
    cupWithTea := addTeaBag(cupWithHotWater, teaBag)
    wait(3 minutes)
    return cupWithTea
}
```


# Leave it better
As the boy scout rule states - "Keep the campground cleaner than you found it". Make the code clean with each pull request. 

And the code will age like a fine wine :blush:
