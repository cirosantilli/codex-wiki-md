<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The two independent [binomial distributions](../../../../../../binomial-distribution.md) give fitted event probabilities $24/99$ and $12/100$. Their [odds ratio](../../../../../../odds-ratio.md) and [log odds ratio](../../../../../../log-odds-ratio.md) are

$$
\widehat{\mathrm{OR}}=\frac{24\cdot88}{75\cdot12}=2.34667,
\qquad \widehat\delta=\log\widehat{\mathrm{OR}}=0.852996.
$$

Using the [log odds ratio variance from a two-by-two table](../../../../../../log-odds-ratio-variance-from-a-two-by-two-table.md),

$$
\widehat{\operatorname{Var}}(\widehat\delta)
=\frac1{24}+\frac1{75}+\frac1{12}+\frac1{88}
=0.149697,\qquad \operatorname{SE}(\widehat\delta)=0.386907.
$$

The stated [normal approximation](../../../../../../normal-approximation.md) and quantile approximately two give the [confidence interval](../../../../../../confidence-interval.md)

$$
\boxed{\delta\in0.852996\pm2(0.386907)=(0.07918,1.62681).}
$$

Exponentiation gives the corresponding [odds ratio](../../../../../../odds-ratio.md) interval $(1.0824,5.0876)$. Its lower endpoint exceeds one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
