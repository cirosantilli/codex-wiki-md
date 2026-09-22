<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Start the [random-to-top card shuffle](../../../../../random-to-top-card-shuffle.md) from a fixed ordering and let $T$ be the first time every card has been selected. Once a card has been selected, its location relative to the other selected cards is determined by their most recent selection times. At $T$ these times have a uniformly random strict order, so the deck is uniform and independent of the event $\{T=t\}$. Thus $T$ is a [strong stationary time](../../../../../strong-stationary-time.md), and

$$
d_{\mathrm{TV}}(t)\leq\mathbb P(T>t).
$$

The [coupon collector problem](../../../../../coupon-collector-problem.md) gives $T=n\log n+O_{\mathbb P}(n)$, so for $c\to\infty$,

$$
d_{\mathrm{TV}}(n\log n+cn)\longrightarrow0.
$$

Before all cards have been selected, the unselected cards form the bottom block of the deck in their original relative order. At time $n\log n-cn$, with $c\to\infty$ sufficiently slowly, the number $U$ of unselected cards tends to infinity in probability. Choose $k\to\infty$ with $\mathbb P(U\geq k)\to1$. The bottom $k$ cards are then in their original relative order, whereas under the uniform distribution this has probability $1/k!$. Hence

$$
d_{\mathrm{TV}}(n\log n-cn)\longrightarrow1.
$$

The random-to-top shuffle therefore has [cutoff for Markov chains](../../../../../cutoff-for-markov-chains.md) at $n\log n$ with window $O(n)$.

The [top-to-random card shuffle](../../../../../top-to-random-card-shuffle.md) is the time reversal of the [random-to-top card shuffle](../../../../../random-to-top-card-shuffle.md) under the uniform stationary distribution. Equivalently, their step distributions on the symmetric group are carried into one another by permutation inversion, which preserves total variation from uniform. Their mixing profiles agree, so **top-to-random has the same cutoff at $n\log n$ with window $O(n)$**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 215](../../paper-215-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
