<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $A_t=[M]_t$. Its continuous, strictly increasing paths start at zero and tend to infinity. Thus the inverse $T_s$ is finite and continuous, and

$$
\{T_s\le u\}=\{A_u\ge s\}\in\mathcal F_u,
$$

so each $T_s$ is a [stopping time](../../../../../../stopping-time.md). Set $\mathcal G_s=\mathcal F_{T_s}$ and $\beta_s=M_{T_s}$. This is the inverse-clock construction in the [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md).

To verify its [martingale](../../../../../../martingale-split.md) property, stop $M$ at times $\tau_n$ bounding its path, its bracket and time itself. The stopped $M$ and $M^2-A$ are bounded [martingales](../../../../../../martingale-split.md). [Optional sampling](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $T_s\wedge\tau_n$ and $T_t\wedge\tau_n$ shows that the time-changed process, stopped at $A_{\tau_n}$, is a [martingale](../../../../../../martingale-split.md) and that its square minus the stopped clock $s\wedge A_{\tau_n}$ is a [martingale](../../../../../../martingale-split.md). These clock [stopping times](../../../../../../stopping-time.md) tend to infinity because $A_\infty=\infty$. Therefore $\beta$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) with $\beta_0=0$ and [quadratic variation](../../../../../../quadratic-variation.md) $[\beta]_s=s$. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) identifies it as a $\mathcal G_s$-Brownian motion.

Strict monotonicity and continuity give $A_{T_s}=s$ and $T_{A_t}=t$, so

$$
\boxed{M_t=\beta_{[M]_t}}.
$$

The inverse-clock argument proves the asserted representation; the random clock need not be independent of the [Brownian motion](../../../../../../brownian-motion-split.md) it produces.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
