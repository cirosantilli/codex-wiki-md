<h1 id="1/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For any $C^2$ function $h$, the [Itô formula](../../../../../../../ito-s-lemma.md) and the ratio equation give

$$
dh(Z_t)=-\frac{\sqrt\kappa\,h'(Z_t)}{D_t}\,d\beta_t
+\frac1{D_t^2}\left[\frac\kappa2h''(Z_t)
+2\left(\frac1{Z_t}+\frac1{Z_t-1}\right)h'(Z_t)\right]dt.
$$

The bracket is zero for the functions just found. On compact localized intervals the stochastic integrand is bounded, so the stochastic integral is a [martingale](../../../../../../../martingale-split.md). Removing localization proves that $h(Z_t)$, on $0\leq t<T(x)$, is a [local martingale](../../../../../../../local-martingale.md). It is nonnegative because $Z_t>1$ and $C>0$.

In particular it is a [nonnegative local martingale](../../../../../../../nonnegative-local-martingale.md), hence a [supermartingale](../../../../../../../supermartingale.md) after the usual stopping and extension by its endpoint limit. This is the justification for using its maximal inequality; it is not automatically an unstopped uniformly integrable [martingale](../../../../../../../martingale-split.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
