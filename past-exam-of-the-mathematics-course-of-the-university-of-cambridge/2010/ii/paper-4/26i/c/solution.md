<h1 id="26i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $\mu=\lambda$, an excursion after the jump from zero to one visits $n$ before its reset with probability

$$
\prod_{j=1}^{n-1}\frac{j+1}{j+2}=\frac2{n+1}.
$$

This tends to zero, so a catastrophe eventually occurs with probability one. Both the original chain and its [jump chain](../../../../../../jump-chain.md) are recurrent.

The expected number of jumps in a return cycle is

$$
1+\sum_{n\ge1}\frac2{n+1}=\infty.
$$

Thus the [jump chain](../../../../../../jump-chain.md) is **null recurrent**. But its holding time at $n\ge1$ has mean $1/[\lambda(n+2)]$, and the initial holding time at zero has mean $1/\lambda$. The expected elapsed cycle time is

$$
\frac1\lambda+\sum_{n\ge1}\frac2{(n+1)\lambda(n+2)}
=\frac2\lambda<\infty.
$$

The [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) is therefore **positive recurrent**. Its equilibrium distribution, computed as mean time in a state per mean cycle time, is

$$
\boxed{\pi_0=\frac12,\qquad
\pi_n=\frac1{(n+1)(n+2)}\quad(n\ge1).}
$$

The entries sum to one by telescoping. The contrast is explained by progressively shorter holding times at the large states, not by a change in return probabilities.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26I](../../26i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
