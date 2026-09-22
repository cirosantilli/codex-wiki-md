<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D=H-h$ be the constant interior depth. Assume a homogeneous hydrostatic interior with depth-independent horizontal velocity, negligible friction, steady small-[Rossby number](../../../../../../rossby-number.md) flow, and no normal flow through the flat bottom. The vertical velocity varies from $w(-H)=0$ to $w(-h)=w_E$, so [incompressible flow](../../../../../../incompressible-flow.md) gives

$$
u_x+v_y=-\frac{w_E}{D}.
$$

The leading horizontal momentum balance is [geostrophic balance](../../../../../../geostrophic-balance.md):

$$
-fv=-\frac1\rho p_x,
\qquad
fu=-\frac1\rho p_y.
$$

Taking its vertical curl on a [beta plane](../../../../../../beta-plane.md) gives

$$
f(u_x+v_y)+\beta v=0.
$$

Combining the last two equations yields [Sverdrup balance](../../../../../../sverdrup-balance.md)

$$
\boxed{
\beta Dv=fw_E},
\qquad
\boxed{
v=\frac{f}{\beta D}w_E}.
$$

The zonal velocity is then fixed, up to its value on one side boundary, by

$$
\boxed{
u_x=-\frac{w_E}{D}
-\frac{\partial}{\partial y}
\left(\frac{fw_E}{\beta D}\right)}.
$$

Equivalently, substituting part a gives the depth-integrated form

$$
\boxed{
\beta Dv
=\frac f\rho
\widehat{\mathbf z}\mathbin\cdot
\nabla_h\times\left(\frac{\boldsymbol\tau}{f}\right)}.
$$

A lateral boundary condition, normally supplied by matching to a boundary current, determines the remaining zonally uniform part of $u$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
