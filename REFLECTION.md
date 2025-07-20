# Reflection – Daily Schedule Simulation

---

## What was your approach to designing the schedule?

I began by imagining what a "normal Mukwaya day" might entail. Instead of being organized like a robot's checklist, I wanted the events to feel genuine. I therefore included relatable elements, such as snoozing while brushing, getting sidetracked and then refocusing, or hitting snooze.

I made an effort to incorporate moods and transitions to give it a sense of life. Additionally, I made the schedule sound like *me*, not like a machine, but like how I would describe my day to a friend.

---

## What was one challenge or unexpected behavior you encountered?

It was more difficult than I anticipated to deal with the lags between events.

Initially, I simply stacked `setTimeout()` calls with fixed times (for example, "do this at 1000ms, the next at 2000ms"). However, because JavaScript operates asynchronously, if I wasn't careful, events would occasionally overlap. It was resolved when I created a `dayProgress` variable to accumulate total time.

---

## What does this assignment teach you about async code?

It effectively illustrates how top-to-bottom code and asynchronous code feel very different.

Everything prints at once in a typical script, but in this case, things happen later and cannot simply "wait" for their turn. The delays occur in real time while JavaScript continues to run. It caused me to consider sequencing and flow more carefully.

Additionally, the story flow can be disrupted by even a minor error, such as placing two timers too close to one another!

---

## What creative element did you add?

Adding the *3:00 PM surprise* with a randomly selected emoji and message was my favorite part. It mimics real life, such as when you unexpectedly feel inspired or experience unpredictable energy spikes. Every "day" feels a little different because the simulation is different each time you run it.

Additionally, adding my name to the log messages made the project feel like it was really mine.

---

## How does this project simulate or differ from real-world scheduling?

It does a great job of capturing **the spirit** of a day, including how events unfold, the pauses between actions, and the impromptu changes in mood. However, it is undoubtedly faster. This driver mimics my day in a matter of seconds rather than sixteen.

Nevertheless, I find it to be a humorous and strangely soothing depiction of time passing. It serves as a reminder that everything deserves a moment, no matter how small.

---


