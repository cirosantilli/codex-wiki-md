# Earth-rotation aperture synthesis

↑ **Parent:** [Interferometric baseline](interferometric-baseline.md)

Earth-rotation aperture synthesis uses [Earth](earth.md)'s changing orientation to vary a fixed ground baseline's projection onto the [plane of the sky](plane-of-the-sky.md). In two dimensions, $u$ and $v$ are the components of $\mathbf b_\perp/\lambda$ along two perpendicular sky tangents. Tracking one field traces a curve in this $(u,v)$ plane; changing the physical baseline supplies other curves. A track samples [Fourier transform](fourier-transform-split.md) coordinates, rather than the brightness along a track across the sky.

For a horizontal east–west baseline of length $B$, choose the sky-axis signs so that

$$
u=\frac{B}{\lambda}\cos H,\qquad v=\frac{B}{\lambda}\sin\delta\sin H,
$$

where $H$ is [hour angle](hour-angle.md) and $\delta$ is [declination](declination.md). The ellipse follows by projecting the rotating baseline onto sky tangents. At a [celestial pole](celestial-pole.md) it is a circle; near the [celestial equator](celestial-equator.md) its minor axis collapses. Thus the same ground layout constrains different sky directions unequally. Rotation improves coverage, but does not fill every [spatial frequency](spatial-frequency.md), and synthesis across many hours assumes that the source changes negligibly during that interval.

## ↑ Ancestors (9)

1. [Interferometric baseline](interferometric-baseline.md)
2. [Radio interferometry](radio-interferometry.md)
3. [Aperture synthesis](aperture-synthesis.md)
4. [Radio astronomy](radio-astronomy.md)
5. [Observational astronomy](observational-astronomy.md)
6. [Astrophysics](astrophysics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Interferometric baseline](interferometric-baseline.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2014/paper-1/3/b/solution.md)
