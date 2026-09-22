<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the drifted [Brownian motion](../../../../../../brownian-motion-split.md) $Y_t=y+B_t+at$ on $(0,\infty)$, the [diffusion generator](../../../../../../diffusion-generator.md) is $\mathcal L=\frac12\frac{d^2}{dz^2}+a\frac{d}{dz}$. Seek a bounded solution of $\mathcal Lu=\lambda u$ with $u(0)=1$. The exponential ansatz $u(z)=e^{rz}$ gives

$$
\frac12r^2+ar=\lambda,\qquad r=-a\pm\sqrt{a^2+2\lambda}.
$$

Because $\lambda>0$, the plus root is positive and the minus root is negative. Boundedness on $[0,\infty)$ therefore selects

$$
u(z)=\exp\left(-z\left(a+\sqrt{a^2+2\lambda}\right)\right).
$$

It satisfies the boundary condition and all hypotheses of part (d). Hence

$$
\boxed{\mathbb E e^{-\lambda S}=\exp\left(-y\left(a+\sqrt{a^2+2\lambda}\right)\right).}
$$

This is the [first-passage Laplace transform for Brownian motion with drift](../../../../../../first-passage-laplace-transform-for-brownian-motion-with-drift.md), with $e^{-\lambda\infty}=0$. At $a=0$ it reduces to $e^{-y\sqrt{2\lambda}}$. As $\lambda\downarrow0$, it gives $\mathbb P(S<\infty)=e^{-2y\max(a,0)}$, agreeing with certainty of hitting when the drift points towards zero and a possible escape when it points away.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
