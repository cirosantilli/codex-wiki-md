<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A left-continuous [adapted process](../../../../../../adapted-process.md) is a [predictable process](../../../../../../predictable-process.md). Define the elementary predictable approximation

$$
H_s^{(n)}=H_{kh_n}\quad\text{for }kh_n<s\le(k+1)h_n,
\qquad h_n=2^{-n}.
$$

At every $s>0$, its sample time approaches $s$ from the left, including when $s$ is itself a grid point. Thus $H_s^{(n)}\to H_s$ pathwise by left continuity.

Use the [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md) $X=X_0+M+A$, with $M$ a [continuous local martingale](../../../../../../continuous-local-martingale.md) and $A$ a continuous [finite-variation process](../../../../../../finite-variation-process.md). Localize so that on a fixed horizon $T$, the integrands are bounded by a deterministic constant, $[M]_T$ is bounded, and the [total-variation process](../../../../../../total-variation-process.md) of $A$ at $T$ is bounded. This is possible using local boundedness and the finite pathwise clock and variation.

For the finite-variation integral, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\sup_{t\le T}\left|\int_0^t(H_s^{(n)}-H_s)\,dA_s\right|
\le\int_0^T|H_s^{(n)}-H_s|\,d|A|_s\longrightarrow0
$$

[almost surely](../../../../../../almost-sure-convergence.md). For the martingale integral, the [Itô isometry](../../../../../../ito-isometry.md) and the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) give

$$
\mathbb E\sup_{t\le T}\left|\int_0^t(H_s^{(n)}-H_s)\,dM_s\right|^2
\le4\mathbb E\int_0^T|H_s^{(n)}-H_s|^2\,d[M]_s\longrightarrow0.
$$

Here the localized bounds justify dominated convergence also in expectation. Remove localization to conclude that the full elementary integrals converge in [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md) to $\int H\,dX$.

The sum of completed intervals differs from the full elementary integral at time $t$ by

$$
H_{h_n\lfloor t/h_n\rfloor}
\left(X_t-X_{h_n\lfloor t/h_n\rfloor}\right).
$$

Its maximum on $[0,T]$ tends to zero [almost surely](../../../../../../almost-sure-convergence.md), by the local bound on $H$ and [uniform continuity](../../../../../../uniform-continuity.md) of $X$. Therefore

$$
\boxed{\sum_{k=0}^{\lfloor t/h_n\rfloor-1}H_{kh_n}
(X_{(k+1)h_n}-X_{kh_n})
\xrightarrow{\mathrm{u.c.p.}}\int_0^tH_s\,dX_s.}
$$

This proves [left-endpoint approximation of a continuous semimartingale integral](../../../../../../left-endpoint-approximation-of-a-continuous-semimartingale-integral.md), including the unfinished interval convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
