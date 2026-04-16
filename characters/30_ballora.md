# Ballora

- **Ballora only appears once.**
- You have 90 to 45 seconds to deal with her depending on AI level, linearly interpolated.
- A warning sound effect occurs if you have 10 seconds left.

## One-timer schedule

These always activate in this order:

- Shadow Freddy
- Ballora
- Coffee
- Animdude

Each of them is given a scheduled time.
Here's how the game determines it:

The game starts each night picking a random value between 45 and 60. Let's call that $T_0$.

For Shadow Freddy, then Ballora, then Coffee, then Animdude:

- $T$ = Pick a random value from 60 to 75
- $T_0 = T_0 + T$
- This animatronic spawns at $T_0$ if active

This scales down proportionally the shorter the night. In the challenge "Minute 2 Win It", they become active immediately.