<h1 id="36d/solution">Solution</h1>

↑ **Parent:** [36D](../36d.md)

Put $f(r)=1-2M/r$. An incoming radial null ray has $dt/dr=-1/f$. The [tortoise coordinate](../../../../../tortoise-coordinate.md) $r_*=r+2M\log|r/(2M)-1|$ obeys $dr_*/dr=1/f$, so $v=t+r_*$ is constant along such a ray. For $r>2M$ this is exactly the printed logarithm. Substituting $dt=dv-dr/f$ gives the metric in [Ingoing Eddington-Finkelstein coordinates](../../../../../ingoing-eddington-finkelstein-coordinates.md)

$$
\boxed{ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega^2.}
$$

The radial null directions satisfy either $dv=0$ or $dr/dv=f/2$. Future-directed ingoing rays have decreasing $r$ on the first family. Outgoing rays increase $r$ outside the horizon, stay at $r=2M$ on its generators, and decrease $r$ inside. Thus inside the horizon every future timelike trajectory also moves toward smaller $r$.

The $(v,r)$ metric block has [determinant](../../../../../determinant.md) minus one and is nonsingular at $r=2M$. The horizon is a null surface, not a [curvature singularity](../../../../../curvature-singularity.md). For example the [Kretschmann scalar](../../../../../kretschmann-scalar.md) $48M^2/r^6$ is finite there and diverges at $r=0$.

Inside, set $A=2M/r-1>0$. For radial timelike motion, the Schwarzschild expression becomes $d\tau^2=A^{-1}dr^2-A\,dt^2$, hence

$$
\boxed{d\tau\le\sqrt{\frac r{2M-r}}\,|dr|.}
$$

Angular motion would only reduce the available [proper time](../../../../../proper-time.md) further. Integrating from the horizon to zero, with $r=2M\sin^2\theta$, gives

$$
\boxed{\Delta\tau\le\int_0^{2M}\sqrt{\frac r{2M-r}}\,dr=4M\int_0^{\pi/2}\sin^2\theta\,d\theta=\pi M.}
$$

The bound is sharp for the zero-energy radial [geodesic](../../../../../geodesic.md) with constant Schwarzschild $t$ in the interior. For a [geodesic](../../../../../geodesic.md) arriving from the exterior with strictly positive conserved energy, the [proper time](../../../../../proper-time.md) is strictly smaller; $\pi M$ is the supremum as that energy tends to zero. Thus the universally available horizon-to-singularity upper bound is $\pi M$, rather than a time attainable by every exterior infaller. Restoring units gives $\pi GM/c^3$.

## ↑ Ancestors (10)

1. [36D](../36d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
