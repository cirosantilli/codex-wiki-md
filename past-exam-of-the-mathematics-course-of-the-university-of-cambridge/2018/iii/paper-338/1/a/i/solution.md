<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [gnomonic projection](../../../../../../../gnomonic-projection.md) associated with an undistorted [focal plane](../../../../../../../focal-plane.md). Write $\Delta=\alpha-A$ and rotate the celestial [Cartesian coordinate system](../../../../../../../cartesian-coordinate-system.md) so that the pointing meridian has longitude zero. The stellar direction and an [orthonormal basis](../../../../../../../orthonormal-basis.md) adapted to the [optical axis](../../../../../../../optical-axis.md) are

$$
\mathbf s=(\cos\delta\cos\Delta,\cos\delta\sin\Delta,\sin\delta),\quad
\mathbf b=(\cos D,0,\sin D),\quad
\mathbf e=(0,1,0),\quad
\mathbf n=(-\sin D,0,\cos D).
$$

Here $\mathbf e$ points east and $\mathbf n$ points north. Intersect the ray $t\mathbf s$ with the plane $\mathbf x\cdot\mathbf b=f$. It gives $t=f/(\mathbf s\cdot\mathbf b)$, so the detector coordinates are

$$
\xi=f\frac{\cos\delta\sin\Delta}{\cos\delta\cos\Delta\cos D+\sin\delta\sin D},\qquad
\eta=f\frac{\sin\delta\cos D-\cos\delta\cos\Delta\sin D}{\cos\delta\cos\Delta\cos D+\sin\delta\sin D}.
$$

These equations also avoid spurious singularities caused by writing individual tangents or cotangents.

To put this [gnomonic projection](../../../../../../../gnomonic-projection.md) in the desired form, let $\rho=(\cos^2\delta\cos^2\Delta+\sin^2\delta)^{1/2}$ and choose $q$ locally by

$$
\rho\cos q=\cos\delta\cos\Delta,\qquad \rho\sin q=\sin\delta.
$$

Thus $\cot q=\cot\delta\cos\Delta$. The denominator becomes $\rho\cos(q-D)$, the numerator for $\eta$ becomes $\rho\sin(q-D)$, and $\cos\delta\sin\Delta=\rho\cos q\tan\Delta$. Consequently

$$
\boxed{\xi=f\frac{\cos q\tan(\alpha-A)}{\cos(q-D)},\qquad \eta=f\tan(q-D).}
$$

Use the local meridian chart $\cos\Delta>0$, with $q\in[-\pi/2,\pi/2]$ chosen continuously near $D$ and $q=D$ at the image centre. A visible [gnomonic projection](../../../../../../../gnomonic-projection.md) requires $\mathbf s\cdot\mathbf b>0$, but this front-hemisphere condition alone does not select that meridian chart. A narrow field near a celestial pole can cross the opposite meridian; for such fields use the Cartesian expressions above and distinguish the oriented [great circle](../../../../../../../great-circle.md) parameter from ordinary [declination](../../../../../../../declination.md). In particular, the small-field limit is $\xi\simeq f\cos D(\alpha-A)$ and $\eta\simeq f(\delta-D)$, with angles in radians. The factor $\cos D$ is the shrinking angular distance per unit [right ascension](../../../../../../../right-ascension.md) near the pole.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
