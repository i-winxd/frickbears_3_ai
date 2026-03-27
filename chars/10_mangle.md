# Mangle

- Don't look at Mangle for too long on the cameras.
- Changes position when the camera is lowered. It will never be on the last camera you were on. You can see a sticky note where Mangle is.
- Has an exposure mechanic, increasing by 60 every second (1 per frame) if you are on Mangle's camera.
- Exposure decays over time when not looking at Mangle, but it decays slower the higher the AI, at `(20-AI)/200` per frame. Notice how the decay is **0** at AI 20.
- If exposure exceeds `180-AI*6`, it's a jumpscare. At AI 20, that would be equivalent to looking at Mangle for 1.0 second.