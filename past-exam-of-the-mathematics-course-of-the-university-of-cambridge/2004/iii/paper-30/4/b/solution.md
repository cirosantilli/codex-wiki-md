<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<\delta<1$, the bracket in the explicit solution is positive and increasing. Its integral is finite on every finite interval because $F$ is continuous and strictly positive there. The same is immediate from the exponential formula for $\delta=1$. Neither solution can reach zero on a finite interval. Hence both cases have global existence almost surely.

For $\delta>1$, put $q=\delta-1>0$ and $K=x_0^{-q}/q$. The [explosion threshold for a Bernoulli stochastic differential equation](../../../../../../explosion-threshold-for-a-bernoulli-stochastic-differential-equation.md) is

$$
\tau=\inf\left\{t:\int_0^tF_s^qds=K\right\},
\qquad
X_t=F_t\left[x_0^{-q}-q\int_0^tF_s^qds\right]^{-1/q}.
$$

If the threshold is reached at a finite time, $F_\tau$ is positive and finite, and $X_t\to\infty$ as $t\uparrow\tau$.

When $\alpha=0$, $F=1$ and $\tau=K$ deterministically. When $\alpha\ne0$, choose a constant $c$ large enough that $e^{qc}>K$. The event

$$
\alpha B_1>\alpha^2+c+1,\qquad
\inf_{1\le s\le2}\alpha(B_s-B_1)>-1
$$

has positive probability: the first part is a Gaussian tail event, the second has positive probability by the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md), and they are independent. On this event $\alpha B_s-\alpha^2s/2>c$ throughout $[1,2]$, so $\int_1^2F_s^qds>e^{qc}>K$. Thus $\mathbb P(\tau\le2)>0$ and global existence is not almost sure. We conclude

$$
\boxed{\text{Global positive existence with probability one holds exactly for }0<\delta\le1.}
$$

This argument asserts positive explosion probability for $\alpha\ne0$, not certain explosion. Indeed $B_t/t\to0$ almost surely makes $\int_0^\infty F_s^qds$ finite in that case; that observation does not remove the positive chance that its value exceeds the threshold.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
