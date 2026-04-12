# Funtime Freddy

`RandomValue` always between 0.8 and 1.2 and is uniform, and is regenerated after attacking.

There are three states: `Waiting`, `Hallway`, and `Attacking`.

- `Waiting` is the initial phase. Funtime Freddy spends `lerp(60,20,AI/20)*RandomValue` seconds in this phase, which means 60 seconds when AI level approaches 0, and **20 seconds when AI approaches 20**, with some randomness added.
- `Hallway` is his hallway phrase. He spends 20 seconds when AI is 0 and **8 seconds when AI is 20**, in this phase. This value is **not** randomized, unlike the hallway wait time.
- Afterwards, he transitions to the `Attack` phase. He announces the attack.
- After Funtime Freddy announces an attack (audio file is finished playing), the game, every frame does this:
    - If the correct door is closed and the other one isn't, this plays a sound and resets Funtime Freddy. He will not appear in the hallway anymore until he does again.
    - If both doors are closed, nothing happens, which means his state won't change. You must open the door the attack isn't happening on to reset him.
    - If the correct door isn't closed, a jumpscare occurs.
- For all his voicelines, the sound is panned.

Voicelines:

- Hallway
    - `*Laughter*`
    - `*Vocalizing*`
    - Hey! Hey! Over here.
- Attack, same side exclusive
    - Let's give the birthday boy a big hug
    - Ready or not, here I come
- Attack, opposite side exclusive
   - Get ready for a surprise!
   - Take it away, Bon-bon!
- Attack, either side
    - Time to blow out the candles
    - Hey, check this out
    - Wanna see something cool?

All possible voicelines are chosen randomly. This means, on attacking, there is a 60% chance Funtime Freddy's voice won't reveal which side the attack will happen.


