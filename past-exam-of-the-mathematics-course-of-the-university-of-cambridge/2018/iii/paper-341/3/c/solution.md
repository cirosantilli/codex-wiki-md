<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $N$ distinct periodic grid points $x_m=m/N$, $0\leq m<N$, and $h=1/N$. Values at the two ends of the interval represent the same point, so the endpoint must not be stored twice. With indices interpreted modulo $N$, set

$$
\boxed{(1+2\mu)U_m^{n+1}
-\mu(U_{m-1}^{n+1}+U_{m+1}^{n+1})=U_m^n.}
$$

This replaces the Dirichlet matrix by the periodic discrete Laplacian. The normalized [Fourier modes](../../../../../../fourier-mode.md) $N^{-1/2}e^{2\pi ijm/N}$ form an [orthonormal basis](../../../../../../orthonormal-basis.md) and have amplification factors

$$
\boxed{g_j=\frac1{1+4\mu\sin^2(\pi j/N)},\qquad 0\leq j<N.}
$$

Each satisfies $0<g_j\leq1$ for every $\mu>0$. The [Parseval identity](../../../../../../parseval-identity.md) therefore gives $\|U^{n+1}\|_h\leq\|U^n\|_h$ in the [discrete L2 norm](../../../../../../discrete-l2-norm.md), uniformly in the grid and time step. Thus **all positive [Courant numbers](../../../../../../courant-number.md) remain stable**. The constant mode has $g_0=1$, expressing preservation of the spatial mean; all nonconstant modes decay. The formula with modulo indices also handles small grids, where two neighbours can coincide.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
