# Withered Bonnie

- Appears in your office. Put your mask on when you see him there.

- Enters your office from his initial state after `(1800 / (AI + 10)) * random_range(0.8, 1.2)` frames. The game runs at 60FPS.
- Will wait until Shadow Freddy leaves if active.
- Normally leaves 4 seconds after appearing.
- At AI 0 (for technical reasons), you have 2 seconds of exposure time. At AI 20, you have 1 second. In between, these values are linearly interpolated.
- Exposure time is how long you can have the mask off while he's in your office.
- When the mask is on, exposure won't go up.
- If he would leave but the exposure is too high, he jumpscares you if your mask is not on. If your mask is on, he jumpscares you when you take it off.
