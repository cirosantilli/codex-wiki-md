<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For time dependence $e^{-i\omega t}$, a scalar Fresnel-Kirchhoff aperture formula for a point-source [amplitude](../../../../../wave-amplitude.md) $A$ is

$$
U(P)=\frac{A}{i\lambda}\int_{\mathcal A}
K(Q)\frac{e^{ik[s(Q)+r(Q)]}}{s(Q)r(Q)}\,dS_Q,\qquad k=\frac{2\pi}{\lambda}.
$$

Here $s=|S-Q|$, $r=|P-Q|$, and $K$ is the [obliquity factor](../../../../../obliquity-factor.md), approximately the mean of the incident and outgoing direction cosines measured with the forward aperture normal. The factors describe incident spherical spreading, outgoing spreading and accumulated phase. This is the scalar Kirchhoff aperture approximation; it does not supply an exact electromagnetic edge boundary solution.

In the Fresnel regime, expand path lengths to quadratic order in aperture coordinates while replacing slowly varying [amplitude](../../../../../wave-amplitude.md) and [obliquity factors](../../../../../obliquity-factor.md) by their axial values. In the Fraunhofer regime the quadratic aperture phase is negligible, leaving the aperture [Fourier transform](../../../../../fourier-transform-split.md). For characteristic aperture size $D$, the latter requires $D^2/(\lambda R)\ll1$ in the relevant finite-source geometry; a [lens](../../../../../lens-optics.md) can supply the Fourier-plane configuration.

For the one-dimensional Cornu construction, put $S,O,P$ on the unobstructed straight ray, with the aperture plane perpendicular at $O$. An element is displaced transversely by $x$, with $|x|\ll a,b$, where $a=SO$ and $b=OP$. A long straight edge or slit makes the other transverse direction separable. Then

$$
\sqrt{a^2+x^2}+\sqrt{b^2+x^2}
=a+b+\frac{x^2}{2}\left(\frac1a+\frac1b\right)+O(x^4),
\qquad
\boxed{\frac1R=\frac1a+\frac1b}.
$$

For [knife-edge diffraction](../../../../../knife-edge-diffraction.md) at the fence, the edge is $h=0.5\ \mathrm m$ above the direct ray, with $a=5\ \mathrm m$, $b=45\ \mathrm m$, $\lambda\simeq0.100\ \mathrm m$, and $R=4.5\ \mathrm m$. The unblocked aperture extends upward from $h$, so its Cornu chord runs from $u_h=h\sqrt{2/(\lambda R)}=1.054$ to infinity. Using $C(\infty)=S(\infty)=1/2$ and normalizing by the full unobstructed chord gives

$$
\boxed{\mathcal T=\frac{I_{\rm fence}}{I_{\rm free}}
=\frac{[1/2-C(u_h)]^2+[1/2-S(u_h)]^2}{2}
\simeq0.038}.
$$

The approximate chord coordinates are $C=0.775$, $S=0.492$. This is the standard single-knife-edge Fresnel normalization.[Annex 1, Sections 2.7 and 4.1, Fresnel integrals and single knife edge](../../../../../propagation-by-diffraction-itu-r-p-526-13-by-international-telecommunication-union.md)

For [geometric spreading in a moving-receiver diffraction measurement](../../../../../geometric-spreading-in-a-moving-receiver-diffraction-measurement.md), set $b=d$ while retaining $a=5$ and $h=0.5$:

$$
u(d)=h\sqrt{\frac2\lambda\left(\frac15+\frac1d\right)},\qquad
I_{\rm received}(d)\propto\frac{\mathcal T[u(d)]}{(5+d)^2}.
$$

**Normalized transmission decreases toward the fence. Absolute received [intensity](../../../../../intensity-physics.md) initially increases**, because the free-space spherical-wave [intensity](../../../../../intensity-physics.md) rises as source–receiver distance decreases. In this model it reaches a maximum near $d\simeq2.3\ \mathrm m$, then falls. The formal paraxial small-$d$ behavior is $I\propto d/(5+d)^3$; extrapolation to $d\lesssim h$ is outside the [small-angle approximation](../../../../../small-angle-approximation.md). The sketch distinguishes the absolute signal from its ratio to the unobstructed signal at each position.

<a id="section-b/b9/image-original-knife-edge-geometry-and-distinct-absolute-intensity-and-normalized-transmission-predictions"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2014/paper-2-fence-diffraction.png)

**[Figure 3](#section-b/b9/image-original-knife-edge-geometry-and-distinct-absolute-intensity-and-normalized-transmission-predictions). Original knife-edge geometry and distinct absolute-intensity and normalized-transmission predictions**.

## ↑ Ancestors (14)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
