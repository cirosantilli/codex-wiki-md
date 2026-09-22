# Vector line integral weighted by a scalar field

↑ **Parent:** [Line integral](line-integral.md)

For an oriented [parametric curve](parametric-curve.md) $\mathbf r(t)$ and scalar field $V$, define the componentwise [line integral](line-integral.md)

$$
\int_C V\,d\mathbf r=\int V(\mathbf r(t))\mathbf r'(t)\,dt.
$$

Its value is a [vector](vector.md) and reversing orientation changes its sign. It differs from the scalar [arc length](arc-length.md) integral $\int_CV\,ds=\int V(\mathbf r(t))|\mathbf r'(t)|\,dt$, which is independent of orientation. A request to integrate a scalar field along a curve should specify which differential is intended.

For the counterclockwise circle $\mathbf r(\phi)=(R\cos\phi,R\sin\phi,z_0)$, suppose the restricted field has [Fourier series](fourier-series-split.md) $V(\phi)=A_0+\sum_{n\geq1}(A_n\cos n\phi+B_n\sin n\phi)$. [Orthogonality](orthogonal-vectors.md) gives

$$
\oint_C V\,d\mathbf r=\pi R(-B_1,A_1,0),\qquad
\oint_C V\,ds=2\pi RA_0.
$$

The oriented vector integral selects the first angular harmonics, whereas the scalar arc-length integral selects the mean.

## ↑ Ancestors (9)

1. [Line integral](line-integral.md)
2. [Vector calculus](vector-calculus.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/16/a/iv/solution.md)
