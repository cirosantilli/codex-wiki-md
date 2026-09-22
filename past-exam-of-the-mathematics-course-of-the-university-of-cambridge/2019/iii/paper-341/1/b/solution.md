<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), put $z=h\lambda$. The amplification roots satisfy

$$
(7-6z+2z^2)\xi^2-8\xi+1=0.
$$

We show that no root can reach the [unit circle](../../../../../../complex-unit-circle.md) for $\operatorname{Re}z<0$. If $\xi=e^{i\theta}$, solving the quadratic in $z$ gives

$$
z=\frac32\pm\sqrt C,\qquad C=-\frac54+4e^{-i\theta}-\frac12e^{-2i\theta}.
$$

Write $c=\cos\theta$, $u=\operatorname{Re}C=-3/4+4c-c^2$, and $v=\operatorname{Im}C=(c-4)\sin\theta$. Then $u\leq9/4$ and

$$
\left(\frac92-u\right)^2-|C|^2
=\frac{81}{4}-9u-v^2
=(c-1)^2(c^2-6c+11)\geq0.
$$

Since $9/2-u>0$, this gives $|C|+u\leq9/2$. Consequently $|\operatorname{Re}\sqrt C|^2=(|C|+u)/2\leq9/4$, so both possible $z$ have nonnegative real part. Equality can occur only at $\theta=0$, which gives $z=0$ or $z=3$.

The leading coefficient has zeros $(3\pm i\sqrt5)/2$, both in the right half-plane. Hence the amplification roots vary continuously as a pair throughout the left half-plane. At $z=-1$ they are $1/3$ and $1/5$; neither can leave the [unit disk](../../../../../../unit-disk.md) without crossing the [unit circle](../../../../../../complex-unit-circle.md), which the preceding calculation excludes. The same conclusion extends to the imaginary axis, with strict inequality away from $z=0$. At zero the roots $1,1/7$ satisfy the simplicity requirement.

Thus the method is **[A-stable](../../../../../../a-stability.md)**. Its third order does not contradict the usual second-order barrier, because it is a [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
