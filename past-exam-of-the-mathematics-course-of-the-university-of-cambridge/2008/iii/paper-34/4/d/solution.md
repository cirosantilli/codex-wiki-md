<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [stopped martingale](../../../../../../stopped-martingale.md) $Z_{n\wedge T}$ is a [martingale](../../../../../../martingale-split.md). For completeness, the bounded-time stopping rule follows directly from

$$
Z_{(n+1)\wedge T}-Z_{n\wedge T}
=\mathbf1_{\{T>n\}}(Z_{n+1}-Z_n),
$$

whose [conditional expectation](../../../../../../conditional-expectation.md) given $\mathcal F_n$ is zero. Integrability at each fixed $n$ follows by expressing the stopped value as a finite sum of the integrable $Z_j$ restricted to disjoint [events](../../../../../../event.md). Therefore $\mathbb E Z_{n\wedge T}=\mathbb E Z_0=1$.

The crucial bound is deterministic. Since $S_{n\wedge T}\leq b$ and $M(\tau)\geq1$,

$$
0<Z_{n\wedge T}=\frac{e^{\tau S_{n\wedge T}}}{M(\tau)^{n\wedge T}}\leq e^{\tau b}.
$$

A bounded family is [uniformly integrable](../../../../../../uniform-integrability.md): for $K>e^{\tau b}$ all its quantities $\mathbb E[|Z_{n\wedge T}|\mathbf1_{\{|Z_{n\wedge T}|>K\}}]$ vanish. Part (c) gives $T<\infty$ [almost surely](../../../../../../almost-sure-convergence.md), and then $S_T=b$. Hence

$$
Z_{n\wedge T}\longrightarrow e^{\tau b}M(\tau)^{-T}\quad\text{almost surely}.
$$

The general result for passing to expectations is the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md): almost-sure convergence under one integrable bound implies [convergence in L1](../../../../../../convergence-in-l1.md) and convergence of expectations. Applying it with the bound $e^{\tau b}$ gives

$$
1=\lim_n\mathbb E Z_{n\wedge T}=e^{\tau b}\mathbb E[M(\tau)^{-T}],
\qquad
\boxed{\mathbb E[M(\tau)^{-T}]=e^{-\tau b}.}
$$

This is the [exponential first-passage transform for an upward skip-free random walk](../../../../../../exponential-first-passage-transform-for-an-upward-skip-free-random-walk.md); it avoids an unjustified use of [optional stopping](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at an unbounded [stopping time](../../../../../../stopping-time.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
