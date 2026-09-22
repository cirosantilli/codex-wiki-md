<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Runge-Kutta method](../../../../../../runge-kutta-method.md), the [stability function](../../../../../../stability-function.md) is $R(z)=1+z b^T(I-zA)^{-1}e$. Solving the stage equations on the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) gives

$$
 R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12}
 =\frac{z^2+6z+12}{z^2-6z+12}.
$$

The denominator has [roots of a polynomial](../../../../../../root-of-a-polynomial.md) $3\pm i\sqrt3$, both in the open right half-plane. If $z=x+iy$, direct expansion gives

$$
 |z^2-6z+12|^2-|z^2+6z+12|^2=-24x(|z|^2+12).
$$

Since $|z|^2+12>0$, the [modulus](../../../../../../modulus.md) of $R$ is at most one exactly when $x\leq0$. Thus

$$
\boxed{\mathcal S=\{z\in\mathbb C:\operatorname{Re}z\leq0\}.}
$$

**The method is [A-stable](../../../../../../a-stability.md).** Its [stability function](../../../../../../stability-function.md) has unit [modulus](../../../../../../modulus.md) on the imaginary axis and tends to one as $z\to-\infty$, so it is not [L-stable](../../../../../../l-stability.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
