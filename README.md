# Daily Schedule Planner

A mobile-friendly web app for planning your day by figuring out what time you need to wake up, when to stop working, and when you can go to sleep — based on the activities you want to fit around three fixed anchors: work start time, dinner, and sleep duration.

**Live app:** [https://calrissian45.github.io/daily-planner/](https://calrissian45.github.io/daily-planner/)

## What it does

You enter three fixed anchors (work start, dinner time, sleep hours) and assign activities to one of three free-time blocks. The app calculates eight values arranged in chronological order:

- **Bed (night before)** — the latest you can go to sleep the night before to get your target sleep hours
- **Sleep** — your target sleep duration (editable)
- **Wake up by** — working backward from work start through your morning activities
- **Work starts** — your fixed work start time (editable)
- **Work available** — hours between work start and stop work
- **Stop work by** — working backward from dinner through your afternoon activities
- **Dinner** — your fixed dinner time (editable)
- **Bed (night after)** — the earliest you can go to sleep after completing your after-dinner activities

Editable values are shown in green — tap any green card to edit it. All calculated values update instantly as you add, remove, or rearrange activities.

## How to use it

Open the app in any modern browser by visiting the URL above. On Android, open it in Chrome and tap the three-dot menu → **Add to Home screen** to install it as a shortcut on your home screen for quick access.

## Three activity blocks

Activities are assigned to one of three free-time blocks using the buttons on each activity row:

- **AM** — morning block, between wake-up and work start
- **PM** — afternoon block, between stop work and dinner
- **Eve** — after-dinner block, between dinner and bed
- **Off** — not scheduled

Tap a button to assign the activity to that block. All calculated values update immediately. Activities within a block can be reordered by dragging the grip handle on the left side of each row.

## Tabs

### Plan tab

The main planning view. Shows the activity blocks and all scheduled/unscheduled activities. Use this to set up your day by assigning activities to blocks.

At the top, preset buttons let you load a saved day configuration with one tap. The app opens on whichever tab you were last using.

### Schedule tab

Shows your full day as a sequential timeline with a start time listed for each activity, anchored by the four fixed points: wake-up, work start, stop work, dinner, and bed (night after). Use this view during the day to track whether you are running on time.

### Edit tab

Manage your activity list:

- Drag the grip handle to reorder activities in the list
- Tap **A–Z** to sort all activities alphabetically
- Rename any activity or change its prep or duration time
- Delete activities you no longer need
- Add new activities with a name, prep time, and duration

## Prep time and duration

Each activity has two time fields:

- **Prep** — time needed to transition to or set up for the activity before it begins (e.g. getting to the gym, setting up equipment). Defaults to 0.
- **Dur** — the actual duration of the activity itself.

The total time consumed by an activity is Prep + Duration. In the plan view, activities with prep time show as `5+90m` (prep + duration). In the schedule view, the breakdown is shown explicitly.

## Presets

Preset buttons at the top of the Plan tab let you load a saved activity configuration for common day types with one tap. After loading a preset you can freely adjust any assignments.

Preset management is in the settings section at the bottom of the Plan tab:

- **Rename** a preset by editing its name field
- **Update** a preset to overwrite it with the current plan
- **Delete** a preset with the trash icon
- **Add** a new preset by typing a name and tapping **Save plan**

## Settings

Settings are at the bottom of each tab:

- **Font size** — tap + or − to increase or decrease text size across the whole app, from 11px to 22px
- **Time format** — toggle between 12h and 24h display; applies to all times in the app including input cards
- **Backup / restore** — Export downloads a timestamped JSON backup of your full configuration; Import restores from a previously exported file
- **Manage presets** — add, rename, update, and delete presets (Plan tab only)

## Data and privacy

All data is saved in your browser's local storage. Nothing is sent to any server. Clearing your browser data will reset the app to its defaults — export a backup first if you want to preserve your configuration. The app remembers your last active tab, font size, time format, activities, durations, prep times, and presets between sessions.
