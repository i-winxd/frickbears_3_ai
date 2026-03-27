# RWQ

- Progression is a product of AI and temperature (temperature below 0 is considered 0).
    - Fades in at a speed of `((1 + (AI / 10)) / 3) * (1 + max(0, global.Temperature / 20));` per frame.
    - Jumpscares when the accumuilated value hits 1.0.

