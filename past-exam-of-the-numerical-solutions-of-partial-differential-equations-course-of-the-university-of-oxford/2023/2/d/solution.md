<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For every admissible $m,n$, the [trigonometric inequality](../../../../trigonometric-inequality.md) $\sin z\leq z$ for $z\geq0$ gives

$$
\frac4{h^2}\sin^2\frac{m\pi h}2\leq m^2\pi^2,\qquad
\frac4{h^2}\sin^2\frac{n\pi h}2\leq n^2\pi^2.
$$

Thus $\Lambda_{m,n}\leq\lambda_{m,n}$, in particular for $m=n=N-1$ and every $N\geq3$.

For these highest-index [eigenvalues](../../../../eigenvalue.md), use $h=1/N$ and $\sin((N-1)\pi/(2N))=\cos(\pi/(2N))$ to obtain

$$
\lambda_{N-1,N-1}-\Lambda_{N-1,N-1}
=2\pi^2(N-1)^2-8N^2\cos^2\frac\pi{2N}.
$$

Divide by $N^2$ and take the [limit](../../../../limit-of-a-function.md):

$$
\boxed{\lim_{N\to\infty}\frac{\lambda_{N-1,N-1}-\Lambda_{N-1,N-1}}{N^2}=2\pi^2-8>0.}
$$

For example, eventually the normalized difference exceeds $(2\pi^2-8)/2$, so the unnormalized difference is at least $(\pi^2-4)N^2$ and tends to $+\infty$. This does not contradict (c): there the indices stay fixed as the grid is refined; here the [eigenfunctions](../../../../eigenfunction.md) oscillate increasingly quickly, with [wavelength](../../../../wavelength.md) comparable to the mesh spacing. It illustrates the [high-frequency eigenvalue error of the discrete Laplacian](../../../../high-frequency-eigenvalue-error-of-the-discrete-laplacian.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
