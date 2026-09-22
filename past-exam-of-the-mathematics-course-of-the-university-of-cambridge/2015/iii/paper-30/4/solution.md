<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $\delta_n=2^{-n}$ and let $Q_n(U)$ denote the printed squared-increment sum for a process $U$, on grid times $k\delta_n$. We construct its limit first for bounded [martingales](../../../../../martingale-split.md), then use [localizing sequences](../../../../../localizing-sequence.md) and the [finite variation](../../../../../total-variation-of-a-function.md) part of a [semimartingale](../../../../../semimartingale.md).

**Continuity and monotonicity of the bounded-[martingale](../../../../../martingale-split.md) limit.** Let $U$ be a uniformly bounded [continuous martingale](../../../../../continuous-martingale.md). The given result supplies a limit $R^U$ in [uniform convergence on compacts in probability](../../../../../uniform-convergence-on-compacts-in-probability.md). Each $Q_n(U)$ is continuous and adapted. A subsequence converges almost surely uniformly on each compact time interval, by choosing summable error probabilities and diagonalizing. Its limit therefore has a continuous version; in the usual completed filtration this version is adapted.

The sums $Q_n(U)$ themselves can decrease between grid points, because the last partial increment is being squared. To establish monotonicity, use instead the [quadratic variation from completed grid increments](../../../../../quadratic-variation-from-completed-grid-increments.md)

$$
S_n(U)_t=\sum_{k\delta_n\leq t}
(U_{k\delta_n}-U_{(k-1)\delta_n})^2.
$$

These step processes are nondecreasing, and pathwise uniform continuity gives

$$
\sup_{t\leq T}|Q_n(U)_t-S_n(U)_t|
\leq\omega_U(\delta_n;T)^2\longrightarrow0,
$$

where $\omega_U(\delta;T)=\sup\{|U_t-U_s|:s,t\leq T,\ |t-s|\leq\delta\}$. Thus the same almost surely uniform subsequence of $S_n$ converges to $R^U$, proving that $R^U$ is nondecreasing. Also $R^U_0=0$.

**Localization of a [continuous local martingale](../../../../../continuous-local-martingale.md).** Subtract the initial value, which does not affect increments, so that $M_0=0$. Set

$$
\tau_m=\inf\{t:|M_t|\geq m\}\wedge m.
$$

Continuity gives $\tau_m\uparrow\infty$ almost surely and makes $M^{\tau_m}$ bounded. The [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) makes it a true [martingale](../../../../../martingale-split.md). Let $R^m$ be its continuous, adapted, nondecreasing limit.

The discrete sums commute exactly with stopping:

$$
Q_n(M^{\tau_m})_t=Q_n(M)_{t\wedge\tau_m}.
$$

For $\ell\leq m$, uniqueness of the probability limit and stability of [uniform convergence on compacts in probability](../../../../../uniform-convergence-on-compacts-in-probability.md) under stopping give

$$
R^m_{t\wedge\tau_\ell}=R^\ell_t
$$

up to indistinguishability. Taking a common null set for the countably many pairs, patch these processes into $R^M$ by setting $R^M_t=R^m_t$ when $t\leq\tau_m$. Compatibility makes this definition independent of $m$. It is continuous, adapted, and nondecreasing. For each $T,\varepsilon>0$,

$$
\mathbb P\left(\sup_{t\leq T}|Q_n(M)_t-R^M_t|>\varepsilon\right)
\leq\mathbb P(\tau_m<T)
+\mathbb P\left(\sup_{t\leq T}|Q_n(M^{\tau_m})_t-R^m_t|>\varepsilon\right).
$$

Let $n\to\infty$ and then $m\to\infty$. This proves the [localization and patching of quadratic variation](../../../../../localization-and-patching-of-quadratic-variation.md).

**Adding [finite variation](../../../../../total-variation-of-a-function.md).** Decompose the continuous [semimartingale](../../../../../semimartingale.md) as $X=X_0+M+A$, where $M$ is a [continuous local martingale](../../../../../continuous-local-martingale.md) starting at zero and $A$ is continuous, adapted, and locally of [finite variation](../../../../../total-variation-of-a-function.md). For every compact interval, the sum of the absolute increments of $A$ is at most its [total variation of a function](../../../../../total-variation-of-a-function.md). Hence, pathwise,

$$
\sup_{t\leq T}Q_n(A)_t
\leq\omega_A(\delta_n;T)\operatorname{Var}_{[0,T]}(A)
\longrightarrow0.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) bounds the mixed increment sum by

$$
\sup_{t\leq T}\left|\sum_k\Delta_kM(t)\Delta_kA(t)\right|
\leq
\left(\sup_{t\leq T}Q_n(M)_t\right)^{1/2}
\left(\sup_{t\leq T}Q_n(A)_t\right)^{1/2}.
$$

The first factor is bounded in probability, since $Q_n(M)\to R^M$ uniformly on compacts in probability; the second tends to zero almost surely. Thus the mixed term tends to zero in probability. Expanding the square proves

$$
\boxed{Q_n(X)\longrightarrow R^M
\quad\text{uniformly on compacts in probability}.}
$$

The constructed $R=R^M$ is continuous, nondecreasing, and adapted. This is the [quadratic variation](../../../../../quadratic-variation.md) of $X$, and expresses the fact that [finite-variation terms do not change quadratic variation](../../../../../finite-variation-terms-do-not-change-quadratic-variation.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
