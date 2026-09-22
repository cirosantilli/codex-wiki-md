<h1 id="section-b/5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Each addition starts a new statistically identical waiting episode at zero gap. Thus the addition rate is the reciprocal of a [mean first-passage time](../../../../../mean-first-passage-time.md), not the reciprocal of the mean gap:

$$
\boxed{\tau=\frac1{j_0}=\frac{e^{\beta F\delta}-\beta F\delta-1}{D\beta^2F^2}.}
$$

This can also be derived without the steady density. If $T(x)$ is the mean time to reach $\delta$ starting at gap $x$, its backward [Smoluchowski equation](../../../../../smoluchowski-equation.md) is

$$
DT''-D\beta FT'=-1,\qquad T'(0)=0,\qquad T(\delta)=0.
$$

The first boundary is reflecting and the second absorbing. An [integrating factor](../../../../../integrating-factor.md) gives $T'(x)=[1-e^{\beta Fx}]/(D\beta F)$, whence

$$
T(0)=-\int_0^\delta T'(x)\,dx
=\frac{e^{\beta F\delta}-1-\beta F\delta}{D\beta^2F^2}=\tau.
$$

At weak [force](../../../../../force-split.md), $\tau\simeq\delta^2/(2D)$ is the time for a freely diffusing wall to move a [monomer](../../../../../monomer.md) length, with reflection at the tip. At strong [force](../../../../../force-split.md), opening the gap requires [work](../../../../../work.md) $F\delta$, with [Boltzmann distribution](../../../../../boltzmann-distribution.md) suppression $e^{-\beta F\delta}$. The drift establishes a near-tip thermal length $\ell_F=k_BT/F$ and a [diffusion](../../../../../diffusion.md) time $\ell_F^2/D$; consequently

$$
\tau\sim\frac{\ell_F^2}{D}e^{\delta/\ell_F}.
$$

The exponentially long wait explains why the growth slows. There is no additional chemical waiting time in the imposed absorbing-threshold model; such a time would be needed to describe the separate [reaction-limited polymerization Brownian ratchet](../../../../../reaction-limited-polymerization-brownian-ratchet.md) regime.

## ↑ Ancestors (14)

1. [F](../f.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
