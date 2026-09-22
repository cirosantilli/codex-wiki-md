<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the shape-rate convention for every [gamma distribution](../../../../../../gamma-distribution.md), with $a,c>0$. Let $A_i=a+y_i$ and $s=\sum_i\theta_i$. The [Poisson distribution](../../../../../../poisson-distribution.md) likelihood and the [Gamma–Poisson hierarchical model](../../../../../../gamma-poisson-hierarchical-model.md) give

$$
\pi(\theta,b\mid y)\propto
b^{na+c-1}e^{-b(1+s)}\prod_{i=1}^n\theta_i^{A_i-1}e^{-t_i\theta_i},
\qquad b>0,\ \theta_i>0.
$$

All factors involving the coordinate being updated must be retained, including $b^{na}$ from the conditional [gamma distributions](../../../../../../gamma-distribution.md). The [full conditional distributions](../../../../../../full-conditional-distribution.md) are

$$
\boxed{\theta_i\mid b,y\sim\operatorname{Gamma}(A_i,b+t_i)\quad\text{independently},\qquad
b\mid\theta,y\sim\operatorname{Gamma}(na+c,1+s).}
$$

For a [blocked Gibbs sampler](../../../../../../blocked-gibbs-sampler.md), draw $b$ from the second [full conditional distribution](../../../../../../full-conditional-distribution.md), then redraw all the $\theta_i$ independently from the first ones. Repeating these two steps preserves the joint [posterior distribution](../../../../../../bayesian-posterior.md); observing $\theta$ after each complete sweep gives the [Markov chain](../../../../../../markov-chain.md) used in the next part. Standard [gamma distribution](../../../../../../gamma-distribution.md) sampling works for noninteger as well as integer shapes. The positive observation-period convention $t_i>0$ is used for the subsequent [geometric drift condition](../../../../../../geometric-drift-condition.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
