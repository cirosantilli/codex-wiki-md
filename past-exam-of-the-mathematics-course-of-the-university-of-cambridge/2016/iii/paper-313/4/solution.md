<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Poisson bivector](../../../../../poisson-bivector.md) is a smooth antisymmetric contravariant two-tensor

$$
\omega=\frac12\omega^{ij}(x)\partial_i\wedge\partial_j
$$

whose bracket on smooth functions,

$$
\boxed{\{F,G\}=\omega(dF,dG)=\omega^{ij}\partial_iF\partial_jG,}
$$

satisfies the [Jacobi identity](../../../../../jacobi-identity.md). Bilinearity and antisymmetry are immediate, and the product rule makes the bracket a derivation in each argument. Together these properties define a [Poisson manifold](../../../../../poisson-manifold.md). Unlike a [symplectic form](../../../../../symplectic-form.md), the [Poisson bivector](../../../../../poisson-bivector.md) need not be nondegenerate.

Apply the [Jacobi identity](../../../../../jacobi-identity.md) to the coordinate functions. Since $\{x^i,x^j\}=\omega^{ij}$,

$$
0=\{x^i,\{x^j,x^k\}\}+\{x^j,\{x^k,x^i\}\}+\{x^k,\{x^i,x^j\}\}
=\sum_m\left(\omega^{im}\partial_m\omega^{jk}
+\omega^{jm}\partial_m\omega^{ki}
+\omega^{km}\partial_m\omega^{ij}\right).
$$

Changing $\omega^{im}$ to $-\omega^{mi}$ and rearranging the three summands gives the printed [coordinate Jacobi condition for a Poisson bivector](../../../../../coordinate-jacobi-condition-for-a-poisson-bivector.md):

$$
\boxed{\sum_m\left(\omega^{mi}\partial_m\omega^{jk}
+\omega^{mk}\partial_m\omega^{ij}
+\omega^{mj}\partial_m\omega^{ki}\right)=0.}
$$

This is also sufficient: expanding the Jacobiator of three arbitrary smooth functions, all terms involving second derivatives cancel in pairs by antisymmetry. The remaining coefficient of $\partial_iF\partial_jG\partial_kH$ is the coordinate-function Jacobiator displayed above.

For a [Lie algebra](../../../../../lie-algebra-split.md), the natural global space carrying the proposed linear bracket is its [dual space](../../../../../dual-space.md) $\mathfrak g^*$. If $v^i$ is the chosen basis, define its linear coordinate function by $x^i(\ell)=\ell(v^i)$. The [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) is

$$
\boxed{\{F,G\}(\ell)=\ell([dF_\ell,dG_\ell])
=c^{ij}_kx^k\partial_iF\partial_jG,}
$$

where $dF_\ell,dG_\ell$ are elements of $\mathfrak g=(\mathfrak g^*)^*$. On a general manifold the same coordinate expression gives a local construction; a global one requires compatible transition rules. The use of $\mathfrak g^*$ supplies that compatibility intrinsically.

Here $\omega^{ij}=c^{ij}_rx^r$ and $\partial_m\omega^{jk}=c^{jk}_m$. The left side of the [coordinate Jacobi condition for a Poisson bivector](../../../../../coordinate-jacobi-condition-for-a-poisson-bivector.md) is therefore

$$
x^r\sum_m\left(c^{mi}_rc^{jk}_m+c^{mk}_rc^{ij}_m+c^{mj}_rc^{ki}_m\right)
=-x^r\sum_m\left(c^{jk}_mc^{im}_r+c^{ij}_mc^{km}_r+c^{ki}_mc^{jm}_r\right)=0.
$$

The final coefficient is the negative of the coefficient of $v^r$ in the [Lie algebra](../../../../../lie-algebra-split.md) identity $[v^i,[v^j,v^k]]+[v^j,[v^k,v^i]]+[v^k,[v^i,v^j]]=0$. Thus the [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) satisfies the [Jacobi identity](../../../../../jacobi-identity.md).

It remains to find the [Lie algebra structure constants](../../../../../structure-constant-of-a-lie-algebra.md) for the printed rotation fields. Distinguish their original spatial coordinates $(x,y,z)$ from the coordinates $(x^1,x^2,x^3)$ on the [dual space](../../../../../dual-space.md). Use the conventional [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md). Their component vectors are $(0,-z,y)$, $(z,0,-x)$ and $(-y,x,0)$, respectively. For example,

$$
[v^1,v^2]=(y,-x,0)=-v^3.
$$

Similarly,

$$
\boxed{[v^2,v^3]=-v^1,\qquad [v^3,v^1]=-v^2,\qquad
c^{ij}_k=-\epsilon_{ijk}.}
$$

The negative sign is essential: these are the fundamental fields of a left rotation action with the stated [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md), and consequently have the [infinitesimal left-action sign convention](../../../../../infinitesimal-left-action-sign-convention.md) discussed above. The first field here has component $y\partial_z$, as printed in the PDF.

The [Lie-Poisson bracket](../../../../../lie-poisson-bracket.md) on the [dual space](../../../../../dual-space.md) consequently has

$$
\{x^1,x^2\}=-x^3,\qquad
\{x^2,x^3\}=-x^1,\qquad
\{x^3,x^1\}=-x^2.
$$

For the evolution convention $\dot F=\{F,H\}$, the [Hamiltonian function](../../../../../hamiltonian-function.md) has derivatives $(2Ax^1,2Bx^2,2Cx^3)$. Substitution gives the [quadratic rotational Lie-Poisson dynamics](../../../../../quadratic-rotational-lie-poisson-dynamics.md)

$$
\boxed{\begin{aligned}
\dot x^1&=2(C-B)x^2x^3,\\
\dot x^2&=2(A-C)x^3x^1,\\
\dot x^3&=2(B-A)x^1x^2.
\end{aligned}}
$$

These are Euler-type [Hamilton's equations](../../../../../hamilton-s-equations.md) on a noncanonical [Poisson manifold](../../../../../poisson-manifold.md). When $A=1/(2I_1)$, $B=1/(2I_2)$ and $C=1/(2I_3)$ with positive principal inertias, they are the [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md) in body angular-momentum coordinates. As a check, $H$ is conserved by antisymmetry of the [Poisson bracket](../../../../../poisson-bracket.md), and $C_0=(x^1)^2+(x^2)^2+(x^3)^2$ is a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md). Direct differentiation of $C_0$ in the three equations cancels the terms $4[(C-B)+(A-C)+(B-A)]x^1x^2x^3$. The [Hamiltonian flow](../../../../../hamiltonian-flow.md) therefore lies on both an energy level and a sphere, a [symplectic leaf](../../../../../symplectic-leaf.md) of this signed rotational bracket.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
