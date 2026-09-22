<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [binomial likelihood](../../../../../../binomial-likelihood.md) is $p(x\mid\theta)=\binom mx\theta^x(1-\theta)^{m-x}$. Multiplication by the [Beta distribution](../../../../../../beta-distribution.md) [prior density](../../../../../../prior-density.md) and [Bayes' theorem](../../../../../../bayes-theorem.md) give the [posterior density](../../../../../../posterior-density.md) kernel $\theta^{a+x-1}(1-\theta)^{b+m-x-1}$. Normalizing by the [beta function](../../../../../../beta-function.md) yields [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md):

$$
\boxed{\theta\mid x\sim\operatorname{Beta}(a+x,b+m-x).}
$$

This is proper for $a,b>0$ and $0\leq x\leq m$, including counts at either boundary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
