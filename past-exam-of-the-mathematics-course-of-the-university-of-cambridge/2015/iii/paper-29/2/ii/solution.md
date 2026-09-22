<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $t>0$ and partition $[0,t]$ into $m$ equal intervals, with $r_k=kt/m$. Round $t\wedge T$ upward within this interval. The corresponding sampled value is

$$
Y_m=X_0\mathbf1_{\{T=0\}}+\sum_{k=1}^{m-1}X_{r_k}\mathbf1_{\{r_{k-1}<T\leq r_k\}}+X_t\mathbf1_{\{T>r_{m-1}\}}.
$$

Every time in this sum is at most $t$. The [stopping time](../../../../../../stopping-time.md) property makes each [indicator function](../../../../../../indicator-function.md) $\mathcal F_t$-[measurable](../../../../../../measurability.md), while the [adapted process](../../../../../../adapted-process.md) property makes each sampled value $\mathcal F_t$-[measurable](../../../../../../measurability.md). Consequently $Y_m$ is $\mathcal F_t$-[measurable](../../../../../../measurability.md).

The rounded times approach $t\wedge T$ from the right, so right continuity gives $Y_m\to X_{t\wedge T}$ for the chosen pathwise [càdlàg](../../../../../../cadlag.md) version. If path regularity is instead stated only [almost surely](../../../../../../almost-sure-convergence.md), the usual complete [filtration](../../../../../../filtration-probability-theory.md) handles the exceptional [null set](../../../../../../null-set.md); on an incomplete [filtration](../../../../../../filtration-probability-theory.md) one should formulate that case as existence of an [adapted](../../../../../../adapted-process.md) version. At $t=0$, the value is simply $X_0$. Thus **$X^T$ is an [adapted process](../../../../../../adapted-process.md)**, by [adaptedness of a stopped right-continuous process](../../../../../../adaptedness-of-a-stopped-right-continuous-process.md). The argument actually needs neither the [martingale](../../../../../../martingale-split.md) property nor boundedness of $T$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
