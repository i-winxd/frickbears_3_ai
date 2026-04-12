# Power

Start with 100.0 power.

Power drains faster if nights are shorter, which mainly impacts custom night:

| Night duration | Lose power this much quickly |
|--------------|-----------------------------|
| 6h | 1.0000 |
| 5h | 1.1500 |
| 4h | 1.3750 |
| 3h | 1.7500 |
| 2h | 2.5000 |
| 1h | 4.7500 |

Power does not drain when you are not using anything.
Otherwise, these contribute to one bar of usage:

- Camera up
- Left door
- Right door
- Flashlight
- Fan

You lose 0.33 power per second per bar of usage.
The table below assumes a 6-hour night length with no early night easing.

| Bars | s to drain 100 | MM:SS |
| ---- | ---- | ---- |
| 0 | $\infty$ | $\infty$ |
| 1 | 303s | 5:03 |
| 2 | 151s | 2:31 |
| 3 | 100s | 1:40 | 
| 4 | 75s | 1:15 |
| 5 | 60s | 1:00 |


If playing on a difficulty easier than Lunatic, during Night 1, you are refunded 20% of your power drain (effectively having 125% power). On Night 2, you are refunded 10% of your power drain (effectively having 111% power).




