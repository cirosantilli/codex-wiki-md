<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $G$ count copies of allele $2$. Under [Hardy-Weinberg equilibrium](../../../../../../hardy-weinberg-principle.md), $G$ has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $2,\phi$, and the [penetrance](../../../../../../penetrance.md) is $q_G=p\theta^G$. Consequently

$$
\begin{aligned}
\Pr(Y=1)
&=p(1-\phi)^2+\theta p\,2\phi(1-\phi)+\theta^2p\phi^2\\
&=p[(1-\phi)+\phi\theta]^2
=p\alpha^2.
\end{aligned}
$$

Thus **the overall penetrance is**

$$
\boxed{K=p\alpha^2,\qquad\alpha=1+\phi(\theta-1).}
$$

The [multiplicative diallelic penetrance](../../../../../../multiplicative-diallelic-penetrance.md) model requires $0\leq\phi\leq1$, $p\geq0$, $\theta\geq0$, and each occupied genotype's value $p\theta^G$ to be at most one. These are probabilities, not unrestricted relative-risk scores.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
