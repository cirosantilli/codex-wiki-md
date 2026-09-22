<h1 id="1/f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume a negative test identifies the recovered state. Person 1 remains infected through day 7 and recovers during $(7,14]$, so their [interval-censored](../../../../../../../interval-censoring.md) contribution is

$$
P_{II}(7)P_{IR}(7).
$$

Person 2 remains infected through day 7 and makes an exact $I\to D$ transition at day 10. A transition at an exact time contributes a transition probability density, giving

$$
P_{II}(7)P_{II}(3)q_{ID}=P_{II}(10)\mu.
$$

Assuming independent individuals, their joint [likelihood contribution](../../../../../../../likelihood-contribution.md) is

$$
\boxed{P_{II}(7)P_{IR}(7)P_{II}(10)\mu.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [F](../../f.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
