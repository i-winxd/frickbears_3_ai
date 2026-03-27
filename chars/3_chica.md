# Bonnie

- Moves every 32 seconds on AI 1; moves every 6.67 seconds on AI 20; actual values are multiplied by a random number between 0.75 to 1.25. Otherwise, these values are linearly interpolated (i.e. every 20s on AI 10).
- Always moves from `ShowStage` $\to$ `DiningArea` $\to$ `Hallway` $\to$ `Doorway`, on the right.
- At your door, a growling sound will play. If Bonnie would move again, it's a jumpscare. If your camera is up 2.5 seconds after Chica arrives at your doorway, it's a jumpscare.
Closing the correct door for 0.5 seconds resets her.

Since Chica, Bonnie, and Freddy calculate movement times in the exact same way, if their AI levels are identical, their arrivals at your doorway should be synced up, and always in expectation. If you've taken stats and know about the central limit theorem, you'll know that it's unlikely this pattern will deviate.
