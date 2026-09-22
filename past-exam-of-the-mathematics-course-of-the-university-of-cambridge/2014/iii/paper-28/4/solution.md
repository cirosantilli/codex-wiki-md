<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a finite [graph](../../../../../graph-split.md) $G=(V,E)$, let $o(\omega)=\sum_{e\in E}\omega(e)$, and let $k_G(\omega)$ count connected components of the spanning open subgraph, including isolated [graph vertices](../../../../../vertex-graph-theory.md). The [random-cluster model](../../../../../random-cluster-model.md) with $p\in[0,1]$ and $q>0$ is

$$
\boxed{\phi_{G,p,q}(\omega)=\frac1{Z_{G,p,q}}
 p^{o(\omega)}(1-p)^{|E|-o(\omega)}q^{k_G(\omega)}.}
$$

The [partition function](../../../../../canonical-partition-function.md) $Z_{G,p,q}$ is the sum of these weights over all configurations, making the expression a [probability measure](../../../../../probability-measure.md).

For the lattice box, take all nearest-neighbor [edges](../../../../../edge-of-a-graph.md) with both endpoints in $\Lambda_n$. A [random-cluster boundary condition](../../../../../random-cluster-boundary-condition.md) $\xi$ is a partition of the boundary [graph vertices](../../../../../vertex-graph-theory.md). Vertices in one block are identified, or wired together, before counting components; the identifications do not add random [edges](../../../../../edge-of-a-graph.md). Let $k_\xi(\omega)$ be the number of components of the resulting quotient open graph. Then

$$
\boxed{\phi^{\xi}_{\Lambda_n,p,q}(\omega)=\frac1{Z^{\xi}_{\Lambda_n,p,q}}
 p^{o(\omega)}(1-p)^{|E(\Lambda_n)|-o(\omega)}q^{k_\xi(\omega)}.}
$$

The [free random-cluster boundary condition](../../../../../free-random-cluster-boundary-condition.md) has singleton blocks, while the [wired random-cluster boundary condition](../../../../../wired-random-cluster-boundary-condition.md) has one boundary block. Arbitrary partitions are allowed; no assumption that the partition itself has a planar realization is needed for the monotonicity statement.

Write $\xi\preceq\zeta$ if every block of $\xi$ is contained in a block of $\zeta$, so $\zeta$ makes at least as many identifications. The precise [boundary monotonicity of the random-cluster measure](../../../../../boundary-monotonicity-of-the-random-cluster-measure.md) is

$$
\boxed{\xi\preceq\zeta\quad\Longrightarrow\quad
\phi^{\xi}_{\Lambda_n,p,q}(A)\leq\phi^{\zeta}_{\Lambda_n,p,q}(A)
\text{ for every increasing event }A,\quad q\geq1.}
$$

Equivalently, the expectation of every real-valued [order-preserving function](../../../../../order-preserving-function.md) is larger under the more wired measure. This is [stochastic domination of probability measures](../../../../../stochastic-domination-of-probability-measures.md) on the coordinatewise configuration order.

To prove it, condition on every [edge](../../../../../edge-of-a-graph.md) except $e=\{u,v\}$. If $u,v$ are already connected using those open [edges](../../../../../edge-of-a-graph.md) and the boundary wiring, opening $e$ does not change $k_\xi$, so its conditional open [probability](../../../../../probability.md) is $p$. If they are not connected, opening it reduces $k_\xi$ by one. The ratio of the open weight to the closed weight is then $p/[q(1-p)]$. Thus the [random-cluster single-edge conditional probability](../../../../../random-cluster-single-edge-conditional-probability.md) is

$$
\phi^{\xi}(\omega(e)=1\mid\omega|_{E\setminus\{e\}})=
\begin{cases}
p,&u\leftrightarrow v\text{ without }e\text{, including the wiring},\\
\displaystyle\frac{p}{p+q(1-p)},&u\not\leftrightarrow v\text{ without }e.
\end{cases}
$$

For $q\geq1$ the second number is at most the first. Adding open [edges](../../../../../edge-of-a-graph.md) or making the boundary partition coarser can only turn a disconnected pair into a connected one. Therefore these conditional open [probabilities](../../../../../probability.md) are increasing in both the exterior configuration and the amount of wiring.

Run a [heat-bath Markov chain](../../../../../heat-bath-markov-chain.md) for each boundary partition. At every step choose the same uniformly sampled [edge](../../../../../edge-of-a-graph.md) in both chains, sample the same independent uniform variable $U$, and set that [edge](../../../../../edge-of-a-graph.md) open if $U$ is below its conditional open [probability](../../../../../probability.md). Start both chains at the all-closed configuration. By the preceding inequality, the two configurations remain ordered at every update. Each marginal chain has its corresponding [random-cluster measure](../../../../../random-cluster-model.md) as its [stationary distribution](../../../../../stationary-distribution.md): resampling one coordinate from its conditional distribution preserves that law. Because $0<p<1$ and $q>0$, every update gives both possible states positive [probability](../../../../../probability.md); the finite chain is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md) with [aperiodicity](../../../../../aperiodic-markov-chain.md), and hence converges to its unique [stationary distribution](../../../../../stationary-distribution.md). Taking expectations of any [order-preserving function](../../../../../order-preserving-function.md) and passing to the limit proves the claimed [stochastic domination of probability measures](../../../../../stochastic-domination-of-probability-measures.md). At $q=1$ the two [conditional probabilities](../../../../../conditional-probability.md) agree, and the boundary condition has no effect on the independent [bond percolation](../../../../../bond-percolation-split.md) law.

For the final identity fix a plane embedding of the finite [planar graph](../../../../../planar-graph.md), and include the unbounded face in its [planar dual graph](../../../../../planar-dual-graph.md). In the dual configuration $\bar\omega^*$, a dual [edge](../../../../../edge-of-a-graph.md) is open exactly when its crossed primal [edge](../../../../../edge-of-a-graph.md) is closed. Let $m=o(\omega)$. The spanning open primal subgraph has $|V|$ [graph vertices](../../../../../vertex-graph-theory.md), $m$ [edges](../../../../../edge-of-a-graph.md), and $k(\omega)$ components. The [Euler formula for a connected planar graph](../../../../../euler-formula-for-a-connected-planar-graph.md), applied componentwise with the common exterior face accounted for, gives its number of faces as

$$
f(\omega)=m-|V|+k(\omega)+1.
$$

Deleting a closed primal [edge](../../../../../edge-of-a-graph.md) merges its incident original faces precisely when its dual [edge](../../../../../edge-of-a-graph.md) joins distinct dual components. Consequently the faces of the open primal subgraph correspond exactly to components of the open complementary dual subgraph. This remains true for bridges and loops, with their dual loops and bridges, and for a disconnected primal graph. Thus the [planar cluster-count identity](../../../../../planar-cluster-count-identity.md) is

$$
\boxed{k(\bar\omega^*)=m-|V|+k(\omega)+1.}
$$

At the [self-dual parameter of the random-cluster model](../../../../../self-dual-parameter-of-the-random-cluster-model.md), put $s=\sqrt q$ and

$$
p_{\mathrm{sd}}(q)=\frac{s}{1+s},\qquad
\frac{p_{\mathrm{sd}}}{1-p_{\mathrm{sd}}}=s.
$$

For fixed $G$ the factor $(1-p_{\mathrm{sd}})^{|E|}$ is independent of $\omega$. The weight is therefore proportional to

$$
s^m q^{k(\omega)}=s^{m+2k(\omega)}
=s^{|V|-1}\,s^{k(\omega)+k(\bar\omega^*)}.
$$

Absorbing the remaining graph-dependent factor into the normalization gives the [symmetric cluster weight at the self-dual parameter](../../../../../symmetric-cluster-weight-at-the-self-dual-parameter.md):

$$
\boxed{\phi_{G,p_{\mathrm{sd}}(q),q}(\omega)
\propto(\sqrt q)^{\,k(\omega)+k(\bar\omega^*)}.}
$$

Counting the outer dual face and all isolated primal [graph vertices](../../../../../vertex-graph-theory.md) is essential for the constant in the Euler identity. No assumption that $G$ is self-dual is required for this proportionality.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
