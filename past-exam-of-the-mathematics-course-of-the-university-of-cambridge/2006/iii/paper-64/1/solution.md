<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [orthonormal coframe](../../../../../orthonormal-coframe-in-spacetime.md) writes a metric as $g=\eta_{ab}\theta^a\otimes\theta^b$ with constant diagonal signature [matrix](../../../../../matrix.md) $\eta$. In [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md), solve

$$
d\theta^a+\omega^a{}_b\wedge\theta^b=0,\qquad
\omega_{ab}=-\omega_{ba},\qquad \omega_{ab}=\eta_{ac}\omega^c{}_b.
$$

These are the torsion-free and metric-compatibility conditions and determine the [Levi-Civita connection](../../../../../levi-civita-connection.md). Then [Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md) gives

$$
\Omega^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b
=\frac12 R^a{}_{bcd}\theta^c\wedge\theta^d.
$$

Contract $R^a{}_{bad}$ to obtain the [Ricci tensor](../../../../../ricci-tensor.md) and then contract again for the [scalar curvature](../../../../../scalar-curvature.md). This fixes the curvature convention; reversing the definition of the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) reverses the resulting curvature signs.

On $z>0$, choose $\theta^0=dt/z$, $\theta^1=dx/z$, $\theta^2=dy/z$, $\theta^3=dz/z$, with $\eta=\operatorname{diag}(-1,1,1,1)$. For $a=0,1,2$,

$$
d\theta^a=\theta^a\wedge\theta^3,\qquad d\theta^3=0.
$$

A torsion-free metric connection therefore has

$$
\omega^a{}_3=-\theta^a,\qquad
\omega^3{}_a=\eta_{aa}\theta^a,\qquad
\omega^a{}_b=0\quad(a,b<3).
$$

For example, $\Omega^a{}_3=-d\theta^a=-\theta^a\wedge\theta^3$, while for $a,b<3$,

$$
\Omega^a{}_b=\omega^a{}_3\wedge\omega^3{}_b
=-\eta_{bb}\theta^a\wedge\theta^b.
$$

Metric antisymmetry supplies the remaining components, giving uniformly

$$
\boxed{\Omega^a{}_b=-\theta^a\wedge\theta_b,\qquad
R_{abcd}=-(\eta_{ac}\eta_{bd}-\eta_{ad}\eta_{bc}).}
$$

Thus the metric has constant [sectional curvature](../../../../../sectional-curvature.md) $-1$. In four dimensions,

$$
\boxed{\operatorname{Ric}_{\mu\nu}=-3g_{\mu\nu},\qquad R=-12.}
$$

It is an [Einstein manifold](../../../../../einstein-manifold.md), with Einstein constant $-3$ in the stated curvature convention.

These are [Poincare coordinates on anti-de Sitter spacetime](../../../../../poincare-coordinates-on-anti-de-sitter-spacetime.md) of unit radius. Constant curvature gives the maximal ten-dimensional local [isometry](../../../../../isometry.md) algebra $\mathfrak{so}(3,2)$. This can also be checked directly: set $u=(t,x,y)$, $\eta_{ab}=\operatorname{diag}(-1,1,1)$ and $u_a=\eta_{ab}u^b$. The ten independent [Killing vector fields](../../../../../killing-vector-field.md) are

$$
P_a=\partial_a,\qquad
M_{ab}=u_a\partial_b-u_b\partial_a,\qquad
D=u^a\partial_a+z\partial_z,\qquad
K_a=2u_aD-(u^bu_b+z^2)\partial_a.
$$

Translations and [Lorentz transformations](../../../../../lorentz-transformation.md) leave the numerator and $z$ unchanged. A dilation rescales numerator and denominator equally. For $K_a$, direct differentiation gives $\mathcal L_{K_a}\eta^{(4)}=4u_a\eta^{(4)}$ and $K_a(z)=2u_a z$, so the [conformal factor](../../../../../conformal-factor.md) cancels and $\mathcal L_{K_a}g=0$.

Hence the maximally extended [Anti-de Sitter spacetime](../../../../../anti-de-sitter-spacetime.md) has connected [isometry](../../../../../isometry.md) group locally $SO_0(3,2)$, with the appropriate covering group if one unwraps its time coordinate. The displayed coordinates cover only a patch. The ten local generators do not all give globally complete flows preserving that patch; for example special conformal flows can cross its horizon. The manifest complete patch symmetries include the boundary Poincare transformations and positive dilations. This distinguishes local maximal symmetry from the global [isometries](../../../../../isometry.md) of a chosen coordinate domain.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
