<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [geodetic precession](../../../../geodetic-effect.md) per orbit is

$$
\boxed{\Delta\psi=2\pi\left(1-\sqrt{1-\frac{3}{400}}\right)
\simeq0.0236063\,\mathrm{rad}=1.35254^\circ.}
$$

The orbital position and [four-velocity](../../../../four-velocity.md) repeat after a full orbit, so the direction to distant Earth in the instantaneous [rest frame](../../../../rest-frame.md) repeats. The freely transported [gyroscope](../../../../gyroscope.md) does not: its beam axis has turned through $\Delta\psi$ relative to the original aiming direction. This applies to any initial in-plane spin direction by linearity of [parallel transport](../../../../parallel-transport.md), not only the radial initial condition used in part (b). The beam's angular diameter is $1^\circ$, giving a half-angle of $0.5^\circ$. Thus **Earth lies outside the beam after one orbit**; comparing the offset with the diameter would already show a miss, but the correct acceptance angle is the half-angle.

The initial radial ray must be outward from the [black hole](../../../../black-hole-split.md) for a direct path to Earth. A precisely inward radial [null geodesic](../../../../null-geodesic.md) falls into the [black hole](../../../../black-hole-split.md) and cannot provide the assumed initial communication. For [outgoing near-radial Schwarzschild light deflection](../../../../outgoing-near-radial-schwarzschild-light-deflection.md), the angular correction is especially small. If a static observer at $R$ measures a small emission angle $\psi$ from the outward radial direction, its [impact parameter](../../../../impact-parameter.md) is $b=R\sin\psi/\sqrt{f(R)}$. The outgoing [null geodesic](../../../../null-geodesic.md) gives

$$
\Delta\phi=\int_R^\infty\frac{b\,dr}{r^2\sqrt{1-f(r)b^2/r^2}}
=\frac{b}{R}+O\left(\frac{b^3}{R^3}\right)
=\frac{\psi}{\sqrt{f(R)}}+O(\psi^3).
$$

Relative to flat propagation, [curvature](../../../../curvature.md) changes the small pointing angle and beam radius by the fraction $f(R)^{-1/2}-1\simeq0.00251$. At an offset of $1.35^\circ$ this is only about $0.0034^\circ$; the beam's $0.5^\circ$ radius changes by about $0.0013^\circ$. The exactly radial central ray has zero angular deflection. This is not the geometry of the usual $4GM/(bc^2)$ scattering formula, which assumes a ray coming from infinity, passing the [black hole](../../../../black-hole-split.md), and returning to infinity.

[Relativistic aberration](../../../../relativistic-aberration.md) also distinguishes a coordinate-radial light ray from a beam aimed radially in the moving crew's frame. Here $v/c=1/\sqrt{398}\simeq0.0501$. Successful initial aiming includes that fixed correction; the same correction applies at the repeated orbital position. More precisely, an outgoing static-radial ray initially has crew-frame angle $\psi'_0=-\arcsin(v/c)$ from the radial axis. The local small-angle aberration factor about that aim is $d\psi/d\psi'=\gamma=\sqrt{398/397}$; including the outgoing propagation factor gives $\gamma/\sqrt f=1/q\simeq1.00377$. Thus the asymptotic miss is about $1.358^\circ$ and the beam half-angle about $0.502^\circ$, with the same conclusion. The small distortion of the outward beam cannot correct the much larger accumulated [geodetic precession](../../../../geodetic-effect.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
