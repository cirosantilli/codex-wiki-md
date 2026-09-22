<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

For

$$
y''+P(z)y'+Q(z)y=0,
$$

a finite point $z_0$ is a [regular singular point](../../../../../regular-singular-point.md) when $(z-z_0)P(z)$ and $(z-z_0)^2Q(z)$ extend holomorphically to $z_0$. A singularity at infinity is classified by applying this criterion after the change of variable $w=1/z$.

For the displayed [Bessel differential equation](../../../../../bessel-differential-equation.md),

$$
P(z)=\frac1z,
\qquad
Q(z)=1-\frac1{4z^2}.
$$

At $z=0$, the functions $zP(z)=1$ and $z^2Q(z)=z^2-1/4$ are holomorphic, so zero is regular singular. To inspect infinity, write $Y(w)=y(1/w)$. The equation becomes

$$
Y''+\frac1wY'
+\left(\frac1{w^4}-\frac1{4w^2}\right)Y=0.
$$

Here $w^2Q(w)=w^{-2}-1/4$ is not holomorphic at zero, so infinity is an [irregular singular point](../../../../../irregular-singular-point.md). Thus

$$
\boxed{z=0\text{ is regular singular, while }z=\infty\text{ is irregular singular}.}
$$

Set $y=z^{-1/2}f$. Direct differentiation makes every lower-order term cancel:

$$
z^2y''+zy'+\left(z^2-\frac14\right)y
=z^{3/2}(f''+f).
$$

Hence $f''+f=0$, and on any domain carrying a branch of $\sqrt z$ two linearly independent solutions are

$$
\boxed{y_1(z)=\frac{\cos z}{\sqrt z},
\qquad
y_2(z)=\frac{\sin z}{\sqrt z}.}
$$

Near the regular singular point, these behave as $z^{-1/2}$ and $z^{1/2}$, the two [Frobenius exponents](../../../../../frobenius-method.md). At infinity their combinations are $z^{-1/2}e^{\pm iz}$; after $w=1/z$ these contain $e^{\pm i/w}$, the exponential behavior characteristic of an irregular singular point.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
