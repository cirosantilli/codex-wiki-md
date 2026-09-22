<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

The [Brouwer fixed-point theorem](../../../../../brouwer-fixed-point-theorem.md) says that every [continuous map](../../../../../continuous-map.md) from a closed Euclidean ball to itself has a [fixed point](../../../../../fixed-point.md). For the closed disc $D\subset\mathbb R^2$ its equivalent [no-retraction theorem](../../../../../no-retraction-theorem.md) says that there is no continuous $r:D\to\partial D$ satisfying $r(z)=z$ on $\partial D$.

Assume the fixed-point theorem and suppose such a [retraction](../../../../../retraction.md) exists. Then $F(x)=-r(x)$ maps $D$ continuously into itself. A [fixed point](../../../../../fixed-point.md) must lie on the boundary, where $r(x)=x$, giving $x=-x$, impossible on the unit circle.

Conversely suppose $F:D\to D$ is continuous and has no [fixed point](../../../../../fixed-point.md). From $F(x)$ draw the ray through $x$ and let $r(x)$ be its exit point on the circle. To check [continuity](../../../../../continuous-function.md) rather than merely relying on the picture, put $v=x-F(x)\ne0$. The exit point is $F(x)+t(x)v$, where

$$
t(x)=\frac{-F(x)\cdot v+\sqrt{(F(x)\cdot v)^2+(1-|F(x)|^2)|v|^2}}{|v|^2}.
$$

This is continuous, lies on the circle and has $t(x)\geq1$. On the boundary the exit point is $x$, so $r$ is a [retraction](../../../../../retraction.md), contradicting the assumed theorem. Hence **the two disc formulations are equivalent**; the same argument works for a ball in any dimension.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
