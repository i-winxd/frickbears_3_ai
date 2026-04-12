# Lefty

```
MoveSpeed = 1
```

Behaves like any other vent animatronic with these differences:

- Lefty will move in the direction that maximizes the distance from the audio lure.
- Overriding the previous statement, will always move downwards if possible (impossible if the audio lure is directly below it, or is not above an opening if on the bottom row)
- If the lure is placed directly on Lefty, Lefty will move in a completely random possible direction. This means that if Lefty is right above an opening, there is a 1 in 4 chance that Lefy will enter your office.

Otherwise, please refer to [Toy Bonnie's page](./08_toy_bonnie.md) for vent animatronic mechanics. The heater works on Lefty.

The game has an intended mechanic, mentioned in the developer's Tweets and in one of the death hints: if Lefty is in this state (this diagram may be reflected horizontally), he is trapped there forever. If you look at my explainations above, you may be able to figure out why.

```
-----
L----
LA---
```

The audio lure, if not set, is at `[-99, 99]`. Very far to the left, very far down.


