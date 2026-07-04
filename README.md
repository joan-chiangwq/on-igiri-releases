# Onigiri

*The smallest possible way to keep your Mac awake.*

Onigiri is a tiny macOS menu bar app with exactly one job: keep your Mac
awake when you need it to stay awake. It lives in your menu bar as a little
rice ball. When you need your Mac to stay on, you feed it a coffee. When
you're done, you let it nap.

There are no preferences. No configuration. No modes to learn. Just a cute
companion with one purpose.

---

## How it works

Click the rice ball in your menu bar and a small panel drops down with a
single switch.

**Flip the switch on.** The rice ball perks up — now caffeinated — and your
Mac stays awake. A small green dot confirms it's working.

**Flip the switch off.** The rice ball goes back to resting, and your Mac is
free to sleep normally again.

That's the entire app. You never see a settings screen, because there isn't
one.

| | |
|---|---|
| **Resting** 🍙 | *"Resting... Toggle to wake!"* — switch off, your Mac sleeps normally |
| **Caffeinated** ☕ | *"Caffeinated! Toggle to snooze."* — switch on, green dot, your Mac stays awake |

---

## Installation

**Requirements:** macOS 11 (Big Sur) or later.

### Option 1: Homebrew

```sh
brew tap joan-chiangwq/onigiri
brew install --cask onigiri
```

(First-time install of a new tap may prompt you to run
`brew trust joan-chiangwq/onigiri` — that's Homebrew's tap-trust check, not
an Onigiri-specific step.)

Homebrew installs the app into `/Applications` but — like every Homebrew
Cask — does **not** open it for you. To start it, either:
- Search for "Onigiri" with Spotlight (<kbd>⌘</kbd><kbd>Space</kbd>) and
  press Return, or
- Open it from Finder → Applications.

Once it's running, look for the 🍙 rice ball in your **menu bar** (top right
of the screen) — Onigiri has no Dock icon and opens no window, so that's the
only place you'll see it. Click it to open the popover and flip the switch.
If nothing shows up right after `brew install` finishes, that's expected —
it just means you haven't opened it yet.

### Option 2: Direct download

1. Go to the [latest release](https://github.com/joan-chiangwq/onigiri-releases/releases/latest)
   and download `Onigiri-<version>.dmg`.
2. Open the downloaded `.dmg` — a window appears with the Onigiri icon and a
   shortcut to your Applications folder.
3. Drag **Onigiri** into **Applications**.
4. Open Onigiri from Applications (or search for it with Spotlight,
   <kbd>⌘</kbd><kbd>Space</kbd>).
5. Look for the 🍙 rice ball in your menu bar, top right of the screen —
   that's the whole app. Click it to open the popover and flip the switch.

The app is signed and notarized by Apple, so macOS opens it normally — no
"unidentified developer" warning, no need to right-click and choose Open.

Once installed, Onigiri checks for new versions automatically in the
background and lets you know when one's available — no need to come back
here to redownload it yourself.

---

## Uninstalling

**If you installed via Homebrew:**
```sh
brew uninstall --cask onigiri
```
This removes the app and Homebrew's own install record for it. If you no
longer want the tap either: `brew untap joan-chiangwq/onigiri`.

**If you installed via direct download:**
Quit Onigiri (open the popover → *Quit Onigiri*), then drag `Onigiri.app`
out of your Applications folder to the Trash.

Either way, there's nothing else to clean up — Onigiri keeps no saved
settings or background files.

---

<sub>This repo hosts only the public, signed release artifacts for Onigiri
(DMGs + the Sparkle auto-update feed) — there's no source code here. Issues
and source live in a private repo.</sub>
