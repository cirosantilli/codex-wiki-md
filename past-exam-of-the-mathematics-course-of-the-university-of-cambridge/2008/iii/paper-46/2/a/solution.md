<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat the two retrieved sets of positive tests as independent binomial samples, each of size 500, and use a two-sided test at significance level $0.05$. The normal-approximation [sample size for comparing two proportions](../../../../../../sample-size-for-comparing-two-proportions.md), with equal numbers $n$ in each group, is

$$
n\simeq\frac{\left[z_{0.975}\sqrt{2\bar p(1-\bar p)}+
z_{0.8}\sqrt{p_0(1-p_0)+p_1(1-p_1)}\right]^2}{(p_0-p_1)^2},
\qquad\bar p=\frac{p_0+p_1}{2}.
$$

For $p_0=0.4$, $p_1=0.3$, this gives $n\simeq355.94$, or 356 per group. Thus **500 positives in each period are sufficient for 80% power under these assumptions**.

More explicitly, a pooled two-proportion test rejects when

$$
\left|\frac{\widehat p_0-\widehat p_1}
{\sqrt{\widehat p(1-\widehat p)(1/500+1/500)}}\right|>1.96,
$$

where $\widehat p$ pools the maximum-readout successes. At the proposed alternative, the difference has [mean](../../../../../../expected-value.md) $0.10$ and [standard deviation](../../../../../../standard-deviation.md) $\sqrt{0.45/500}=0.03$. The planning null critical difference is $1.96\sqrt{0.455/500}\simeq0.0591$, giving approximate power

$$
\Phi\left(\frac{0.10-0.0591}{0.03}\right)
+\Phi\left(\frac{-0.10-0.0591}{0.03}\right)
\simeq0.913.
$$

This compares the readout percentage among positive tests. It assumes comparable measurement rules and independent observations; a change in that percentage alone does not identify its causal explanation or the prevalence of drug use in the full tested population.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
