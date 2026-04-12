# Frickbear 3 Animatronic AI Deconstructions

Tags: Five Nights at Frickbear's 3, Wiki

These are datamined from Five Nights at Frickbear's 3. https://gamejolt.com/games/frickbears3/930477

Feel free to copy-paste this into any Wiki you like. While this is mostly accurate, beware of mindslips. I am not responsible if you follow what happens to be misinformation.

This assumes you know what the animatronics do based on their descriptions.

This is accurate as of the last commit time.

**AI values are linearly interpolated unless mentioned otherwise. When I say: $A$ on AI 0 and $B$ on AI 20, think of drawing a number line with endpoints $A$ and $B$, and using AI out of 20 as a percentage of where on that line segment the value should be on**. To calculate that value for AI $K$, it's: $A+(B-A)K$ For example, for AI level 10, just average the two extremes out. There may be some uncertainty if I mention AI 1 instead. Since an animatronic is disabled on AI 0, I might say "as their AI approaches 0."

**All randomized values follow a uniform distribution.**

**When I say: A to B depending on AI**, I implicitly mean A on AI 0 and B on AI 20.

Spoilers!!!!
