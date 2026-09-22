<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The spatial shift in the PDF also requires a boundary value beyond the supplied right endpoint: if $m$ is the last interior index, the newest $m+2$ value is outside the interval. Thus **the printed Dirichlet method has no specified boundary closure, and no unique stability range can be assigned to it as stated**.

For completeness, the literal interior formula has an exact [von Neumann stability analysis](../../../../../../von-neumann-stability-analysis.md) on an infinite or periodic grid. Substitution of a [Fourier mode](../../../../../../fourier-mode.md) $U_m^n=\xi^ne^{im\theta}$ gives

$$
A(\theta)\xi^2-4\xi+1=0,\qquad
A(\theta)=3e^{2i\theta}+8\mu\sin^2(\theta/2).
$$

For the [root of a polynomial](../../../../../../root-of-a-polynomial.md) tending to one as $\theta\to0$, expansion gives

$$
\xi=1-3i\theta-(\mu+3/2)\theta^2+O(\theta^3),
\qquad
|\xi|^2=1+(6-2\mu)\theta^2+O(\theta^4).
$$

Consequently $\mu<3$ is unstable: sufficiently small nonzero frequencies have a [root of a polynomial](../../../../../../root-of-a-polynomial.md) of [modulus](../../../../../../modulus.md) greater than one, and arbitrarily fine periodic grids contain such frequencies.

Conversely, if $\mu\geq3$ and $s=\cos\theta$, then

$$
\operatorname{Re}A-3
=6(s-1)^2+4(\mu-3)(1-s)\geq0.
$$

For $A=u+iv$ with $u\geq3$,

$$
(|A|^2-1)^2-16|A-1|^2
=(u-1)^2(u-3)(u+5)+2(u^2-9)v^2+v^4\geq0.
$$

Since $|A|\geq3$, the [complex quadratic Schur criterion](../../../../../../complex-quadratic-schur-criterion.md) yields both [roots of a polynomial](../../../../../../root-of-a-polynomial.md) in the [unit disk](../../../../../../unit-disk.md), strictly inside except at $\theta=0$, where they are $1$ and $1/3$. Uniform [stability](../../../../../../stability-of-a-numerical-method.md) follows directly from the [BDF2 discrete energy identity](../../../../../../bdf2-discrete-energy-identity.md): the modal recurrence is $3v^{n+2}-4v^{n+1}+v^n=-(A-3)v^{n+2}$, whose [energy](../../../../../../energy.md) decreases because $\operatorname{Re}(A-3)\geq0$. Summing the modal energies proves a bound independent of the grid and even of $\mu\geq3$; no eigenvector-separation assumption is needed. This is the [stability of a spatially shifted BDF2 stencil](../../../../../../stability-of-a-spatially-shifted-bdf2-stencil.md). Thus the literal periodic-grid result is

$$
\boxed{\mu\geq3\quad\text{for the printed shifted stencil on a periodic grid}}.
$$

This cannot establish stability of an unspecified [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) closure. It also does not restore [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md).

For the intended unshifted [backward differentiation formula](../../../../../../backward-differentiation-formula.md), a spatial [eigenvalue](../../../../../../eigenvalue.md) $-\beta\leq0$ gives

$$
(3+2k\beta)\xi^2-4\xi+1=0.
$$

The [Schur stability criterion](../../../../../../schur-stability-criterion.md) gives the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) for every $k\beta\geq0$, with strict inequalities for $\beta>0$. A useful uniform [energy method](../../../../../../energy-method.md) proof, including the repeated interior roots that a bare separation argument would miss, is the [BDF2 discrete energy identity](../../../../../../bdf2-discrete-energy-identity.md). With $\delta^2U=U^{n+2}-2U^{n+1}+U^n$ and

$$
\mathcal E_n=\|U^{n+1}\|_h^2+\|2U^{n+1}-U^n\|_h^2,
$$

the corrected [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) scheme satisfies

$$
\mathcal E_{n+1}-\mathcal E_n+\|\delta^2U\|_h^2
+4k\|D_+U^{n+2}\|_h^2=0.
$$

This follows by taking the [inner product](../../../../../../inner-product.md) of $3U^{n+2}-4U^{n+1}+U^n=2kL_hU^{n+2}$ with $U^{n+2}$ and using [summation by parts](../../../../../../abel-s-summation-formula.md). It controls both time levels uniformly, regardless of the mesh ratio. Hence the corrected method is stable for

$$
\boxed{\text{every }\mu>0}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
