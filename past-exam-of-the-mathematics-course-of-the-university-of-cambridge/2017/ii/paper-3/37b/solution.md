<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

Write $Q=U_jx_j$ and use repeated-index summation. Direct differentiation gives

$$
 \partial_ju_i=\frac a2\left[-\frac{U_ix_j}{r^3}+\frac{U_jx_i}{r^3}
 +\frac{Q\delta_{ij}}{r^3}-\frac{3Qx_ix_j}{r^5}\right].
$$

Tracing yields $\partial_i u_i=0$. Since $\nabla^2(1/r)=0$ for $r>a$, and $\nabla^2(Qx_i/r^3)=2U_i/r^3-6Qx_i/r^5$, we get

$$
 \mu\nabla^2u_i=\mu a\left(\frac{U_i}{r^3}-\frac{3Qx_i}{r^5}\right)=\partial_i p.
$$

Hence the incompressible [Stokes equations](../../../../../stokes-equation.md) hold everywhere outside the bubble.

The Newtonian [viscous stress tensor](../../../../../viscous-stress-tensor.md) $T_{ij}=-p\delta_{ij}+\mu(\partial_ju_i+\partial_iu_j)$ simplifies to

$$
\boxed{T_{ij}=-\frac{3\mu aQx_ix_j}{r^5}.}
$$

At $r=a$ with $n=x/a$, $u=\tfrac12[U+(U\cdot n)n]$, so $u\cdot n=U\cdot n$: the interface is impermeable in the bubble frame. Also $Tn=-(3\mu/a)(U\cdot n)n$ is purely normal, so the tangential traction vanishes, appropriate to a clean bubble with negligible internal viscosity. The tangential fluid [velocity](../../../../../velocity.md) need not equal the bubble's [velocity](../../../../../velocity.md). At infinity $u,p\to0$. The calculation assumes the usual spherical, negligible-deformation [limit](../../../../../limit-of-a-function.md); exact normal-stress balance includes interior [pressure](../../../../../pressure.md), [surface tension](../../../../../surface-tension.md) and any buoyancy sustaining the motion.

Integrate the outer-fluid traction with the normal pointing from the bubble into the fluid:

$$
 F_i=-\frac{3\mu}{a}U_j\int n_in_j\,dS=-4\pi\mu aU_i.
$$

Thus $\boxed{F_{\rm drag}=-4\pi\mu aU}$, smaller than the no-slip rigid-[sphere](../../../../../sphere.md) [Stokes drag law](../../../../../stokes-s-law.md) $-6\pi\mu aU$.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
