<h1 id="2f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The planar [Brouwer fixed-point theorem](../../../../../../brouwer-fixed-point-theorem.md) says that every continuous map from the closed disk $D$ to itself has a [fixed point](../../../../../../fixed-point.md). If a [retraction](../../../../../../retraction.md) $r:D\to\partial D$ existed, $x\mapsto-r(x)$ would be a continuous self-map of $D$. At a [fixed point](../../../../../../fixed-point.md) $x=-r(x)$, $x$ lies on the boundary, where $r(x)=x$; this would give $x=-x$, impossible on the unit circle.

Conversely, suppose a continuous self-map $f:D\to D$ has no [fixed point](../../../../../../fixed-point.md). For each $x$, take the ray starting at $f(x)$ through $x$, and let $r(x)$ be its exit point on $\partial D$. The denominator $|x-f(x)|$ never vanishes, and solving the quadratic intersection with the circle shows that the exit point depends continuously on $x$. More explicitly, with $v=x-f(x)$,

$$
r(x)=f(x)+\lambda(x)v,\qquad \lambda(x)=\frac{-f(x)\cdot v+\sqrt{(f(x)\cdot v)^2+(1-|f(x)|^2)|v|^2}}{|v|^2}.
$$

The ray exits beyond or at $x$, so $\lambda\ge1$, and when $x\in\partial D$ its exit point is $x$. Hence $r$ is a [retraction](../../../../../../retraction.md). **Nonexistence of a boundary retraction and the planar fixed-point theorem are equivalent.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2F](../../2f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
