<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use discrete dates $j=0,\ldots,N$, a [bank account](../../../../../../bank-account.md) $B_j=R^j$ with $R=1+r>0$, and a positive stock with each one-period gross return either $u$ or $d$, where $0<d<u$. On the natural tree assume both moves have positive physical probability. The [Cox--Ross--Rubinstein model](../../../../../../cox-ross-rubinstein-model.md) is arbitrage-free precisely when

$$
\boxed{d<R<u.}
$$

Otherwise a stock/bank position gives nonnegative profit in both states and positive profit in at least one. Under the condition, the unique [equivalent martingale measure](../../../../../../risk-neutral-measure.md) has independent upward moves with [conditional probability](../../../../../../conditional-probability.md)

$$
\boxed{q=\frac{R-d}{u-d}\in(0,1).}
$$

Indeed $qu+(1-q)d=R$, making the discounted stock a [martingale](../../../../../../martingale-split.md). Both branches have positive probability under this [measure](../../../../../../measure.md), ensuring equivalence. The uniqueness/completeness claim is for the stock-generated binomial tree; an enlarged filtration carrying additional untraded risk would change that claim.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
