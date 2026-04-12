# Withered Bonnie

- Appears in your office. Put your mask on when you see him there.

- Enters your office from his initial state after `(1800 / (AI + 10)) * random_range(0.8, 1.2)` seconds. The game runs at 60FPS.
- Will wait until Shadow Freddy leaves if active.
- Normally leaves 4 seconds after appearing.
- At AI 0 (for technical reasons), you have 2 seconds of exposure time. At AI 20, you have 1 second. In between, these values are linearly interpolated.
- Exposure time is how long you can have the mask off while he's in your office.
- When the mask is on, exposure won't go up.
- If he would leave but the exposure is too high, he jumpscares you if your mask is not on. If your mask is on, he jumpscares you when you take it off.


*Before being multipled by random 0.75 to 1.25*

| AI | Wait time |
|----|------------------|
| 1 | 163.6364 |
| 2 | 150.0000 |
| 3 | 138.4615 |
| 4 | 128.5714 |
| 5 | 120.0000 |
| 6 | 112.5000 |
| 7 | 105.8824 |
| 8 | 100.0000 |
| 9 | 94.7368 |
| 10 | 90.0000 |
| 11 | 85.7143 |
| 12 | 81.8182 |
| 13 | 78.2609 |
| 14 | 75.0000 |
| 15 | 72.0000 |
| 16 | 69.2308 |
| 17 | 66.6667 |
| 18 | 64.2857 |
| 19 | 62.0690 |
| 20 | 60.0000 |