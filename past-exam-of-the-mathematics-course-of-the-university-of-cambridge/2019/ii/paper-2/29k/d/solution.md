<h1 id="29k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each period set

$$
\widetilde\sigma_i=-\frac{m_i+\sigma_i^2/2}{\sigma_i}
$$

and define

$$
\frac{d\mathbb Q}{d\mathbb P}
=\prod_{i=1}^T
\exp\!\left(\widetilde\sigma_iZ_i-\frac12\widetilde\sigma_i^2\right).
$$

Independence of the $Z_i$ shows that this strictly positive density has expectation one. Under $\mathbb Q$, the conditional mean of each gross return is

$$
\mathbb E_{\mathbb Q}
\left[e^{\sigma_iZ_i+m_i}\mid\mathcal F_{i-1}\right]
=\exp\!\left(m_i+\frac12\sigma_i^2
+\sigma_i\widetilde\sigma_i\right)=1.
$$

Consequently

$$
\mathbb E_{\mathbb Q}[S_t^1\mid\mathcal F_{t-1}]=S_{t-1}^1,
$$

so the discounted price process is a $\mathbb Q$-martingale. This equivalent martingale measure rules out arbitrage.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [29K](../../29k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
