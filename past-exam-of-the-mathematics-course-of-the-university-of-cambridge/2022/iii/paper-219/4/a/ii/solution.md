<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiplying the Gaussian likelihood and prior and [completing the square](../../../../../../../completing-the-square.md) gives

$$
p(\theta\mid y)
\propto
\exp\!\left[-\frac12\left\{
\frac{(y-\theta)^2}{\sigma^2}+\frac{\theta^2}{\tau^2}
\right\}\right].
$$

Therefore [normal-normal conjugacy](../../../../../../../normal-normal-conjugacy-with-known-observation-variance.md) gives

$$
\boxed{\theta\mid y\sim N(m,v),
\qquad
m=\frac{\tau^2}{\sigma^2+\tau^2}y,
\qquad
v=\frac{\sigma^2\tau^2}{\sigma^2+\tau^2}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
