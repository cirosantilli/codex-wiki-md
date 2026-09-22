<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Choose a star centre $a$ of the open [star-shaped set](../../../../../star-shaped-set.md) $D$ and define the candidate [antiderivative](../../../../../antiderivative.md) by a straight-segment [contour integral](../../../../../contour-integral.md):

$$
F(z)=\int_{[a,z]}f(\zeta)\,d\zeta.
$$

For each fixed $z\in D$ and all sufficiently small $h$, the filled [triangle](../../../../../triangle.md) with vertices $a,z,z+h$ lies in $D$. Indeed, the [compact](../../../../../compact-space.md) segment $[a,z]$ has a neighbourhood of some positive radius contained in the open set $D$, and every point of this [triangle](../../../../../triangle.md) lies within $|h|$ of that segment. The zero [triangle](../../../../../triangle.md) integral consequently gives

$$
F(z+h)-F(z)=\int_{[z,z+h]}f(\zeta)\,d\zeta
=h\int_0^1f(z+th)\,dt.
$$

By [continuity](../../../../../continuous-function.md), the last integral tends to $f(z)$ as $h\to0$. Hence

$$
\boxed{F'(z)=f(z)\quad(z\in D)}.
$$

In particular, this proves the existence of the [antiderivative](../../../../../antiderivative.md) without incorrectly assuming the [star-shaped set](../../../../../star-shaped-set.md) is [convex](../../../../../convex-function.md).

On a general [domain](../../../../../domain-mathematical-analysis.md), **the conclusion can fail**. Take $D=\mathbb C\setminus\{0\}$ and $f(z)=1/z$. Every filled [triangle](../../../../../triangle.md) contained in $D$ has zero boundary integral by [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md), but the unit [circle](../../../../../circle.md) has integral $2\pi i$. An [antiderivative](../../../../../antiderivative.md) would make every closed [contour integral](../../../../../contour-integral.md) zero. This is the [period obstruction to a holomorphic antiderivative](../../../../../period-obstruction-to-a-holomorphic-antiderivative.md): the local conclusion of [Morera's theorem](../../../../../morera-s-theorem.md) does not remove the global obstruction.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
