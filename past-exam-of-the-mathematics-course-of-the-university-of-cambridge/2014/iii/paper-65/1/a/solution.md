<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $C=\mathbb R^n$, the family of proper containing half-spaces is empty and its intersection is, by convention, $\mathbb R^n$. If $C=\varnothing$, every [closed half-space](../../../../../../closed-half-space.md) contains it and their intersection is empty. Now suppose $C$ is a nonempty proper closed [convex set](../../../../../../convex-set.md). Take $x\notin C$ and let $z$ be its [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md). This projection exists: a minimizing sequence can be restricted to a bounded ball, and closedness gives attainment. It is unique by [convexity](../../../../../../convex-function.md) and strict [convexity](../../../../../../convex-function.md) of squared distance.

For $y\in C$, the segment $z+t(y-z)$ remains in $C$ for $0\leq t\leq1$. Minimality at $t=0$ implies

$$
\left.\frac{d}{dt}\|x-z-t(y-z)\|^2\right|_{t=0+}\geq0,
\qquad\langle x-z,y-z\rangle\leq0.
$$

Thus the [closed half-space](../../../../../../closed-half-space.md) $H_x=\{y:\langle x-z,y-z\rangle\leq0\}$ contains $C$ but excludes $x$, since $\langle x-z,x-z\rangle>0$. Every point outside $C$ is excluded by at least one containing half-space. The reverse inclusion is immediate, giving

$$
\boxed{C=\bigcap\{H:H\text{ is a closed half-space and }C\subseteq H\}.}
$$

This is the [half-space representation of a closed convex set](../../../../../../half-space-representation-of-a-closed-convex-set.md). The argument gives an explicit separating hyperplane rather than just citing a [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
