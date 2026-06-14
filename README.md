# Daily Schedule Planner

A mobile-friendly web app for planning your day by figuring out what time you need to wake up, when to stop working, and when you can go to sleep — based on the activities you want to fit around three fixed anchors: work start time, dinner, and sleep duration.

**Live app:** [https://calrissian45.github.io/daily-planner/](https://calrissian45.github.io/daily-planner/)

## What it does

You enter your fixed anchors (work start, dinner time, sleep hours) and assign activities to one of three free-time blocks. The app calculates:

- **Wake up by** — working backward from work start through your morning activities
- **Bed tonight** — wake-up time minus your target sleep hours; this is when you need to go to sleep tonight
- **Stop work by** — working backward from dinner through your afternoon activities
- **Work available** — hours between work start and stop work
- **Lights out** — dinner time plus your after-dinner activities; the earliest you can go to sleep

All values update instantly as you add, remove, or rearrange activities.

## How to use it

Open the app in any modern browser by visiting the URL above. On Android, open it in Chrome and tap the three-dot menu → **Add to Home screen** to install it as a shortcut on your home screen for quick access.

### Settings (top of the screen)

- **Work starts** — the fixed time you need to begin your workday
- **Dinner** — the fixed time you sit down for dinner; this is the hard cutoff for your afternoon block
- **Sleep (hours)** — your target sleep duration; used to calculate tonight's bedtime
- **Earliest wake-up** — a floor for your wake-up time; if your morning activities require waking earlier than this, the Wake up card turns red as a warning

### Three activity blocks

Activities are assigned to one of three free-time blocks using the buttons on each activity row:

- **AM** — morning block, between wake-up and work start
- **PM** — afternoon block, between stop work and dinner
- **Eve** — after-dinner block, between dinner and lights out
- **Off** — not scheduled

Tap a button to assign the activity to that block. All calculated times update immediately. Activities within a block can be reordered by dragging the grip handle on the left side of each row.

### Presets

**Weightlift**, **Cardio**, and **Rest** buttons load pre-configured activity selections for common day types. After loading a preset you can freely adjust any assignments.

To save your current configuration as a preset, use the **Save current plan as** row — select which preset to overwrite and tap **Save**.

### Schedule tab

The Schedule tab shows your full day as a sequential timeline with a start time for each activity, anchored by the four fixed points (wake-up, work start, stop work, dinner, lights out). Use this view during the day to track whether you are running on time.

### Edit tab

The Edit tab lets you manage your activity list:

- Drag the grip handle to reorder activities in the list
- Tap **A–Z** to sort all activities alphabetically
- Rename any activity or change its duration in minutes
- Delete activities you no longer need
- Add new activities with a name and duration

The **Buffer between activities (%)** setting adds a percentage buffer on top of each activity's duration to account for transition time. At 10%, a 30-minute activity counts as 33 minutes in the schedule.

A 12h/24h time format toggle is at the bottom of each tab.

### Backup and restore

Use **Export** to download a timestamped backup file of your full configuration (activities, durations, presets, and settings). Use **Import** to restore from a previously exported file. This is useful when switching devices or after clearing browser data.

## Data and privacy

All data is saved in your browser's local storage. Nothing is sent to any server. Clearing your browser data will reset the app to its defaults — export a backup first if you want to preserve your configuration.
