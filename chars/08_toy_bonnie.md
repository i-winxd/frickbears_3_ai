# Toy Bonnie

- Toy Bonnie has a lure chance of 0.75 and a move speed of 1.15.

## Vent Animatronics

Most vent animatronic logic is shared.

- Vent step time is `lerp(25, 5, AI / 20) * (RandomValue / MoveSpeed);`
  - Where: `lerp(25, 5, AI / 20)` is 25s at AI 0 and 5s at AI 20.
  - `RandomValue` is between 0.75 to 1.1, uniformly.
  - At AI 5, step time is roughly 20 seconds, and at AI 20, it's 5 to 7 seconds.
- The heater stalls all vent animatronics. If on for long enough, it pushes animatronics back vertically (the heater needs to be on for longer if the AI level is higher). Hold the heater, pushback resets if the heater button is released.
- If the animatronic is fooled by the mask, the mask must be on for 1 second.

### Step Movement (Except for Lefty)

- **If the audio lure is adjacent to them:** if the lure chance roll succeeds, their target location will be the audio lure.
- Otherwise: if they are horizontally aligned with an opening to the office, their target location will be one spot down.
- Otherwise: their target location will be horizontal, in the direction of the opening.

Movement:

- When an animatronic actually moves, they may offset their movement horizontally by up to -2 or 2 units, clamped by vent bounds
    - Unless they are on the bottom row, then they will always move to a vent opening, whichever one is closest, or to a random one if they're in the center.
