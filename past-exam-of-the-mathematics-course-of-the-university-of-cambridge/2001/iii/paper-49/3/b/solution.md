<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $q=\dot\gamma\tau$ and $f=1+\alpha\operatorname{tr}A$. With $L_{ij}=\partial_jv_i$, the steady homogeneous [upper-convected derivative](../../../../../../upper-convected-derivative.md) is $-LA-AL^T$. Its diagonal and shear equations give

$$
f a_{22}=f a_{33}=0,\qquad f a_{12}=q,\qquad f a_{11}=2q a_{12}.
$$

On the physical branch $f>0$, the other off-diagonal components vanish too. Thus $a_{22}=a_{33}=0$, $a_{11}=2a_{12}^2$ and

$$
\boxed{q=(1+2\alpha a_{12}^2)a_{12}.}
$$

For $\alpha\geq0$ the right side has derivative $1+6\alpha a_{12}^2>0$, so the shear stress determines a unique shear rate. The [shear viscosity](../../../../../../dynamic-viscosity.md) is $G_0\tau/f$ and decreases with shear magnitude when $\alpha>0$. This is the shear part of [shear and pipe flow of an affine linear PTT fluid](../../../../../../shear-and-pipe-flow-of-an-affine-linear-ptt-fluid.md).

For fully developed pipe flow take $\mathbf v=w(r)\widehat{\mathbf z}$ and the signed axial [pressure gradient](../../../../../../pressure-gradient.md) $dp/dz=\Delta p$. Regularity at the axis and the supplied momentum balance determine the shear stress without using the constitutive equation:

$$
\frac{d}{dr}(r\sigma_{rz})=\Delta p r,\qquad
\sigma_{rz}=\frac{\Delta p r}{2},\qquad a_{rz}=\frac{\Delta p r}{2G_0}.
$$

Locally the constitutive equations have the same shear form, with axial flow replacing the Cartesian flow direction and $\dot\gamma=w'(r)$ carrying its sign. Hence

$$
w'(r)=\frac1\tau(a_{rz}+2\alpha a_{rz}^3)
=\frac{\Delta p r}{2G_0\tau}+\frac{\alpha\Delta p^3 r^3}{4G_0^3\tau}.
$$

Integrating and imposing [no-slip boundary conditions](../../../../../../no-slip-boundary-condition.md) at $r=R$ gives

$$
\boxed{w(r)=-\frac{\Delta p}{4G_0\tau}(R^2-r^2)-\frac{\alpha\Delta p^3}{16G_0^3\tau}(R^4-r^4).}
$$

A negative pressure gradient produces positive axial flow. At $\alpha=0$ this is the ordinary [Hagen-Poiseuille flow](../../../../../../hagen-poiseuille-equation.md); positive $\alpha$ increases the flux at a fixed pressure drop through [shear thinning](../../../../../../shear-thinning.md). The nonzero axial normal stress varies radially, but its axial derivative vanishes in fully developed flow, so it does not change the axial momentum balance used here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
