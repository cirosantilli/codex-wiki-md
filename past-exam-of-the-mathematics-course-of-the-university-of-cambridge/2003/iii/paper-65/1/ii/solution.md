<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Continue on the branch of [steady planar ideal-MHD field-line invariants](../../../../../../steady-planar-ideal-mhd-field-line-invariants.md), with $k\ne0$ and positive $\rho,T$. Adiabatic entropy transport gives $\mathbf u\cdot\nabla s=0$. As all quantities are $z$-independent,

$$
\mathbf u\cdot\nabla=\frac{k}{\rho}\mathbf B\cdot\nabla,
\qquad\boxed{\mathbf B\cdot\nabla s=0}.
$$

The axial component of the [ideal magnetohydrodynamic momentum equation](../../../../../../ideal-magnetohydrodynamic-momentum-equation.md) has no pressure or gravitational term. Magnetic tension gives

$$
\rho\mathbf u_h\cdot\nabla u_z=\frac1{\mu_0}\mathbf B_h\cdot\nabla B_z.
$$

Since $k$ is constant along a [magnetic field line](../../../../../../magnetic-field-line.md), this becomes

$$
\boxed{\mathbf B\cdot\nabla V=0,\qquad V=u_z-\frac{B_z}{\mu_0k}}.
$$

Subtracting the two axial invariants yields the useful compatibility relation

$$
\boxed{B_z\left(\frac{\mu_0k^2}{\rho}-1\right)=\mu_0k(V-U)}.
$$

The squared ratio of horizontal flow speed to horizontal [Alfvén speed](../../../../../../alfven-speed.md) is $M_h^2=\mu_0k^2/\rho$; vector equality with the horizontal [Alfvén velocity](../../../../../../alfven-velocity.md) additionally requires $k>0$. If $V-U\ne0$, the right side is a nonzero constant along the field line, so a regular finite $B_z$ cannot permit $M_h^2=1$ anywhere. This is the nondegenerate exclusion.

However, $B_z\not\equiv0$ does not imply $V-U\ne0$. The [Alfvénic degeneracy of steady planar MHD](../../../../../../alfvenic-degeneracy-of-steady-planar-mhd.md) is a genuine exception: take constant $\rho,p,s$, $\Phi=0$, and a constant magnetic field with nonzero horizontal and axial components, and set

$$
\mathbf u=\frac{\mathbf B}{\sqrt{\mu_0\rho}},\qquad
k=\sqrt{\rho/\mu_0},\qquad U=V=0.
$$

Every equation holds, but the horizontal velocity equals the horizontal [Alfvén velocity](../../../../../../alfven-velocity.md) everywhere despite $B_z\ne0$. Therefore **the printed pointwise exclusion needs a nondegeneracy hypothesis, such as $V\ne U$**. The general conclusion is the boxed compatibility relation; when $V=U$, it says $(M_h^2-1)B_z=0$ and allows the Alfvénic branch.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
