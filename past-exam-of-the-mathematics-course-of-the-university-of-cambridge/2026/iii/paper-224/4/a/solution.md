<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\mu>0$, let $Q$ be the [geometric distribution](../../../../../../geometric-distribution.md)

$$
Q(k)=\frac1{1+\mu}\left(\frac\mu{1+\mu}\right)^k,
\qquad k\geq0.
$$

If $P$ is the law of $X$, [Gibbs inequality](../../../../../../gibbs-inequality.md) gives

$$
0\leq D(P\Vert Q)
=-H(X)+\log(1+\mu)+\mu\log\frac{1+\mu}{\mu}.
$$

Therefore

$$
H(X)\leq\log(1+\mu)+\mu\log\frac{1+\mu}{\mu}
=(1+\mu)h\left(\frac1{1+\mu}\right).
$$

For $\mu=0$, the nonnegative random variable $X$ is zero almost surely and both sides vanish. This proves that the [maximum entropy distribution on the nonnegative integers](../../../../../../maximum-entropy-distribution-on-the-nonnegative-integers.md) with fixed [expected value](../../../../../../expected-value.md) is geometric.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
