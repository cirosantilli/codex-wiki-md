<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Identify a configuration with its set $S$ of open [edges](../../../../../../edge-of-a-graph.md). Let $k(S)$ count the [connected components of a graph](../../../../../../component-graph-theory.md) on the full [graph vertex](../../../../../../vertex-graph-theory.md) set, including isolated [graph vertices](../../../../../../vertex-graph-theory.md). The [random-cluster measure](../../../../../../random-cluster-model.md) is

$$
\mu_{p,q}(S)=\frac1{Z_{p,q}}p^{|S|}(1-p)^{|E|-|S|}q^{k(S)}.
$$

For $p\in(0,1)$ and finite $q\ge1$ all its weights are positive. We compare $1\le q_1\le q_2$, taking $\mu_1=\mu_{p,q_1}$ and $\mu_2=\mu_{p,q_2}$.

The key fact is [supermodularity of graph component count](../../../../../../supermodularity-of-graph-component-count.md):

$$
k(S\cap T)+k(S\cup T)\ge k(S)+k(T).
$$

To prove it, orient the graph [edges](../../../../../../edge-of-a-graph.md) arbitrarily and let $U_S$ be the real span of their incidence vectors for [edges](../../../../../../edge-of-a-graph.md) in $S$. Its [dimension of a vector space](../../../../../../dimension-vector-space.md) is $r(S)=|V|-k(S)$: on each [connected component of a graph](../../../../../../component-graph-theory.md) these vectors span the vectors whose coordinates sum to zero. Since $U_{S\cup T}=U_S+U_T$ and $U_{S\cap T}\subset U_S\cap U_T$, the [dimension formula for a sum of subspaces](../../../../../../dimension-formula-for-a-sum-of-subspaces.md) gives

$$
r(S\cup T)+r(S\cap T)\le r(S)+r(T),
$$

which is exactly the component-count inequality.

Put $a=k(S)-k(S\cup T)\ge0$ and $b=k(S\cap T)-k(T)\ge0$. The preceding inequality gives $b\ge a$. In the ratio of the two sides of [Holley's condition](../../../../../../holley-condition.md), the normalization constants and Bernoulli [edge](../../../../../../edge-of-a-graph.md) factors cancel, because $|S\cup T|+|S\cap T|=|S|+|T|$. The ratio is therefore

$$
\frac{\mu_1(S\cup T)\mu_2(S\cap T)}{\mu_1(S)\mu_2(T)}
=q_1^{-a}q_2^b
=\left(\frac{q_2}{q_1}\right)^a q_2^{b-a}\ge1.
$$

By the [Holley inequality](../../../../../../holley-inequality.md), $\mu_{p,q_1}$ [stochastically dominates](../../../../../../stochastic-domination-of-probability-measures.md) $\mu_{p,q_2}$. Thus **increasing [cluster weight](../../../../../../cluster-weight-in-the-random-cluster-model.md) suppresses every [increasing event](../../../../../../increasing-event.md)**:

$$
\boxed{\mu_{p,q_1}(A)\ge\mu_{p,q_2}(A)\quad(q_1\le q_2).}
$$

The [random-cluster single-edge conditional probability](../../../../../../random-cluster-single-edge-conditional-probability.md) confirms the mechanism: it is $p$ when the endpoints are already connected, and $p/(p+q(1-p))$ otherwise. Larger $q$ favours configurations with more separate components. The condition $q\ge1$ enters explicitly in the last factor $q_2^{b-a}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
