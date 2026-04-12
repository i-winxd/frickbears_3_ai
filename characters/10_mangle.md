# Mangle

- Don't look at Mangle for too long on the cameras.
- Changes position when the camera is **lowered**. It will never be on the last camera you were on. You can see a sticky note where Mangle is.
    - A **shuffled** list of all cameras `[1,2,3,4,5,6,7,8]` is generated on the start of the night and is stepped through each camera flip, skipping cameras where the player is on. Due to this, if Mangle was in a camera, they won't be in it for about the same amount of times you need to get another I-piece in Tetrio, roughly.
- Has an exposure mechanic, increasing by 60 every second (1 per frame) if you are on Mangle's camera.
- Exposure decays over time when not looking at Mangle, but it decays slower the higher the AI, at `(20-AI)/200` per frame. Notice how the decay is **0** at AI 20 (meaning it's permanent).
- If exposure exceeds `180-AI*6`, it's a jumpscare. At AI 20, that would be equivalent to looking at Mangle for 1.0 second.