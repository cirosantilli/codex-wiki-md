<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The scalar contraction of the [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) is

$$
F_{\mu\nu}F^{\mu\nu}=2(B^2-E^2).
$$

With orientation $\epsilon^{0123}=+1$, define the [dual electromagnetic field tensor](../../../../dual-electromagnetic-field-tensor.md) by $\widetilde F^{\mu\nu}=\tfrac12\epsilon^{\mu\nu\rho\sigma}F_{\rho\sigma}$. Direct substitution gives

$$
\boxed{E^2-B^2=-\frac12F_{\mu\nu}F^{\mu\nu},\qquad
\mathbf E\cdot\mathbf B=-\frac14F_{\mu\nu}\widetilde F^{\mu\nu}.}
$$

The first is a [Lorentz scalar](../../../../lorentz-scalar.md); the second is a [pseudoscalar](../../../../pseudoscalar.md), invariant under proper [Lorentz transformations](../../../../lorentz-transformation.md) such as boosts and rotations. Under spatial inversion $\mathbf E$ changes sign while $\mathbf B$ does not, so $\mathbf E\cdot\mathbf B$ reverses sign. For example, $\mathbf E=\mathbf B=\widehat{\mathbf z}$ has product $+1$ before inversion and $-1$ afterwards. Thus the unrestricted statement including improper transformations needs this qualification.

For the spacetime integral, assume a globally regular [electromagnetic four-potential](../../../../electromagnetic-four-potential.md) on ordinary Minkowski space and sufficient boundary decay. Using $\nabla\cdot\mathbf B=0$ and $\partial_t\mathbf B=-\nabla\times\mathbf E$,

$$
\begin{aligned}
\partial_t(\mathbf A\cdot\mathbf B)
&=(-\mathbf E-\nabla\phi)\cdot\mathbf B-\mathbf A\cdot(\nabla\times\mathbf E)\\
&=-2\mathbf E\cdot\mathbf B-\nabla\cdot(\phi\mathbf B+\mathbf E\times\mathbf A).
\end{aligned}
$$

Consequently

$$
\boxed{\mathbf E\cdot\mathbf B=-\frac12\partial_t(\mathbf A\cdot\mathbf B)
-\frac12\nabla\cdot(\phi\mathbf B+\mathbf E\times\mathbf A).}
$$

The [magnetic helicity boundary term](../../../../magnetic-helicity-boundary-term.md) controls the integral. If its surface flux vanishes and the [magnetic helicity](../../../../magnetic-helicity.md) $H_B(t)=\int\mathbf A\cdot\mathbf B\,d^3x$ vanishes at both temporal ends, then

$$
\boxed{\int_{\mathbb R^4}\mathbf E\cdot\mathbf B\,d^4x
=-\frac12[H_B(+\infty)-H_B(-\infty)]=0.}
$$

Compactly supported smooth potentials are one sufficient version of the intended falloff assumption. The local identity is exact, but **vanishing fields at spatial infinity alone is insufficient**. For a concrete counterexample, take $\phi=0$ and, in dimensionless coordinates,

$$
\mathbf A=a(t)e^{-(x^2+y^2+z^2)}(-y,x,\lambda),\qquad \lambda\ne0,
$$

where $a$ changes smoothly from zero to one and $\dot a$ has compact temporal support. Both [electric fields](../../../../electric-field-split.md) and [magnetic fields](../../../../magnetic-field-split.md) vanish rapidly at spatial infinity, but

$$
H_B(t)=2\lambda\left(\frac\pi2\right)^{3/2}a(t)^2,
\qquad
\int\mathbf E\cdot\mathbf B\,d^4x
=-\lambda\left(\frac\pi2\right)^{3/2}\ne0.
$$

The counterexample leaves a final magnetic field and therefore fails the extra temporal boundary condition. It shows exactly why the printed integral cannot follow from a merely spatial reading of “at infinity”; vanishing of the full boundary term is the needed hypothesis.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
