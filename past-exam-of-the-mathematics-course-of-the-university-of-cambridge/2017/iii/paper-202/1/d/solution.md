<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix a [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md) $M$. Its [quadratic-variation measure](../../../../../../quadratic-variation-measure.md) on the [predictable sigma-algebra](../../../../../../predictable-sigma-algebra.md) is

$$
\nu_M(A)=\mathbb E\int_0^\infty\mathbf1_A(\omega,s)\,d[M]_s.
$$

It is finite, since $\nu_M(\Omega\times[0,\infty))=\mathbb E[M]_\infty=\mathbb E M_\infty^2-\mathbb E M_0^2$. The source [Hilbert space](../../../../../../hilbert-space-split.md) is $L^2(M)=L^2(\Omega\times[0,\infty),\mathcal P,\nu_M)$: [predictable processes](../../../../../../predictable-process.md) with finite $\mathbb E\int H^2d[M]$, identified when equal $\nu_M$-almost everywhere. Its [norm](../../../../../../norm.md) is $\|H\|_{L^2(M)}^2=\mathbb E\int H^2d[M]$.

The target $\mathcal M_0^2$ consists of [L2-bounded continuous martingales](../../../../../../l2-bounded-continuous-martingale.md) starting at zero, identified up to [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md), with [norm](../../../../../../norm.md) $\|K\|_{\mathcal M_0^2}=\|K_\infty\|_2$. It is a [Hilbert space](../../../../../../hilbert-space-split.md): terminal values belong to the closed [linear subspace](../../../../../../vector-subspace.md) of $L^2(\mathcal F_\infty)$ whose [conditional expectation](../../../../../../conditional-expectation.md) given $\mathcal F_0$ is zero and whose associated [martingales](../../../../../../martingale-split.md) have continuous versions. Closure of that continuous-version subspace follows from the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) and an almost surely uniformly convergent subsequence.

The [Itô isometry](../../../../../../ito-isometry.md) says that integration extends uniquely from [simple predictable processes](../../../../../../simple-predictable-process.md) to a linear [isometry](../../../../../../isometry.md) $L^2(M)\longrightarrow\mathcal M_0^2$, with

$$
\boxed{\mathbb E|(H\mathbin\cdot M)_\infty|^2=\mathbb E\int_0^\infty H_s^2\,d[M]_s.}
$$

For every finite $t$, the same identity holds with the integral restricted to $[0,t]$ and the left side $\mathbb E|(H\mathbin\cdot M)_t|^2$. No claim of surjectivity onto all of $\mathcal M_0^2$ is needed: that would require an additional [Martingale representation theorem](../../../../../../martingale-representation-theorem.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
