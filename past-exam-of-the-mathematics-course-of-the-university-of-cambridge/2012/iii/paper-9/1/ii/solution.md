<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

It suffices to prove the assertion after replacing $\omega$ by $\min\{\omega,\sqrt{\log n}\}$: that replacement gives a tighter interval. Thus assume $\omega\to\infty$ and $\omega=o(\log n)$, and put

$$
p_\pm=\frac{\log n\pm\omega/2}{2n},\qquad
m_\pm=\frac n4(\log n\pm\omega).
$$

At $p_-$, let $J$ count [isolated vertices](../../../../../../isolated-vertex.md) in $L$. The same [indicator random variable](../../../../../../indicator-random-variable.md) calculation as for all [isolated vertices](../../../../../../isolated-vertex.md) gives

$$
\mathbb EJ=\ell(1-p_-)^{n-1}=(1+o(1))e^{\omega/4}\to\infty,\qquad
\frac{\operatorname{var}J}{(\mathbb EJ)^2}\leq\frac1{\mathbb EJ}+\frac{p_-}{1-p_-}=o(1).
$$

By the [Chebyshev inequality](../../../../../../chebyshev-inequality.md), $J>0$ [with high probability](../../../../../../with-high-probability.md). Since $\ell\geq2$ eventually, the marked [vertices](../../../../../../vertex-graph-theory.md) are then not all connected.

At $p_+$, the [logarithmic-regime giant component](../../../../../../logarithmic-regime-giant-component.md) result applies with $k=2$ and any fixed $\gamma_0\in(1/3,1/2)$. Its unique [giant component](../../../../../../giant-component.md) misses $(1+o(1))n^{1/2}e^{-\omega/4}$ [vertices](../../../../../../vertex-graph-theory.md). On the event that it misses at most twice that number, [exchangeability](../../../../../../exchangeable-random-variables.md) makes the missed vertex set uniform conditional on its size. A [union bound](../../../../../../boole-s-inequality.md) therefore gives

$$
\mathbb P(L\text{ meets the complement of the giant})
\leq o(1)+2\ell n^{-1/2}e^{-\omega/4}=o(1).
$$

Thus all of $L$ is connected at $p_+$ [with high probability](../../../../../../with-high-probability.md).

For the [uniform random graph process](../../../../../../uniform-random-graph-process.md), assign uniform labels to the [edges](../../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../../complete-graph.md) as [independent random variables](../../../../../../independent-random-variables.md) and reveal them in label order. The [binomial random graph](../../../../../../binomial-random-graph.md) $G(n,p)$ is the prefix containing the $M(p)$ labels at most $p$, where $M(p)$ has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $N=\binom n2$ and $p$. Its [variance](../../../../../../variance-split.md) at $p_\pm$ is $O(n\log n)$, whereas the gap between $\mathbb EM(p_\pm)$ and the relevant endpoint $m_\pm$ is $(1+o(1))\omega n/8$. The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) gives $M(p_-)\geq m_-$ and $M(p_+)\leq m_+$ [with high probability](../../../../../../with-high-probability.md), with harmless integer rounding. The [monotone graph property](../../../../../../monotone-graph-property.md) that all marked [vertices](../../../../../../vertex-graph-theory.md) are connected now implies

$$
\boxed{\frac n4(\log n-\omega)\leq\tau\leq\frac n4(\log n+\omega)\quad\text{with high probability}.}
$$

The [marked-set connectivity threshold](../../../../../../marked-set-connectivity-threshold.md) is lower than the threshold for connecting every [vertex](../../../../../../vertex-graph-theory.md), because only about $\sqrt n$ specified [vertices](../../../../../../vertex-graph-theory.md) need to avoid the small [graph components](../../../../../../component-graph-theory.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
