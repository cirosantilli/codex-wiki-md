<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $C_x^b$ and $C_x^s$ be the out-clusters in [directed percolation](../../../../../../directed-percolation.md), with the [site percolation](../../../../../../site-percolation-split.md) cluster empty when $x$ is closed. Write $\theta_b(p)=\mathbb P_p(|C_x^b|=\infty)$ and $\chi_b(p)=\mathbb E_p|C_x^b|$, and similarly for [site percolation](../../../../../../site-percolation-split.md). The [survival and susceptibility thresholds for directed percolation](../../../../../../survival-and-susceptibility-thresholds-for-directed-percolation.md) are the infima of the parameters at which these quantities become positive and infinite, respectively.

We construct a [coupling of probability distributions](../../../../../../coupling.md) that compares the whole clusters. First condition the [site percolation](../../../../../../site-percolation-split.md) root to be open. Explore its out-cluster, using a fixed order of the finitely many outgoing bonds at each vertex. When a previously untested vertex $v$ is first encountered along a bond $u\to v$ from an already reached vertex, use a fresh [Bernoulli random variable](../../../../../../bernoulli-distribution.md) of parameter $p$ both for the state of $v$ and for the state of this particular bond. If $v$ is open, add it to the exploration; if it is closed, mark it as tested and never add it. Assign fresh [independent random variables](../../../../../../independent-random-variables.md) of the same parameter to every other bond, including bonds leading to vertices already tested. The choice of the next unassigned bond depends only on previously revealed information. Its assigned coin is therefore independent of that information, so the resulting bond configuration has exactly the product [bond percolation](../../../../../../bond-percolation-split.md) law. Parallel bonds cause no difficulty; loops may be discarded.

Every reached site has an open parent bond leading from a previously reached site. Consequently the conditional [site percolation](../../../../../../site-percolation-split.md) cluster is contained in the [bond percolation](../../../../../../bond-percolation-split.md) cluster. The [connected graph](../../../../../../connected-graph.md) is countable because it is a [locally finite graph](../../../../../../locally-finite-graph.md); taking increasing finite stages of the exploration proves the same containment for infinite clusters. Removing the conditioning on the root gives

$$
\theta_s(p)\le p\theta_b(p),\qquad \chi_s(p)\le p\chi_b(p).
$$

Thus positive [site percolation](../../../../../../site-percolation-split.md) survival implies positive [bond percolation](../../../../../../bond-percolation-split.md) survival at the same parameter, and infinite [percolation susceptibility](../../../../../../percolation-susceptibility.md) for [site percolation](../../../../../../site-percolation-split.md) implies infinite [percolation susceptibility](../../../../../../percolation-susceptibility.md) for [bond percolation](../../../../../../bond-percolation-split.md). Taking the infima in the definitions proves **both comparisons**:

$$
\boxed{p_H^b(\vec\Lambda;x)\le p_H^s(\vec\Lambda;x),\qquad p_T^b(\vec\Lambda;x)\le p_T^s(\vec\Lambda;x).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
