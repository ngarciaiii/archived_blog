---
layout: post
title: "Black Belt Text-Fu"
date: 2022-05-19 00:00:00 -0400
categories: PWK
tags: [OSCP]
years: ['2022']
comments: true
---

## This is the Advanced Text-Fu section from [Linux Journey][Linux Journey]

## Regex (Regular expression)
Regular expression is a tool that uses special notations as an universal language with almost any programming language. I would guess that it is a stone age retrocomputer's early language. Ok this part wants to create a file with a string.

```bash
# remove sample.txt if you already have it
# actually don't need to, '>' will overwrite, I am just paranoid
$ rm sample.txt

# create a file with two lines string like this
$ echo "sally sells shells\nby the seashore" > sample.txt
$ cat sample.txt

# result:
sally sells shells
by the seashore

# ^ looks for beginning of a matching line
$ grep ^by sample.txt
# result:
by the seashore

# $ looks for ending of a matchining line
grep seashore$
# result:
by the seashore

# . looks for any matching single character
grep b. sample.txt
# result:
by the seashore

# [ ] specify characters found within bracket
# there are many tricks inside bracket notations
# [iou] looks for anything that has iou in between
$grep d[iou]g sample.txt

# [^i] excludes anything that has i in between
$grep d[^i]g sample.txt

# [a-c] looks for anything from a to c in between
# bracket notations are case sensitive, so might need to use [A-C]
$grep d[a-c]g sample.txt

```

## Text Editors

I am still sort of new with linux to be honest. I am unfamilar with ***Vim*** and ***Emacs***, however these two are recommended by [Linux Journey][Linux Journey]. I have seen professional programmers/hackers in youtube using either vim or emacs or nano. Some like to use GUI text editors like Sublime Text, or Geany. Okay emacs looks like a GUI!

vim  | emacs
:-------------------------:|:-------------------------:
![vim](/public/img/vim.png){:height="270px" width="auto"} |  ![emacs](/public/img/emacs.png){:height="270px" width="auto"}

## Vim, short for vi + IMproved

I didn't know there's a text editor ***vi***, but apparently Vim is the improved version. Gonna play with vim for awhile and using the same sample.txt from previous exercise. 

```bash
# type colon key --> : literally in the vim to start something
# :e is what opens a file, I am guessing e for execute
:e sample.txt

# you will see 
sally sells shells
by the seashore

# Try navigate by using 
# h, j, k, l == left, up, down, right 
# not a clockwise ¯\_(ツ)_/¯ 

# can feel like stuck inside vim, no clue of how to exit or whatever
# type ":" and you will see it on the bottom, type h
# it calls vim's very own "help.txt", and navigate with h, j, k ,l. 
:h

# too much, and it has its own tutorial for beginner, I will do that!
# let's exit by doing this
:qa!
```

After looking into help, I realize vim has its own tutorial. I think I am going to do a post on vim alone and same with emacs. It is too much to cover in this post. [Linux Journey][Linux Journey] did great by recommending these text editors and highlights.






[Linux Journey]:https://linuxjourney.com