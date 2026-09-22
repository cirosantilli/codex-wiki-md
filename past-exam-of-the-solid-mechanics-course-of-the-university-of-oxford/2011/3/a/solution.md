<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [displacement field](../../../../displacement-field-mechanics.md) is $u(x)=y(x)-x$, and its [gradient](../../../../gradient.md) is $Du=Dy-I$. [Linear elasticity](../../../../linear-elasticity.md) expands about an undeformed stress-free reference state, taking $y=x+\epsilon v$ with $|Du|\ll1$ and external loads of the same small order. A rigid translation need not itself be small; it is the [deformation gradient](../../../../deformation-gradient.md) that controls the [infinitesimal strain tensor](../../../../infinitesimal-strain-tensor.md).

For $W\in C^2$ with $DW(I)=0$, a [Taylor series](../../../../taylor-series.md) gives

$$
W(I+H)=W(I)+\frac12\mathbb A_{iA jB}H_{iA}H_{jB}+o(|H|^2),\qquad
\mathbb A_{iA jB}=\frac{\partial^2W}{\partial F_{iA}\partial F_{jB}}(I).
$$

The constant $W(I)$ can be set to zero. The [tensor](../../../../tensor.md) $\mathbb A$ is the [elasticity tensor](../../../../elasticity-tensor.md). Commutation of continuous [mixed partial derivatives](../../../../mixed-partial-derivative.md) proves its major [symmetry](../../../../symmetry-physics.md):

$$
\boxed{\mathbb A_{iA jB}=\mathbb A_{jB iA}.}
$$

[Material frame indifference](../../../../material-frame-indifference.md) at a stress-free reference also makes the quadratic energy depend only on the [infinitesimal strain tensor](../../../../infinitesimal-strain-tensor.md) $e=(H+H^T)/2$, leading to the usual minor [symmetries](../../../../symmetry-physics.md) after spatial and reference indices are identified.

In this scaling, an external [force](../../../../force-split.md) of order $\epsilon$ may be evaluated on the reference geometry: its change due to the order-$\epsilon$ displacement contributes only at order $\epsilon^2$. Thus the leading forces are fixed [dead loads](../../../../dead-loading.md). Likewise $F=I+O(\epsilon)$, $J=1+O(\epsilon)$ and $S=O(\epsilon)$, so the Piola transformation gives $T=J S F^{-T}=S+O(\epsilon^2)$. Hence **Cauchy and first Piola stresses agree to linear order**. This reasoning uses the usual small-load, stress-free linearization; an order-one prestress or leading follower-load effect requires a different expansion.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
