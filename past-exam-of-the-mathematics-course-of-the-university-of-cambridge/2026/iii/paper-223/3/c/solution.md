<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $k=2r+1$ and $m=n/k$. The [central limit theorem](../../../../../../central-limit-theorem.md) gives jointly

$$
\frac{\sqrt m(\overline X_j-\mu)}\sigma
\Longrightarrow Z_j,
$$

where the $Z_j$ are independent standard normal variables. Hence

$$
\sqrt n(\widehat\mu_{\mathrm{MOM}}-\mu)
\Longrightarrow\sigma\sqrt k,Z_{(r+1)}.
$$

Its limiting cumulative distribution function is

$$
\boxed{\sum_{j=r+1}^k\binom kj
\Phi\left(\frac{x}{\sigma\sqrt k}\right)^j
\left[1-\Phi\left(\frac{x}{\sigma\sqrt k}\right)\right]^{k-j}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
