+++
template = "page.html"
title = "Tutorial on Narisatu"
description = "Tutorial on How to play Narisatu"

[extra]
keywords = "non-arithmetic saturated subset"
+++

# How to play Narisatu?

Below, you can find a quick tutorial on how to play the game of Narisatu.

## Board

The game is played on a board containing consecutive numbers from 1 to *N*. For best gameplay, we recommend using *N* values of 4, 8, 16, 32, or 64.

The game board is rectangular, and you can adjust its width using a slider at the top to make gameplay more comfortable. The width setting doesn't affect the game's outcome.

An example of a gameboard with *N*=16 numbers is shown in the following image.

<p align="center">
<img src="/narisatu/no-arith-0.png" />
</p>

## Gameplay

The player selects a set of numbers from the board. By clicking the number, the number is selected if it is not yet selected, otherwise, it is deselected.

The selected numbers must obey the *no arithmetic sequence* condition (explained below). The board is saturated if each possible number is either
* selected or
* covered by the no arithmetic sequence condition.

The game has two possible goals:

- Maximize: select the largest possible set of numbers.
- Minimize: select the smallest possible set of numbers, while making the board saturared.

Notice that, in the maximize case, good solutions consists of the saturated boards.

## No arithmetic sequence

This condition means that any three of the selected numbers must **not** form an arithmetic sequence. To explain this a bit further, let *x*, *y,* and *z* be any three of the selected numbers, and let them be sorted, so *x < y < z*. Now, the difference *y - x* must **not** be equal to the difference *z - y*.

As an example, consider a game board with numbers from 1 to 16. The numbers 6 and 8 are already selected (shown in dark green color). The no arithmetic sequence condition prevents selecting numbers 4, 7, and 10. If any of these is selected, it forms the arithmetic sequence between the other two. Particularly:
- Selecting 4 creates the arithmetic sequence 4, 6, 8 as 6 - 4 = 10 - 8 = 2.
- Selecting 10 creates the arithmetic sequence 6, 8, 10 as 10 - 8 = 8 - 6 = 2.
- Selecting 7 creates the arithmetic sequence 6, 7, 8 as 8 - 7 = 7 - 6 = 1.

<p align="center">
<img src="/narisatu/no-arith-1.png" />
</p>

So far, we have learned that selecting the numbers 6 and 8 results in the numbers 4, 7, and 10 being covered, and, thus, unavailable for selection.

When selected numbers form an arithmetic sequence, they will be highlighted in red. For instance, after selecting 6 and 8, selecting 4 will highlight 4, 6, and 8 in red, indicating that one must be deselected.

<p align="center">
<img src="/narisatu/no-arith-2.png" />
</p>

## Saturation

Consider the following board. It is saturated because every number is either:
* selected (dark green numbers),
* covered (ordinary green colored numbers).

<p align="center">
<img src="/narisatu/no-arith-3.png" />
</p>

> Can you select more than 8 numbers while keeping the board green?

> Can you make the board saturated by selecting only 4 numbers?
