# Springtrap

- `RandomValue` is between 0.75 to 1.25 and is reset every move.
- Moves every `(lerp(42, 12, AI / 20) * RandomValue * 60) + 300;` frames (game runs at 60FPS)
- Flashlight must be held longer at higher AI levels
- Parts and service $\to$ showstage $\to$ left hallway $\to$ left hallway near camera
- Once at left hallway near camera, he cannot be pushed back. At this phase, if your doors are left open for a total of 17 seconds on AI 20, or up to 47 seconds as AI approaches 0, and with some random noise - and that value accumulates and does not reset when your doors are closed, springtrap advances to the kill phase.
- In the kill phase, he jumpscares you after 1 second.

| AI | Movement time |
|----|-------|
| 1 | 45.5 |
| 2 | 44.0 |
| 3 | 42.5 |
| 4 | 41.0 |
| 5 | 39.5 |
| 6 | 38.0 |
| 7 | 36.5 |
| 8 | 35.0 |
| 9 | 33.5 |
| 10 | 32.0 |
| 11 | 30.5 |
| 12 | 29.0 |
| 13 | 27.5 |
| 14 | 26.0 |
| 15 | 24.5 |
| 16 | 23.0 |
| 17 | 21.5 |
| 18 | 20.0 |
| 19 | 18.5 |
| 20 | 17.0 |