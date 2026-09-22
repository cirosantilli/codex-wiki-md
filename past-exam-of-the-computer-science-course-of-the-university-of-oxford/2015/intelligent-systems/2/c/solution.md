<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Move the three coins as follows, with $c_1$ smallest:

| Step | Coin | Source | Destination |
| --- | --- | --- | --- |
| 1 | $c_1$ | $s_1$ | $s_3$ |
| 2 | $c_2$ | $s_1$ | $s_4$ |
| 3 | $c_3$ | $s_1$ | $s_2$ |
| 4 | $c_2$ | $s_4$ | $s_2$ |
| 5 | $c_1$ | $s_3$ | $s_2$ |

Every moved coin is exposed, and the last two moves put a smaller coin on a larger one. Thus

$$
\boxed{5<2^3-1=7\text{ moves}.}
$$

Five is also optimal here: before the first move of $c_3$, both smaller coins must leave $s_1$. Neither can make its only move directly to the final destination and remain there, because it would obstruct the eventual arrival of $c_3$. Each smaller coin therefore needs at least two moves. Those four small-coin moves and at least one move of $c_3$ give the matching lower bound.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
