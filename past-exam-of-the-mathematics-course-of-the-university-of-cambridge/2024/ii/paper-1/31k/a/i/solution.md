<h1 id="31k/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\varepsilon_1,\ldots,\varepsilon_n$ be independent Rademacher signs. For the set of evaluation [vectors](../../../../../../../vector.md)

$$
\mathcal F(z_{1:n})=\left\{(f(z_1),\ldots,f(z_n)):f\in\mathcal F\right\},
$$

the empirical [Rademacher complexity](../../../../../../../rademacher-complexity.md) is

$$
\widehat R(\mathcal F(z_{1:n}))
=\mathbb E_\varepsilon\left[
\sup_{f\in\mathcal F}\frac1n\sum_{i=1}^n\varepsilon_i f(z_i)
\right].
$$

For an independent sample $Z_1,\ldots,Z_n$,

$$
R_n(\mathcal F)=\mathbb E_{Z_{1:n}}
\widehat R(\mathcal F(Z_{1:n})).
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [31K](../../../31k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
