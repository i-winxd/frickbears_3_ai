# Nightmare BB

- Won't appear in the same camera as Mangle.
- Each camera switch or flip, when eligible, may spawn Nightmare BB with a probability of 1/6 (as AI $\to$ 0) to 1/2 (at AI 20)
- Only needs to be clicked when you see him. No need to search for him.
- Won't appear once you've dealt with him in the same camera flip.
- No. of times you must click on him ranges from 3 to 8, linearly, depending on AI level.
- Timer of `lerp(10, 3, AI / 20)` exists until jumpscare the moment he appears. Hitting him gives you one additional second (clamped at the initial window you have). (This means 3s at AI 20)