# Dev Log
## Day 0
### Afternoon
After reviewing the specification and sample code, I gave Conor an estimate of four working days (Tuesday).

It should take about 2-2.5 days of dev time at max.

The unit tests will take some extra time. I'll need to look at how to implement them for a static application. The unpkg scripts should be able to help.

I started off by planning and breaking down the requirements on my Trello board. Then, I created a git repository to track progress.

I will begin development tomorrow.

### Evening
Conor spoke with Andrew, and passed on a request that the code challenge be completed by Monday 12pm. I said this was possible, and that there would not be time for unit tests as a result.

The focus from here on out is to provide a complete solution as per the documented requirements.

## Day 1
### Morning
I decided to use the pomodoro technique/Chrome extension to best manage my time while working on this coding challenge.

For context, one pomodoro is about 25-30 minutes, and then I take a 5-15 minute break depending on the schedule.

It took about 1.5 hours in the morning to implement responsive styles. I knew I had to use media queries, but ran into a couple of issues.

Here's what I learnt:
- In vanilla CSS, media queries cannot be used within classes. They must be implemented on the root level, compared to CSS preprocessors (Emotion, Sass) that allow queries to be written inside classes.
- A meta tag specifying the viewport and device-width was required. However, when I copy/pasted it, I didn't realise that it came across as the wrong style of quote (” instead of "). This is just another of those instances where something small went wrong and it just needed a pair of fresh eyes after a break to resolve.

### Lunchtime
I refactored the styles from flex to grid as there was an issue with more white space on the right-hand side. I also added the checkboxes and the first draft of the bulk edit overlay. WIP.

I took some time to answer the questions, too. Now I need to attend a doctor's appointment, so I will resume working in the afternoon.

### Late afternoon
I've started to implement the logic, and began by converting the default state definition to the React.useState format. After that, I added React.useEffect to monitor when the bulk edit popup should be shown.

Over the course of the day, I completed 8 pomodoros, or roughly four hours of work. I would've accomplished a little more if I didn't need to head out, but I have plenty of time tomorrow to finish the project.

## Day 2
### Morning
I was thinking about the easiest way to handle the bulk edit functionality and the answer came to me in the form of a callback function. Knowing exactly what I needed to do, I made the change this morning.

However, the item checkboxes weren't linked to the selected state, so they weren't clearing. Found an easy fix by mapping "checked" to the item "selected" property, and added some more feedback for the users via hover states and a selected item count.

I was also able to complete the logic for hiding and showing the buttons, reviewed my answers to the questions, and refactored the way the item id is handled. Finally, I ran the code through the Prettier online formatter.

I'm really happy that I was able to complete the work this morning within four pomodoros (2 hours). Last steps are to format this log on Google Docs and send it all through to Matt.

### Lunchtime
I opted to create a README.md document and place the questions and dev log all in one place.
