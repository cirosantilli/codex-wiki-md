<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $w=v'-v$ and $D(v)=\operatorname{sym}\nabla v$. The supporting-hyperplane inequality for the convex [viscous dissipation potential](../../../../../../viscous-dissipation-potential.md) gives

$$
\Omega(D')-\Omega(D)\geq\sigma_{ij}(D'_{ij}-D_{ij}).
$$

The [stress](../../../../../../stress.md) is symmetric because its argument is a symmetric [rate-of-strain tensor](../../../../../../strain-rate-tensor.md), so $\sigma_{ij}(D'_{ij}-D_{ij})=\sigma_{ij}w_{i,j}$. Subtracting the two functional values yields

$$
\mathcal F(v')-\mathcal F(v)
\geq\int_{\mathcal D}\sigma_{ij}w_{i,j}\,dx
-\int_{\mathcal D}\rho g_iw_i\,dx
-\int_{S_t}t_i^0w_i\,dS.
$$

[Integration by parts](../../../../../../integration-by-parts.md) turns the first integral into

$$
\int_{\partial\mathcal D}\sigma_{ij}n_jw_i\,dS
-\int_{\mathcal D}\sigma_{ij,j}w_i\,dx.
$$

Inertialess [force balance](../../../../../../force-balance.md) is $\sigma_{ij,j}+\rho g_i=0$. The variation vanishes on $S_v$, and the [traction](../../../../../../traction.md) is $t_i^0$ on $S_t$. Thus both the volume and boundary contributions cancel exactly, proving the [convex viscous potential minimum principle](../../../../../../convex-viscous-potential-minimum-principle.md)

$$
\boxed{\mathcal F(v')\geq\mathcal F(v)
\quad\text{for every admissible }v'.}
$$

Only convexity, not strict convexity, is required, so no uniqueness follows just from this argument. For [incompressible flow](../../../../../../incompressible-flow.md), admissible trial [velocities](../../../../../../velocity.md) must also be divergence free. The [pressure](../../../../../../pressure.md) term then does no work, because $(-pI):(D'-D)=-p\,\operatorname{div}w=0$; the same proof applies to the deviatoric constitutive law.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
