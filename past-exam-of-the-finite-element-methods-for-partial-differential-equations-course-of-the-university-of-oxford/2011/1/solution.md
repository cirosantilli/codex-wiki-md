<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the usual bounded [Lipschitz domain](../../../lipschitz-domain.md) assumptions so that the [Sobolev trace](../../../trace-operator.md) is defined. Multiplication by $v\in H^1(\Omega)$ and [Green's first identity](../../../green-s-first-identity.md) give

$$
\int_\Omega\nabla u\cdot\nabla v-\int_{\partial\Omega}\frac{\partial u}{\partial n}v=\int_\Omega fv.
$$

The [Robin boundary condition](../../../robin-boundary-condition.md) substitutes $\partial_nu=-u$ in the boundary integral. The resulting [Weak formulation of the Robin Poisson problem](../../../weak-formulation-of-the-robin-poisson-problem.md) is therefore: find $u\in H^1(\Omega)$ such that

$$
\boxed{a(u,v):=\int_\Omega\nabla u\cdot\nabla v+\int_{\partial\Omega}uv=\int_\Omega fv\quad\text{for every }v\in H^1(\Omega).}
$$

The boundary values in the integral mean [Sobolev traces](../../../trace-operator.md); no classical normal [derivative](../../../derivative.md) is required of the weak solution. For uniqueness, subtract two solutions and test by their difference $w$. This yields $\int_\Omega|\nabla w|^2+\int_{\partial\Omega}w^2=0$. Thus $\nabla w=0$, so $w$ is constant on each [connected component](../../../connected-component.md), and its vanishing boundary [Sobolev trace](../../../trace-operator.md) makes each constant zero. **The weak solution is unique.**

For a [bilinear square finite element](../../../bilinear-square-finite-element.md) with corners numbered anticlockwise from the lower-left corner, introduce local coordinates $\xi=(x-x_L)/h$, $\eta=(y-y_B)/h$. The four [shape functions](../../../shape-function.md) are

$$
N_1=(1-\xi)(1-\eta),\quad N_2=\xi(1-\eta),\quad N_3=\xi\eta,\quad N_4=(1-\xi)\eta.
$$

The local [stiffness matrix](../../../stiffness-matrix.md) has entries $K_{ij}=\int_E\nabla N_j\cdot\nabla N_i$. The factor $h^2$ from the area element cancels the two factors $h^{-1}$ from the [gradients](../../../gradient.md). Symmetry leaves three types: diagonal, adjacent corners, and opposite corners. For representatives,

$$
\begin{aligned}
K_{11}&=\int_0^1\!\int_0^1[(1-\eta)^2+(1-\xi)^2],d\xi\,d\eta=2/3,\\
K_{12}&=\int_0^1\!\int_0^1[-(1-\eta)^2+\xi(1-\xi)],d\xi\,d\eta=-1/6,\\
K_{13}&=\int_0^1\!\int_0^1[-\eta(1-\eta)-\xi(1-\xi)],d\xi\,d\eta=-1/3.
\end{aligned}
$$

Consequently

$$
\boxed{K_E=\frac16\begin{pmatrix}4&-1&-2&-1\\-1&4&-1&-2\\-2&-1&4&-1\\-1&-2&-1&4\end{pmatrix}.}
$$

For an element whose left edge lies on $x=0$, the boundary term in the [weak formulation](../../../weak-formulation.md) adds $B_{ij}=\int_eN_jN_i\,ds$. Only $N_1=1-\eta$ and $N_4=\eta$ are nonzero on that edge. Integrating $h(1-\eta)^2$, $h\eta(1-\eta)$ and $h\eta^2$ gives the extra contribution

$$
\boxed{B_e=\frac h6\begin{pmatrix}2&0&0&1\\0&0&0&0\\0&0&0&0\\1&0&0&2\end{pmatrix}.}
$$

Its entries are added at the corresponding global node numbers during [finite element assembly](../../../finite-element-assembly.md). Additional boundary edges contribute their own analogous edge matrices. The [Robin boundary condition](../../../robin-boundary-condition.md) is represented by these integrals, so boundary nodes remain unknowns.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2011](../../2011-split.md)
3. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../split.md)
4. [Finite element methods for partial differential equations course of the University of Oxford](../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
