<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The joint law is the [Edwards-Sokal coupling](../../../../../edwards-sokal-coupling.md). For a fixed spin configuration, the sum over each [edge](../../../../../edge-of-a-graph.md) state contributes $(1-p)+p\delta_e(\sigma)$. Since $\delta_e$ is either zero or one, setting $\beta=-\log(1-p)$ gives

$$
(1-p)+p\delta_e(\sigma)=(1-p)e^{\beta\delta_e(\sigma)}.
$$

Consequently the spin [marginal distribution](../../../../../marginal-distribution.md) is the [Potts measure](../../../../../potts-model.md)

$$
\boxed{\mu_1(\sigma)=\frac1{Z'}\exp\left(\beta\sum_{e\in E}\delta_e(\sigma)\right),
\qquad e^{-\beta}=1-p,\qquad Z'=\frac{Z}{(1-p)^{|E|}}}.
$$

This follows from a finite sum that factorizes over [edges](../../../../../edge-of-a-graph.md), without any [independence](../../../../../independent-random-variables.md) assumption on the spin marginal.

For a fixed [edge](../../../../../edge-of-a-graph.md) configuration, the joint weight vanishes unless the spins agree across every open [edge](../../../../../edge-of-a-graph.md), equivalently unless they are constant on each open [percolation cluster](../../../../../percolation-cluster.md). Each of the $k(\omega)$ clusters, including [isolated vertices](../../../../../isolated-vertex.md), may independently be assigned any of $q$ colors. Thus exactly $q^{k(\omega)}$ spin configurations have nonzero weight, and their common weight is the [edge](../../../../../edge-of-a-graph.md)-product factor divided by $Z$. The [edge](../../../../../edge-of-a-graph.md) [marginal distribution](../../../../../marginal-distribution.md) is therefore the [random-cluster measure](../../../../../random-cluster-model.md)

$$
\boxed{\mu_2(\omega)=\frac1Z\left[\prod_{e\in E}p^{\omega(e)}(1-p)^{1-\omega(e)}\right]q^{k(\omega)}}.
$$

In this convention $Z''=Z$. Dividing the joint mass by this positive marginal gives the [conditional distribution](../../../../../conditional-distribution.md)

$$
\boxed{\mu(\sigma\mid\omega)=q^{-k(\omega)}
\mathbf1\{\sigma\text{ is constant on every open cluster}\}}.
$$

Equivalently the clusters receive independent uniformly chosen colors. Conversely, conditionally on the spins, [edges](../../../../../edge-of-a-graph.md) are independent: an unequal-spin [edge](../../../../../edge-of-a-graph.md) must be closed, while an equal-spin [edge](../../../../../edge-of-a-graph.md) is open with [probability](../../../../../probability.md) $p$. These two conditional descriptions explain the [Edwards-Sokal coupling](../../../../../edwards-sokal-coupling.md) directly.

If $x$ and $y$ lie in the same open cluster, their conditional spin-equality [probability](../../../../../probability.md) is one. If they lie in different clusters, their two independent uniform colors agree with [probability](../../../../../probability.md) $1/q$. Averaging over the [random-cluster measure](../../../../../random-cluster-model.md) yields

$$
\mu_1(\sigma(x)=\sigma(y))
=\mu_2(x\leftrightarrow y)+\frac1q\bigl[1-\mu_2(x\leftrightarrow y)\bigr],
$$

and hence the [spin-connectivity identity for the Potts model](../../../../../spin-connectivity-identity-for-the-potts-model.md)

$$
\boxed{\mu_1(\sigma(x)=\sigma(y))-\frac1q
=\left(1-\frac1q\right)\mu_2(x\leftrightarrow y)}.
$$

The identity also includes $x=y$, when connectivity and spin equality are both certain.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
