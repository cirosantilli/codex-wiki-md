<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $p=p(n)$ and let $T$ be the [triangle count in a binomial random graph](../../../../../../triangle-count-in-a-binomial-random-graph.md). For every three-element [set](../../../../../../set-split.md) $S$ of [vertices](../../../../../../vertex-graph-theory.md), let $I_S$ be the [indicator random variable](../../../../../../indicator-random-variable.md) that its three [edges](../../../../../../edge-of-a-graph.md) are present. Then

$$
T=\sum_{|S|=3}I_S,\qquad \mu=\mathbb ET=\binom n3p^3.
$$

For two distinct triples $S,R$, their [indicator random variables](../../../../../../indicator-random-variable.md) are [independent random variables](../../../../../../independent-random-variables.md) unless they share an [edge](../../../../../../edge-of-a-graph.md). Sharing just one [vertex](../../../../../../vertex-graph-theory.md) still leaves the sets of relevant [edges](../../../../../../edge-of-a-graph.md) disjoint. If they share an [edge](../../../../../../edge-of-a-graph.md), their union has five [edges](../../../../../../edge-of-a-graph.md), and therefore

$$
\operatorname{Cov}(I_S,I_R)=p^5-p^6.
$$

There are $\binom n2\binom{n-2}2$ unordered pairs of distinct [triangles in a graph](../../../../../../triangle-in-a-graph.md) sharing an [edge](../../../../../../edge-of-a-graph.md): choose that [edge](../../../../../../edge-of-a-graph.md), and then choose their two additional [vertices](../../../../../../vertex-graph-theory.md). The [variance of a sum](../../../../../../variance-of-a-sum.md) consequently gives the exact formula

$$
\operatorname{Var}T=\binom n3(p^3-p^6)+2\binom n2\binom{n-2}2(p^5-p^6).
$$

For sufficiently large $n$, the hypothesis $np\to\infty$ ensures $p>0$, so $\mu>0$. Dropping negative terms and simplifying the [binomial coefficients](../../../../../../binomial-coefficient.md),

$$
\frac{\operatorname{Var}T}{\mu^2}\leq\frac{1}{\binom n3p^3}+\frac{18(n-3)}{n(n-1)(n-2)p}
=O\!\left(\frac1{(np)^3}+\frac1{n^2p}\right)\longrightarrow0.
$$

Here $n^2p=n(np)\to\infty$ as well. The event $T\geq2\mu$ implies $|T-\mu|\geq\mu$. Applying the [Chebyshev inequality](../../../../../../chebyshev-inequality.md) from part (i) gives the requested conclusion:

$$
\boxed{\mathbb P\!\left(T\geq2p^3\binom n3\right)\leq\frac{\operatorname{Var}T}{\mu^2}\longrightarrow0.}
$$

Thus the [triangle count](../../../../../../triangle-count.md) is concentrated around its [expectation](../../../../../../expected-value.md) throughout this range of the [binomial random graph](../../../../../../binomial-random-graph.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
