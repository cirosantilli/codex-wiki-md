<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the [Lévy construction of Brownian motion](../../../../../levy-construction-of-brownian-motion.md), start with $B_0=0$ and $B_1=Z_0$, where $Z_0$ has the [standard normal distribution](../../../../../standard-normal-distribution.md). Suppose values are defined at the endpoints $u=k2^{-n}$ and $v=(k+1)2^{-n}$. Set

$$
B_{(u+v)/2}=\frac{B_u+B_v}{2}+\frac{\sqrt{v-u}}2Z_{n,k},
$$

using fresh [independent](../../../../../independent-random-variables.md) [standard normal random variables](../../../../../standard-normal-random-variable.md) $Z_{n,k}$, also [independent](../../../../../independent-random-variables.md) of everything previously used. Join the values by straight segments to obtain a continuous piecewise linear process $B^{(n)}$ on the dyadic grid.

To verify the [Brownian increments](../../../../../brownian-increment.md), write $D=B_v-B_u$ and $\ell=v-u$. The two new increments are $D/2+\sqrt\ell Z_{n,k}/2$ and $D/2-\sqrt\ell Z_{n,k}/2$. If $D\sim N(0,\ell)$, their [variances](../../../../../variance-split.md) are $\ell/2$ and their [covariance](../../../../../covariance.md) is zero. They are [Jointly Gaussian](../../../../../multivariate-normal-distribution.md), so they are [independent](../../../../../independent-random-variables.md). Induction proves the required [Brownian increments](../../../../../brownian-increment.md) on every dyadic grid.

For convergence, successive interpolants differ by tents of disjoint interiors, so

$$
\|B^{(n+1)}-B^{(n)}\|_\infty
=2^{-n/2-1}\max_{0\leq k<2^n}|Z_{n,k}|.
$$

The [Gaussian tail bound](../../../../../gaussian-tail-bound.md) and the [union bound](../../../../../boole-s-inequality.md) give

$$
\mathbb P\!\left(\max_{k<2^n}|Z_{n,k}|>n\right)
\leq2^{n+1}e^{-n^2/2}.
$$

These [probabilities](../../../../../probability.md) are summable. The [First Borel-Cantelli lemma](../../../../../borel-cantelli-first-lemma.md) and $\sum_n n2^{-n/2}<\infty$ therefore prove [uniform convergence](../../../../../uniform-convergence.md) of the interpolants [almost surely](../../../../../almost-sure-convergence.md). Their limit has continuous [sample paths](../../../../../sample-path.md). Approximating any finite set of times by dyadic times passes the [Jointly Gaussian](../../../../../multivariate-normal-distribution.md) increment laws to the limit, giving a standard [Brownian motion](../../../../../brownian-motion-split.md) on $[0,1]$.

Equivalently, with $\psi_{n,k}(t)=\int_0^tH_{n,k}(s)\,ds$, these tents give the [Lévy-Ciesielski expansion](../../../../../levy-ciesielski-expansion.md)

$$
\boxed{B_t=Z_0t+\sum_{n=0}^\infty\sum_{k=0}^{2^n-1}Z_{n,k}\psi_{n,k}(t),
\quad\text{uniformly almost surely on }[0,1].}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
