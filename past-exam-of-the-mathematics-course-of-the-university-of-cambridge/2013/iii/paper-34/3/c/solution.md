<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume [conditional independence](../../../../../../conditional-independence.md) of the [Poisson distributions](../../../../../../poisson-distribution.md), and write $u_i=\mu_{i1}$, $S_i=\sum_k e^{\eta_{ik}}$. The correct Poisson mass function has $e^{-\mu}$; the positive sign in the PDF's reminder is erroneous. The group likelihood is

$$
p(\mathbf y_i\mid u_i,\beta)=
\frac{u_i^{n_i}\exp\{\sum_k y_{ik}\eta_{ik}\}e^{-u_iS_i}}
{\prod_k y_{ik}!}.
$$

Multiply by the shape–rate [Gamma distribution](../../../../../../gamma-distribution.md) prior $b^au_i^{a-1}e^{-bu_i}/\Gamma(a)$ and integrate. The gamma integral gives

$$
\boxed{p(\mathbf y_i\mid\beta,a,b)=
\frac{b^a\Gamma(n_i+a)}{\Gamma(a)\prod_k y_{ik}!}
\frac{\exp\{\sum_k y_{ik}\eta_{ik}\}}
{(S_i+b)^{n_i+a}}.}
$$

Independent baseline priors give the product over groups. For fixed $a,b$, the leading factors do not depend on $\beta$, proving the requested [Gamma-integrated baseline Poisson likelihood](../../../../../../gamma-integrated-baseline-poisson-likelihood.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
