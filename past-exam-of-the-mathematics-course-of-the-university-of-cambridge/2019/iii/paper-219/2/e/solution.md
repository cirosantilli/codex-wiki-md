<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $p(m)=P(m\mid\mathbf d)$ and draw independently from an importance density $q$. The unbiased estimator

$$
\widehat I=\frac1n\sum_{j=1}^n\frac{m_jp(m_j)}{q(m_j)}
$$

of $I=\int mp(m)\,dm$ has one-sample second moment

$$
\int\frac{m^2p(m)^2}{q(m)}\,dm.
$$

By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md),

$$
\left(\int |m|p(m)\,dm\right)^2
\leq
\left(\int\frac{m^2p(m)^2}{q(m)}\,dm\right)
\left(\int q(m)\,dm\right).
$$

Equality holds precisely when $q(m)\propto|m|p(m)$, giving the [optimal importance density for a single integral](../../../../../../optimal-importance-density-for-a-single-integral.md)

$$
\boxed{q^*(m)=\frac{|m|p(m)}{\int|u|p(u)\,du}.}
$$

This is circular in practice: constructing and normalizing $q^*$ requires detailed knowledge of the posterior and the expectation of $|m|$. Here log masses are positive, so the unknown normalizer is the posterior mean being estimated. It is also optimal only for this one integral, not for general posterior summaries.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
