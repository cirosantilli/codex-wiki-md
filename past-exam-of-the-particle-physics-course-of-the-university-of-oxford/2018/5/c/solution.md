<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [binary strip readout](../../../../binary-strip-position-resolution.md), report the centre of the hit strip. With uniform impact position across pitch $w$, the position error is uniformly distributed on $[-w/2,w/2]$, so

$$
\sigma_x^2=\frac1w\int_{-w/2}^{w/2}x^2dx=\frac{w^2}{12},\qquad
\boxed{\sigma_x=\frac{100\,\mu\mathrm m}{\sqrt{12}}=28.87\,\mu\mathrm m.}
$$

This assumes no analogue charge sharing between strips.

The [magnetic force](../../../../lorentz-force.md) is $d\mathbf p/dt=q\mathbf v\times\mathbf B$. Since relativistic [momentum](../../../../momentum-split.md) is parallel to [velocity](../../../../velocity.md), $d(p^2)/dt=2\mathbf p\cdot q(\mathbf v\times\mathbf B)=0$. A uniform transverse field therefore changes [momentum](../../../../momentum-split.md) direction but not magnitude. If the trajectory turns at angular [speed](../../../../speed.md) $v/R$, then $|d\mathbf p/dt|=p_Tv/R$. Equating force magnitudes yields

$$
\boxed{R=\frac{p_T}{|q|B}.}
$$

This is the positive [radius](../../../../radius.md). The sign of $q$ determines the direction of [curvature](../../../../curvature.md); the source's signed formula can describe an oriented [radius](../../../../radius.md). In practical tracking units,

$$
p_T[\mathrm{GeV}/c]=0.299792458\,|q/e|B[\mathrm T]R[\mathrm m].
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
