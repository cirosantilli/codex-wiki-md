<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [first-order Sobolev space](../../../../first-order-sobolev-space.md) is $H^1(\Omega)=\{v\in L^2(\Omega):\partial_1v,\partial_2v\in L^2(\Omega)\}$, with derivatives understood as [weak derivatives](../../../../weak-derivative.md) and norm squared $\int_\Omega(v^2+|\nabla v|^2)$.

**The printed normal boundary condition must be distinguished from a conormal condition.** Take $K$ symmetric positive definite, as required for the symmetric matrix requested later. [Integration by parts](../../../../integration-by-parts.md) gives

$$
\int_\Omega\nabla v\cdot K\nabla u-\int_{\partial\Omega}v\,\mathbf n\cdot K\nabla u=\int_\Omega fv.
$$

The natural boundary term contains the [conormal derivative](../../../../conormal-derivative.md) $\mathbf n\cdot K\nabla u$, not the ordinary [normal derivative](../../../../normal-derivative.md) $\partial_nu$. On a smooth boundary, writing $\mathbf t$ for its unit tangent, the literal condition $\partial_nu=0$ leaves the term $b\partial_{\mathbf t}u$, where $b=\mathbf n\cdot K\mathbf t$. Its weak form therefore retains a boundary pairing:

$$
\int_\Omega\nabla v\cdot K\nabla u-\left\langle b\,\partial_{\mathbf t}(\operatorname{Tr}u),\operatorname{Tr}v\right\rangle=\int_\Omega fv.
$$

Here the tangential derivative of the [Sobolev trace](../../../../trace-operator.md) can be interpreted in $H^{-1/2}$ and paired against $H^{1/2}$ on a smooth boundary. This form is generally nonsymmetric; the requested usual symmetric energy construction does not follow from the literal boundary condition.

For an explicit failure of the claimed mean-zero compatibility, take the unit disk, $K=\operatorname{diag}(2,1)$ and $u=(x^2-y^2)[1-(x^2+y^2)/2]$. It has $\partial_nu=0$ on the circle, but

$$
f=-\nabla\cdot K\nabla u=-2+12x^2-6y^2,\qquad \int_\Omega f=-\frac\pi2\ne0.
$$

Thus replacing the printed normal condition by a zero conormal flux is not harmless.

For the intended zero-[conormal derivative](../../../../conormal-derivative.md) problem, the requested variational and finite element conclusions are as follows. Seek $u\in H^1(\Omega)$ with

$$
\boxed{a(u,v):=\int_\Omega\nabla v\cdot K\nabla u=\ell(v):=\int_\Omega fv\quad(v\in H^1(\Omega)).}
$$

Putting $v=1$ gives $\int_\Omega f=0$. On a connected domain this condition permits a solution unique modulo constants; the [Poincare-Wirtinger inequality](../../../../poincare-wirtinger-inequality.md) gives coercivity after fixing the mean.

The energy is $J(v)=\tfrac12a(v,v)-\ell(v)$. A minimizer satisfies $\frac d{dt}J(u+tv)|_{t=0}=a(u,v)-\ell(v)=0$. Conversely, a weak solution satisfies

$$
J(v)-J(u)=\frac12a(v-u,v-u)\geq0,
$$

so it is a minimizer. Testing by $u$ gives the minimum value

$$
\boxed{J_{\min}=-\frac12\ell(u)=-\frac12a(u,u).}
$$

This value is independent of the arbitrary additive constant when $\int f=0$. If the compatibility fails, constant shifts make $J$ unbounded below.

Write $u_h=\sum_jc_j\phi_j$. The [Galerkin method](../../../../galerkin-method.md) gives

$$
\boxed{Ac=F,\qquad A_{ij}=\int_\Omega\nabla\phi_i\cdot K\nabla\phi_j,\qquad F_i=\int_\Omega f\phi_i.}
$$

Symmetry of $K$ gives $A^T=A$. For $v_h=\sum_jz_j\phi_j$, $z^TAz=\int_\Omega\nabla v_h\cdot K\nabla v_h\geq0$. Equality forces $v_h$ constant by positive definiteness and connectedness. Since the basis sums to one, the coefficient vector $\mathbf1=(1,\ldots,1)^T$ represents that constant, giving

$$
\boxed{\ker A=\operatorname{span}(\mathbf1),\qquad \mathbf1^TF=\int_\Omega f=0.}
$$

Thus the [stiffness matrix](../../../../stiffness-matrix.md) is symmetric positive semidefinite and singular; the displayed compatibility condition is necessary and sufficient for the finite system. Positive definiteness of $K$ controls every gradient direction, preventing additional zero-energy directions and supplying ellipticity. A degenerate coefficient can introduce further kernel modes, while an indefinite one destroys the minimizing-energy argument.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../split.md)
5. [Approximation theory and finite element methods course of the University of Oxford](../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
