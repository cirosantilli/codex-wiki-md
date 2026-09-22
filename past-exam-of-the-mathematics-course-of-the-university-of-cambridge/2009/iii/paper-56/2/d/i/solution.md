<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the superextreme [Kerr metric](../../../../../../../kerr-metric.md),

$$
\Delta=(r-M)^2+a^2-M^2>0
$$

for all real $r$, so there are no coordinate singularities at horizon roots. The only stipulated [curvature singularity](../../../../../../../curvature-singularity.md) is $\Sigma=0$, which forces $r=0$, $\theta=\pi/2$. In the supplied Cartesian coordinates this is the [Kerr ring singularity](../../../../../../../kerr-ring-singularity.md) $x^2+y^2=a^2$, $z=0$.

Write $\rho^2=x^2+y^2$. The coordinate transformation implies

$$
\rho^2=(r^2+a^2)\sin^2\theta,\qquad z=r\cos\theta,
$$

and hence

$$
r^4-(\rho^2+z^2-a^2)r^2-a^2z^2=0.
$$

The positive-radius Cartesian sheet uses

$$
r^2=\frac12\left[\rho^2+z^2-a^2+
\sqrt{(\rho^2+z^2-a^2)^2+4a^2z^2}\right],\qquad r\geq0.
$$

Its zero set is the disk $z=0$, $\rho\leq a$. At an interior disk point, $\rho<a$, one has $\cos\theta\ne0$, so $\Sigma=a^2\cos^2\theta>0$. The disk interior is therefore not a singularity: in signed $(r,\theta,\phi)$ coordinates, the metric is analytic through $r=0$. In particular, $g_{rr}=\Sigma/\Delta$ is finite and the metric determinant $-\Sigma^2\sin^2\theta$ is nonzero away from the ordinary polar coordinate axis. The polar axes are regular using Cartesian angular charts and $2\pi$ periodicity.

The required [two-sheeted extension of superextremal Kerr spacetime](../../../../../../../two-sheeted-extension-of-superextremal-kerr-spacetime.md) is constructed by taking a second Cartesian sheet with the negative root $r\leq0$, cutting both sheets along the disk, and gluing the upper bank of one to the lower bank of the other, and conversely. Signed $r$ then passes continuously through zero as the disk is crossed. The ring is omitted. A useful check near an interior disk point is

$$
z=r\cos\theta,\qquad \cos^2\theta\big|_{r=0}=1-\rho^2/a^2>0,
$$

so signed $r$ is a smooth transverse coordinate there. The apparent factors $z/r$ in the Cartesian metric represent $\cos\theta$ and have regular signed-coordinate limits; they do not justify deleting the whole disk. Identifying the two signs of $r$ on a single Cartesian copy would also identify two physically different metric values, since the Kerr-Schild coefficient changes sign.

Continue the two sheets out to $r\to\pm\infty$. Both ends are asymptotically flat; at the negative-radius end the mass term has the opposite sign, as $g_{tt}=-1+2M/r+O(r^{-2})$. There are no further finite-radius horizon boundaries requiring additional blocks. Removing only the curvature-singular ring, and removing coordinate artifacts with the charts described above, gives the standard maximal analytic extension. The ring cannot be filled by an analytic nondegenerate metric because its curvature diverges. This extension is not globally hyperbolic; analyticity of an extension should not be confused with unique evolution from Cauchy data.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Paper 56](../../../../paper-56-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
