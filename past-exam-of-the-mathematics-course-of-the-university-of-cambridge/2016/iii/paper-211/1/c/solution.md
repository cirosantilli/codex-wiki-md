<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First work with the [filtration](../../../../../../filtration-probability-theory.md) $\mathcal G_t=\mathcal F_t^W\vee\sigma(\mathbf1_{\{u\leq\tau\}}:0\leq u\leq t)$, which records the [Brownian motion](../../../../../../brownian-motion-split.md) and whether [default](../../../../../../credit-default.md) has occurred. On $\{s>\tau\}$ all subsequent [defaultable stock](../../../../../../defaultable-stock.md) prices vanish. On $\{s\leq\tau\}$, the [memoryless property](../../../../../../memorylessness-of-the-exponential-distribution.md) of the [exponential distribution](../../../../../../exponential-distribution.md) gives survival from $s$ to $t$ with [conditional probability](../../../../../../conditional-probability.md) $e^{-\lambda(t-s)}$. The residual survival event is [independent](../../../../../../independent-random-variables.md) of the future [independent increments](../../../../../../independent-increments.md) of the [Brownian motion](../../../../../../brownian-motion-split.md). Thus, for deterministic $s<t$,

$$
\mathbb E[\widehat S_t\mid\mathcal G_s]
=\mathbf1_{\{s\leq\tau\}}e^{\lambda t}
   e^{-\lambda(t-s)}\mathbb E[S_t\mid\mathcal F_s^W]
=\mathbf1_{\{s\leq\tau\}}e^{\lambda s}S_s
=\widehat S_s.
$$

Also $\mathbb E\widehat S_t=e^{\lambda t}e^{-\lambda t}S_0=S_0$, so this is a true [martingale](../../../../../../martingale-split.md), with no localization needed. Its [natural filtration](../../../../../../natural-filtration.md) is contained in $\mathcal G$; applying the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) to the displayed identity yields **the requested natural-filtration martingale property**:

$$
\boxed{\mathbb E[\widehat S_t\mid\mathcal F_s^{\widehat S}]=\widehat S_s.}
$$

The printed convention keeps the [stock](../../../../../../stock.md) alive at $t=\tau$. It is a left-continuous convention at that one random time. Replacing it by $\mathbf1_{\{t<\tau\}}$ gives the usual [càdlàg](../../../../../../cadlag.md) [zero-recovery default model](../../../../../../zero-recovery-default-model.md); since $\mathbb P(\tau=t)=0$ at each fixed $t$, the fixed-time [martingale](../../../../../../martingale-split.md) calculations above are unchanged.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
