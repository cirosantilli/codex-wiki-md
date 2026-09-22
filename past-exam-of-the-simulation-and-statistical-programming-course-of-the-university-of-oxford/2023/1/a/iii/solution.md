<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [central limit theorem](../../../../../central-limit-theorem.md) gives $\sqrt n(\widehat\theta_n^{\mathrm{MC}}-\theta)\Rightarrow N(0,1)$, so, with $\Phi$ the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the [standard normal distribution](../../../../../standard-normal-distribution.md),

$$
\mathbb P\!\left(\left|\widehat\theta_n^{\mathrm{MC}}-\theta\right|<0.01\right)
\approx 2\Phi(0.01\sqrt n)-1.
$$

The error has two tails. Using the supplied $2.58$ [quantile](../../../../../quantile-function.md), whose two-sided coverage is approximately $0.9902$, gives

$$
0.01\sqrt n\geq2.58,
\qquad
\boxed{N:=n=\left\lceil\frac{2.58^2}{0.01^2}\right\rceil=66{,}564.}
$$

The supplied $2.33$ [quantile](../../../../../quantile-function.md) would be appropriate for a one-sided $99\%$ calculation; it would give only approximately $98.02\%$ two-sided coverage. Using the exact $0.995$ [quantile](../../../../../quantile-function.md) instead of $2.58$ would give $66{,}349$ draws; we consistently use the paper's rounded value $N=66{,}564$ below.

For routine [Monte Carlo integration](../../../../../monte-carlo-integration.md), the [central limit theorem](../../../../../central-limit-theorem.md) calculation is preferable as a practical budget: it uses about one fifteenth as many draws as the [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) bound. However, its coverage is approximate. Finite [variance](../../../../../variance-split.md) alone supplies no universal rate of convergence to the [normal distribution](../../../../../normal-distribution.md); an integrand with large [skewness](../../../../../skewness.md) or a [heavy-tailed distribution](../../../../../heavy-tailed-distribution.md) can make the approximation poor even at a large sample count. If an unconditional finite-sample $99\%$ guarantee is required under only the stated assumptions, use the [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) budget.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
