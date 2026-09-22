<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Decomposing a plane [displacement](../../../../displacement.md) into components parallel and perpendicular to its [wavevector](../../../../wavevector.md) gives compressional and shear speeds

$$
\boxed{c_p=\sqrt{(\lambda+2\mu)/\rho},\qquad c_s=\sqrt{\mu/\rho},\qquad
k_p=\omega/c_p,\quad k_s=\omega/c_s.}
$$

The incident [polarization](../../../../polarization-waves.md) is longitudinal. Its reflected [longitudinal wave](../../../../longitudinal-wave.md) reverses the vertical [wavevector](../../../../wavevector.md) component while retaining its horizontal component. The converted [shear wave](../../../../shear-wave.md) has [wavevector](../../../../wavevector.md) $k_s(\sin\beta,-\cos\beta)$ perpendicular to [polarization](../../../../polarization-waves.md) $(\cos\beta,\sin\beta)$.

Every term must have the same [phase](../../../../phase-waves.md) along the rigid boundary. Thus

$$
\boxed{k_s\sin\beta=k_p\cos\alpha,\qquad
\sin\beta=\frac{c_s}{c_p}\cos\alpha.}
$$

Choose $\cos\beta>0$ so the reflected [shear wave](../../../../shear-wave.md) propagates downward into $y<0$. At $y=0$, both [displacement](../../../../displacement.md) components must vanish for every boundary [phase](../../../../phase-waves.md):

$$
(1+R_1)\cos\alpha+R_2\cos\beta=0,\qquad
(1-R_1)\sin\alpha+R_2\sin\beta=0.
$$

Solving this two-by-two system yields

$$
\boxed{R_1=\frac{\sin(\alpha-\beta)}{\sin(\alpha+\beta)},\qquad
R_2=-\frac{\sin2\alpha}{\sin(\alpha+\beta)}.}
$$

For a stable isotropic material $0<c_s/c_p<1$. An incident wave directed toward the boundary has $0<\alpha<\pi$; choosing $\beta\in(-\pi/2,\pi/2)$ by the sine relation gives real reflected waves throughout this range and no zero denominator. In the usual convention restricting incident horizontal propagation to positive $x$, this is $0<\alpha\leq\pi/2$. Grazing endpoints have no incoming normal energy flux and are limiting cases. There is no [critical angle](../../../../critical-angle-for-total-internal-reflection.md) for incident compressional-to-shear conversion here, because the converted wave is slower; the opposite incident-wave type has different critical-angle behaviour. At [normal incidence](../../../../normal-incidence.md) $\alpha=\pi/2$, $\beta=0$, $R_1=1$ and $R_2=0$, cancelling the incident [displacement](../../../../displacement.md) with the reversed longitudinal [polarization](../../../../polarization-waves.md). This is [compressional-wave reflection from a rigid elastic boundary](../../../../compressional-wave-reflection-from-a-rigid-elastic-boundary.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [2](../../2.md)
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
