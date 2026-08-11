# MyBI — what's new

Release notes, in the words of the person using MyBI rather than the person who wrote it.
The app reads this file once per version and keeps a copy, so a correction here reaches
everyone on that version without shipping an update.

FORMAT — the app parses this, so the shape matters:

    ## <version>              a release, exactly as it appears in the app (26.1.0, not v26.1)
    ### <section title>       a heading inside that release
    - <note>                  a note everyone sees
    - [windows] <note>        only shown on Windows
    - [mac] <note>            only shown on macOS

Anything outside that shape — this preamble included — is ignored. A release with no
section, or a version the app cannot find, simply shows nothing, which is the right
answer for a release whose notes have not been written yet.

Newest first. Do not edit a published release's notes to describe a later one: people
who already read them keep the copy they were given.

## 26.1.0

### Appearance

- How MyBI looks is one question with one answer now: Light or Dark. The switch in the top bar offers exactly those two, and "Follow this device" has moved to Settings → Personalise, where a preference you set once and forget belongs.
- Grey and OLED Black are palettes rather than separate themes. Apply either while you are in Dark and it repaints the surfaces without turning the lights on — so the look you want stops being tangled up with the mode you are in.
- Dark is built on eigengrau, #16161d. That is the grey your own eyes produce behind closed lids, and so the darkest thing you can actually perceive — which is why it reads as calmer than the pure black a screen is capable of emitting.
- Grey or Gray, following whichever English you are reading.

### Installing on Windows

- MyBI now starts on a Windows PC that has never run it before, without asking you to hunt down a Microsoft component first. Everything it needs travels with the app.

### What's new, kept current

- These notes are fetched once when a version first starts, so a correction reaches you without waiting for another update. They are then kept on your machine and never fetched again.

### Bug fixes and improvements

- Version numbers read the way people say them: a release with no patches shows as 26.1 rather than 26.1.0.

## 26.0.4

### Bug fixes and improvements

- [windows] A repackaged 26.0.3 for the Microsoft Store. Nothing in the app changed — see the 26.0.3 notes for what you actually got.

## 26.0.3

### Shared views

- A shared view keeps its name and its controls in the app's top bar — how it fits the window, its settings and the way out — so the way to close it is always in the same place.
- [windows] The controls for a shared view are no longer hidden behind the app's own bar, so the button that closes it is visible again.

### Recent

- Recent lists dashboards as well as projects, and every row says what it is before it says what it is called.
- A read-only view is marked READ ONLY, and one that asked you for a password says so too.
- Projects can be switched out of the list, so Recent holds just the things you were reading. The choice is remembered.
- Deleting a project takes its dashboards out of the list with it, instead of leaving rows that open nothing.

### Your account

- Setting your name shows up straight away, on the account row and the avatar together — and it survives a restart with no connection.

### Light mode

- The page and the surfaces on it are further apart, so cards, tiles and diagram nodes read on their own rather than leaning on their borders.

### Boot screen

- Matrix rain falls in binary by default, which stays readable at any size on any machine. The original character mix is still there as Text.
- The Auto and Custom backdrops wear marks of their own.

### Tips

- Nine new tips name things the app can actually do — the format painter, the + on the sheet strip, New field, the Page editor chips, cross-filter — in the same words the ribbon uses for them.

### Settings

- Advance options has moved to App settings, under About. Nothing on it was ever about one dashboard, and it now opens with no dashboard open — which is usually when you want it.

### Bug fixes and improvements

- Card actions stay on one row, so Delete never drops onto a line of its own.
- The View menu's Background tick follows the backdrop you picked.
- Empty states draw the app's own marks instead of borrowed characters that changed shape from machine to machine.

## 26.0.2

### Start where you left off

- The Welcome screen now opens on a single Recent list: the projects you opened, the projects you built and the dashboards you read, each marked so you can tell one from another at a glance.
- Everything else you might want to begin sits right underneath, as six equal tiles.

### Open a protected dashboard once, not every time

- Ask MyBI to remember the password for a read-only dashboard and it will open straight away from then on.
- Remembered passwords are held in this device's own secure store and you can look through them or forget any of them whenever you like.

### Your profile, your name

- Set the name you want to be known by, edit your first, middle and family name in place and copy any of them in a tap.
- Signing in with Apple no longer leaves you without a name.

### Bug fixes and improvements

- [mac] Leaving MyBI from full screen is smooth again and a clear Saving indicator shows while your work is put away.
- Light mode reads correctly across the app.
- A steadier launch screen and a tidier status bar.
- [windows] One MyBI build now serves both the Microsoft Store and the download, working out for itself which it is.

## 26.0.1

### The first release

- MyBI brings your spreadsheets and databases together on your own machine, and turns them into dashboards you can read, filter and share.
- Your data stays where you put it. Nothing is uploaded to build a dashboard.
