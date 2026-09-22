<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use recovery rate one and infection rate $\lambda$ along each directed nearest-neighbour [edge](../../../../../../edge-of-a-graph.md). The [graphical representation of the contact process](../../../../../../graphical-representation-of-the-contact-process.md) places independent rate-one recovery marks at [graph vertices](../../../../../../vertex-graph-theory.md) and rate-$\lambda$ arrows on directed [edges](../../../../../../edge-of-a-graph.md). Infection travels along time-directed paths following arrows and avoiding recovery marks. The same clocks couple all initial configurations and preserve coordinatewise order. Denote its semigroup by $P_t$.

The empty configuration is absorbing, so the lower invariant measure is $\underline\nu=\delta_0$. To construct the upper one, put $\mu_t=\delta_1P_t$, where $1$ is the all-infected configuration. Since $\delta_1P_s\le_{\mathrm{st}}\delta_1$, order preservation and the semigroup property imply

$$
\mu_{t+s}=\delta_1P_sP_t\le_{\mathrm{st}}\delta_1P_t=\mu_t.
$$

Thus these laws decrease in stochastic order. More concretely, use clocks on the entire time axis and start from all infected at time $-t$, looking at the configuration at time zero. These configurations decrease pointwise as $t$ increases: an infection arriving from an earlier start is also obtainable from the all-infected later start. Each coordinate therefore has a limit. Their joint law $\overline\nu$ satisfies $\mu_t\to\overline\nu$ in [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md) on the compact product space.

This limit is invariant. The graphical construction is Feller: for finitely many sites and a bounded time interval, the backward ancestor exploration is almost surely finite, since its size is dominated by a finite-rate [branching process](../../../../../../branching-process.md). Hence a cylinder function evolved for a fixed time is continuous in the initial configuration, by approximation with finite ancestor sets. Cylinder functions uniformly approximate continuous functions on the product space. We may therefore pass to the limit in

$$
\mu_tP_s=\mu_{t+s}
$$

to get $\overline\nu P_s=\overline\nu$. These are indeed the [extremal invariant measures of the contact process](../../../../../../extremal-invariant-measures-of-the-contact-process.md): if $\nu$ is any [invariant probability law of a Markov process](../../../../../../invariant-probability-law-of-a-markov-process.md), apply $P_t$ to $\delta_0\le_{\mathrm{st}}\nu\le_{\mathrm{st}}\delta_1$ and take limits to obtain $\underline\nu\le_{\mathrm{st}}\nu\le_{\mathrm{st}}\overline\nu$.

For the relation with survival, reverse the graphical paths in the interval $[0,t]$, also reversing arrows. The law is unchanged because the rates are symmetric between neighbours. The set of ancestors of a site $x$ has the law of the [contact process](../../../../../../contact-process.md) started from $\{x\}$. Consequently

$$
\mathbb P^1(\eta_t(x)=1)=\mathbb P^{\{x\}}(\eta_t\ne0).
$$

This is [duality of the contact process](../../../../../../duality-of-the-contact-process.md). The events on the right decrease with time because the empty state is absorbing, and their limiting [probability](../../../../../../probability.md) is $\theta(\lambda)$. It follows that

$$
\boxed{\overline\nu(\eta(x)=1)=\theta(\lambda).}
$$

If $\theta(\lambda)=0$, every coordinate is zero almost surely under $\overline\nu$; a countable union over the sites gives $\overline\nu=\delta_0=\underline\nu$. Conversely, if the two invariant measures coincide, this one-site marginal is zero, so $\theta(\lambda)=0$. Hence

$$
\boxed{\underline\nu=\overline\nu\quad\Longleftrightarrow\quad\theta(\lambda)=0.}
$$

A convention that divides the infection rate by the degree only rescales the parameter; the argument and equivalence are unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
