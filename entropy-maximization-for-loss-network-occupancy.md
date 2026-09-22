# Entropy maximization for loss-network occupancy

↑ **Parent:** [Product-form stationary distribution of a loss network](product-form-stationary-distribution-of-a-loss-network.md)

For positive arrival rates and capacities with every route nonempty, maximizing $H_\nu(x)$ over $x\geq0$, $Ax\leq C$ has a unique positive optimizer $x^*$. The [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) give $x_r^*=\nu_r e^{-(A^Tz)_r}$ for nonnegative link prices with [complementary slackness](complementary-slackness.md). Under proportional scaling by $N$, the [Stirling formula](stirling-formula.md) gives a uniform logarithmic weight approximation $\log w_N(n)=NH_\nu(n/N)+O(\log N)$. Strict [concavity](concave-function.md) and compactness give an objective gap away from $x^*$, while only polynomially many feasible states exist. Thus the [stationary distribution](stationary-distribution.md) has $n/N\to x^*$ in probability, with exponentially small probabilities outside any fixed neighborhood of $x^*$. In particular $\mathbb E[n]=Nx^*+o(N)$.

**Table of contents**

- [Poisson exponential tilting for a loss network](poisson-exponential-tilting-for-a-loss-network.md)

## ↑ Ancestors (10)

1. [Product-form stationary distribution of a loss network](product-form-stationary-distribution-of-a-loss-network.md)
2. [Fixed routing](fixed-routing.md)
3. [Loss network](loss-network.md)
4. [Stochastic network](stochastic-network.md)
5. [Queueing theory](queueing-theory-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [User-network decomposition of concave utility maximization](user-network-decomposition-of-concave-utility-maximization.md)
