<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $P\ll Q$, the [chi-squared divergence](../../../../../../chi-squared-divergence.md) is $\chi^2(P\Vert Q)=\mathbb E_Q[(dP/dQ-1)^2]$. Write $L_j=dQ_j/dP_0$ for the [likelihood ratios](../../../../../../likelihood-ratio.md) of the complete $n$-ball sample. Since $dP_1/dP_0=d^{-1}\sum_jL_j$ and $\mathbb E_0L_j=1$, the [second moment of a mixture likelihood ratio](../../../../../../second-moment-of-a-mixture-likelihood-ratio.md) gives

$$
\boxed{\chi^2(P_1\Vert P_0)=\frac1{d^2}\sum_{j,\ell=1}^d\mathbb E_0[L_jL_\ell]-1.}
$$

If instead $L_j$ denotes a one-ball [likelihood ratio](../../../../../../likelihood-ratio.md), its cross moment must be raised to the $n$th power for the full sample, by [independence](../../../../../../independent-random-variables.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
