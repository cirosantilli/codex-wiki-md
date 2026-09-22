<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [delta-shell Born amplitude](../../../../delta-shell-born-amplitude.md) is first order in the potential strength:

$$
f_B=-gR\frac{\sin(qR)}{qR}.
$$

It retains finite-energy angular dependence and includes the leading weak-coupling contributions of all [partial waves](../../../../partial-wave.md). By contrast, the supplied $-gR/(1+g)=-a_0$ is the _zero-energy limit_ of the exact [S-wave scattering](../../../../s-wave-quantum-scattering.md) amplitude. It is isotropic, depends nonlinearly on $g$, and captures the scattering-length pole missed by first-order perturbation theory.

At finite energy the exact S-wave amplitude is instead

$$
f_0(k)=\frac{e^{2i\delta_0}-1}{2ik}
=\frac1{k\cot\delta_0-ik},
$$

which is generally complex and obeys elastic unitarity. Its zero-energy limit is $-a_0$ for finite [scattering length](../../../../scattering-length-from-a-partial-wave-s-matrix.md). Thus the two expressions printed in the question represent different approximations; the energy-independent S-wave expression is not the full finite-$k$ result of part (c).

Their common regime requires **both weak coupling and low energy**:

$$
\boxed{|g|\ll1,\qquad kR\ll1}.
$$

Then $qR\leq2kR\ll1$, so

$$
f_B=-gR\left[1-\frac{(qR)^2}{6}+O((qR)^4)\right],\qquad
-a_0=-\frac{gR}{1+g}=-gR+g^2R+O(g^3R).
$$

Consequently

$$
\boxed{f_B\sim f_0\sim-gR=-\frac{2mV_0R^2}{\hbar^2}}
$$

in that joint regime. Low energy alone does not remove the nonperturbative denominator $1+g$, while weak coupling alone does not remove higher-partial-wave angular dependence.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
