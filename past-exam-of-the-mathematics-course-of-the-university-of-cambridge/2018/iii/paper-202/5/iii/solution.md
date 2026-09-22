<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [dyadic power variation of a continuous local martingale](../../../../../../dyadic-power-variation-of-a-continuous-local-martingale.md), write $\Delta_i^nM=M_{i2^{-n}}-M_{(i-1)2^{-n}}$, $\delta_n=\max_i|\Delta_i^nM|$ and $Q_n=\sum_i(\Delta_i^nM)^2$. [Uniform continuity](../../../../../../uniform-continuity.md) on $[0,1]$ gives $\delta_n\to0$ [almost surely](../../../../../../almost-sure-convergence.md), while the deterministic-partition characterization of [quadratic variation](../../../../../../quadratic-variation.md) gives $Q_n\to\langle M\rangle_1$ in [probability](../../../../../../probability.md). In particular $(Q_n)$ is [bounded in probability](../../../../../../boundedness-in-probability.md).

If $p>2$, then $Z_n\leq\delta_n^{p-2}Q_n$, and a factor tending to zero in [probability](../../../../../../probability.md) times a sequence [bounded in probability](../../../../../../boundedness-in-probability.md) tends to zero in [probability](../../../../../../probability.md). Thus

$$
\boxed{Z_n\xrightarrow[n\to\infty]{\mathbb P}0\qquad(p>2).}
$$

If $1<p<2$, the reverse comparison is $Q_n\leq\delta_n^{2-p}Z_n$. The assumed finite $\limsup Z_n$ makes $Z_n$ eventually bounded [almost surely](../../../../../../almost-sure-convergence.md), so $Q_n\to0$ [almost surely](../../../../../../almost-sure-convergence.md). By [uniqueness of a limit in probability](../../../../../../uniqueness-of-a-limit-in-probability.md), $\langle M\rangle_1=0$ [almost surely](../../../../../../almost-sure-convergence.md). Its monotonicity gives $\langle M\rangle_t=0$ for $t\leq1$.

To finish without assuming any integrability of $M$, apply the bound from part (i) to both $M$ and $-M$, with $t=1$, and then let $b\downarrow0$. For each $a>0$ the [probability](../../../../../../probability.md) of a positive or negative excursion beyond $a$ is zero. Taking countably many $a\downarrow0$ proves **$M$ is indistinguishable from zero on $[0,1]$.** The same argument in fact works for every $0<p<2$ under the stated pathwise boundedness assumption.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
