<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $a=2\pi m+r$, where $m$ is an [integer](../../../../../../../integer-split.md) and $0\leq r<2\pi$. The [change of variables](../../../../../../../change-of-variables-formula.md) $x=y+2\pi m$ and the fact that $f$ is a [periodic function](../../../../../../../periodic-function.md) give

$$
\int_a^{a+2\pi}f(x)\,dx=\int_r^{r+2\pi}f(y)\,dy.
$$

Split at $2\pi$, then substitute $y=z+2\pi$ in the second piece:

$$
\begin{aligned}
\int_r^{r+2\pi}f(y)\,dy
&=\int_r^{2\pi}f(y)\,dy+\int_{2\pi}^{2\pi+r}f(y)\,dy\\
&=\int_r^{2\pi}f(y)\,dy+\int_0^r f(z+2\pi)\,dz\\
&=\int_r^{2\pi}f(y)\,dy+\int_0^r f(z)\,dz.
\end{aligned}
$$

Therefore

$$
\boxed{\int_a^{a+2\pi}f(x)\,dx=\int_0^{2\pi}f(x)\,dx\quad\text{for every }a\in\mathbb R.}
$$

This proves [translation invariance of an integral over one period](../../../../../../../translation-invariance-of-an-integral-over-one-period.md) without assuming that $f$ is [differentiable](../../../../../../../differentiable-function.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
