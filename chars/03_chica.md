# Bonnie

- Moves every 32 seconds on AI 1; moves every 6.67 seconds on AI 20; actual values are multiplied by a random number between 0.75 to 1.25. Otherwise, these values are linearly interpolated (i.e. every 20s on AI 10).
- Always moves from `ShowStage` $\to$ `DiningArea` $\to$ `Hallway` $\to$ `Doorway`, on the right.
- At your door, a growling sound will play. If Bonnie would move again, it's a jumpscare. If your camera is up 2.5 seconds after Chica arrives at your doorway, it's a jumpscare.
Closing the correct door for 0.5 seconds resets her.

Bonnie and Chica will take 3 seconds to move once they decide to move. This time doesn't count towards anything else. This is considered a transition. Note that Freddy doesn't have this.

Since Bonnie and Chica behave identically, they should arrive at your door at about the same time.

*Pre-random*

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