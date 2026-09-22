<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [probability distributions](../../../../../../probability-distribution.md) on a finite [set](../../../../../../set-split.md), the [total variation distance](../../../../../../total-variation-distance.md) is

$$
\|\mu-\nu\|_{\mathrm{TV}}=\max_{A\subseteq S}|\mu(A)-\nu(A)|=\frac12\sum_{z\in S}|\mu(z)-\nu(z)|.
$$

The equality follows by taking $A=\{z:\mu(z)\geq\nu(z)\}$: the positive and negative parts of $\mu-\nu$ have the same mass, since its total mass is zero.

Use the [stationary distribution](../../../../../../stationary-distribution.md) identity $\pi P^t=\pi$. For each initial state $x$,

$$
P^t(x,\cdot)-\pi=\sum_y\pi(y)\bigl(P^t(x,\cdot)-P^t(y,\cdot)\bigr).
$$

The [triangle inequality](../../../../../../triangle-inequality.md) for [total variation distance](../../../../../../total-variation-distance.md), followed by the definition of the [pairwise mixing diameter](../../../../../../pairwise-mixing-diameter.md), gives

$$
\|P^t(x,\cdot)-\pi\|_{\mathrm{TV}}\leq\sum_y\pi(y)\bar d(t)=\bar d(t).
$$

Taking the maximum over $x$ proves $\boxed{d(t)\leq\bar d(t)}$. This particular inequality only needs a [stationary distribution](../../../../../../stationary-distribution.md); it does not require an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) or an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
