<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose one plane requiring the longest runway and assign it the entire cost $c(N)$; assign every other plane zero. These nonnegative payments sum to $c(N)$. Any [coalition](../../../../../coalition-game-theory.md) containing that chosen plane also requires the whole longest runway, so its payment is exactly its standalone cost. Any coalition without it pays zero, which is at most its nonnegative standalone cost.

Hence **this payment vector is in the cost core**, proving the desired sharing always exists. This is an existence certificate, not a fairness assertion. If there are no planes, the empty allocation has total zero. The [Shapley value of an airport game](../../../../../shapley-value-of-an-airport-game.md) gives a more symmetric sharing rule and also lies in the [core](../../../../../core-game-theory.md) of this [cooperative cost game](../../../../../cooperative-cost-game.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
