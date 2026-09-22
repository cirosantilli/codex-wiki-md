<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The construction is a [convex roof extension](../../../../../convex-roof-extension.md). First establish its [convexity](../../../../../convex-function.md), without assuming that the minimizing [quantum state ensemble](../../../../../quantum-state-ensemble.md) exists. If $\tau=\sum_jw_j\tau_j$, choose a [pure state](../../../../../pure-state.md) ensemble for each $\tau_j$ whose average value of $\mu$ is within $\varepsilon$ of $F(\tau_j)$. Combining these ensembles, with their weights multiplied by $w_j$, gives a [pure state](../../../../../pure-state.md) ensemble for $\tau$. Taking arbitrarily small $\varepsilon>0$ proves

$$
F\left(\sum_jw_j\tau_j\right)\leq\sum_jw_jF(\tau_j).
$$

Also, **$F(\pi)=\mu(\pi)$ for a pure state $\pi$**. Indeed, if $\pi=\sum_jp_j\pi_j$ and $v$ is orthogonal to its one-dimensional support, then $0=\sum_jp_j\langle v|\pi_j|v\rangle$. All terms are nonnegative, so every positive-weight $\pi_j$ has that same support and equals $\pi$.

Represent outcome $k$ of the operation by a linear unnormalized map $\mathcal I_k$, as for a [quantum instrument](../../../../../quantum-instrument.md). Normalization is performed only after applying this map: $\mathcal I_k(\rho)=P_k\rho_k$. For any preparation ensemble $\rho=\sum_jp_j\pi_j$, put

$$
\mathcal I_k(\pi_j)=q_{k|j}\sigma_{jk},\qquad
P_k=\sum_jp_jq_{k|j}.
$$

Linearity gives $P_k\rho_k=\sum_jp_jq_{k|j}\sigma_{jk}$. For $P_k>0$, [Bayes' theorem](../../../../../bayes-theorem.md) identifies the conditional preparation weights

$$
w_{j|k}=\frac{p_jq_{k|j}}{P_k},\qquad \rho_k=\sum_jw_{j|k}\sigma_{jk}.
$$

Outcomes with zero [probability](../../../../../probability.md) contribute nothing; normalized states on such branches need not be defined. The conditional states $\sigma_{jk}$ may be mixed, so convexity of the [convex roof](../../../../../convex-roof-extension.md) is essential here.

Applying that convexity separately for each recorded outcome, and then the assumed average monotonicity for each pure preparation, yields

$$
\begin{aligned}
\sum_kP_kF(\rho_k)
&\leq\sum_{j,k}p_jq_{k|j}F(\sigma_{jk})\\
&\leq\sum_jp_jF(\pi_j)
=\sum_jp_j\mu(\pi_j).
\end{aligned}
$$

The left side depends only on the initial [density operator](../../../../../density-matrix.md) and the operation, not on the chosen preparation ensemble. Taking the [infimum](../../../../../infimum.md) of the last expression over all its [pure state](../../../../../pure-state.md) ensembles proves

$$
\boxed{F(\rho)\geq\sum_kP_kF(\rho_k).}
$$

Equivalently, choose an ensemble within $\varepsilon$ of the [infimum](../../../../../infimum.md) and then let $\varepsilon\downarrow0$. This is the [monotonicity of a convex roof under a quantum instrument](../../../../../monotonicity-of-a-convex-roof-under-a-quantum-instrument.md). It uses linearity of the unnormalized branches, not a false assumption that normalized conditional states depend linearly on the input. As usual, the averages are assumed well defined; finite-valued roofs and finitely many outcomes suffice. If an input roof is $-\infty$, taking ensembles with averages tending to $-\infty$ gives the same conclusion in the extended-real interpretation whenever the output average is defined.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
