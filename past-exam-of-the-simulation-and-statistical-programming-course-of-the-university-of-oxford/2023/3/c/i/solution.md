<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Each state has exactly $k(n-k)$ neighbours: choose one occupied coordinate and one unoccupied coordinate to swap. The normalized [proposal distribution](../../../../../proposal-distribution.md) is therefore

$$
q(v\mid u)=\frac1{k(n-k)}\mathbf1_{\{v\sim u\}}.
$$

The swap relation is symmetric and the number of neighbours is constant, so $q(v\mid u)=q(u\mid v)$. The [discrete uniform distribution](../../../../../discrete-uniform-distribution.md) used as the [prior distribution](../../../../../prior-probability.md) is also constant on $S_k$, with mass $\binom nk^{-1}$. Both factors cancel in the [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md).

Let $Q=\Sigma^{-1}$ and $d=v-u$. The displayed [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) presupposes that the [covariance matrix](../../../../../covariance-matrix.md) $\Sigma$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md), so $Q$ is a [symmetric matrix](../../../../../symmetric-matrix.md). Expanding the difference of [quadratic forms](../../../../../quadratic-form-split.md) gives

$$
\begin{aligned}
\log\frac{\pi(v\mid x)}{\pi(u\mid x)}
&=-\tfrac12\{(x-v)^TQ(x-v)-(x-u)^TQ(x-u)\}\\
&=d^TQ(x-u)-\tfrac12d^TQd\\
&=d^TQ\left(x-\frac{u+v}{2}\right).
\end{aligned}
$$

Consequently

$$
\boxed{\log\alpha(u,v)=\min\!\left\{0,\ (v-u)^T\Sigma^{-1}\left(x-\frac{u+v}{2}\right)\right\}.}
$$

The truncation at zero is essential: a log acceptance ratio can be positive, but the [logarithm](../../../../../logarithm.md) of an acceptance [probability](../../../../../probability.md) cannot.

For the particular proposed swap, let $a=i_1$ be the coordinate changing from zero to one and $b=i_2$ the coordinate changing from one to zero. Then $d=e_a-e_b$, and the untruncated scalar simplifies further to

$$
\boxed{(Q(x-u))_a-(Q(x-u))_b-\tfrac12(Q_{aa}+Q_{bb}-2Q_{ab}).}
$$

Only two rows and four entries of $Q$ are needed for this evaluation. This is [Metropolis sampling on fixed-cardinality subsets](../../../../../metropolis-sampling-on-fixed-cardinality-subsets.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
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
