<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every reachable state $i$ reaches zero deterministically in $i$ steps. For $j\in E$, choose a supported lifetime $k>j$; zero can jump to $k-1$ and then count down to $j$. Thus the chain is an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) on $E$. Its positive-probability first return lengths are exactly the support of $Y_1$; all other return lengths are sums of such lengths. Their [greatest common divisor](../../../../../../greatest-common-divisor.md) is therefore one by assumption, so the chain is an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md).

The [equilibrium residual-life distribution](../../../../../../equilibrium-residual-life-distribution.md) is

$$
\pi_j=\frac{\mathbb P(Y_1>j)}\mu,\qquad j\in E.
$$

It is a probability distribution because the tail-sum identity gives $\sum_{j\ge0}\mathbb P(Y_1>j)=\mathbb EY_1=\mu$. With zero masses outside $E$,

$$
(\pi P)_j=\pi_{j+1}+\pi_0\mathbb P(Y_1=j+1)
=\frac{\mathbb P(Y_1>j+1)+\mathbb P(Y_1=j+1)}\mu=\pi_j,
$$

so it is a [stationary distribution](../../../../../../stationary-distribution.md). This also displays why finite mean is needed for normalization.

Use the [countable-state Markov chain convergence theorem](../../../../../../countable-state-markov-chain-convergence-theorem.md): an irreducible, aperiodic, positive recurrent discrete-time chain on a countable state space has a unique stationary distribution and $P^n(i,j)\to\pi_j$ for every pair of states. All hypotheses were verified, including positive recurrence in part (b). Since $X_0=0$ and $\mathbb P(Y_1>0)=1$,

$$
\boxed{\lim_{n\to\infty}\mathbb P(X_n=0)=\pi_0=\frac1\mu.}
$$

The finite-state convergence theorem alone would not suffice when the lifetimes are unbounded. The gcd hypothesis is also necessary for this ordinary limit: deterministic lifetime 2, for example, produces alternating renewal probabilities rather than convergence.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
