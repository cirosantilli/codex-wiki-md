<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

Write $D=\partial_nA_n$ and use repeated-index summation. Because every $A_i$ is a [harmonic function](../../../../../harmonic-function.md),

$$
\partial_iu_i=D-\partial_kA_k-x_k\nabla^2A_k=0,
$$

and

$$
\nabla^2u_i=-2\partial_k\partial_iA_k=-2\partial_iD,\qquad \partial_ip=-2\mu\partial_iD.
$$

Thus $\mu\nabla^2u_i-\partial_ip=0$, the incompressible [Stokes equation](../../../../../stokes-equation.md). Moreover

$$
\partial_ju_i=\partial_jA_i-\partial_iA_j-x_k\partial_i\partial_jA_k.
$$

The antisymmetric first two terms cancel in the sum with $\partial_iu_j$, giving the [Newtonian fluid](../../../../../newtonian-fluid.md) [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md)

$$
\boxed{\sigma_{ij}=-p\delta_{ij}+\mu(\partial_ju_i+\partial_iu_j)=2\mu(\delta_{ij}D-x_k\partial_i\partial_jA_k).}
$$

For $A_i=V_i(1-a/(2r))$, harmonic outside the origin,

$$
\partial_iA_k=\frac{aV_kx_i}{2r^3},\quad u_i=V_i\left(1-\frac a{2r}\right)-\frac{ax_i(\mathbf V\cdot\mathbf x)}{2r^3},\quad p=-\frac{\mu a(\mathbf V\cdot\mathbf x)}{r^3}.
$$

At $r=a$ this gives $\mathbf u=\tfrac12[\mathbf V-(\mathbf V\cdot\mathbf n)\mathbf n]$, where $\mathbf n=\mathbf x/a$, so the normal velocity is zero. Also

$$
\partial_i\partial_jA_k=\frac{aV_k}{2}\left(\frac{\delta_{ij}}{r^3}-\frac{3x_ix_j}{r^5}\right),\qquad \sigma_{ij}=\frac{3\mu a(\mathbf V\cdot\mathbf x)x_ix_j}{r^5}.
$$

Hence on the surface,

$$
\boxed{\sigma_{ij}n_j=\frac{3\mu}{a}(\mathbf V\cdot\mathbf n)n_i,}
$$

a purely normal [traction](../../../../../traction.md), appropriate to a shear-free sphere rather than a no-slip solid sphere. Finally rotational symmetry gives $\int_{S^2}n_in_j\,d\Omega=(4\pi/3)\delta_{ij}$, so the fluid's force on the sphere is

$$
\boxed{\mathbf F=\int_{r=a}\boldsymbol\sigma\mathbf n\,dS=4\pi\mu a\mathbf V.}
$$

This is the [clean-bubble Stokes drag](../../../../../clean-bubble-stokes-drag.md) in the far-field velocity $\mathbf V$.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
