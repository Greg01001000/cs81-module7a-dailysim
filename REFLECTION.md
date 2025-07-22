### CS 81 Module 7 Assignment 7B: Daily Schedule Async Simulator, by GregH, 7/21/25

# Reflection – Daily Schedule Simulator

## What was your approach to designing the schedule?
##### Explain how you chose your activities and what made them personal or interesting.
In most weeks, my most fun and interesting day is the day that I do ministry work and go to our Bible meeting. Those are also the most important activities that I do, and they are usually family activities. So I used my typical activities on that day.

## What was one challenge or unexpected behavior you encountered?
##### Describe anything surprising that happened when you tested the timing.
At first, I wrote the code incorrectly, not using '.then()' to connect all the activities in a chain. So of course all the activities appeared on the web page at once. I assume all their Promise timers were running asynchronously. When I figured out how to chain the activities using '.then()', they behaved as I expected.

## What does this assignment teach you about async code?
##### Compare this to a regular script that runs top to bottom without delays.
By connecting two or more actions with '.then()', we can make sure that some action doesn't happen until a previous action is complete, whether the previous action is a timed delay, a response from a user or another computer, or something else.

A synchronous script without delays would display all the activities so fast (because computers are so fast) that they would seem to appear simultaneously, ruining the perception of separate events happening over a period of time.

## What creative element did you add?
##### Did you add randomization, surprise content, a twist, or other enhancements?
For my last activity before getting ready for bed, I coded a 50% chance of either doing schoolwork or watching a movie.

## How does this project simulate or differ from real-world schedules?
##### Explain how well your simulation represents how time works in real life.
In the simulation, I can change the amount of time an activity takes just by changing a number in my code. I can set the numbers to realistically mimic typical actual amounts of time that various activities have taken in the past. (I never actually tested that; I always used much shorter intervals, to save time. I watched a stopwatch a few times while watching the output, and as far as I could tell, the actual output intervals, according to my stopwatch, matched what I specified in my code.) I wish it were that easy in real life to control how long an activity takes. But real life activities never take the exact amount of time expected, down to the millisecond. In reality, we have to keep working effectively at something, or waiting for something beyond our control, before we can reasonably consider an activity to be finished. And that is the more important application of asynchronous code--to keep working at or waiting for something to be completed, before attempting an action whose success depends on the completion of that previous action, and possibly to be more efficient and/or improve the user's experience by working on and/or waiting for multiple actions simultaneously.