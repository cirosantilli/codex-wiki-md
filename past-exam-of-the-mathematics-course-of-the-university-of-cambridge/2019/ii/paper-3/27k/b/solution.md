<h1 id="27k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $K=N+s$, the total capacity. The customer count is an [M-M-s-K queue](../../../../../../m-m-s-k-queue.md), hence a [birth-death process](../../../../../../birth-death-process.md) on $\{0,1,\ldots,K\}$. Its nonzero transition rates are

$$
q_{n,n+1}=\lambda
\quad(0\leq n<K),
\qquad
q_{n,n-1}=\mu\min(n,s)
\quad(1\leq n\leq K).
$$

The first rate is zero at $K$ because an arrival finding the shop full is rejected. The second rate is the number of busy servers times the individual service rate.

Write $\rho=\lambda/\mu$. The [detailed balance for a birth-death process](../../../../../../detailed-balance-for-a-birth-death-process.md) recursion is

$$
\frac{\pi_n}{\pi_{n-1}}
=\frac{\lambda}{\mu\min(n,s)}.
$$

Therefore

$$
\boxed{\begin{gathered}
\pi_n=\frac{w_n}{Z},
\qquad
w_n=
\begin{cases}
\rho^n/n!,&0\leq n\leq s,\\
\rho^n/(s!s^{n-s}),&s<n\leq K,
\end{cases}
\end{gathered}}
$$

where

$$
Z=\sum_{n=0}^{s}\frac{\rho^n}{n!}
+\frac{\rho^s}{s!}\sum_{j=1}^{N}\left(\frac\rho s\right)^j.
$$

This is the [stationary distribution of an M-M-s-K queue](../../../../../../stationary-distribution-of-an-m-m-s-k-queue.md).

The state space is finite, and every state communicates with every other through successive births and deaths because $\lambda,\mu>0$. The chain is therefore an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md), so its invariant distribution is unique. Finally the adjacent-state identities

$$
\pi_n\lambda
=\pi_{n+1}\mu\min(n+1,s)
$$

are detailed balance, while all nonadjacent rates vanish in both directions. Part a now shows that the queue is reversible in equilibrium.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27K](../../27k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
