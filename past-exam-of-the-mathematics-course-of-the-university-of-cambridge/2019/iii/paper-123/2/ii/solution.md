<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the coefficient $a_n=1/n!$, the [p-adic absolute value](../../../../../../p-adic-absolute-value.md) gives $|a_n|_p=p^{v_p(n!)}$. By [Legendre formula](../../../../../../legendre-s-formula.md),

$$
v_p(n!)=\sum_{j\geq1}\left\lfloor\frac n{p^j}\right\rfloor
=\frac{n-s_p(n)}{p-1},
$$

where $s_p(n)$ is the sum of the base-$p$ digits of $n$. Thus $v_p(n!)/n\to1/(p-1)$. The [Cauchy-Hadamard theorem](../../../../../../cauchy-hadamard-theorem.md) now yields

$$
R^{-1}=\limsup_{n\to\infty}|a_n|_p^{1/n}=p^{1/(p-1)},
$$

and therefore the [radius of convergence of the p-adic exponential](../../../../../../radius-of-convergence-of-the-p-adic-exponential.md) is

$$
\boxed{R=p^{-1/(p-1)}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
