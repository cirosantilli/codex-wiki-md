<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

For the complete uniform disc, the surface density is $\sigma=M/(\pi a^2)$. An annular strip of radius $r$ and thickness $dr$ has mass $dm=2\pi\sigma r\,dr$, so its contribution to the axial [moment of inertia](../../../../../moment-of-inertia.md) is $r^2dm$. Hence

$$
\boxed{I_{\rm disc}=2\pi\sigma\int_0^ar^3\,dr=\frac12Ma^2.}
$$

This derives the [moment of inertia of a uniform disc](../../../../../moment-of-inertia-of-a-uniform-disc.md) rather than assuming it.

Removing a concentric disc of radius $a/2$ at the same density removes mass $M/4$ and inertia $\tfrac12(M/4)(a/2)^2=Ma^2/32$. The remaining annulus therefore has mass $m_A=3M/4$ and

$$
\boxed{I_A=\frac12Ma^2-\frac1{32}Ma^2=\frac{15}{32}Ma^2=\frac58m_Aa^2.}
$$

The [moment of inertia of a uniform annulus](../../../../../moment-of-inertia-of-a-uniform-annulus.md) gives the same value directly.

Let $A_c$ be the downhill centre-of-mass [acceleration](../../../../../acceleration.md) and let $F$ denote the magnitude of the uphill [static friction](../../../../../static-friction.md). Translation, rotation about the centre, and [rolling without slipping](../../../../../rolling-without-slipping.md) give

$$
m_AA_c=m_Ag\sin\alpha-F,\qquad I_A\dot\omega=Fa,\qquad A_c=a\dot\omega.
$$

Thus $F=I_AA_c/a^2=(5/8)m_AA_c$. Eliminating $F$ gives the [rolling acceleration with rotational inertia](../../../../../rolling-acceleration-with-rotational-inertia.md)

$$
\boxed{A_c=\frac{g\sin\alpha}{1+5/8}=\frac8{13}g\sin\alpha.}
$$

Substitution gives the contact forces

$$
\boxed{F=\frac{15}{52}Mg\sin\alpha\quad\text{up the plane},\qquad N=\frac34Mg\cos\alpha.}
$$

The [normal force](../../../../../normal-force.md) balances the perpendicular component of gravity because the centre remains at a constant distance from the plane. Although the annulus accelerates downhill, friction must act uphill to supply the [torque](../../../../../torque.md) that increases its rolling angular speed. For a plane with $0\leq\alpha<\pi/2$, the assumed no-slip motion requires a coefficient of [static friction](../../../../../static-friction.md) satisfying $\mu_s\geq F/N=(5/13)\tan\alpha$. With that condition, contact friction does no work because the instantaneous contact point is stationary; it redistributes the gravitational energy between translational and rotational [kinetic energy](../../../../../kinetic-energy.md).

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
