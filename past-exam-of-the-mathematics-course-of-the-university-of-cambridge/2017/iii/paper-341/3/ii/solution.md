<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The printed formula is not a consistent spatial discretization of the stated PDE.** The original PDF genuinely has $1/\Delta x$, rather than $1/(\Delta x)^2$. Writing $h=\Delta x$, the [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
h^{-1}\bigl(u(x-h)-2u(x)+u(x+h)\bigr)=h\,u_{xx}(x)+O(h^3),
$$

so it approximates a diffusion coefficient tending to zero. Moreover, $m=1,\ldots,M$ and $h=1/(M+1)$ cover $(0,1)$, whereas the given [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) belong to $(-1,1)$. No value at the interior location $x=0$ was prescribed. These are actual source defects, not repairs justified by the TeX conversion.

A conditional analysis of the literal [ordinary differential equation](../../../../../../ordinary-differential-equation.md) system is still possible. If it is closed by imposing $u_0=u_{M+1}=0$ on the displayed grid, the negative [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) has positive frequencies squared

$$
\kappa_j(h)=\frac4h\sin^2\frac{j\pi}{2(M+1)},\qquad j=1,\ldots,M,
$$

and each [normal mode](../../../../../../normal-mode.md) obeys $q_j''=(\alpha-\kappa_j)q_j$. For a fixed mesh, every solution is bounded for all time exactly when

$$
\boxed{\alpha<\kappa_1(h)=\frac4h\sin^2\frac{\pi h}{2}}.
$$

Equality produces a linearly growing [normal mode](../../../../../../normal-mode.md) for nonzero modal initial velocity; above the threshold there is an exponentially growing [normal mode](../../../../../../normal-mode.md). Since $\kappa_1(h)\sim\pi^2h\to0$, any $0<\alpha<\pi^2/4$ gives bounded continuous solutions but unbounded literal discrete solutions on sufficiently fine meshes. For example, $\alpha=1$, $M=99$ gives $\kappa_1<1$, and a growing first sine [normal mode](../../../../../../normal-mode.md). At $\alpha=0$, every fixed mesh is bounded for all time, but unit first-mode initial velocity has maximal displacement $1/\sqrt{\kappa_1(h)}$, which diverges on mesh refinement. For uniform-in-mesh, all-time displacement bounds for arbitrary bounded displacement/velocity data in the mesh-weighted [L2 norm](../../../../../../l2-norm.md), the literal closed system therefore requires $\alpha<0$.

This differs from finite-time [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md), governed here by [displacement stability of a symmetric semidiscrete wave equation](../../../../../../displacement-stability-of-a-symmetric-semidiscrete-wave-equation.md). For the conditional closure above, [diagonalization of a matrix](../../../../../../diagonalization-of-a-matrix.md) gives, with $\alpha_+=\max(\alpha,0)$,

$$
\|U(t)\|_h\leq e^{\sqrt{\alpha_+}t}
\bigl(\|U(0)\|_h+t\|U'(0)\|_h\bigr),\qquad
\|U\|_h^2=h\sum_m|U_m|^2.
$$

Oscillatory modes use $|\sin(\omega t)/\omega|\leq t$, including its value $t$ at $\omega=0$; growing modes use $\sinh(\beta t)/\beta\leq t e^{\beta t}$. Thus the displacement map is mesh-uniformly bounded on each fixed finite time interval for every fixed real $\alpha$. This is a legitimate finite-time displacement [stability](../../../../../../stability-of-a-numerical-method.md) estimate, but neither [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) nor the all-time conclusion of part (i). It does not assert a velocity bound in the unweighted displacement norm.

If the intended method instead uses $h^{-2}$ and the full interval, take interior indices $m=-M,\ldots,M$, $h=1/(M+1)$, with zeros at $m=\pm(M+1)$. Its first positive discrete [eigenvalue](../../../../../../eigenvalue.md) is

$$
\lambda_{1,h}=\frac4{h^2}\sin^2\frac{\pi h}{4}<\frac{\pi^2}{4},
\qquad \lambda_{1,h}\longrightarrow\frac{\pi^2}{4}.
$$

The corrected, fixed-mesh all-time condition is $\alpha<\lambda_{1,h}$, with the same strictness at equality. For every fixed $\alpha<\pi^2/4$, this holds on all sufficiently fine meshes. This corrected interpretation is stated separately rather than silently replacing the PDF.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
