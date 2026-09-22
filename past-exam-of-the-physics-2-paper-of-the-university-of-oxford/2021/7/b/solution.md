<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Rayleigh criterion](../../../../rayleigh-criterion.md) gives a separation in the sensor plane $\delta=f\Delta\theta=2.44\,\mu\mathrm m$, using the $5\,\mathrm{mm}$ image distance. Counting one square [pixel](../../../../pixel.md) per such [spatial resolution element](../../../../spatial-resolution-element.md) gives

$$
\boxed{N_{\rm Rayleigh}\simeq\frac{(4\,\mathrm{mm})(3\,\mathrm{mm})}{(2.44\,\mu\mathrm m)^2}=2.02\times10^6.}
$$

This is an estimate of the number of optically distinguishable elements. To sample all the spatial information, specify a [signal sampling](../../../../signal-sampling.md) criterion as well. For [incoherent imaging](../../../../incoherent-imaging.md) through an ideal circular [aperture](../../../../aperture.md), the [optical transfer function](../../../../optical-transfer-function.md) has cutoff spatial frequency $\nu_c=D/(\lambda f)$. The [Nyquist–Shannon sampling theorem](../../../../nyquist-shannon-sampling-theorem.md) requires a [pixel](../../../../pixel.md) pitch

$$
p\leq\frac1{2\nu_c}=\frac{\lambda f}{2D}=1.00\,\mu\mathrm m,
\qquad \boxed{N_{\rm Nyquist}\geq4000\times3000=1.20\times10^7.}
$$

A common intermediate rule, two [pixels](../../../../pixel.md) per Rayleigh separation, gives about $8.1$ million [pixels](../../../../pixel.md); it is a heuristic and does not quite sample the full ideal [optical transfer function](../../../../optical-transfer-function.md) bandwidth. Thus about $2$ million is the elementary [spatial resolution element](../../../../spatial-resolution-element.md) count, while $12$ million is the ideal monochrome [Nyquist–Shannon sampling theorem](../../../../nyquist-shannon-sampling-theorem.md) answer to “full use.” Color-filter layout and finite [pixel](../../../../pixel.md) area would impose further practical conditions.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
