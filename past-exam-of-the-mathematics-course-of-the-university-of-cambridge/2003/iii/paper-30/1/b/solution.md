<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $T_y=\inf\{n\ge0:X_n=y\}$ and the positive return time $T_x^+=\inf\{n\ge1:X_n=x\}$. The walk has transitions $p_{uv}=c_{uv}/d(u)$, $d(u)=\sum_vc_{uv}$; its transition matrix defines a [reversible Markov chain](../../../../../../reversible-markov-chain.md), although the [transition probabilities](../../../../../../transition-probability.md) need not be symmetric.

The voltage $h(u)=P_u(T_x<T_y)$ equals one at $x$, zero at $y$, and is a [harmonic function on a graph](../../../../../../discrete-harmonic-function.md) away from the terminals: $h(u)=\sum_vp_{uv}h(v)$. For this unit [electric potential difference](../../../../../../electric-potential-difference.md) the [electric current](../../../../../../electric-current.md) is

$$
I=\sum_vc_{xv}(1-h(v))=\frac1{R(x,y)}.
$$

The [first-step analysis](../../../../../../first-step-analysis.md) therefore proves the [return probability from effective resistance](../../../../../../return-probability-from-effective-resistance.md) identity:

$$
P_x(T_x^+<T_y)=\sum_vp_{xv}h(v)
=1-\frac{I}{d(x)}
=\boxed{1-\frac1{d(x)R(x,y)}}.
$$

Finite irreducibility ensures eventual hitting of one of the terminals, so no missing escape event appears in this finite-network calculation.

For an infinite locally finite [connected graph](../../../../../../connected-graph.md), exhaust it by finite sets and wire their exteriors to one sink. The event of exiting before the first return decreases to the event of never returning. Thus

$$
P_o(T_o^+=\infty)=\frac1{d(o)R(o,\infty)},
$$

with $1/\infty=0$. In particular [recurrence](../../../../../../recurrent-markov-chain.md) is equivalent to infinite [effective resistance to infinity](../../../../../../effective-resistance-to-infinity.md).

After deleting an [edge](../../../../../../edge-of-a-graph.md), consider any infinite component and choose a root $o$ away from that [edge](../../../../../../edge-of-a-graph.md)'s endpoints. Its [vertex degree](../../../../../../degree-graph-theory.md) $d(o)$ is unchanged. On every finite wired exhaustion the [Rayleigh monotonicity principle](../../../../../../rayleigh-monotonicity-principle.md) makes the resistance no smaller; the [limit of a sequence](../../../../../../limit-of-a-sequence.md) does too. A [recurrent](../../../../../../recurrent-markov-chain.md) original network consequently leaves a [recurrent](../../../../../../recurrent-markov-chain.md) component. Finite components give [recurrent](../../../../../../recurrent-markov-chain.md) walks as well, with an isolated [graph vertex](../../../../../../vertex-graph-theory.md) viewed as an [absorbing state](../../../../../../absorbing-state.md). This proves that [edge deletion preserves recurrence](../../../../../../edge-deletion-preserves-recurrence.md). The phrase “no less [recurrent](../../../../../../recurrent-markov-chain.md)” refers to this [recurrence](../../../../../../recurrent-markov-chain.md) comparison: at a deleted-edge endpoint the [vertex degree](../../../../../../degree-graph-theory.md) factor also changes, so monotonicity of its first-return [probability](../../../../../../probability.md) alone should not be inferred.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
