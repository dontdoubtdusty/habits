# Big Healthy Habits

Stretch routines, an interval timer, breathing exercises, water and medication check-offs. It's part of the Big apps, alongside [Big Minty Finances](https://github.com/dontdoubtdusty/budget), [Big Saucy Recipes](https://github.com/dontdoubtdusty/cooking), [Big Skinny Health](https://github.com/dontdoubtdusty/diet), [Big Tidy Reminders](https://github.com/dontdoubtdusty/reminders) and [Big Shiny Rounds](https://github.com/dontdoubtdusty/cleaning). It's one file (`index.html`) with no build step and no server.

## Features

- Three tabs: **Today** for what's due today, **Move** for stretch, interval and breathing routines, and **Meds** for your medications
- Routines on **Move**, grouped into Stretch, Intervals and Breathing, with starter routines to begin with (Morning stretch, Desk break, Intervals 30/15, Box breathing and 4-7-8 breathing)
- Edit any routine: its name, kind, number of rounds, and steps with their seconds. Drag steps to reorder, and delete with Undo. Make your own with **New routine**.
- A full-screen player for every routine: a 5-second get-ready, a countdown ring, the next step, round count, pause, skip and back. Beeps mark each new step and the last 3 seconds. The screen stays awake while it plays, but if you lock the phone the browser may pause it.
- Breathing routines show a soft circle that grows as you breathe in, holds still, and shrinks as you breathe out, with a gentle tone at each change instead of countdown beeps
- Finished routines show under **Recently** on the Move tab
- Medications on **Meds**: name, dose and one or more times a day, edited in place, with drag to reorder and Undo on delete
- Today's doses on **Today** in time order: tick each one off as you take it, see when you took it, and spot missed ones by their **Due** tag
- While the app is open, a pop-up tells you when a dose comes due. It can't alert you when the app is closed, so keep a phone alarm for anything you can't miss.
- Water tracking on **Today**: tap a glass for each one you drink, with a progress bar toward your daily goal (8 glasses unless you change it under **Settings > Daily water goal**)
- Light, dark and automatic themes, plus a Day/Night option that switches to dark at 6pm and back to light at 6am
- Light haptic ticks when you save, delete, finish or toggle something, and buttons that visibly press in on every tap. Turn haptics off under **Settings > Haptics**.
- Backups you can share, download and import, with a weekly reminder
- Optional sync across devices with an email sign-in

## Using it

Turn on GitHub Pages for this repo (**Settings > Pages > Deploy from a branch > `main` / root**) and open the link it gives you. You can also open `index.html` straight from your computer, but installing and offline use only work from the GitHub Pages link.

### Install it as an app

- **iPhone or iPad (Safari):** tap Share, then **Add to Home Screen**.
- **Android (Chrome):** tap the menu, then **Install app** (or **Add to Home screen**).
- **Computer (Chrome or Edge):** click the install icon at the right end of the address bar.

Once it's installed, it opens full screen with its own icon and works without an internet connection.

### Files

| File | What it does |
| --- | --- |
| `index.html` | The whole app |
| `sync.js` | Optional sync across devices (shared by all the Big apps) |
| `feedback.js` | Haptic ticks and button press feedback (shared by all the Big apps) |
| `manifest.webmanifest` | The app's name, colors and icons, used when it's installed |
| `sw.js` | Saves a copy of the app so it opens offline |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | The app icon at each size browsers and phones ask for |

**When you update the app:** nothing extra to do. The app always checks for a newer copy first and only falls back to the saved one when you're offline.

## Your data

Everything you enter is saved in your browser's `localStorage` on your device, and none of it is stored in this repository.

Each website address keeps its own separate storage, so your data doesn't follow you to a new address or device by itself. On iPhone, the home-screen app also keeps separate storage from the same page opened in Safari. Two ways to move it:

- **Backup:** go to **Settings > Share backup** (or **Download backup**) in the old place, then **Import backup file** in the new one.
- **Sync:** sign in under **Settings > Sync across devices** on each device. Your data is then also kept in the Big apps' Firebase database under your account. Sync is off until you sign in.

## Credits

The fonts are [Fredoka](https://fonts.google.com/specimen/Fredoka) and [Nunito](https://fonts.google.com/specimen/Nunito), loaded from Google Fonts.
