<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First replace $u$ by $u+\varepsilon$ and later let $\varepsilon\downarrow0$. In the weak subsolution inequality use the admissible truncations approximating $\eta^2u^{\alpha-1}$. Uniform ellipticity, the coefficient bound, [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md), and [Young inequality](../../../../../../../young-s-inequality-for-products.md) give

$$
(\alpha-1)\lambda\int\eta^2u^{\alpha-2}|Du|^2
\leq2\Lambda\int\eta u^{\alpha-1}|Du||D\eta|
$$

and therefore

$$
\int|Du|^2u^{\alpha-2}\eta^2
\leq\frac{C(\lambda,\Lambda)}{(\alpha-1)^2}\int u^\alpha|D\eta|^2.
$$

Apply the [Sobolev embedding theorem](../../../../../../../sobolev-embedding-theorem.md) to $w=\eta u^{\alpha/2}$. The preceding estimate yields, for concentric balls $B_r\subset B_R\subset B_1$,

$$
\|u\|_{L^{\alpha\sigma}(B_r)}
\leq\left(\frac{C\alpha^2}{(\alpha-1)^2(R-r)^2}\right)^{1/\alpha}
\|u\|_{L^\alpha(B_R)}.
$$

Starting with $\alpha=p>1$, taking $\alpha_k=p\sigma^k$, and choosing radii decreasing to $1/2$, the product of constants converges because $\sum_k\alpha_k^{-1}<\infty$. Letting $k\to\infty$ proves

$$
\sup_{B_{1/2}}u\leq C(n,\lambda,\Lambda,p)\|u\|_{L^p(B_1)}.
$$

This exponent-raising argument is [Moser iteration](../../../../../../../moser-iteration.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
