# Volume of a spherical cap

↑ **Parent:** [Spherical cap](spherical-cap.md)

For a solid [spherical cap](spherical-cap.md) of height $0\leq h\leq2R$ cut from a [sphere](sphere.md) of [radius](radius.md) $R$,

$$
\boxed{V=\pi h^2\left(R-\frac h3\right).}
$$

Centre the [sphere](sphere.md) at the origin with the cap on the side $z\geq R-h$. Its cross-section at height $z$ is a [circle](circle.md) of squared [radius](radius.md) $R^2-z^2$. A [volume integral](volume-integral.md) in [cylindrical coordinates](cylindrical-coordinate-system.md) gives

$$
V=\int_{R-h}^{R}\int_0^{2\pi}\int_0^{\sqrt{R^2-z^2}}r\,dr\,d\phi\,dz=\pi\int_{R-h}^{R}(R^2-z^2)\,dz=\pi h^2(R-h/3).
$$

The formula includes caps larger than a [hemisphere](hemisphere.md), when $h>R$, and the whole solid [sphere](sphere.md), when $h=2R$. For the retained region $z\geq-d$ with $0<d<R$, set $h=R+d$ to obtain $V=\pi(2R^3/3+R^2d-d^3/3)$. Multiplying by uniform [mass density](density.md) gives its [mass](mass.md).

## ↑ Ancestors (6)

1. [Spherical cap](spherical-cap.md)
2. [Euclidean geometry](euclidean-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/12/c/solution.md)
- [Solution](past-exam-of-the-soft-condensed-matter-course-of-the-university-of-cambridge/2022/section-a/1/solution.md)
