<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First prove the concentration statement with its correct scale. Let $U_i=R_i^2$, the $i$th [uniform order statistic](../../../../../../uniform-order-statistic.md). The number of sample points at most $z$ is $B_z\sim\operatorname{Bin}(n,z)$. Therefore $U_i>z$ [means](../../../../../../expected-value.md) $B_z<i$, and $U_i<z$ [means](../../../../../../expected-value.md) $B_z\ge i$, up to probability-zero ties. Take $\varepsilon_n=1/\log n$ and $M=\lceil n^{1/10}\rceil$. Applying [Chernoff bounds](../../../../../../chernoff-bound.md) at $z=(1\pm\varepsilon_n)^2i/n$ gives, for an absolute $c_0>0$ and sufficiently large $n$,

$$
\Pr\left(R_i\notin\left[(1-\varepsilon_n)\sqrt{i/n},(1+\varepsilon_n)\sqrt{i/n}\right]\right)\le2e^{-c_0\varepsilon_n^2i}.
$$

When the upper endpoint exceeds one its upper-tail event is empty. A [union bound](../../../../../../boole-s-inequality.md) makes the total failure [probability](../../../../../../probability.md) for all $M\le i\le n$ at most $2n\exp(-c_0M/(\log n)^2)=o(1)$. On this event,

$$
\sum_{i=M}^n\frac1{R_i}=(1+o(1))\sqrt n\sum_{i=M}^ni^{-1/2}=(2+o(1))n,
$$

where integral comparison gives $\sum_{i=M}^ni^{-1/2}=2\sqrt n+O(\sqrt M)$.

The first [vertex](../../../../../../vertex-graph-theory.md) block has right endpoint $R_1$ and always contains $L_1$, so its initial chord contributes [vertex degree](../../../../../../degree-graph-theory.md) two. All its other endpoints are those $L_i$ with $i\ge2$ that fall below $R_1$. Conditional on the right endpoints, these events are [independent](../../../../../../independent-random-variables.md) with [probabilities](../../../../../../probability.md) $R_1/R_i$. Thus

$$
d_1(n)=2+\sum_{i=2}^n\mathbf1_{\{L_i\le R_1\}},\qquad \mu(R):=\mathbb E[d_1(n)\mid R]=2+R_1\sum_{i=2}^nR_i^{-1},\qquad\operatorname{Var}(d_1(n)\mid R)\le\mu(R).
$$

The fewer than $M$ early summands contribute at most $M=o(\sqrt n)$ to this conditional [mean](../../../../../../expected-value.md). For the rest, the uniform estimate and [uniform tightness](../../../../../../uniform-tightness.md) of $\sqrt nR_1$ give

$$
\frac{\mu(R)}{\sqrt n}-2\sqrt nR_1\xrightarrow{\mathbb P}0.
$$

To control the actual fluctuations without assuming unconditional [independence](../../../../../../independent-random-variables.md), restrict to the concentration event and $\sqrt nR_1\le A$. Then $\mu(R)\le M+2+C A\sqrt n$. Conditional [Chebyshev inequality](../../../../../../chebyshev-inequality.md) bounds the [probability](../../../../../../probability.md) of a deviation exceeding $\eta\sqrt n$ by $(M+2+C A\sqrt n)/(\eta^2n)=o(1)$. The discarded endpoint event has limiting [probability](../../../../../../probability.md) $e^{-A^2}$; let $A\to\infty$. Therefore

$$
\frac{d_1(n)}{\sqrt n}-2\sqrt nR_1\xrightarrow{\mathbb P}0,\qquad\frac{d_1(n)}{\sqrt n}\Rightarrow2W.
$$

Since $W$ has a continuous distribution, the corrected [first-vertex degree in the LCD model](../../../../../../first-vertex-degree-in-the-lcd-model.md) tail is

$$
\boxed{\Pr(d_1(n)\ge y\sqrt n)\longrightarrow e^{-y^2/4}\quad(y>0).}
$$

This disproves the printed exponent $-y^2/8$ for $G_n^{(1)}$. The hint's factor is independently contradicted at $i=n$: its proposed upper bound tends to $1/\sqrt2$, whereas

$$
\Pr\left(R_n\le\frac{1+\varepsilon_n}{\sqrt2}\right)=\left(\frac{(1+\varepsilon_n)^2}{2}\right)^n\longrightarrow0.
$$

Thus the printed concentration event has [probability](../../../../../../probability.md) tending to zero, not one. Replacing its $2n$ by $n$ leads to the proven exponent $-y^2/4$. The exponent $-y^2/8$ would instead arise for $d_1(2n)/\sqrt n$, but then the [graph](../../../../../../graph-split.md) has $2n$ [vertices](../../../../../../vertex-graph-theory.md) and the part (b) endpoint limit at $x/\sqrt n$ becomes $e^{-2x^2}$. It cannot repair all the printed claims with one convention. **The literal part (c) is false for the named model; the full corrected limit and the source of the discrepancy are established above.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
