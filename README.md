# Daily Schedule Planner

A mobile-friendly web app for figuring out what time you need to wake up and stop working based on the activities you want to fit into your day.

## What it does

You set a fixed work start time and dinner time, then select which activities you want to accomplish before work (morning block) and after work before dinner (evening block). The app calculates:

- **Wake up by** — the latest you can wake up and still complete your morning activities before work
- **Bedtime** — what time you need to go to bed the night before to get your target sleep hours
- **Stop work by** — the latest you can finish work and still complete your evening activities before dinner
- **Work available** — how many hours you have between work start and stop work times

All times update instantly as you add or remove activities.

## How to use it

### Settings (top of the screen)
- **Work starts** — the time you need to be at work or starting your workday
- **Dinner** — the time you want to sit down for dinner; this is the hard stop for your evening block
- **Sleep (hours)** — how many hours of sleep you want; used to calculate your bedtime
- **Earliest wake-up** — a floor on your wake-up time; if your morning block requires waking up earlier than this, the wake-up card turns red as a warning

### Assigning activities
Each activity has three buttons: **AM**, **PM**, and **Off**.
- **AM** — schedules the activity in your morning block (before work)
- **PM** — schedules the activity in your evening block (after work, before dinner)
- **Off** — removes it from both blocks

Tap the button for the block you want. The wake-up and stop-work times update immediately. If the required wake-up is earlier than your earliest wake-up floor, the card turns red — you can then move activities to the evening block or remove them entirely.

Activities in the morning and evening blocks can be reordered by dragging the grip handle on the left.

### Presets
The **Weightlift**, **Cardio**, and **Rest** buttons load pre-configured activity selections for common day types. After loading a preset you can freely adjust which activities are assigned.

To save your current morning/evening configuration as a preset, use the **Save current plan as** row — select which preset to overwrite and tap **Save preset**.

### Editing activities
The **Edit activities** tab lets you:
- Rename any activity
- Change its duration in minutes
- Delete activities you don't need
- Add new activities with a custom name and duration

The **Buffer between activities (%)** setting adds a percentage on top of each activity's duration to account for transition time between activities. At 10%, a 30-minute activity is counted as 33 minutes.

### Time format
A 12h/24h toggle is available at the bottom of each tab.

## Data and privacy
Everything is saved locally in your browser's storage. No data is ever sent to a server. Clearing your browser data will reset the app to its defaults.

For the best experience on Android, open the app in Chrome and use the three-dot menu → **Add to Home screen** to install it as a shortcut.
