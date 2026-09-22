<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [Schwarzschild metric](../../../../../../../schwarzschild-spacetime.md) in [Ingoing Eddington-Finkelstein coordinates](../../../../../../../ingoing-eddington-finkelstein-coordinates.md) as $ds^2=-f\,dv^2+2dv\,dr+r^2d\Omega^2$, with $f=1-2M/r$. Ingoing radial [null geodesics](../../../../../../../null-geodesic.md) have $v,\theta,\phi$ constant. Since $\Gamma^a{}_{rr}=0$, choose their future affine tangent $U=-E\partial_r$, where $E>0$ is constant along a ray; a common normalization sets $E=1$. The [parallel null partner for ingoing Schwarzschild rays](../../../../../../../parallel-null-partner-for-ingoing-schwarzschild-rays.md) is

$$
\boxed{N=\frac1E\left(\partial_v+\frac f2\partial_r\right).}
$$

The radial conditions give $U\cdot N=-EN^v=-1$ and $N^2=-f/E^2+2(E^{-1})(f/(2E))=0$. Parallel transport can be checked explicitly: $\Gamma^v{}_{rv}=0$ and $\Gamma^r{}_{rv}=-f'/2$, so

$$
\nabla_rN^v=0,\qquad
\nabla_rN^r=\frac{f'}{2E}-\frac{f'}2\frac1E=0,
$$

with angular components also zero. Thus $\nabla_UN=0$. The field is regular at $r=2M$ and throughout the regular advanced chart $r>0$; no vector field can be defined at the curvature-singular endpoint. If the affine normalization differs between rays, the same formula works for $E$ constant along each ray, since $\partial_rE=0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Paper 56](../../../../paper-56-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
