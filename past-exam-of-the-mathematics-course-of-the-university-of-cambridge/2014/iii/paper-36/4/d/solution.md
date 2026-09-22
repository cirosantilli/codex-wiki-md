<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $p=1/M$ and $v_f=\int\phi^2f-\theta^2$. The Bernoulli [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\boxed{\frac{N-\mathbb EN}{\sqrt n}\ \Longrightarrow\ N(0,p(1-p)).}
$$

If $M=1$, all proposals are accepted and this limit is degenerate.

Conditional on $N=m$, the accepted sample is iid from $f$. Since $N/n\to p>0$, its size tends to infinity, and the ordinary target-sample CLT therefore gives

$$
\boxed{\sqrt N\left(\frac1N\sum_{i=1}^N\phi(Y_i)-\theta\right)\ \Longrightarrow\ N(0,v_f).}
$$

Assign any fixed value to the estimator on $N=0$; the probability of that event tends to zero, so it does not change this limit. This is the [random-count central limit theorem for accepted rejection samples](../../../../../../random-count-central-limit-theorem-for-accepted-rejection-samples.md).

For comparison at the same budget of $n$ proposals, Slutsky's theorem rescales this as

$$
\boxed{\sqrt n(\widehat\theta_2-\theta)\ \Longrightarrow\ N(0,Mv_f).}
$$

The distinction between accepted-sample size and proposal count is essential for the final efficiency comparison.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
