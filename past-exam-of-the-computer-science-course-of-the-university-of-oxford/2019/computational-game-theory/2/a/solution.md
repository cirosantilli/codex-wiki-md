<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p$ be the row player's [probability](../../../../../probability.md) of $T$. Its [expected payoffs](../../../../../expected-payoff.md) against $L$ and $R$ are $6-5p$ and $2+p$. The [security level payoff](../../../../../security-level-payoff.md) is therefore

$$
\max_{0\leq p\leq1}\min\{6-5p,2+p\}.
$$

The first line decreases and the second increases, so their intersection is optimal: $6-5p=2+p$ gives $p=2/3$. Hence

$$
\boxed{\text{Security level }=8/3,\qquad\Pr(T)=2/3,\quad\Pr(B)=1/3.}
$$

The two column actions then give the same [expected payoff](../../../../../expected-payoff.md), so an opposing [mixed strategy](../../../../../mixed-strategy.md) cannot reduce it further.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
