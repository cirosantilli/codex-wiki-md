<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the usual completed right-continuous [Brownian filtration](../../../../../../brownian-filtration.md). The strict passage process $(T_a)_{a\geq0}$ is finite at every level on one probability-one [event](../../../../../../event.md): finiteness at all integer levels from (a) suffices by monotonicity. Also $T_0=0$ [almost surely](../../../../../../almost-sure-convergence.md) by (b).

For each fixed $a$, $T_a$ is a [stopping time](../../../../../../stopping-time.md) with $B_{T_a}=a$. The [Strong Markov property](../../../../../../strong-markov-property.md) shows that the passage times above this level depend on a new independent standard [Brownian motion](../../../../../../brownian-motion-split.md). Thus for $0\leq a<b$, $T_b-T_a$ is independent of the past at $T_a$ and has the same law as $T_{b-a}$. Iteration gives [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md) in the level parameter. From (a) and fixed-level equality,

$$
\mathbb E e^{-\lambda T_a}=e^{-a\sqrt{2\lambda}}.
$$

For $\lambda,\eta>0$, this also proves continuity in probability at zero, since

$$
\mathbb P(T_h>\eta)\leq\frac{1-e^{-h\sqrt{2\lambda}}}{1-e^{-\lambda\eta}}\longrightarrow0.
$$

Finally, with $M_t=\sup_{s\leq t}B_s$, we have $T_a=\inf\{t:M_t>a\}$. This [strict generalized inverse of a nondecreasing function](../../../../../../strict-generalized-inverse-of-a-nondecreasing-function.md) is right-continuous: if $a_n\downarrow a$, then for any $t>T_a$ we have $M_t>a$, and eventually $M_t>a_n$, which forces $T_{a_n}\leq t$. Monotonicity gives the reverse bound. Monotonicity and local finiteness also give finite left limits. Hence $T$ is the [Brownian first-passage subordinator](../../../../../../brownian-first-passage-subordinator.md), with [càdlàg](../../../../../../cadlag.md) paths.

Now condition on this clock, which is independent of $W$. For a deterministic partition $0=a_0<a_1<\cdots<a_k$, write $\Delta T_j=T_{a_j}-T_{a_{j-1}}$ and $\Delta X_j=W_{T_{a_j}}-W_{T_{a_{j-1}}}$. Conditional on the clock these are independent centered Gaussian increments, with respective variances $\Delta T_j$. Consequently

$$
\mathbb E\exp\!\left(i\sum_{j=1}^ku_j\Delta X_j\right)
=\mathbb E\exp\!\left(-\frac12\sum_{j=1}^ku_j^2\Delta T_j\right)
=\prod_{j=1}^k\exp\bigl(-(a_j-a_{j-1})|u_j|\bigr).
$$

Factorization and dependence only on interval lengths prove [independent increments](../../../../../../independent-increments.md) and [stationary increments](../../../../../../stationary-increments.md) for $X$. For small $h$, $T_h\to0$ in probability, and [independence](../../../../../../independent-random-variables.md) and continuity of $W$ imply $W_{T_h}\to0$ in probability. For example, bound its deviation probability by $\mathbb P(T_h>\eta)+\mathbb P(\sup_{t\leq\eta}|W_t|>\varepsilon)$ and then let $h\downarrow0$ and $\eta\downarrow0$. [Stationary increments](../../../../../../stationary-increments.md) give [stochastic continuity](../../../../../../stochastic-continuity.md) at every deterministic level. Composition of the continuous path of $W$ with the nondecreasing [càdlàg](../../../../../../cadlag.md) clock gives [càdlàg](../../../../../../cadlag.md) paths for $X$, and $X_0=0$. Thus

$$
\boxed{(X_a)_{a\geq0}\text{ is a Lévy process}.}
$$

This is [subordination of a Lévy process](../../../../../../subordination-of-a-levy-process.md). Using strict passage times ensures the required right-continuous path choice, despite their fixed-level equality with the non-strict times.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
