<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $L>0$, as needed for a nontrivial interval. Since $X$ is continuous and [adapted](../../../../../adapted-process.md), for every level $a$ and $t\geq0$,

$$
\{T_a\leq t\}
=\left\{\inf_{0\leq s\leq t}|X_s-a|=0\right\}.
$$

The infimum is attained on this compact interval and can be computed on the countable dense set $(\mathbb Q\cap[0,t])\cup\{t\}$. It is therefore $\mathcal F_t$-measurable. Thus $T_a$ is a [stopping time](../../../../../stopping-time.md), and so is $T=T_{-L}\wedge T_L$, because $\{T\leq t\}=\{T_{-L}\leq t\}\cup\{T_L\leq t\}$.

By continuity, $X_{t\wedge T}\in[-L,L]$, even before knowing that $T$ is finite. Hence

$$
e^{-L}\leq M_{t\wedge T}\leq e^L.
$$

Stopping preserves the [local martingale](../../../../../local-martingale.md) property. The [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) now shows that $M^T=(M_{t\wedge T})_{t\geq0}$ is a [uniformly integrable martingale](../../../../../uniformly-integrable-martingale.md); its deterministic bound also gives square integrability. In particular,

$$
\boxed{\mathbb EM_{t\wedge T}=1,\qquad
\mathbb EM_{t\wedge T}^2\leq e^{2L}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
