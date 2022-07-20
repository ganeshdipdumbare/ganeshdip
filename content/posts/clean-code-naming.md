---
title: "Clean Code Naming"
date: 2022-07-20T18:26:22+02:00
draft: false
author: "Ganeshdip"
description: "Meaningful Names"
tags: ["clean code", "programming", "design"]
series: ["Clean Code"]
ShowToc: true
TocOpen: true
---

What is the importance of the names in coding? Let's find out.

<!--more-->

# Naming 
The names are tied to the identity. Our names carry personal, cultural and historical connections and most important in starting the communication.

The same applies for the naming in software engineering. The names represents particular part of the code tied with particular responsibility. 

# Intentions
Names must show the intentions behind using it.

eg. Following variable represent time passed in terms of days
```go
var elapsedTimeInDays int
```
Be direct in naming as it shows the exact purpose and useful while reading the code.

# Avoid disinformation
Names with shortform, suffix or similar spelling must be avoided as it makes the programmer confused. 

Dont use same meaning names to specify different parts of the code. Dont use sum and addition in the same function.

# Use pronounceable names
The pronounceable names are always easy to read and easy to discuss.

eg. instead of using dob, use the following variable 
```go
var dateOfBirth time.Time
```

# Use searchable names
The searchable names are easy to lookup while reading and debugging the code and easy to replace. 

The terms which are similar in spellings will appear while searching and will make reading difficult.

The editor will show autocompletion where searchable terms are useful.

# Avoid mental mapping
Avoid mental mapping of names as it will be familiar for you but the reader will not be aware of the same. 
eg. I am mapping s as sum in the mind but the user who is reading the code will be clueless.

# Class/Interface names
The class/interface names should be noun or noun phrase.

eg.

```go
type Reader interface{}
```

# Method names
The method names should be verb or verb phrase.

eg.

```go
func ReadFile() error
```

# Pick one word per concept
Pick one word per concept throughout the code as it makes the reading easy.

eg. 

Do not use fetch, retrive or get all over the places. Choose only one out of these 3 names.

# Dont pun
Dont use same name for different concepts.

eg.

Use `append()/insert()` instead of add() when adding an element to the list.

# Use solution domain names
The program is read by programmers and the names which are solution specific are always easy to read and understand.

eg. Use `quickSort()` if quick sort is getting used for sorting.

# Use problem domain names
The problem domain names or business domain names are used to understand the program easily.

eg. Use `bookTaxi()` instead of updateTaxi().

# Add meaningful context
The names with the context are always easier to read and understand.

eg.

Instead of using addState, create a struct named `Address` and add a field called `State`.

As state can be anything with state or state of matter. 

# Keep it straighforward
In conclusion, use names which are easy to understand and dont need to be memorized.

The simple and contextful names are easy to search and change.