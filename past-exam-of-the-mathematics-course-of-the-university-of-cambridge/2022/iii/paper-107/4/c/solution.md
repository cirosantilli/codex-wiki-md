<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First replace $u$ by $u+\varepsilon$ and later let $\varepsilon\downarrow0$. In the supersolution inequality use the nonnegative test function

$$
\eta^2/(u+\varepsilon),
$$

where $\eta$ is compactly supported. Ellipticity and [Young inequality](../../../../../../young-s-inequality-for-products.md) give the [Logarithmic Caccioppoli inequality](../../../../../../logarithmic-caccioppoli-inequality.md)

$$
\int_B\eta^2|D\log(u+\varepsilon)|^2
\leq C(n,\lambda,\Lambda)\int_B|D\eta|^2.
$$

Choose $\eta=1$ on $B_\rho$, supported in $B$, with $|D\eta|\leq C(1-\rho)^{-1}$. Letting $\varepsilon\downarrow0$ and using [Fatou lemma](../../../../../../fatou-s-lemma.md) gives

$$
\boxed{
\int_{B_\rho}\frac{|Du|^2}{u^2}
\leq C(1-\rho)^{-2}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
