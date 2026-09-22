<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\mathbb T^n=\mathbb R^n/(2\pi\mathbb Z)^n$ and the [periodic Sobolev space](../../../../../../periodic-sobolev-space.md) convention

$$
\|f\|_{H^s}^2=\sum_{k\in\mathbb Z^n}(1+|k|^2)^s|\widehat f(k)|^2.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_k|\widehat f(k)|\leq\|f\|_{H^s}\left(\sum_k(1+|k|^2)^{-s}\right)^{1/2}.
$$

To check the last sum, partition the lattice into $|k|<1$ and dyadic shells $2^j\leq|k|<2^{j+1}$. A shell contains at most $C_n2^{jn}$ points and contributes at most $C_n2^{j(n-2s)}$. This is a convergent [geometric series](../../../../../../geometric-series.md) exactly when $s>n/2$.

Thus the [Fourier series](../../../../../../fourier-series-split.md) $\sum_k\widehat f(k)e^{ik\cdot x}$ converges absolutely and uniformly on the [torus](../../../../../../torus.md). Its sum is a [continuous function](../../../../../../continuous-function.md) and has the original [Fourier coefficients](../../../../../../fourier-coefficient.md), so it represents the original periodic [distribution](../../../../../../distribution-mathematical-analysis.md). In particular the representative is unique and

$$
\boxed{H^s(\mathbb T^n)\hookrightarrow C(\mathbb T^n),\qquad\|f\|_\infty\leq C_{s,n}\|f\|_{H^s}\quad(s>n/2).}
$$

This proves the requested inclusion, with its continuous [Sobolev embedding](../../../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md) estimate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
