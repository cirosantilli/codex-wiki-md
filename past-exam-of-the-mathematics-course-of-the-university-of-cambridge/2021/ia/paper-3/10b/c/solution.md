<h1 id="10b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In [polar coordinates](../../../../../../polar-coordinates.md), the circle is $r=2$, the line $y=\sqrt3x$ is $\theta=\pi/3$, and $y=1$ is $r\sin\theta=1$. The inequalities select

$$
\boxed{
\frac\pi6<\theta<\frac\pi3,\qquad
\csc\theta<r<2}.
$$

The surface height is

$$
z=\frac{xy}{x^2+y^2}
=\sin\theta\cos\theta.
$$

Thus the required volume is

$$
\begin{aligned}
V
&=\int_{\pi/6}^{\pi/3}
\int_{\csc\theta}^{2}
\sin\theta\cos\theta\,r\,dr\,d\theta\\
&=\int_{\pi/6}^{\pi/3}
\left(2\sin\theta\cos\theta-\frac12\cot\theta\right)d\theta\\
&=\boxed{\frac12-\frac14\log3}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10B](../../10b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
