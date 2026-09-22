<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), put $z=h\lambda$. Eliminating the stages of the [Runge-Kutta method](../../../../../../runge-kutta-method.md) gives the [stability function](../../../../../../stability-function.md)

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\boxed{\frac{1+z/3}{1-2z/3+z^2/6}}.
$$

Its poles are $2\pm i\sqrt2$, strictly in the right half-plane. To prove [A-stability](../../../../../../a-stability.md) directly, write $z=-r+iy$ with $r\geq0$. With $D(z)=1-2z/3+z^2/6$ and $N(z)=1+z/3$, elementary expansion gives

$$
|D(z)|^2-|N(z)|^2
=2r+\frac23r^2+\frac29r^3+\frac1{36}r^4
+\frac29ry^2+\frac1{18}r^2y^2+\frac1{36}y^4\geq0.
$$

Therefore $|R(z)|\leq1$ throughout the closed left half-plane; the inequality is strict except at $z=0$. **The method is [A-stable](../../../../../../a-stability.md).** Moreover $R(z)\to0$ as $|z|\to\infty$, so the [Radau IIA method](../../../../../../radau-iia-method.md) is also [L-stable](../../../../../../l-stability.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
