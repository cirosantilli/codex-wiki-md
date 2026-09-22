<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the specified time $t$. With the path modulus $\eta_n$ on $[0,t+1]$ as above, comparison of increment powers now gives

$$
V_t^{n,|\cdot|^2}\le\eta_n^{2-p}V_t^{n,|\cdot|^p}.
$$

The hypothesis makes the second factor eventually bounded [almost surely](../../../../../../almost-sure-convergence.md), while the first tends to zero [almost surely](../../../../../../almost-sure-convergence.md) because $2-p>0$. Thus the squared-increment sums tend to zero [almost surely](../../../../../../almost-sure-convergence.md). They also converge in [probability](../../../../../../probability.md) to the [quadratic variation](../../../../../../quadratic-variation.md) $[X]_t$, so uniqueness of the limit in [probability](../../../../../../probability.md) implies $[X]_t=0$ [almost surely](../../../../../../almost-sure-convergence.md).

The [quadratic variation](../../../../../../quadratic-variation.md) is nondecreasing, hence it vanishes throughout $[0,t]$. To see explicitly that the [continuous local martingale](../../../../../../continuous-local-martingale.md) must then be constant, localize it to square-integrable stopped [martingales](../../../../../../martingale-split.md). The [Itô isometry](../../../../../../ito-isometry.md) gives

$$
\mathbb E\bigl|X_{s\wedge\sigma_N}-X_0\bigr|^2
=\mathbb E[X]_{s\wedge\sigma_N}=0\qquad(s\le t).
$$

Remove the localization, apply the conclusion at every rational $s\le t$, and use continuity. Since $X_0=0$, this proves

$$
\boxed{\mathbb P(X_s=0\text{ for every }s\in[0,t])=1.}
$$

Thus $X$ is indistinguishable from the zero process on that interval. This is the subquadratic case of [dyadic power variation of a continuous local martingale](../../../../../../dyadic-power-variation-of-a-continuous-local-martingale.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
