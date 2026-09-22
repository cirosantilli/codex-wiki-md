<h1 id="6/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A general-purpose high-dimensional choice is [Monte Carlo integration](../../../../../../monte-carlo-integration.md). Draw [independent](../../../../../../independent-random-variables.md) [vectors](../../../../../../vector.md) $W_r$ uniformly from the unit cube and evaluate $H(W_r)=\sum_{i=1}^{100}e^{\|W_r-a_i\|^2}$. The cube has volume $1$, so its [integral](../../../../../../integral-split.md) is the [expected value](../../../../../../expected-value-split.md) of $H(W_1)$. The iterative estimator is

$$
y_N=\frac1N\sum_{r=1}^NH(W_r),\qquad
y_{N+1}=y_N+\frac{H(W_{N+1})-y_N}{N+1}.
$$

The integrand is [continuous](../../../../../../continuous-function.md) on a compact [set](../../../../../../set-split.md), hence bounded with finite [variance](../../../../../../variance-split.md). The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives almost sure convergence, and the square root of the [mean squared error](../../../../../../mean-squared-error.md) is exactly $\sigma/\sqrt N$, where $\sigma^2=\operatorname{Var}(H(W_1))$. Thus the standard stochastic accuracy rate is **$O(N^{-1/2})$**; the dimension affects the [variance](../../../../../../variance-split.md) and evaluation cost, not this exponent.

There is also an important structure-specific improvement here: $e^{\|x-a_i\|^2}=\prod_{j=1}^{100}e^{(x_j-a_{ij})^2}$ is a [separable integrand](../../../../../../separable-integrand.md). The [Fubini theorem](../../../../../../fubini-s-theorem.md) reduces the requested value exactly to

$$
y=\sum_{i=1}^{100}\prod_{j=1}^{100}\int_0^1e^{(t-a_{ij})^2}\,dt.
$$

One can therefore replace high-dimensional sampling by $10000$ one-dimensional [composite Simpson's rule](../../../../../../composite-simpson-s-rule.md) calculations. For each factor use even $n$, $h=1/n$, and

$$
Q_n(g)=\frac h3\left[g(0)+g(1)+4\sum_{r=1,\ r\text{ odd}}^{n-1}g(rh)+2\sum_{r=2,\ r\text{ even}}^{n-2}g(rh)\right],
$$

then iterate $n\leftarrow2n$ and form the sum of the products. These smooth factors give **$O(n^{-4})$ deterministic discretization error** for fixed centres. Thus [Monte Carlo integration](../../../../../../monte-carlo-integration.md) is a valid generic answer, while exploiting separability is the more efficient specialized alternative; a large dimension alone does not force a tensor-product grid.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
