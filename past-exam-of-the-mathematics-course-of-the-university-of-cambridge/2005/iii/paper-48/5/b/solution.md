<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The event that the first arrival exceeds $t$ is exactly the event $N_t=0$. Thus $\mathbb P(\tau_1>t)=e^{-\lambda t}$ for $t\geq0$, and differentiation gives the [exponential distribution](../../../../../../exponential-distribution.md) density $\boxed{f_{\tau_1}(t)=\lambda e^{-\lambda t}}$ for $t>0$.

Integration by parts, or the gamma integral, yields $\mathbb E\tau_1=\int_0^\infty e^{-\lambda t}dt=1/\lambda$ and $\mathbb E\tau_1^2=2\int_0^\infty te^{-\lambda t}dt=2/\lambda^2$. Therefore **$\boxed{\mathbb E\tau_1=1/\lambda,\quad\operatorname{Var}\tau_1=1/\lambda^2}$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
