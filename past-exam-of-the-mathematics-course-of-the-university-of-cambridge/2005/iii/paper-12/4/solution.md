<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Relative to a [filtration](../../../../../filtration-probability-theory.md) $(\mathcal F_i)$, a [martingale](../../../../../martingale-split.md) is an [adapted process](../../../../../adapted-process.md) of integrable [random variables](../../../../../random-variable-split.md) satisfying $\mathbb E[X_i\mid\mathcal F_{i-1}]=X_{i-1}$. With no separate [filtration](../../../../../filtration-probability-theory.md) specified, take the [natural filtration](../../../../../natural-filtration.md) $\sigma(X_0,\ldots,X_i)$. For deterministic increment bounds $|X_i-X_{i-1}|\le c_i$, the [Hoeffding-Azuma inequality](../../../../../azuma-s-inequality.md) states

$$
\boxed{\Pr(|X_n-X_0|\ge t)\le2\exp\left(-\frac{t^2}{2\sum_{i=1}^n c_i^2}\right)\quad(t>0).}
$$

To prove it, let $D_i=X_i-X_{i-1}$. For $c_i>0$, convexity on $[-c_i,c_i]$ gives

$$
e^{sD_i}\le\frac{c_i+D_i}{2c_i}e^{sc_i}+\frac{c_i-D_i}{2c_i}e^{-sc_i}.
$$

Its conditional [expectation](../../../../../expected-value.md) is at most $\cosh(sc_i)\le e^{s^2c_i^2/2}$. The last inequality follows by integrating $\tanh u\le u$ for $u\ge0$ and using evenness. If $c_i=0$ the bound is immediate. Conditional iteration now yields $\mathbb E e^{s(X_n-X_0)}\le\exp(s^2\sum c_i^2/2)$. The exponential [Markov inequality](../../../../../markov-inequality.md), minimized at $s=t/\sum c_i^2$, bounds the upper tail by the displayed exponential without the factor two. Apply it to $-X_i$ and use the [union bound](../../../../../boole-s-inequality.md) for the two-sided assertion. When every $c_i=0$, the deviation [probability](../../../../../probability.md) is zero.

For the [chromatic number of a binomial random graph](../../../../../chromatic-number-of-a-binomial-random-graph.md), put $q=1-p$, $b=1/q>1$, and $L_n=\log_b n$. We prove matching bounds; treating $0<\varepsilon<1$ suffices. A colour class is an [independent set](../../../../../independent-set-graph-theory.md), so $\chi\ge n/\alpha(G)$. For $r=\lceil(2+\delta)L_n\rceil$ with fixed $\delta>0$, the [expected value](../../../../../expected-value.md) of the number of [independent](../../../../../independent-random-variables.md) $r$-sets is

$$
\binom nrq^{\binom r2}\le\exp\left(r\log n-\tfrac12r(r-1)\log b\right)=\exp(-\Theta((\log n)^2))=o(1).
$$

The [first moment method](../../../../../first-moment-method.md) gives $\alpha(G)<r$ with [probability](../../../../../probability.md) tending to one. Choosing $\delta$ sufficiently small then gives $\chi\ge(1-\varepsilon)n/(2L_n)$ for all sufficiently large $n$ on that event.

The upper bound must work uniformly on the adaptive [vertex](../../../../../vertex-graph-theory.md) sets left by a colouring procedure. Set

$$
m=\left\lceil\frac n{(\log n)^2}\right\rceil,\qquad k=\lfloor(2-\delta)\log_b m\rfloor,\qquad0<\delta<1.
$$

For a specified $m$-set $U$, its [complement graph](../../../../../complement-graph.md) has distribution $G(m,q)$. Let $X$ count its $k$-[cliques](../../../../../clique-graph-theory.md), $Y$ count distinct ordered pairs sharing an [edge](../../../../../edge-of-a-graph.md), and $Z$ be the maximum [edge-disjoint clique packing](../../../../../edge-disjoint-clique-packing.md). The allowed clique-count estimates at this value of $k$ give

$$
\mathbb EX=\binom mkq^{\binom k2},\qquad \frac1{\mathbb EX}=o(m^{-2}),\qquad\frac{\mathbb EY}{(\mathbb EX)^2}\le C_{q,\delta}\frac{k^4}{m^2}.
$$

The overlap quantity, if the diagonal is included, has the exact expression $\sum_{j=2}^k\binom kj\binom{m-k}{k-j}q^{-\binom j2}/\binom mk$ after division by $(\mathbb EX)^2$; the same bound holds. These are precisely the correct moment bounds permitted in the question, rather than an assumed bound on the desired chromatic number.

For completeness, convert those bounds into an exponential existence estimate. In the [clique conflict graph](../../../../../clique-conflict-graph.md) the [vertices](../../../../../vertex-graph-theory.md) are the $X$ existing [cliques](../../../../../clique-graph-theory.md), with an [edge](../../../../../edge-of-a-graph.md) between each conflicting pair. A random ordering keeps every [vertex](../../../../../vertex-graph-theory.md) that precedes all its neighbours. No two retained [vertices](../../../../../vertex-graph-theory.md) are adjacent. Their [mean](../../../../../expected-value.md) number is $\sum_v1/(d_v+1)\ge X^2/(X+Y)$ by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Thus, with a zero ratio when $X=0$,

$$
Z\ge\frac{X^2}{X+Y},\qquad\mathbb EZ\ge\frac{(\mathbb EX)^2}{\mathbb EX+\mathbb EY}\ge c\frac{m^2}{k^4}.
$$

The middle inequality follows from $(\mathbb EX)^2\le\mathbb E[X^2/(X+Y)]\,\mathbb E(X+Y)$. Toggling one ambient [edge](../../../../../edge-of-a-graph.md) changes $Z$ by at most one: at most one member of a packing uses it. Reveal the $\binom m2$ [independent](../../../../../independent-random-variables.md) [edges](../../../../../edge-of-a-graph.md) successively and form the [edge-exposure martingale](../../../../../edge-exposure-martingale.md) for $Z$. Coupling the unrevealed [edges](../../../../../edge-of-a-graph.md) identically under the two values of the next [edge](../../../../../edge-of-a-graph.md) shows its conditional [expectations](../../../../../expected-value.md) differ by at most one, hence its increments have magnitude at most one. The one-sided [Hoeffding-Azuma inequality](../../../../../azuma-s-inequality.md) gives

$$
\Pr(X=0)=\Pr(Z=0)\le\exp\left(-\frac{(\mathbb EZ)^2}{2\binom m2}\right)\le\exp(-c' m^2/k^8).
$$

This is [clique-packing amplification of moment bounds](../../../../../clique-packing-amplification-of-moment-bounds.md). A [union bound](../../../../../boole-s-inequality.md) over all $m$-sets is now strong enough:

$$
\Pr(\exists U,\ |U|=m,\ \alpha(G[U])<k)\le2^n\exp(-c'm^2/k^8)\longrightarrow0,
$$

since $m^2/k^8=\Theta(n^2/(\log n)^{12})\gg n$. Thus every such set contains an [independent set](../../../../../independent-set-graph-theory.md) of size $k$. Repeatedly remove and colour one whenever at least $m$ [vertices](../../../../../vertex-graph-theory.md) remain; then colour each of the fewer than $m$ remaining [vertices](../../../../../vertex-graph-theory.md) separately. This [greedy colouring by removing independent sets](../../../../../greedy-colouring-by-removing-independent-sets.md) uses at most

$$
\frac nk+m=\left(\frac2{2-\delta}+o(1)\right)\frac n{2L_n}.
$$

Choose $\delta$ so $2/(2-\delta)<1+\varepsilon$. Combining the two high-probability events proves

$$
\boxed{(1-\varepsilon)\frac n{2\log_{1/q}n}\le\chi(G(n,p))\le(1+\varepsilon)\frac n{2\log_{1/q}n}\quad\text{with probability }1-o(1).}
$$

The uniform subset estimate avoids incorrectly treating a graph-dependent remainder as a fresh [independent](../../../../../independent-random-variables.md) [random graph](../../../../../random-graph.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
