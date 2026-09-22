<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [stability function](../../../../../../stability-function.md) of a [Runge-Kutta method](../../../../../../runge-kutta-method.md) is $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$. Substitution gives

$$
\boxed{R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}.}
$$

Writing the numerator and denominator as $N(z)$ and $D(z)$,

$$
|D(z)|^2-|N(z)|^2=-2\operatorname{Re}z\left(1+\frac{|z|^2}{12}\right).
$$

The denominator has zeros $3\pm i\sqrt3$, both in the right half-plane. Therefore $|R(z)|\leq1$ throughout the closed left half-plane, with strict inequality in its interior. The method is **[A-stable](../../../../../../a-stability.md)**. Since $R(z)\to1$ at infinity, it is not [L-stable](../../../../../../l-stability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
