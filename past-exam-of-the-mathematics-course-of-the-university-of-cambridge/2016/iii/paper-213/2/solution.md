<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In a [loss network](../../../../../loss-network.md) with [fixed routing](../../../../../fixed-routing.md), calls of type $r$ arrive as independent [Poisson processes](../../../../../poisson-process.md) with rates $\nu_r$. Every accepted call occupies $A_{jr}$ units of resource $j$ throughout its holding time. The [link-route incidence matrix](../../../../../link-route-incidence-matrix.md) $A$ has nonnegative integer entries, $C$ is the resource-capacity vector, $n_r$ counts calls currently present, and $e_r$ is the $r$th coordinate unit vector. The feasible occupancy space is

$$
S(C)=\{n\in\mathbb Z_{\geq0}^{R}:An\leq C\}.
$$

The inequalities are coordinatewise. A call that would leave this space is rejected immediately, without queuing or changing $n$. With independent unit-rate [exponential distributions](../../../../../exponential-distribution.md) for holding times, the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md) makes $n$ a [continuous-time Markov chain](../../../../../continuous-time-markov-chain.md), whose nonzero off-diagonal [transition rates](../../../../../transition-intensity.md) are

$$
\boxed{q(n,n+e_r)=\nu_r\quad(n+e_r\in S(C)),
\qquad q(n,n-e_r)=n_r\quad(n_r>0).}
$$

There are $n_r$ independent clocks of rate one for the second transition. Rejected arrivals are not jumps and do not appear in the off-diagonal [transition rates](../../../../../transition-intensity.md).

Let $a(n)=\prod_r\nu_r^{n_r}/n_r!$. For every feasible adjacent pair,

$$
a(n)\nu_r=a(n+e_r)(n_r+1).
$$

Thus [detailed balance for a continuous-time Markov chain](../../../../../detailed-balance-for-a-continuous-time-markov-chain.md) gives the [product-form stationary distribution of a loss network](../../../../../product-form-stationary-distribution-of-a-loss-network.md):

$$
\boxed{\pi(n)=G(C)\prod_r\frac{\nu_r^{n_r}}{n_r!},\qquad
G(C)=\left[\sum_{n\in S(C)}\prod_r\frac{\nu_r^{n_r}}{n_r!}\right]^{-1}.}
$$

In this convention $G(C)$ is the reciprocal normalizing sum. If every route consumes some resource, finite capacities make $S(C)$ finite. Even zero-resource routes cause no normalization difficulty: the sum is at most $\exp(\sum_r\nu_r)$. With positive arrival rates the reachable feasible class is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md), since calls can depart to the empty state and any feasible occupancy can be built from it. The [stationary distribution](../../../../../stationary-distribution.md) is therefore unique on that class.

The vector $m=C-An$ records the free units of each resource. Its [probability distribution](../../../../../probability-distribution.md) $\pi'(m)$ sums $\pi(n)$ over all occupancies with the same free resources. The map from $n$ to $m$ generally loses information: different call mixtures may consume exactly the same resources.

For $\pi'(m)>0$, the [conditional expectation](../../../../../conditional-expectation.md) can be computed by removing one call. The factorial identity $n_r\pi(n)=\nu_r\pi(n-e_r)$ gives

$$
\sum_{n:\,An=C-m} n_r\pi(n)
=\begin{cases}
\nu_r\pi'(m+Ae_r),&Ae_r\leq C-m,\\
0,&\text{otherwise}.
\end{cases}
$$

Indeed, $n\mapsto n-e_r$ is a bijection from the occupancies in this sum with $n_r>0$ to occupancies using $C-m-Ae_r$ units. Conversely, adding one call to any such occupancy is feasible because its final resource use is $C-m$. Consequently

$$
\boxed{\mathbb E[n_r\mid m]=
\frac{\nu_r\pi'(m+Ae_r)}{\pi'(m)}
\quad\text{if }Ae_r\leq C-m,}
$$

and the [conditional expectation](../../../../../conditional-expectation.md) is zero otherwise. Conditioning the identity $\sum_r A_{jr}n_r=C_j-m_j$ and multiplying by $\pi'(m)$ now yields

$$
\boxed{(C_j-m_j)\pi'(m)=
\sum_{r:\,Ae_r\leq C-m}A_{jr}\nu_r\pi'(m+Ae_r).}
$$

Alternatively, multiply the preceding unnormalized factorial identity by $A_{jr}$ and sum over $r$ directly; this proves the same formula even when $\pi'(m)=0$, without dividing by a zero [probability](../../../../../probability.md). This gives both the [conditional expectation](../../../../../conditional-expectation.md) argument and the direct summation argument.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 213](../../paper-213-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
