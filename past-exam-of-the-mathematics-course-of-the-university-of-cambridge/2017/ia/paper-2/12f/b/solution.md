<h1 id="12f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The vertices visited by a [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) form an integer interval: nearest-neighbour steps cannot skip a vertex. At the [stopping time](../../../../../../stopping-time.md) $T_k$, write that interval as $[\ell,r]$, with $r-\ell+1=k$. The walk is at one of its endpoints, because the $k$th new vertex must extend the earlier interval. This also covers $k=1$, when both endpoints coincide.

The [Strong Markov property](../../../../../../strong-markov-property.md) restarts the walk from this endpoint. Visiting a new vertex is exactly exiting $[\ell,r]$, or reaching $\ell-1$ or $r+1$. Translate these absorbing boundaries to $0,k+1$. The starting point becomes either $1$ or $k$, so the [expected duration of symmetric gambler's ruin](../../../../../../expected-duration-of-symmetric-gambler-s-ruin.md) is $k$ in both cases. Taking [conditional expectations](../../../../../../conditional-expectation.md) and then [expected values](../../../../../../expected-value.md) gives the [expected time to expand a random-walk range](../../../../../../expected-time-to-expand-a-random-walk-range.md):

$$
\boxed{\mathbb E[T_{k+1}-T_k]=k.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
