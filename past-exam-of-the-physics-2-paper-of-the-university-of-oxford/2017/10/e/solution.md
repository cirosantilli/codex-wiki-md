<h1 id="10/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

At [focal length](../../../../focal-length.md) $f=80\,\mathrm m$, the stroke maps to a focal-plane width $w_i=fs/H=12\,\mathrm{\mu m}$. A practical estimate with two detector samples across that stroke is

$$
\boxed{p\lesssim\frac{fs}{2H}=6.0\,\mathrm{\mu m},\qquad
N\gtrsim\frac{f(500\,\mathrm m)/H}{p}\simeq3.33\times10^4\ \text{pixels across}.}
$$

The required sensor extent in that direction is $f(500\,\mathrm m)/H=0.20\,\mathrm m$. One $12\,\mathrm{\mu m}$ pixel per stroke would give about $1.67\times10^4$ pixels across, but cannot reliably encode a stroke's position and contrast as the image moves relative to the pixel grid.

For a precise interpretation of “fully resolve” as sampling the entire diffraction-limited incoherent image, use the optical intensity-transfer cutoff $\nu_c=D/(\lambda f)$. The [Nyquist–Shannon sampling theorem](../../../../nyquist-shannon-sampling-theorem.md) requires $1/(2p)\ge\nu_c$. With the circular mirror chosen in 10d,

$$
\boxed{p\le\frac{\lambda f}{2D}=\frac{fs}{2(1.22)H}=4.92\,\mathrm{\mu m},\qquad
N\ge4.07\times10^4.}
$$

This stricter value retains the full circular-aperture spatial [bandwidth](../../../../bandwidth-signal-processing.md); the $6\,\mathrm{\mu m}$ and $3.3\times10^4$ estimates use two samples per specified feature instead. An engineering design would provide further sampling and contrast margin. The distinction states the sampling convention rather than treating the order-of-magnitude estimates as contradictory.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [10](../../10.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
