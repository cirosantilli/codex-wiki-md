<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take a complete, right-continuous [filtration](../../../../../../filtration-probability-theory.md) $(\mathcal F_t)$, an increasing family of sigma-algebras. Adapted means that $X_t$ is $\mathcal F_t$-measurable at each $t$; [càdlàg](../../../../../../cadlag.md) means right-continuous with left limits. A [local martingale](../../../../../../local-martingale.md) is an adapted [càdlàg](../../../../../../cadlag.md) process $X$, with integrable initial value, for which there are [stopping times](../../../../../../stopping-time.md) $\tau_n\uparrow\infty$ almost surely such that each [stopped process](../../../../../../stopped-process.md) $X^{\tau_n}_t=X_{t\wedge\tau_n}$ is a true [martingale](../../../../../../martingale-split.md). Such a sequence is a localizing sequence. A true [martingale](../../../../../../martingale-split.md) is integrable at each time and satisfies $\mathbb E(X_t\mid\mathcal F_s)=X_s$ for $s\le t$.

The necessary and sufficient condition is that $X$ is a [Class DL process](../../../../../../class-dl-process.md):

$$
\boxed{X\text{ is a martingale}\ \Longleftrightarrow\ \{X_\tau:\tau\le T\text{ a stopping time}\}\text{ is uniformly integrable for every finite }T.}
$$

A family $\mathcal Z$ is [uniformly integrable](../../../../../../uniform-integrability.md) if its members are integrable and $\sup_{Z\in\mathcal Z}\mathbb E(|Z|\mathbf1_{\{|Z|>K\}})\to0$ as $K\to\infty$. A [stopping time](../../../../../../stopping-time.md) $\tau$ satisfies $\{\tau\le t\}\in\mathcal F_t$ for all $t$.

For necessity, on $[0,T]$ the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $X_\tau=\mathbb E(X_T\mid\mathcal F_\tau)$; [conditional expectations](../../../../../../conditional-expectation.md) of one integrable variable form a [uniformly integrable](../../../../../../uniform-integrability.md) family. For sufficiency, $X_{t\wedge\tau_n}\to X_t$ almost surely, and [Class DL](../../../../../../class-dl-process.md) upgrades this convergence to $L^1$ on each finite horizon. Pass to the limit in $\mathbb E(X_{t\wedge\tau_n}\mid\mathcal F_s)=X_{s\wedge\tau_n}$ to obtain the [martingale](../../../../../../martingale-split.md) identity. Requiring [uniform integrability](../../../../../../uniform-integrability.md) of all times on the entire half-line would be stronger than necessary; [Brownian motion](../../../../../../brownian-motion-split.md) is already a counterexample to that stronger requirement.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
