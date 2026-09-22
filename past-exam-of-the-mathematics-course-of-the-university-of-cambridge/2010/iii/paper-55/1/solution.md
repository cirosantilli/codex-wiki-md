<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Treat the [orthonormal coframe in spacetime](../../../../../orthonormal-coframe-in-spacetime.md) and the Lorentz [connection 1-form](../../../../../connection-1-form-split.md) as independent variables, with nondegenerate coframe and $\omega_{ab}=-\omega_{ba}$. Fix the curvature convention

$$
R^a{}_b=d\omega^a{}_b+\omega^a{}_c\wedge\omega^c{}_b,qquad
T^a=dE^a+\omega^a{}_b\wedge E^b.
$$

The second expression is [Cartan's first structure equation](../../../../../cartan-s-first-structure-equation.md); the first is [Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md). Use compactly supported variations, or boundary data that make the variation's surface term vanish.

For a connection variation, $\delta R^{ab}=D\delta\omega^{ab}$, where $D$ is the [covariant exterior derivative](../../../../../exterior-covariant-derivative.md). Since $D\epsilon_{abc}=0$, its graded product rule gives

$$
\delta_\omega I=\int_M\epsilon_{abc}\delta\omega^{ab}\wedge T^c
+\int_{\partial M}\epsilon_{abc}\delta\omega^{ab}\wedge E^c.
$$

For a coframe variation, relabeling the dummy indices makes the three variations of the cubic term identical. Hence

$$
\delta_E I=\int_M\epsilon_{abc}\delta E^c\wedge
\left(R^{ab}+3\lambda E^a\wedge E^b\right).
$$

The independent variations therefore give $\epsilon_{abc}T^c=0$ and $\epsilon_{abc}(R^{ab}+3\lambda E^a\wedge E^b)=0$. In three dimensions the alternating symbol identifies an antisymmetric index pair with a single index, so these equations are equivalent to

$$
\boxed{T^a=0,\qquad R^{ab}=-3\lambda E^a\wedge E^b.}
$$

These are the equations of [first-order three-dimensional gravity](../../../../../first-order-three-dimensional-gravity.md). The first selects the [Levi-Civita connection](../../../../../levi-civita-connection.md); the second fixes [constant sectional curvature](../../../../../constant-sectional-curvature.md) $K=-3\lambda$. The factor of three follows from varying the coefficient exactly as printed.

On a static coordinate patch where $f>0$, choose the Lorentz frame metric $\eta_{ab}=\operatorname{diag}(-1,1,1)$ and coframe

$$
E^0=\sqrt f\,dt,\qquad E^1=\frac{dr}{\sqrt f},\qquad E^2=r\,d\theta.
$$

Put $A=f'/(2\sqrt f)$ and $B=\sqrt f/r$. Exterior differentiation gives $dE^0=-AE^0\wedge E^1$, $dE^1=0$, and $dE^2=BE^1\wedge E^2$. Solving the equation of vanishing [torsion forms](../../../../../torsion-form.md) gives

$$
\omega^{01}=AE^0=\frac{f'}2dt,\qquad
\omega^{12}=-BE^2=-\sqrt f\,d\theta,\qquad
\omega^{02}=0.
$$

Here antisymmetry is in the two raised or two lowered frame indices; mixed time-space components have equal, rather than opposite, signs. This is the [Lorentzian connection-form antisymmetry](../../../../../lorentzian-connection-form-antisymmetry.md) needed to retain the curvature signs.

Using [Cartan's second structure equation](../../../../../cartan-s-second-structure-equation.md), the nonzero [curvature 2-forms](../../../../../curvature-2-form.md) are

$$
R^{01}=-\frac{f''}2 E^0\wedge E^1,\qquad
R^{02}=-\frac{f'}{2r}E^0\wedge E^2,\qquad
R^{12}=-\frac{f'}{2r}E^1\wedge E^2.
$$

For example, $d(AE^0)=-(\sqrt f A'+A^2)E^0\wedge E^1=-f''E^0\wedge E^1/2$, while the $02$ form is the product $\omega^0{}_1\wedge\omega^{12}=-AB E^0\wedge E^2$. Thus the field equations require $f''/2=3\lambda$ and $f'/(2r)=3\lambda$. Integrating the latter gives $f=C+3\lambda r^2$; the former is then satisfied automatically. The origin condition fixes $C=1$, yielding

$$
\boxed{f(r)=1+3\lambda r^2.}
$$

As a sign and normalization check, the [Ricci tensor](../../../../../ricci-tensor.md) is $R_{\mu\nu}=-6\lambda g_{\mu\nu}$ and the [scalar curvature](../../../../../scalar-curvature.md) is $R=-18\lambda$. The coframe calculation applies initially in the region with $f>0$; if $\lambda<0$, $f$ vanishes at $r=1/\sqrt{-3\lambda}$, delimiting that static chart without changing the derived function.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
