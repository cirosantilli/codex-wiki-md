<h1 id="m/m5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Q=H_N$ and define

$$
\pi_N=\frac1Q,\qquad
\pi_k=\frac1{(k+1)Q}\quad(1\leq k<N).
$$

The probabilities sum to $Q^{-1}(1+\sum_{k=1}^{N-1}(k+1)^{-1})=1$. For $k<N$, the incoming [probability](../../../../../../probability.md) is

$$
(\pi P)_k=\sum_{j=k+1}^{N}\frac{\pi_j}{j}
=\frac1Q\left(\sum_{j=k+1}^{N-1}\frac1{j(j+1)}+\frac1N\right)
=\frac1{(k+1)Q}=\pi_k,
$$

using a telescoping sum. Similarly,

$$
(\pi P)_N=\sum_{j=1}^N\frac{\pi_j}{j}
=\frac1Q\left(\sum_{j=1}^{N-1}\frac1{j(j+1)}+\frac1N\right)
=\frac1Q=\pi_N.
$$

Thus $\pi$ is a [stationary distribution](../../../../../../stationary-distribution.md). Every state can reach $N$ in one step, and $N$ can reach every lower positive state in one step, so the chain is [irreducible](../../../../../../irreducible-markov-chain.md). The self-loop at $N$ has [probability](../../../../../../probability.md) $1/N>0$, hence the chain is [aperiodic](../../../../../../aperiodic-markov-chain.md). The convergence theorem for a finite irreducible aperiodic [Markov chain](../../../../../../markov-chain-split.md) now gives

$$
\boxed{\lim_{n\to\infty}P(X_n=k)=\pi_k.}
$$

For $N=1$, the conclusion follows directly from the single absorbing/refilled state.

This is the limiting law of the [uniform depletion and refill Markov chain](../../../../../../uniform-depletion-and-refill-markov-chain.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
