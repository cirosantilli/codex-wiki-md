<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $c>0$ and $e>0$, as required for the displayed sparse scaling and the later normalization. A [strictly balanced graph](../../../../../strictly-balanced-graph.md) satisfies $e(F)/v(F)<e/v$ for every proper nonempty [subgraph](../../../../../subgraph.md) $F\subset H$. This forces $H$ to be connected and to have no isolated [vertices](../../../../../vertex-graph-theory.md): otherwise a component of at least the average density, or deletion of the isolated [vertices](../../../../../vertex-graph-theory.md), violates strict balance. Copies here are [subgraphs](../../../../../subgraph.md), not induced [subgraphs](../../../../../subgraph.md).

For fixed $r$, the [factorial moment](../../../../../factorial-moment.md) $\mathbb E_r(X_H)$ counts ordered $r$-tuples of distinct copies all present in the [binomial random graph](../../../../../binomial-random-graph.md). The contribution of vertex-disjoint copies is exactly

$$
\frac{(n)_{rv}}{a^r}p^{re}\longrightarrow\left(\frac{c^e}{a}\right)^r.
$$

The factor $a^{-r}$ removes the multiple embeddings of each copy coming from its [graph automorphisms](../../../../../graph-automorphism.md). For an overlapping tuple, let $U$ be its union. There are $O(n^{v(U)})$ placements of each fixed union type, and the [probability](../../../../../probability.md) its [edges](../../../../../edge-of-a-graph.md) are present is $p^{e(U)}$. When adding a copy meeting the earlier union in $f$ [vertices](../../../../../vertex-graph-theory.md) and $g$ [edges](../../../../../edge-of-a-graph.md), the exponent $v(U)-(v/e)e(U)$ changes by

$$
-f+(v/e)g\le0.
$$

It is strictly negative if this intersection is a proper nonempty [subgraph](../../../../../subgraph.md), and zero only for an empty intersection or a whole copy. In particular the first vertex-overlapping copy has a proper nonempty intersection: the preceding copies are vertex-disjoint, and a connected copy contained in their union would have to equal one of them, contrary to distinctness. Its contribution is therefore strictly negative; later additions cannot undo that loss. Only finitely many union types occur for fixed $r$, so their total contribution is $o(1)$. We have proved all the [factorial moment](../../../../../factorial-moment.md) limits, and the allowed [factorial-moment criterion for Poisson convergence](../../../../../factorial-moment-criterion-for-poisson-convergence.md) gives

$$
\boxed{X_H(G(n,cn^{-v/e}))\Rightarrow\operatorname{Po}(c^e/a).}
$$

This is the [Poisson limit for strictly balanced subgraph counts](../../../../../poisson-limit-for-strictly-balanced-subgraph-counts.md).

The pendant-edge [graph](../../../../../graph-split.md) has density $7/5$, whereas its proper $K_4$ core has density $6/4$. Thus **$K_4^+$ is not strictly balanced**. The [complete graph](../../../../../complete-graph.md) $K_4$ is strictly balanced, with 24 [graph automorphisms](../../../../../graph-automorphism.md), so at $p=cn^{-2/3}$ its copy count $Z$ tends to $\operatorname{Po}(c^6/24)$.

Every $K_4^+$ copy has a unique four-vertex clique core and one selected [edge](../../../../../edge-of-a-graph.md) joining it to a fifth [vertex](../../../../../vertex-graph-theory.md). For any four-set $C$, let $D_C$ count the ambient [edges](../../../../../edge-of-a-graph.md) between $C$ and its complement. Then $D_C\sim\operatorname{Bin}(4(n-4),p)$, with [mean](../../../../../expected-value.md) $\mu_n\sim4cn^{1/3}$. It is [independent](../../../../../independent-random-variables.md) of the internal [edges](../../../../../edge-of-a-graph.md) determining whether $C$ is a [clique](../../../../../clique-graph-theory.md). Choose $\delta_n=n^{-1/12}$. A [Chernoff bound](../../../../../chernoff-bound.md) and a [union bound](../../../../../boole-s-inequality.md) give

$$
\Pr\bigl(\exists C:|D_C-\mu_n|>\delta_n\mu_n\bigr)\le2\binom n4\exp(-\delta_n^2\mu_n/3)=o(1).
$$

Therefore, simultaneously for every actual core, its number of pendant extensions is $(1+o(1))4cn^{1/3}$. Extra ambient [edges](../../../../../edge-of-a-graph.md) cause no overcount: each selected seven-edge [subgraph](../../../../../subgraph.md) has exactly one core and one pendant [edge](../../../../../edge-of-a-graph.md). Summing over the cores yields

$$
\frac{X_{K_4^+}}{4cn^{1/3}}=(1+o_{\mathbb P}(1))Z,\qquad \frac{X_{K_4^+}}{4cn^{1/3}}-Z\xrightarrow{\mathbb P}0,
$$

because $Z$ is [uniformly tight](../../../../../uniform-tightness.md). This is the [pendant extensions of sparse clique copies](../../../../../pendant-extensions-of-sparse-clique-copies.md) mechanism. For $0<\varepsilon<1$, neither endpoint of $(k-\varepsilon,k+\varepsilon)$ is an integer, and its only nonnegative integer is $k$. [Convergence in distribution](../../../../../convergence-in-distribution.md) consequently gives

$$
\boxed{\Pr\left(k-\varepsilon<\frac{X_{K_4^+}}{4cn^{1/3}}<k+\varepsilon\right)\longrightarrow e^{-c^6/24}\frac{(c^6/24)^k}{k!}.}
$$

The positive-$c$ assumption matters: the quotient printed in the question is undefined when $c=0$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
