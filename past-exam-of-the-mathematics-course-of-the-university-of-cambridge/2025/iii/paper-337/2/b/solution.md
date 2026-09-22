<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The tree-level Cooper-pair scattering amplitude is simply $V$. Define the density of states at the Fermi surface, in the normalization of the question, by

$$
\nu_F=\int_{\rm FS}\frac{d^2k}{(2\pi)^3|v_F(k)|}.
$$

In the one-loop Cooper diagram the two internal fermions have opposite momenta. After integrating over internal frequency, the remaining normal-energy integral contains

$$
\int_{|\omega|}^{\Lambda}\frac{d\xi}{\xi}
=\log\frac{\Lambda}{|\omega|}.
$$

Consequently

$$
\Gamma(\omega)=V-\nu_FV^2\log\frac{\Lambda}{|\omega|}+O(V^3\log^2),
$$

and summing the leading geometric series gives the running [BCS theory](../../../../../../bcs-theory.md) coupling

$$
\boxed{
V_R(\omega)=\frac{V}
{1+\nu_FV\log(\Lambda/|\omega|)}.}
$$

For repulsive $V>0$ it flows logarithmically toward zero. For attractive $V<0$, its denominator vanishes at the [Cooper instability](../../../../../../cooper-instability.md) scale

$$
\boxed{|\omega_*|=\Lambda
\exp\left[-\frac1{\nu_F|V|}\right].}
$$

At this scale the normal Fermi liquid becomes unstable: opposite-momentum fermions form Cooper pairs, a superconducting or superfluid condensate develops, and a gap opens.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
