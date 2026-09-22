<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $m=|V|\geq1$ and put $H(\sigma)=\sum_{\{x,y\}\in E}\sigma_x\sigma_y$, counting each [edge](../../../../../edge-of-a-graph.md) once. If only the [spin](../../../../../spin.md) at $x$ changes from $-1$ to $+1$, the change in $H$ is $2N(x)$, so

$$
\frac{\pi(\sigma^x)}{\pi(\sigma_x)}=e^{2N(x)}.
$$

The given opposite transition probabilities have the same ratio. More explicitly,

$$
\pi(\sigma_x)P(\sigma_x,\sigma^x)
=\frac{\pi(\sigma_x)}m\frac{e^{2N(x)}}{1+e^{2N(x)}}
=\frac{\pi(\sigma^x)}m\frac1{1+e^{2N(x)}}
=\pi(\sigma^x)P(\sigma^x,\sigma_x).
$$

For pairs differing at more than one site both sides vanish, and for equal configurations balance is automatic. This proves [detailed balance](../../../../../detailed-balance.md), hence **the chain is reversible with stationary law $\pi$**. All single-[spin](../../../../../spin.md) changes have positive [probability](../../../../../probability.md), so the finite chain is [irreducible](../../../../../irreducible-representation.md); it also has positive holding [probability](../../../../../probability.md) and is aperiodic.

Its random-map version is a [heat-bath Markov chain](../../../../../heat-bath-markov-chain.md). Choose a vertex $I$ uniformly and a uniform $U\in[0,1]$, independently, and set its [spin](../../../../../spin.md) to $+1$ when

$$
U\leq h(N(I)),\qquad h(z)=\frac{e^{2z}}{1+e^{2z}},
$$

and to $-1$ otherwise, leaving all other [spins](../../../../../spin.md) unchanged. This also specifies the holding probabilities omitted from the off-diagonal formulas. The conditional [Ising](../../../../../ising-model.md) law at $I$ is exactly this [Bernoulli](../../../../../bernoulli-distribution.md) choice.

Order [spin](../../../../../spin.md) configurations coordinatewise with $-1<+1$. Since both the neighbour sum and $h$ are increasing, every map defined by a fixed $(I,U)$ preserves this order. For [monotone coupling from the past](../../../../../monotone-coupling-from-the-past.md), generate one two-sided independent sequence of such maps $F_n$, $n\in\mathbb Z$, and, for a horizon $T$, apply $F_{-T},\ldots,F_{-1}$ to the all-minus and all-plus states at time $-T$. If their time-zero images agree, every initial state has that same image by [monotonicity](../../../../../monotonic-function.md). Return it. Otherwise enlarge $T$, for example by doubling it, retaining all maps already generated at existing negative times. Any earlier starting configuration is also forced to the same output once a horizon coalesces, so the result is consistent under further backward extension.

To prove termination, let $D=\max_x\deg(x)$ and

$$
a=h(-D)=\frac1{1+e^{2D}}>0.
$$

List the vertices $v_1,\ldots,v_m$. A block of $m$ updates choosing them in that order and having every uniform less than $a$ sets every vertex to $+1$, regardless of the starting configuration. Each choice has [probability](../../../../../probability.md) $1/m$, and every uniform condition has [probability](../../../../../probability.md) $a$. Thus a block is a universal reset with [probability](../../../../../probability.md)

$$
\varepsilon=(a/m)^m>0.
$$

Independent disjoint blocks in the past give

$$
\mathbb P(\text{no coalescence from }-T\text{ to }0)
\leq(1-\varepsilon)^{\lfloor T/m\rfloor}\longrightarrow0.
$$

Once such a block occurs, later maps preserve agreement. Therefore **the backward search terminates in finite time [almost surely](../../../../../almost-sure-convergence.md)**, including the doubling implementation.

Finally we prove that the common output $Y$ has law $\pi$. For a deterministic horizon $T$, independently start another chain at time $-T$ with initial law $\pi$ and use the same maps. Its time-zero state $Z_0^{(T)}$ has law $\pi$ by stationarity. On the event that this deterministic horizon coalesces, $Z_0^{(T)}=Y$, so for every event $B\subseteq\Sigma$,

$$
\left|\mathbb P(Y\in B)-\pi(B)\right|
\leq\mathbb P(Y\ne Z_0^{(T)})
\leq(1-\varepsilon)^{\lfloor T/m\rfloor}.
$$

Letting deterministic $T\to\infty$ proves

$$
\boxed{Y\sim\pi}.
$$

This argument justifies exact sampling without treating a random, data-dependent horizon as a deterministic stationary run.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
