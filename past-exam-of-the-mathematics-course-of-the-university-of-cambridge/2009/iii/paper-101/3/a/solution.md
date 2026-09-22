<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A discrete-time [martingale](../../../../../../martingale-split.md) relative to a [filtration](../../../../../../filtration-probability-theory.md) $(\mathcal F_n)$ is an [adapted process](../../../../../../adapted-process.md) $(M_n)$ with $\mathbb E|M_n|<\infty$ and

$$
\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n\quad\text{almost surely}.
$$

Iterating [conditional expectation](../../../../../../conditional-expectation.md) also gives $\mathbb E[M_m\mid\mathcal F_n]=M_n$ for $m\geq n$. It is bounded in $L^2$ when each $M_n$ is square integrable and

$$
\boxed{\sup_{n\geq0}\mathbb E|M_n|^2<\infty.}
$$

This is a uniform bound on the second moments, not a pathwise bound on all sample values.

The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) for bounded [stopping times](../../../../../../stopping-time.md) says that, if $\sigma\leq\tau\leq K$ for a deterministic finite $K$, then

$$
\boxed{\mathbb E[M_\tau\mid\mathcal F_\sigma]=M_\sigma,\qquad
\mathbb EM_\tau=\mathbb EM_0.}
$$

Here $\mathcal F_\sigma$ is the [stopping-time sigma-algebra](../../../../../../stopping-time-sigma-algebra.md). The second assertion follows by taking $\sigma=0$ and then [expectations](../../../../../../expected-value.md). An $L^2$ bound is not needed: integrability at the finitely many deterministic times suffices.

For a proof, both stopped values are integrable since $|M_\tau|,|M_\sigma|\leq\sum_{j=0}^K|M_j|$. Expand

$$
M_\tau-M_\sigma=\sum_{k=0}^{K-1}\mathbf1_{\{\sigma\leq k<\tau\}}(M_{k+1}-M_k).
$$

If $A\in\mathcal F_\sigma$, then $A\cap\{\sigma\leq k\}\in\mathcal F_k$ by the definition of the [stopping-time sigma-algebra](../../../../../../stopping-time-sigma-algebra.md), and $\{\tau>k\}\in\mathcal F_k$ because $\tau$ is a [stopping time](../../../../../../stopping-time.md). Thus the indicator of $A\cap\{\sigma\leq k<\tau\}$ is $\mathcal F_k$-measurable. Multiplying the sum by $\mathbf1_A$, taking [expectations](../../../../../../expected-value.md), and conditioning each summand on $\mathcal F_k$ gives zero, by the [martingale](../../../../../../martingale-split.md) increment property. Therefore $\mathbb E[\mathbf1_AM_\tau]=\mathbb E[\mathbf1_AM_\sigma]$ for every $A\in\mathcal F_\sigma$. Since $M_\sigma$ is $\mathcal F_\sigma$-measurable, this is exactly the claimed [conditional expectation](../../../../../../conditional-expectation.md) identity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
