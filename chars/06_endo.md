# Endo

- Don't use your flashlight if Endo is looking through the window.

- Never appears with Foxy or Dreadbear. If they're already there, Endo will show up immediately after you deal with them.
- After 48 seconds on AI 1 or 10 seconds on AI 20; actual values are multiplied by a random number between 0.75 to 1.25, value being linearly interpolated inbetween (i.e. 30s on AI 10), endo shows up.
- It takes `(120-(AI*3))/60` seconds for Endo to reveal itself. This is the time you have to react.
- Endo is active for `(120+3*AI)/60` seconds. Don't use your flashlight during this time.
- After that, Endo resets.
- **You are given 0.5 to 0.25 seconds of leeway frames (time your flashlight can be on while Endo is up)** depending on AI (0.25 for AI 20).