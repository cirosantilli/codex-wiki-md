<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $A=\{a,b\}$ and let $\tau_x^+=\min\{t\geq1:X_t=x\}$. The conductance-hitting identity for an [electrical network](../../../../../../electrical-network.md) is

$$
\mathbb P_x(\tau_D<\tau_x^+)
=\frac{1}{c(x)R_{\mathrm{eff}}(x,D)},
\qquad c(x)=\sum_yc(x,y),
$$

where the vertices of $D$ are wired together. It follows by taking the hitting probability of $D$ before returning to $x$ as a voltage and computing its total current out of $x$.

Split the walk into successive excursions from $x$. The first excursion that hits $A$ determines whether $a$ or $b$ is hit first. Its conditional probability of hitting $a$ is at most the probability that an arbitrary excursion hits $a$, divided by the probability that it hits $A$. Hence

$$
\begin{aligned}
\mathbb P_x(\tau_a<\tau_b)
&\leq
\frac{\mathbb P_x(\tau_a<\tau_x^+)}
{\mathbb P_x(\tau_A<\tau_x^+)}\\
&=\boxed{\frac{R_{\mathrm{eff}}(x,A)}{R_{\mathrm{eff}}(x,a)}}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
