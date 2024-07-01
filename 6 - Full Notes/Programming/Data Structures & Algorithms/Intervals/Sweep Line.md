
2024-06-15 09:12

Tag: [[Data Structures & Algorithms]] | [[Interval]]

## Overview

The idea with this algorithm is we will use an events array with elements of the structure `[time, type]` to keep track of currently active events. The `type` property of an event is an enum that represents if an event is starting or ending.

We loop thru the events, checking the type, and incrementing (or decrementing) the number of currently active events.

### Problems:

- [Meeting Schedule II](https://neetcode.io/problems/meeting-schedule-ii)

## References:

[Wiki Link](https://en.wikipedia.org/wiki/Sweep_line_algorithm)
[Medium Article](https://panda-man.medium.com/mastering-efficiency-exploring-line-sweep-algorithm-with-python-673e4522e979#:~:text=The%20Line%20Sweep%20Algorithm%20is%20a%20computational%20technique%20that%20simulates,of%20objects%20in%20the%20plane.)