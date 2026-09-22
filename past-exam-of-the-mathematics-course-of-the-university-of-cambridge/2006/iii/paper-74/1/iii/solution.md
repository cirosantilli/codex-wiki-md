<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There is a minor operator misprint to resolve first. Interpreting $(\mathbf x\cdot\nabla)^2$ as composition, the [Cartesian formula for the angular Laplacian](../../../../../../cartesian-formula-for-the-angular-laplacian.md) is

$$
\mathcal L^2=-\Delta_{S^2}
=-r^2\Delta+(\mathbf x\cdot\nabla)^2+\mathbf x\cdot\nabla.
$$

The last term is missing from the printed Cartesian expression. For example, its truncated expression maps $x_1$ to $x_1$, whereas a degree-one [spherical harmonic](../../../../../../spherical-harmonic.md) must have angular [eigenvalue](../../../../../../eigenvalue.md) two. In what follows, use the stated angular spectrum $l(l+1)$ and the supplied poloidal-energy identity; these are consistent with the corrected operator.

The [divergence theorem](../../../../../../divergence-theorem.md) and the [solenoidal magnetic-field constraint](../../../../../../solenoidal-magnetic-field-constraint.md) imply zero [magnetic flux](../../../../../../magnetic-flux.md) through every sphere. Consequently $P=rB_r$ has zero angular mean and no $l=0$ component. Expand in orthonormal [spherical harmonics](../../../../../../spherical-harmonic.md):

$$
P(r,\Omega)=\sum_{l\geq1}\sum_{m=-l}^lp_{lm}(r)Y_{lm}(\Omega),\qquad
\mathcal L^{-2}P=\sum_{l\geq1,m}\frac{p_{lm}(r)}{l(l+1)}Y_{lm}(\Omega).
$$

By angular [orthogonality](../../../../../../orthogonal-vectors.md), with

$$
D_{lm}=\int_0^\infty\left[r^2|p'_{lm}(r)|^2+l(l+1)|p_{lm}(r)|^2\right]\,dr\geq0,
$$

the gradient norm and the supplied [poloidal-toroidal decomposition](../../../../../../poloidal-toroidal-decomposition.md) identity become

$$
D=\sum_{l\geq1,m}D_{lm},\qquad
M_P:=\int_{\mathbb R^3}|\mathbf B_P|^2\,dV
=\sum_{l\geq1,m}\frac{D_{lm}}{l(l+1)}.
$$

Since $l(l+1)\geq2$, this proves the [poloidal magnetic energy bound by the radial scalar gradient](../../../../../../poloidal-magnetic-energy-bound-by-the-radial-scalar-gradient.md):

$$
\boxed{M_P\leq\frac12D.}
$$

Equality holds when the radial scalar contains only degree-one angular components.

Define the poloidal and total [magnetic energies](../../../../../../magnetic-energy.md) by $E_P=M_P/(2\mu_0)$ and $E_{\mathrm{total}}=M/(2\mu_0)$. Combining the [radial-flow dynamo energy bound](../../../../../../radial-flow-dynamo-energy-bound.md) with $D\geq2M_P$ gives the necessary condition

$$
\boxed{\left(\frac{\max_V|\mathbf u\cdot\mathbf x|}{\eta}\right)^2
\geq2\,\frac{E_P}{E_{\mathrm{total}}}.}
$$

It has the same temporal interpretation as the bound in the preceding part; statistically steady versions use the corresponding time-averaged energies. It quantifies why [dynamo action](../../../../../../dynamo-action.md) with a substantial poloidal fraction requires radial motion, while a purely tangential flow has $Q=0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
