<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Where its denominator is nonzero, normalization enforces **[cooperative-game efficiency](../../../../../efficiency-of-a-cooperative-game-value.md)** and preserves **[cooperative-game symmetry](../../../../../symmetry-of-a-cooperative-game-value.md) and the [null player](../../../../../null-player.md) axiom**. The violated axiom is **[cooperative-game additivity](../../../../../additivity-of-a-cooperative-game-value.md)**.

For an exact counterexample on three players, let $v$ be the majority game, and let $w$ be the dictatorship in which a [coalition](../../../../../coalition-game-theory.md) wins precisely when it contains player one. Their [probabilistic Banzhaf indices](../../../../../probabilistic-banzhaf-index.md) are

$$
\beta(v)=(1/2,1/2,1/2),\qquad\beta(w)=(1,0,0),
$$

with $v(N)=w(N)=1$. Hence

$$
\beta'(v)=(1/3,1/3,1/3),\qquad\beta'(w)=(1,0,0).
$$

Unnormalized indices add, so $\beta(v+w)=(3/2,1/2,1/2)$. Their [sum](../../../../../sum.md) is $5/2$, while $(v+w)(N)=2$. Therefore

$$
\boxed{\beta'(v+w)=(6/5,2/5,2/5)\ne(4/3,1/3,1/3)=\beta'(v)+\beta'(w).}
$$

The sum game is a valid [transferable utility game](../../../../../transferable-utility-game.md), although it is not binary; that is the natural domain of the additivity axiom. The failure comes from a game-dependent scaling factor. A zero denominator, as for the zero game, makes the displayed normalization undefined unless a separate convention is supplied; none of the counterexample's denominators vanish.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
