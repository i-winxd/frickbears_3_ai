# Toy Bonnie

- Toy Bonnie has a lure chance of 0.75 and a move speed of 1.15.

## All Vent Animatronic Stats

| Animatronic | Move speed | Audio Lure Chance | Heater pushback |
| --- |--- |--- |--- |
| Withered Chica | 0.80 | 0.25 | 0.75 |
| Toy Bonnie | 1.15 | 0.75 | 1.0 |
| JJ | 0.5 | 1.0 | 0.0 |
| Mr Hippo | 1.0 | 0.5 | 1.0 |
| Lefty | 1 | N/A | 1 | 

## Basic Vent Animatronics

The vent layout is like this:

```
  X -2 -1  0  1  2
 Y
-1   O  O  O  O  O
 0   O  O  O  O  O
 1   O  O  O  O  O
 2      |     |
```

The openings are the ones in your office, which you can see. If an opening is already occupied and a vent animatronic would have moved to it, they move to the opposite one.

## Movement

Where `RandomValue` is from 0.75 to 1.25, rerolled each time a move occurs for each animatronic:


As AI approaches 0, the **base** wait time is 25 seconds. At AI 20, it is 5 seconds.

This is then **divided** by the move speed and multiplied by `RandomValue`. Meaning:

```
WaitTime = lerp(25, 5, AI/20) * (RandomValue / MoveSpeed)
```

### Audio Lure

The audio lure is only effective if the lure is placed in an adjacent vent or is on top of them.

```
  X
X A X
  X
```

Each animatronic has a lure chance. That is the probability, each time they move, and if the audio lure is adjacent, they will be fooled by the lure. If this roll succeeds, they are immediately moved to the lure position.

<!-- TODO: Does standard movement noise apply? -->

### Standard Movement

Each vent animatronic has an X-axis target they will always move to. This only rerolls if they are on the bottom, are fooled by the audio lure, or if they are already on the target.

If they aren't at this target, without the effects of the audio lure, they will move horizontally towards it, one step at a time.

If they were to move and the X-target is met, they move **downwards** and pick a new X-target.

The X-target is always above either opening if they are on the bottom. Otherwise, it is random.

When they are reset, they are pushed to the top and at a random X-coordinate. Their X-target is also effectively reset.

### Masking

- An audio cue plays when an animatronic enters the vent opening in your office.
- You have 6 seconds + `WaitTime/5` to put your mask on once they arrive. This means that this window is weakly tied to their AI level, although that addition is usually around a second or less at high AI levels.
  - This time doesn't tick when your mask is on.
- The mask is ineffective for the first second an animatronic appears in your vent opening.
- You need to mask for 2 seconds. For every second you don't mask, you need to mask an additional 0.25 seconds.
- The duration you need to mask is not impacted by their AI level.

### Heater

The heater stalls all vent animatronics. If on for long enough, it pushes animatronics back vertically (the heater needs to be on for longer if the AI level is higher). Hold the heater, pushback resets if the heater button is released.
