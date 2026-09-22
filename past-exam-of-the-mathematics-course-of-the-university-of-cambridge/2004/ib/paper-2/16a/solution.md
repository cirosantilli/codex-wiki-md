<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

Define a candidate [antiderivative](../../../../../antiderivative.md) by integration along the straight segment from zero:

$$
g(z)=\int_{[0,z]}f(w)\,dw.
$$

For $z$ in the open unit disc and sufficiently small $h$, the triangle with vertices $0,z,z+h$ lies within the disc, since the disc is convex. By the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md), its boundary [contour integral](../../../../../contour-integral.md) vanishes. Consequently

$$
g(z+h)-g(z)=\int_{[z,z+h]}f(w)\,dw
=h\int_0^1 f(z+th)\,dt.
$$

For $h\ne0$, subtract $f(z)$ after division by $h$. The absolute value of the remainder is at most $\sup_{0\leq t\leq1}|f(z+th)-f(z)|$, which tends to zero by continuity of the [holomorphic function](../../../../../holomorphic-function.md) $f$ at $z$. Hence the complex [derivative](../../../../../derivative.md) exists and **$g'(z)=f(z)$ for every point of the disc**. This proves that $g$ is a [holomorphic function](../../../../../holomorphic-function.md) and supplies the requested primitive directly from the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md).

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
