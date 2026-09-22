<h1 id="1/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $e_t=\mathbf1_{[0,t]}$ as an element of [L2 space](../../../../../l2-space-is-a-hilbert-space.md). Parts (iii) and (iv) show that $B_t=We_t$ is a centered [Gaussian process](../../../../../gaussian-process-split.md) with [covariance function](../../../../../covariance-function.md)

$$
\mathbb E[B_sB_t]=\langle e_s,e_t\rangle=\min(s,t).
$$

In particular $B_t-B_s\sim N(0,|t-s|)$. The fourth [moment](../../../../../moment.md) of a centered [normal random variable](../../../../../gaussian-random-variable.md) of [variance](../../../../../variance-split.md) $v$ is $3v^2$, so

$$
\mathbb E|B_t-B_s|^4=3|t-s|^2.
$$

The [Kolmogorov continuity theorem](../../../../../kolmogorov-continuity-theorem.md), with moment exponent $4$ and time exponent $2>1$, provides a [continuous modification](../../../../../continuous-modification.md) $\widehat B$. At each finite set of times this [modification of a stochastic process](../../../../../modification-of-a-stochastic-process.md) has the same joint law as $B$.

For $0\leq t_0<t_1<\cdots<t_m\leq1$, the successive increments are [Jointly Gaussian](../../../../../multivariate-normal-distribution.md). The [covariance](../../../../../covariance.md) of two increments on disjoint intervals equals the [inner product](../../../../../inner-product-split.md) of their disjoint interval indicators and is zero. Zero cross-[covariances](../../../../../covariance.md) of [Jointly Gaussian](../../../../../multivariate-normal-distribution.md) variables imply [independence](../../../../../independent-random-variables.md), and each increment has [variance](../../../../../variance-split.md) $t_j-t_{j-1}$. Finally $e_0=0$ in [L2 space](../../../../../l2-space-is-a-hilbert-space.md), so $\widehat B_0=0$ [almost surely](../../../../../almost-sure-convergence.md). Therefore

$$
\boxed{\widehat B\text{ is standard Brownian motion on }[0,1].}
$$

Independence from the whole past in its [natural Brownian filtration](../../../../../natural-brownian-filtration.md) follows by extending finite-dimensional [independence](../../../../../independent-random-variables.md) to the generated [sigma-algebra](../../../../../sigma-algebra.md).

## ↑ Ancestors (13)

1. [V](../v.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
