# Reflection – Daily Schedule Simulator

## What was your approach to designing the schedule?
Explain how you chose your activities and what made them personal or interesting.
- Using the example code from Mod 7a, I used the approach where an array of elements essentially holds the list of frames. My frame is a schedule view of all of my activities. I used a 'for' loop, where every activity appears after 2 seconds of the previous activity. I used the .innerHTML method to have each subsequent activity build onto the previous one so that it would not simply overwrite the previous value/activity and display only one activity at a time essentially.  

## What was one challenge or unexpected behavior you encountered?
Describe anything surprising that happened when you tested the timing.
- Nothing surprising happened, as each activity was spaced out equally because I had used a 'for' loop.

## What does this assignment teach you about async code?
Compare this to a regular script that runs top to bottom without delays.
- I learned that you can use asynchronous commands to produce synchronous behavior. Because I used my setTimeout function in a 'for' loop, the activities were displayed one after the other without any obvious delay.

## What creative element did you add?
Did you add randomization, surprise content, a twist, or other enhancements?
- I did; within my setTimeout function's parameters, in the 'return'ed function, I made the mood change to 'happy' when I got off of work and until I had to do some more work at night again. 

## How does this project simulate or differ from real-world schedules?
Explain how well your simulation represents how time works in real life.
- While my schedule's content is accurately depicts my real life, I would make several improvements.
First, I would space out the activities appearing based on how much time actually passes in between them.
For example, if 4 hours passes between when I first log into work and when I take my lunch, I would want the 'ms' argument of the setTimeout function to be 4000. If 1.5 hrs passes between when I log out and when I take a shower, I would want the 'ms' argument of the setTimeout function to be 1500. I would do this potentially by taking the difference between the two times of 'this' event and the 'previous' event, then convert that difference into an 'ms' value. 
- I would also try to change the background color to reflect time of day by checking whether the time of the activity falls within a specific range of time during the day.
