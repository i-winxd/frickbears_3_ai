# Endo Chaser

This applies for all states. In order to see the player:

- You can draw a ray between the player and the Endo without it colliding with anything else (preventing the endo chaser from aggroing if it's behind a wall), **AND**
    - The player is in the endo's sight angle (25 deg both directions) and is at a distance of 512 units, **OR**
    - The player is at a distance to the endo that is lower than the loudness the player is making.
        - Loudness is proportional to the **square** of the player's movement speed.


The endo starts in the `Wander` state. It finds a random patrol point and makes a path to it.

When the endo sees the player, it starts chasing. It speeds up by 10x, increases its sight angle to 45 (both direcctions) and runs to where it saw you the last (this updates as long as it can see you).

If the Endo reaches the place where it can see you (where obviously you aren't there or you are jumpscared), it pauses for 1 second. If it sees you again, it starts chasing you again.

After the 1-second pause, it resets to the wandering state and resets the sight angle.
