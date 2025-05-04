+++
template = "section.html"
title = "Narisatu"
description = "Narisatu: simple puzzle with a complex solution"

[extra]
keywords = "non-arithmetic saturated subset"
app_name = "Narisatu"
app_motto = "Simple arithmetic puzzle with a complex solution"
+++

# Narisatu

Narisatu is a simple arithmetic puzzle with a complex solution. You are given a set of consecutive numbers from 1 to some number, say 16. The goal is to select some numbers while following a constraint: no three of the selected numbers can form an arithmetic sequence.

Trying to remember, what is an arithmetic sequence. Here, let us consider one example:
- 2, 5, 8, 11, 14, 17, ...

The difference between two consecutive elements is always the same: 3 = 5 - 2 = 8 - 5 = 11 -8 etc. Just a simple puzzle, where you have to continue the sequence, right? No, Narisatu is much harder. It requires that there is no arithmetic sequence, no matter which three of the selected numbers you check.

Check out a bit more comprehensive [tutorial](/narisatu/tutorial) on how to play Narisatu.

## Screenshots

{{ gallery(path="/narisatu/", images=["ss-1.png", "ss-2.png"]) }}

## Play

You can play [Narisatu online](/narisatu/web/) or install a mobile app for Android phones.

{{ playstore(appid='Narisatu', question='Do you like puzzles?', motto='Narisatu is a simple puzzle with a complex solution.') }}
