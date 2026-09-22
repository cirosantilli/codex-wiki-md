<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [magnetization](../../../../../magnetization.md) correlator is an average of a [phase difference](../../../../../phase-difference.md), not merely its lowest Taylor expansion. [Gaussian phase averaging](../../../../../gaussian-phase-averaging.md) gives

$$
C_m(r)=\bar m^2\langle\cos[\theta(\mathbf x)-\theta(0)]\rangle
=\bar m^2\exp\!\left[-\frac12D(r)\right],
$$

where

$$
D(r)=\langle[\theta(\mathbf x)-\theta(0)]^2\rangle
=\frac2{\bar K}\int\frac{d^dq}{(2\pi)^d}\frac{1-\cos(\mathbf q\cdot\mathbf x)}{q^2}
=2[G(0)-G(r)].
$$

The coincident value is ultraviolet-regularized at a microscopic scale $a$. At large $r$:

- For $d>2$, the infrared integral for $G(0)$ converges. Choosing $G(\infty)=0$, $D(\infty)=2G(0)<\infty$, so **$C_m(\infty)=m_0^2=\bar m^2e^{-G(0)}>0$** within the low-temperature [spin wave](../../../../../spin-wave.md) [thermodynamic phase](../../../../../thermodynamic-phase.md).
- For $d=2$, $D(r)=(\pi\bar K)^{-1}\log(r/a)+O(1)$, hence **$C_m(r)\propto r^{-1/(2\pi\bar K)}\to0$**.
- For $0<d<2$, the leading growth is $D(r)=2r^{2-d}/[(2-d)S_d\bar K]+O(1)$, hence **$C_m(r)\propto\exp\{-r^{2-d}/[(2-d)S_d\bar K]\}\to0$**. In particular $d=1$, $S_1=2$, gives $C_m(r)\propto e^{-r/(2\bar K)}$.

<a id="2/b/image-infrared-spin-wave-correlation-limits"></a>
![](../../../../../past-exam-of-the-phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge/2012/paper-1-ptcp2012-correlations.png)

**[Figure 1](#2/b/image-infrared-spin-wave-correlation-limits). Infrared spin-wave correlation limits**. Original regulated phase-only model curves for dimensions one, two and three. They illustrate exponential decay, algebraic decay and a nonzero limit respectively; no experimental dataset or phase-transition temperature is fitted.

Thus **two is the [lower critical dimension](../../../../../lower-critical-dimension.md) for conventional positive-temperature continuous-symmetry order** under the short-range assumptions. Two dimensions can still have [quasi-long-range order](../../../../../quasi-long-range-order.md) and a thermodynamic transition; zero limiting [magnetization](../../../../../magnetization.md) does not forbid them. The $d>2$ [spin wave](../../../../../spin-wave.md) result describes an admissible low-temperature ordered [thermodynamic phase](../../../../../thermodynamic-phase.md), not order at arbitrarily high [temperature](../../../../../temperature-split.md). The [Mermin-Wagner theorem](../../../../../mermin-wagner-theorem.md) supplies the more general no-order statement below or at two dimensions.[§4.2.3: infrared phase fluctuations and continuous-symmetry order](../../../../../statistical-field-theory-by-david-tong.md)

## ↑ Ancestors (14)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the phase transitions and collective phenomena course of the University of Cambridge](../../../../split.md)
6. [Phase Transitions and Collective Phenomena course of the University of Cambridge](../../../../../phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
