# Freddy

- Moves every 32 seconds on AI 1; moves every 6.67 seconds on AI 20; actual values are multiplied by a random number between 0.75 to 1.25. Otherwise, these values are linearly interpolated (i.e. every 20s on AI 10).
- Path: `ShowStage` $\to$ `DiningArea` $\to$ `Hallway` (Left/right, chosen randomly) $\to$ `Doorway`.
- Freddy laughs when he moves, but **louder** when he moves to `Doorway`.
- The moment he moves to your doorway, he will jumpscare you the next time he would normally move, or if 3 seconds have passed and if your camera is up.
- Closing the correct door for 0.5 seconds will reset him. Try not to close the doors shorter than that.

This may look similar to Bonnie and Chica but there is no 3-second delay when moving.

*Pre-random (this is multipled randomly between 0.75 to 1.25)*

| AI | Movement time |
|----|---------------|
| 1 | 32.00 |
| 2 | 30.67 |
| 3 | 29.33 |
| 4 | 28.00 |
| 5 | 26.67 |
| 6 | 25.33 |
| 7 | 24.00 |
| 8 | 22.67 |
| 9 | 21.33 |
| 10 | 20.00 |
| 11 | 18.67 |
| 12 | 17.33 |
| 13 | 16.00 |
| 14 | 14.67 |
| 15 | 13.33 |
| 16 | 12.00 |
| 17 | 10.67 |
| 18 | 9.33 |
| 19 | 8.00 |
| 20 | 6.67 |
