<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

In SI units, [Maxwell's equations](../../../maxwell-equations-split.md) in [vacuum](../../../vacuum.md), allowing [charge density](../../../charge-density.md) $\rho$ and [electric current density](../../../current-density.md) $\mathbf J$, are

$$
\boxed{\begin{aligned}
\nabla\cdot\mathbf E&=\rho/\epsilon_0,&\nabla\cdot\mathbf B&=0,\\
\nabla\times\mathbf E&=-\partial_t\mathbf B,&
\nabla\times\mathbf B&=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E.
\end{aligned}}
$$

The source-free specialization sets $\rho=0$ and $\mathbf J=0$; it cannot describe the charged objects at their locations. Applying the [divergence theorem](../../../divergence-theorem.md) to the first equation gives [Gauss's law](../../../gauss-s-law.md):

$$
\oint_{\partial\Omega}\mathbf E\cdot d\mathbf S
=\int_\Omega\nabla\cdot\mathbf E\,d^3x
=\frac{Q_{\mathrm{enc}}}{\epsilon_0}.
$$

For an isolated [point charge](../../../point-charge.md) $q_1$, [spherical symmetry](../../../spherical-symmetry.md) makes the [electric field](../../../electric-field-split.md) radial and constant in magnitude on a concentric sphere. Therefore $4\pi r^2E_r=q_1/\epsilon_0$. Multiplying by a second [point charge](../../../point-charge.md) gives [Coulomb's law](../../../coulomb-s-law.md),

$$
\boxed{\mathbf E=\frac{q_1}{4\pi\epsilon_0r^2}\hat{\mathbf r},\qquad
\mathbf F_{2}=\frac{q_1q_2}{4\pi\epsilon_0r^2}\hat{\mathbf r}.}
$$

The [force](../../../force-split.md) points away from the first charge for like signs and toward it for opposite signs.

For the [spherical capacitor](../../../spherical-capacitor.md), a Gaussian sphere between the shells encloses $q$, so $E_r=q/(4\pi\epsilon_0r^2)$ for $a<r<b$. Integrating the [electric field](../../../electric-field-split.md) inward from the outer shell yields

$$
V(r)-V(b)=-\int_b^r\frac{q}{4\pi\epsilon_0s^2}\,ds
=\frac{q}{4\pi\epsilon_0}\left(\frac1r-\frac1b\right).
$$

An arbitrary constant $V(b)$ remains unless a reference is specified. The [capacitance](../../../capacitance.md) is determined by the potential difference:

$$
\boxed{C=\frac{q}{V(a)-V(b)}=4\pi\epsilon_0\frac{ab}{b-a}.}
$$

For the subsequent charging operation, take the initial outer shell to be earthed, or interpret the stated $V$ as the inner-to-outer [voltage](../../../voltage.md) with the outer reference zero. Isolating the inner shell fixes its [electric charge](../../../electric-charge-split.md) at $q=CV$. Removing the outer shell leaves an isolated conducting sphere. Its [electric field](../../../electric-field-split.md) and [electric potential](../../../electric-potential.md), now with zero at infinity, are

$$
\mathbf E(r)=\begin{cases}0,&r<a,\\q\hat{\mathbf r}/(4\pi\epsilon_0r^2),&r>a,\end{cases}
\qquad
V(r)=\frac{q}{4\pi\epsilon_0r}\quad(r\geq a).
$$

Consequently

$$
\boxed{V_{\mathrm{surface}}=\frac{bV}{b-a},\qquad
V_{\mathrm{old\ outer\ position}}=\frac{aV}{b-a}.}
$$

These changes of [electric potential](../../../electric-potential.md) are compatible with constant [electric charge](../../../electric-charge-split.md). Without the initial reference convention the absolute stated $V$ does not determine $q=CV$: for example, if the outer shell were initially isolated and neutral, the absolute inner [electric potential](../../../electric-potential.md) would instead be $q/(4\pi\epsilon_0a)$.

Finally take the connected spheres to be sufficiently far apart that the long wire's [capacitance](../../../capacitance.md) and their mutual influence can be neglected. Their common [electric potential](../../../electric-potential.md) requires

$$
\frac{q_a}{a}=\frac{q_{2a}}{2a},\qquad q_a+q_{2a}=q,
$$

so $q_a=q/3$ and $q_{2a}=2q/3$. The magnitudes of the surface [electric fields](../../../electric-field-split.md) are

$$
E_a=\frac{q}{12\pi\epsilon_0a^2},\qquad E_{2a}=\frac{q}{24\pi\epsilon_0a^2},\qquad
\boxed{E_a:E_{2a}=2:1.}
$$

This is the usual widely separated-sphere approximation. A wire enforces an [equipotential](../../../equipotential.md), but alone does not make this ratio exact for arbitrary arrangements. As a concrete counterexample, if the second shell enclosed the first concentrically and they were connected, all net [electric charge](../../../electric-charge-split.md) would reside on the exterior and the inner sphere's surface [electric field](../../../electric-field-split.md) would be zero.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
