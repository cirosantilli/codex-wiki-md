<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The third fit is a [negative binomial regression](../../../../../../negative-binomial-regression.md). The Poisson model is obtained at the boundary where the negative-binomial overdispersion tends to zero, so the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) has the asymptotic null distribution $\tfrac12\chi_0^2+\tfrac12\chi_1^2$. Since model3 has one additional parameter,

$$
D=2(\ell_3-\ell_1)
=\operatorname{AIC}_1-\operatorname{AIC}_3+2.
$$

The supplied output gives $\mathbb P(\chi_1^2\geq D)=0.04608555$, and hence the boundary-corrected p-value is

$$
\boxed{p=\frac12(0.04608555)=0.023042775.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
