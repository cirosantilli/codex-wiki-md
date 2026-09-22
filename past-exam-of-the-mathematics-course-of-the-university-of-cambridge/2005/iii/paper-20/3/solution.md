<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work on a [closed](../../../../../closed-set.md) [compact](../../../../../compact-space.md) smooth [Riemannian manifold](../../../../../riemannian-manifold.md) $M$ without [boundary](../../../../../boundary-of-a-set.md), as in the usual discrete spectral setting here. Use the paper's $\Delta=\operatorname{tr}_g\operatorname{Hess}_g$, and put $P=-\Delta$. The [Riemannian heat kernel](../../../../../riemannian-heat-kernel.md) $H(t,x,y)$ is the smooth kernel, for $t>0$, representing the solution of

$$
\partial_tu=\Delta u,\qquad u(0,\cdot)=f,\qquad
u(t,x)=\int_M H(t,x,y)f(y)\,dV(y).
$$

Thus $(\partial_t-\Delta_x)H=0$ and its distributional initial value in $x$ is the [Dirac delta distribution](../../../../../dirac-delta-function.md) at $y$. The [heat trace](../../../../../heat-trace.md) is

$$
Z_M(t)=\int_M H(t,x,x)\,dV(x)=\operatorname{Tr}(e^{-tP}).
$$

The [heat invariants](../../../../../heat-invariants.md) are the coefficients $a_r(M)$ in the short-time [heat trace](../../../../../heat-trace.md) expansion specified below.

To derive its spectral form, take an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) $P\phi_j=\lambda_j\phi_j$, with $0=\lambda_0\le\lambda_1\le\cdots$, repeating [eigenvalues](../../../../../eigenvalue.md) according to [multiplicity](../../../../../multiplicity-mathematics.md). For the initial datum $\phi_j$, the function $e^{-t\lambda_j}\phi_j$ solves the [heat equation](../../../../../heat-equation.md). Uniqueness identifies it with the heat-kernel solution. Expanding arbitrary initial data in this basis therefore gives the [spectral expansion of the Riemannian heat kernel](../../../../../spectral-expansion-of-the-riemannian-heat-kernel.md):

$$
H(t,x,y)=\sum_{j=0}^\infty e^{-t\lambda_j}\phi_j(x)\overline{\phi_j(y)}.
$$

Standard elliptic estimates and [eigenvalue](../../../../../eigenvalue.md) growth imply smooth convergence for $t$ bounded away from zero: polynomial bounds on derivatives of [eigenfunctions](../../../../../eigenfunction.md) are dominated by the exponential factors. On the diagonal all summands are nonnegative, so [monotone convergence](../../../../../monotone-convergence-theorem.md) also justifies integration without needing an interchange of conditionally convergent terms. Since each [eigenfunction](../../../../../eigenfunction.md) has unit $L^2$ norm,

$$
\boxed{Z_M(t)=\sum_{j=0}^\infty e^{-t\lambda_j}.}
$$

Equivalently, if the paper's [Laplacian eigenvalues](../../../../../laplacian-eigenvalue.md) are written $\nu_j=-\lambda_j$, the formula is $\sum_j e^{t\nu_j}$; a growing exponential is not the [heat semigroup](../../../../../heat-semigroup.md).

Here are the needed [heat kernel expansion](../../../../../heat-kernel-expansion.md) facts, stated without proof. On a [closed](../../../../../closed-set.md) $d$-dimensional smooth [Riemannian manifold](../../../../../riemannian-manifold.md),

$$
H(t,x,x)\sim(4\pi t)^{-d/2}\sum_{r=0}^\infty u_r(x)t^r,\qquad u_0(x)=1,
$$

with the diagonal remainder uniform in $x$ after any finite truncation. The coefficients are smooth local geometric quantities; $u_1=R/6$. [Compactness](../../../../../compact-space.md) therefore allows integration term by term:

$$
Z_M(t)\sim(4\pi t)^{-d/2}\sum_{r=0}^\infty a_r(M)t^r,
\qquad a_r(M)=\int_Mu_r(x)\,dV(x),\qquad a_0(M)=\operatorname{Vol}(M)>0.
$$

These integrated coefficients are the [heat invariants](../../../../../heat-invariants.md). The uniform leading remainder in particular gives $Z_M(t)=(4\pi t)^{-d/2}(\operatorname{Vol}(M)+O(t))$.

[Isospectral manifolds](../../../../../isospectral-manifolds.md) have identical [heat traces](../../../../../heat-trace.md) by the derived spectral formula. If their dimensions were $d<e$, multiplying the common [trace](../../../../../matrix-trace.md) by $t^{d/2}$ would give a finite positive limit on the $d$-dimensional [manifold](../../../../../topological-manifold.md) but divergence on the $e$-dimensional one. Thus the dimensions are equal, and equality of the leading coefficient gives equal [Riemannian volume](../../../../../riemannian-volume.md). Explicitly,

$$
\boxed{d=2\lim_{t\downarrow0}\frac{\log Z_M(t)}{\log(1/t)},\qquad
\operatorname{Vol}(M)=\lim_{t\downarrow0}(4\pi t)^{d/2}Z_M(t).}
$$

The absence of a [boundary](../../../../../boundary-of-a-set.md) fixes this particular integer-power expansion. With a [boundary](../../../../../boundary-of-a-set.md) one must first specify [boundary conditions](../../../../../boundary-condition.md) and include the appropriate half-integer [boundary](../../../../../boundary-of-a-set.md) terms; the leading dimension-and-volume conclusion remains valid in the usual [compact](../../../../../compact-space.md) smooth setting.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
