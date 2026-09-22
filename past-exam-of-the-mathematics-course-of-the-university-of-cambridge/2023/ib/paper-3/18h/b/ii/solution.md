<h1 id="18h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\theta_1>\theta_0$, the [likelihood ratio](../../../../../../../likelihood-ratio.md) is

$$
\frac{f(x\mid\theta_1)}{f(x\mid\theta_0)}
=e^{-(\theta_1-\theta_0)}
\left(\frac{1+e^{x-\theta_0}}
{1+e^{x-\theta_1}}\right)^2,
$$

which is increasing in $x$. Thus the logistic location family has a [monotone likelihood ratio](../../../../../../../monotone-likelihood-ratio.md) in $X$.

The upper-tail rejection probability is increasing in the location parameter, since $X=\theta+Z$ with $Z$ having the standard [logistic distribution](../../../../../../../logistic-distribution.md). Hence for the critical value from part (i),

$$
\sup_{\theta\leq0}\mathbb P_\theta(X>c)
=\mathbb P_0(X>c)=\alpha.
$$

The test has size $\alpha$ for the composite null.

Now fix any alternative $\theta_1>0$. The [Neyman-Pearson lemma](../../../../../../../neyman-pearson-lemma.md) applied to the simple hypotheses $\theta=0$ and $\theta=\theta_1$ says that this same upper-tail test is most powerful among all tests whose rejection probability at $0$ is at most $\alpha$. Every test of size at most $\alpha$ for the composite null satisfies that restriction. The upper-tail test is therefore most powerful at every $\theta_1>0$, so it is the [uniformly most powerful upper-tail test for a logistic location](../../../../../../../uniformly-most-powerful-upper-tail-test-for-a-logistic-location.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [18H](../../../18h.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
