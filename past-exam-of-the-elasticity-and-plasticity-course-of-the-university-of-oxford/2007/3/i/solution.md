<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For antiplane [displacement](../../../../displacement.md) $u=(0,0,w)$ the only nonzero [strain](../../../../strain.md) components are $e_{xz}=w_x/2$ and $e_{yz}=w_y/2$. Commutation of [mixed partial derivatives](../../../../mixed-partial-derivative.md) gives the necessary local compatibility condition

$$
\boxed{\partial_ye_{xz}-\partial_xe_{yz}=0.}
$$

The supplied [stress](../../../../stress.md) is symmetric, independent of $z$ and trace-free. Its first two [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) equations are automatic; its third gives

$$
\partial_x\left(-\frac{\mu y}{x^2+y^2}\right)+
\partial_y\left(\frac{\mu x}{x^2+y^2}\right)=0
$$

away from the origin. [Antiplane shear](../../../../antiplane-shear.md) has zero trace, so isotropic [Hooke's law](../../../../hooke-s-law.md) reduces to $\boxed{e=\tau/(2\mu)}$. Hence

$$
\boxed{w_x=-\frac y{x^2+y^2},\qquad w_y=\frac x{x^2+y^2}.}
$$

Locally this integrates to $w=\arg(x+iy)+C$, represented on a suitable branch by $\arctan(y/x)+C$. The [strain](../../../../strain.md) condition is satisfied at every point of the [punctured plane](../../../../punctured-complex-plane.md), but the [displacement](../../../../displacement.md) cannot be made globally single-valued there:

$$
\boxed{\oint_{r=R}(w_x\,dx+w_y\,dy)=2\pi.}
$$

A [gradient](../../../../gradient.md) of a globally single-valued smooth [displacement](../../../../displacement.md) would instead integrate to zero around any [closed curve](../../../../closed-curve.md). Local compatibility is therefore not sufficient on this [multiply connected region](../../../../multiply-connected-region.md).

A physical construction is a Volterra [screw dislocation](../../../../screw-dislocation.md): cut the cylinder along a radial half-plane ending on its axis, shift one cut face relative to the other parallel to the axis, and rejoin. The axial mismatch is the [Burgers vector](../../../../burgers-vector.md). In the given normalization its magnitude is $2\pi$; with a dimensional mismatch $b$ one uses $w=b\arg(x+iy)/(2\pi)$. An intact pristine solid cannot reach this state by a smooth single-valued elastic deformation alone. The axis is a [dislocation core](../../../../dislocation-core.md) where the continuum elastic field is singular and must be regularized by microscopic structure or [plastic deformation](../../../../plastic-deformation.md). On the punctured domain the differential condition holds locally; globally its nonzero [circulation](../../../../circulation-physics.md) detects the defect. In a distributional description, that incompatibility is concentrated on the axis. This is [local strain compatibility versus screw-dislocation circulation](../../../../local-strain-compatibility-versus-screw-dislocation-circulation.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [3](../../3.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
