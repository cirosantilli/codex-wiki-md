<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For normalized target density $p(m\mid d)$ and proposal $q$, the unbiased importance estimator $K^{-1}\sum_i m_i p(m_i\mid d)/q(m_i)$ has variance

$$
\frac1K\left[
\int\frac{m^2p(m\mid d)^2}{q(m)}\,dm
-\mathbb E[m\mid d]^2
\right].
$$

By [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
\int\frac{m^2p(m\mid d)^2}{q(m)}\,dm
\geq\left(\int|m|p(m\mid d)\,dm\right)^2,
$$

with equality exactly when

$$
q^*(m)=\frac{|m|p(m\mid d)}{\int|m|p(m\mid d)\,dm}.
$$

This is rarely useful because constructing and sampling from it already requires detailed knowledge of the posterior and its absolute first moment, the objects importance sampling was meant to avoid computing.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
