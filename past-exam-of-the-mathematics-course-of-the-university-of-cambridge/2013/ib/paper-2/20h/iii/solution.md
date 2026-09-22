<h1 id="20h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For an active monster, independence gives

$$
\mathbb P(\text{capture})\leq\sum_{n\geq0}\mathbb P_{(100,0)}(X_n=0)\mathbb P_{(0,100)}(Y_n=0).
$$

Both probabilities vanish before time $100$ and at odd times. By convolution and [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md), $p_{2m}(a,0)\leq p_{2m}(0,0)<1/m$: indeed, write the $2m$-step probability as the inner product of two translates of the $m$-step probability mass function. Therefore

$$
\boxed{0<\mathbb P(\text{active capture})\leq\sum_{m\geq50}\frac1{m^2}<\frac1{49}<1.}
$$

Positivity follows by prescribing $100$ simultaneous steps taking both walkers straight to the origin; that event has probability $4^{-200}$. An active monster thus leaves a positive escape probability.

For a sleepy monster, the [origin capture by a sufficiently sleepy planar random walk](../../../../../../origin-capture-by-a-sufficiently-sleepy-planar-random-walk.md) can be proved using the printed schedule: during $I_j=\{n_j+1,\ldots,n_{j+1}\}$ it occupies $Y_{j+1}$. For any $M$, let $J_M$ be the first $j\geq M$ with $Y_{j+1}=0$. [Markov-chain recurrence](../../../../../../recurrent-markov-chain.md) of $Y$ makes $J_M$ finite almost surely, and it is independent of $X$. By conditioning on $J_M$ and using the stated block bound,

$$
\mathbb P(\text{some capture in a block }j\geq M)\geq\mathbb P(X\text{ visits }0\text{ in }I_{J_M})>\tfrac12.
$$

As $M\to\infty$, continuity of probability for decreasing events shows that the event $C_\infty$ of infinitely many simultaneous origin visits has probability at least $1/2$. Regard the independent trajectories as continuing even after a possible first capture.

To turn this into probability one, use the [eventual coupling of planar symmetric random walks](../../../../../../eventual-coupling-of-planar-symmetric-random-walks.md); the block events need not be independent. Two planar [simple symmetric random walks](../../../../../../simple-symmetric-random-walk.md) begun at sites of the same parity can be coupled to agree eventually. Run them independently until they meet. Their difference walk is [irreducible](../../../../../../irreducible-representation.md) on the even-parity sublattice, and its $m$-step return probability is $p_{2m}(0,0)$, by convolution and symmetry. The preceding divergent-series criterion makes this difference walk a [recurrent Markov chain](../../../../../../recurrent-markov-chain.md), so it hits zero almost surely. After that [stopping time](../../../../../../stopping-time.md), use identical increments for both copies, preserving their marginal laws by the [Strong Markov property](../../../../../../strong-markov-property.md).

Fix any finite calendar time $N$ and any two possible histories up to that time. Corresponding princess positions have the same parity, as do the corresponding monster positions at its internal walk time. Apply the eventual [probabilistic coupling](../../../../../../coupling.md) separately to the two princess futures and the two monster futures, keeping the princess and monster walks independent in each pair. Both the calendar clock and the monster's internal clock tend to infinity. Hence after a finite calendar time the two pairs of trajectories agree, so either both realize $C_\infty$ or neither does. The conditional probability of $C_\infty$ is therefore the same for every possible finite history.

Consequently $\mathbb E(\mathbf1_{C_\infty}\mid\mathcal F_N)=\mathbb P(C_\infty)$ for every $N$. By the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md), these conditional expectations converge to $\mathbf1_{C_\infty}$ as the histories exhaust the trajectories. Thus $\mathbb P(C_\infty)$ is zero or one. Since it is at least $1/2$, it is one. In particular,

$$
\boxed{\mathbb P(\text{sleepy capture})=1.}
$$

This argument uses the supplied unconditional block probabilities; it does not silently strengthen them to conditional probabilities given past failures.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
