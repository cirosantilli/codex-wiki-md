<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed realization $\xi=a$ and $\operatorname{Re}z>1$, direct integration gives

$$
\begin{aligned}
\int_{-\infty}^{\infty}(e^a-e^k)^+z(z-1)e^{(z-1)k}\,dk
&=z(z-1)\int_{-\infty}^a(e^a-e^k)e^{(z-1)k}\,dk\\
&=z(z-1)\left(\frac{e^{za}}{z-1}-\frac{e^{za}}z\right)=e^{za}.
\end{aligned}
$$

To interchange the integral and [expectation](../../../../../../expected-value.md), write $x=\operatorname{Re}z>1$ and estimate

$$
\mathbb E\int_{-\infty}^{\infty}\left|(e^\xi-e^k)^+z(z-1)e^{(z-1)k}\right|dk
=\frac{|z(z-1)|}{x(x-1)}\mathbb Ee^{x\xi}<\infty.
$$

The [Fubini's theorem](../../../../../../fubini-s-theorem.md) now proves the [Mellin transform of call prices](../../../../../../mellin-transform-of-call-prices.md) identity

$$
\boxed{M(z)=\int_{-\infty}^{\infty}C(k)z(z-1)e^{(z-1)k}\,dk\qquad(\operatorname{Re}z>1).}
$$

The required [exponential moment](../../../../../../exponential-moment.md) is $\mathbb Ee^{x\xi}<\infty$ at the chosen real part; the assertion for every $x>1$ presupposes these [exponential moments](../../../../../../exponential-moment.md) for every such $x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
