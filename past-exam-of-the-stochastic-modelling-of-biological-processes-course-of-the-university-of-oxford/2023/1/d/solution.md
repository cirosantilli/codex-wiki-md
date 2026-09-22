<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [product-Poisson stationary distribution](../../../../product-poisson-stationary-distribution.md) is suggested by balancing the three reaction fluxes around the directed cycle of [reaction complexes](../../../../reaction-complex.md). If their [mean](../../../../expected-value-split.md) counts are $a,b$, this [complex balance](../../../../complex-balance.md) condition is

$$
2=\frac a2=ab,
$$

which gives $a=4$ and $b=1/2$. This suggests the [joint probability mass function](../../../../joint-probability-mass-function.md)

$$
\pi(n,m)=e^{-9/2}\frac{4^n}{n!}\frac{(1/2)^m}{m!},\qquad n,m\geq0.
$$

It is normalized because it is the product of two [Poisson distributions](../../../../poisson-distribution.md). We verify it directly in the [chemical master equation](../../../../chemical-master-equation.md), rather than assuming a [product-Poisson stationary distribution](../../../../product-poisson-stationary-distribution.md) theorem. The three incoming terms satisfy

$$
\begin{aligned}
2\pi(n-1,m)&=\frac n2\pi(n,m),\\
\frac n2\pi(n,m-1)&=nm\pi(n,m),\\
(n+1)(m+1)\pi(n+1,m+1)&=2\pi(n,m).
\end{aligned}
$$

With negative-index values set to zero, these identities also hold on the axes. Their sum equals $(2+n/2+nm)\pi(n,m)$, precisely the outgoing [probability](../../../../probability.md) flux. The stationary average total exit rate is $2+\mathbb E_\pi n/2+\mathbb E_\pi(nm)=6<\infty$, so these [stationary balance equations](../../../../global-balance-for-a-continuous-time-markov-chain.md) do define an [invariant distribution of a continuous-time Markov chain](../../../../invariant-distribution-of-a-continuous-time-markov-chain.md) for the nonexplosive model verified below. This is [complex balance](../../../../complex-balance.md); it does not assert pairwise [detailed balance](../../../../detailed-balance.md) for the irreversible [chemical reactions](../../../../chemical-reaction-split.md).

To identify this [invariant distribution](../../../../stationary-distribution.md) with the limiting [probability distribution](../../../../probability-distribution-split.md) in the question, first check that the model is a [nonexplosive continuous-time Markov chain](../../../../nonexplosive-continuous-time-markov-chain.md). On any finite time interval, $A_1$ is bounded by its initial count plus the finite number of arrivals in a rate-$2$ [Poisson process](../../../../poisson-process-split.md). Conditional on that bound, the rate of producing $A_2$ is bounded, so only finitely many such productions occur. The number of joint removals cannot exceed the available molecules. Thus only finitely many [chemical reactions](../../../../chemical-reaction-split.md) occur in finite time.

The [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md) is also an [irreducible Markov chain](../../../../irreducible-markov-chain.md). From a [Markov chain state](../../../../markov-chain-state.md) with both counts positive, repeated joint removals reduce both. On the $A_2=0$ axis, producing one $A_2$ and then removing a pair reduces $A_1$ by one. On the $A_1=0$ axis, adding one $A_1$ and then removing a pair reduces $A_2$ by one. Each prescribed finite sequence has positive [probability](../../../../probability.md), so every [Markov chain state](../../../../markov-chain-state.md) reaches $(0,0)$. Conversely, arrivals followed by productions reach any $(n,m)$ with $n>0$; to reach $(0,m)$, reach $(1,m+1)$ and remove one pair. The [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md) is therefore [positive recurrent](../../../../positive-recurrent-markov-chain.md), and the [continuous-time Markov chain convergence theorem](../../../../continuous-time-markov-chain-convergence-theorem.md) gives $\phi=\pi$ from the empty [initial condition](../../../../initial-condition.md).

The two [Poisson](../../../../poisson-distribution.md) factors happen to have cancelling numerical coefficients at $(2,2)$:

$$
\boxed{\phi(2,2)=e^{-9/2}\frac{4^2}{2!}\frac{(1/2)^2}{2!}=e^{-9/2}.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
