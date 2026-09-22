<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $x(S)=\sum_{i\in S}x_i$. The [core of a cooperative game](../../../../../core-game-theory.md) is

$$
C(v)=\{x\in\mathbb R^n:x(N)=v(N),\quad x(S)\ge v(S)\text{ for every }S\subseteq N\}.
$$

Take any $x,y\in C(v)$ and $\alpha\in[0,1]$, and form the [convex combination](../../../../../convex-combination.md) $z=\alpha x+(1-\alpha)y$. Its total [payoff](../../../../../payoff.md) is $z(N)=\alpha v(N)+(1-\alpha)v(N)=v(N)$. For every [coalition](../../../../../coalition-game-theory.md) $S$,

$$
z(S)=\alpha x(S)+(1-\alpha)y(S)\ge\alpha v(S)+(1-\alpha)v(S)=v(S).
$$

Hence $z$ remains in the [core](../../../../../core-game-theory.md). **The [core](../../../../../core-game-theory.md) is a [convex set](../../../../../convex-set-split.md)**, even when the [transferable utility game](../../../../../transferable-utility-game.md) is not a [convex cooperative game](../../../../../convex-cooperative-game.md). An empty [core](../../../../../core-game-theory.md) is a [convex set](../../../../../convex-set-split.md) vacuously; the argument does not claim nonemptiness. Geometrically, the same conclusion follows because the constraints intersect an [affine hyperplane](../../../../../affine-hyperplane.md) with [closed half-spaces](../../../../../closed-half-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2022](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
