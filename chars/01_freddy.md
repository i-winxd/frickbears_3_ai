# Freddy

- Moves every 32 seconds on AI 1; moves every 6.67 seconds on AI 20; actual values are multiplied by a random number between 0.75 to 1.25. Otherwise, these values are linearly interpolated (i.e. every 20s on AI 10).
- Path: `ShowStage` $\to$ `DiningArea` $\to$ `Hallway` (Left/right, chosen randomly) $\to$ `Doorway`.
- Freddy laughs when he moves, but **louder** when he moves to `Doorway`.
- The moment he moves to your doorway, he will jumpscare you the next time he would normally move, or if 3 seconds have passed and if your camera is up.
- Closing the correct door for 0.5 seconds will reset him. Try not to close the doors shorter than that.

Since Chica, Bonnie, and Freddy calculate movement times in the exact same way, if their AI levels are identical, their arrivals at your doorway should be synced up, and always in expectation. If you've taken stats and know about the central limit theorem, you'll know that it's unlikely this pattern will deviate.
