<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [stability function](../../../../../../stability-function.md) $R(z)=(z^2+6z+12)/(z^2-6z+12)$. Its denominator vanishes only at $3\pm i\sqrt3$, both in the open right half-plane. For $z=x+iy$,

$$
|z^2-6z+12|^2-|z^2+6z+12|^2
=-24x(|z|^2+12).
$$

This is nonnegative whenever $x\leq0$, so $|R(z)|\leq1$ throughout the closed left half-plane. The internal stage equations are also solvable there, since $\det(I-zA)=1-z/2+z^2/12$. Therefore **the method is [A-stable](../../../../../../a-stability.md)**.

The inequality is strict in the open left half-plane, while $|R(iy)|=1$. Moreover $R(z)\to1$ as $|z|\to\infty$, so the method is **not [L-stable](../../../../../../l-stability.md)**. These conclusions follow directly from the definitions of [A-stability](../../../../../../a-stability.md) and [L-stability](../../../../../../l-stability.md), rather than from the order of the method.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
