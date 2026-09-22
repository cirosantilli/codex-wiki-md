<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $o(\omega)$ be the number of open [edges](../../../../../edge-of-a-graph.md), $k(\omega)$ the number of connected components in the open subgraph, counting isolated vertices, and $m=|E|$. Summing the joint weight over [spins](../../../../../spin.md) requires a constant [spin](../../../../../spin.md) on every open component. There are exactly $q^{k(\omega)}$ choices. Thus the [edge](../../../../../edge-of-a-graph.md) marginal is

$$
\boxed{\phi_{p,q}(\omega)=\frac1{Z_{\rm RC}}p^{o(\omega)}(1-p)^{m-o(\omega)}q^{k(\omega)}}.
$$

This is the [random-cluster measure](../../../../../random-cluster-model.md), and the joint normalizing constant is $Z_{\rm RC}$.

Summing instead over [edge](../../../../../edge-of-a-graph.md) configurations factors independently over [edges](../../../../../edge-of-a-graph.md). For a fixed [spin](../../../../../spin.md) configuration the resulting weight is

$$
\prod_{\{x,y\}\in E}\left[(1-p)+p\mathbf1_{\sigma_x=\sigma_y}\right]
=e^{-\beta m}\exp\left(\beta\sum_{\{x,y\}\in E}\mathbf1_{\sigma_x=\sigma_y}\right),
$$

since $1-p=e^{-\beta}$. The factor $e^{-\beta m}$ is independent of the [spins](../../../../../spin.md). Hence the [spin](../../../../../spin.md) marginal is exactly the ferromagnetic [Potts measure](../../../../../potts-model.md) in the convention

$$
\boxed{\pi_{\beta,q}(\sigma)=\frac1{Z_{\rm P}}\exp\left(\beta\sum_{\{x,y\}\in E}\mathbf1_{\sigma_x=\sigma_y}\right),\qquad p=1-e^{-\beta}}.
$$

Its [partition function](../../../../../canonical-partition-function.md) satisfies $Z_{\rm RC}=e^{-\beta m}Z_{\rm P}$.

Conditionally on $\sigma$, [edge](../../../../../edge-of-a-graph.md) states are independent: an [edge](../../../../../edge-of-a-graph.md) with different endpoint [spins](../../../../../spin.md) is closed with [probability](../../../../../probability.md) one, while one with equal endpoint [spins](../../../../../spin.md) is open with [probability](../../../../../probability.md) $p$. Conditionally on $\omega$, color its $k(\omega)$ open components independently and uniformly from $\{1,\ldots,q\}$. Equivalently, every compatible [spin](../../../../../spin.md) configuration has [conditional probability](../../../../../conditional-probability.md) $q^{-k(\omega)}$, and all incompatible configurations have [probability](../../../../../probability.md) zero. These are the two conditional laws of the [Edwards-Sokal coupling](../../../../../edwards-sokal-coupling.md).

If $x,y$ belong to the same open component, their colors agree surely; otherwise the two independent component colors agree with [probability](../../../../../probability.md) $1/q$. Therefore

$$
\pi_{\beta,q}(\sigma_x=\sigma_y)
=\phi_{p,q}(x\leftrightarrow y)+\frac1q\left(1-\phi_{p,q}(x\leftrightarrow y)\right).
$$

Rearranging proves the [spin-connectivity identity for the Potts model](../../../../../spin-connectivity-identity-for-the-potts-model.md):

$$
\boxed{\left(1-\frac1q\right)\phi_{p,q}(x\leftrightarrow y)
=\pi_{\beta,q}(\sigma_x=\sigma_y)-\frac1q}.
$$

[Phase transitions](../../../../../phase-transition.md) refer to infinite-volume limits, not a single finite graph. The identity shows that connectivity is exactly the excess [spin](../../../../../spin.md) agreement above its independent-color baseline. More directly, use a wired [random-cluster boundary condition](../../../../../random-cluster-boundary-condition.md) and fix the corresponding boundary [spin](../../../../../spin.md) to color $1$. Its component has color $1$, while every finite component has a uniform color. In the compatible infinite-volume [coupling](../../../../../coupling.md),

$$
\pi^1_{\beta,q}(\sigma_0=1)
=\frac1q+\left(1-\frac1q\right)\phi^{\rm w}_{p,q}(0\leftrightarrow\infty).
$$

Consequently normalized [spontaneous magnetization](../../../../../spontaneous-magnetization.md) is

$$
\boxed{M(\beta)=\frac{q\pi^1_{\beta,q}(\sigma_0=1)-1}{q-1}
=\theta^{\rm w}(p,q)}.
$$

The onset of a wired infinite cluster and the onset of [spontaneous magnetization](../../../../../spontaneous-magnetization.md) in the [Potts model](../../../../../potts-model.md) are the same transition under $p=1-e^{-\beta}$, giving $\beta_c(q)=-\log(1-p_c(q))$. This also transfers any jump or continuity of that order parameter between the two descriptions; it makes no assumption about behavior exactly at the critical point.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
