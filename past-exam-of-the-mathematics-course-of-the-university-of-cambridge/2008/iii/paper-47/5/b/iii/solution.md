<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

[Reversible-jump Markov chain Monte Carlo](../../../../../../../reversible-jump-markov-chain-monte-carlo.md) requires the reciprocal density/proposal ratio for the matched reverse transformation, so the death acceptance probability is

$$
\boxed{A_-=\min(1,R_+^{-1}).}
$$

Expressed directly in the current residual $r'=y-X_{k+1}\beta'$ and the recovered lower-order parameters, this is

$$
R_-=\frac{p_kb_k}{p_{k+1}d_{k+1}}\,
\frac1{\sigma_\beta}\sqrt{\frac{|\Sigma_{k+1}|}{|\Sigma_k|}}
\exp\left[
-\frac{zv^Tr'+z^2v^Tv/2}{s}
+\frac{Q_{k+1}-Q_k}{2}
-\frac{z^2}{2\sigma_\beta^2}
\right].
$$

Indeed $r=r'+zv$ makes this exponent the negative of the birth exponent, and all prefactors invert. Thus $R_-R_+=1$ for matched states. This reciprocity, including the normalized [prior distributions](../../../../../../../prior-probability.md) and auxiliary proposal density, gives the required detailed balance between models.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
