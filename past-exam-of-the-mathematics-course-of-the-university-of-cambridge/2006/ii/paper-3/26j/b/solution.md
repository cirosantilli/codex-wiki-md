<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Restrict to the positive-weight support. From a state $\theta$, propose $\theta'$ according to $q(\theta,\theta')$ and accept with probability

$$
\alpha(\theta,\theta')=\min\left(1,\frac{w(\theta')q(\theta',\theta)}{w(\theta)q(\theta,\theta')}\right).
$$

Otherwise stay at $\theta$. For distinct states, the accepted transition kernel satisfies

$$
\pi(\theta)P(\theta,\theta')=\min\{\pi(\theta)q(\theta,\theta'),\pi(\theta')q(\theta',\theta)\}=\pi(\theta')P(\theta',\theta).
$$

Thus [detailed balance](../../../../../../detailed-balance.md) holds, and summing over $\theta$ proves stationarity. Irreducibility of the accepted kernel makes this [stationary distribution](../../../../../../stationary-distribution.md) unique. Proposal irreducibility by itself is insufficient if proposed edges have zero reverse probability and are always rejected.

For convergence of the distribution from an arbitrary start, also require aperiodicity, which can always be supplied by making the chain lazy. In a finite irreducible aperiodic chain, some power $P^m$ has all entries positive. Its rows then share a fixed positive probability component, so repeated application contracts total variation distance geometrically. This proves that the chain's distribution approaches $\pi$.

The stronger fact needed for averages is

$$
\boxed{\frac1M\sum_{j=1}^Mh(\Theta_j)\longrightarrow\sum_\theta\pi(\theta)h(\theta)\quad\text{almost surely}.}
$$

One can justify this directly by returns to a chosen state. Successive excursions are independent identically distributed cycles by the [Strong Markov property](../../../../../../strong-markov-property.md). In a finite irreducible chain, return times have finite mean: from every state there is a path of uniformly bounded length and uniformly positive probability to the chosen state, giving a geometric tail bound. Apply the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) to cycle lengths and accumulated rewards. Their ratio converges; the mean visits per cycle, normalized by the mean cycle length, form a [stationary distribution](../../../../../../stationary-distribution.md) and hence equal $\pi$. The unfinished final cycle is negligible. This proves the displayed average law, even when the chain is periodic. **Under these conditions, Metropolis–Hastings delivers the required posterior expectations.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
