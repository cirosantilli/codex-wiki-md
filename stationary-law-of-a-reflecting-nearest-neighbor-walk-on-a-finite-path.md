# Stationary law of a reflecting nearest-neighbor walk on a finite path

↑ **Parent:** [Stationary distribution](stationary-distribution.md)

On states $0,\ldots,m$, take an interior step of $+1$ or $-1$ with probability $p$ each and hold with probability $1-2p$. At an endpoint take the inward step with probability $2p$ and hold with probability $1-2p$. For $m\geq1$ and $0<p\leq1/2$, the chain is [irreducible](irreducible-markov-chain.md) and its [stationary distribution](stationary-distribution.md) has endpoint weights $1/(2m)$ and interior weights $1/m$.

[Detailed balance](detailed-balance.md) proves this: the doubled inward endpoint transition requires its stationary mass to be half that of an adjacent interior point, and all interior points have equal mass. The total unnormalized weight is $1+2(m-1)+1=2m$. For $m=1$ there are just two equal endpoint masses.

When $p<1/2$, positive self-loops make the chain [aperiodic](aperiodic-markov-chain.md), so its transition probabilities converge to this law. At $p=1/2$ every move changes parity and two-step returns are possible, giving period two and no such convergence from a fixed starting state. At $p=0$ every state is absorbing and uniqueness of the stationary law is lost.

## ↑ Ancestors (8)

1. [Stationary distribution](stationary-distribution.md)
2. [Markov chain](markov-chain-split.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2008/m/m2/solution.md)
