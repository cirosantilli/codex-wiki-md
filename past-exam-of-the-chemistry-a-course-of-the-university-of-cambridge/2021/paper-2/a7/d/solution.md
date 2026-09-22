<h1 id="a7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $\theta_{\rm rot}=\hbar^2/(2Ik_{\rm B})$. Summing the spatial states counted in part (c),

$$
q_{\rm planar}^{\rm labelled}=\sum_{m=-\infty}^{\infty}e^{-m^2\theta_{\rm rot}/T}
=1+2\sum_{J=1}^{\infty}e^{-J^2\theta_{\rm rot}/T}.
$$

When $T\gg\theta_{\rm rot}$ the closely spaced terms can be replaced by a [Gaussian integral](../../../../../gaussian-integral.md):

$$
\boxed{q_{\rm planar}^{\rm labelled}\simeq\int_{-\infty}^{\infty}
e^{-m^2\theta_{\rm rot}/T}\,dm
=\sqrt{\frac{\pi T}{\theta_{\rm rot}}}
=\frac{\sqrt{8\pi^3Ik_{\rm B}T}}h.}
$$

Here labelled means that the two ends of the molecular axis were distinguished in the angular count. In the usual high-temperature molecular convention that removes equivalent orientations and factors out nuclear-spin multiplicity, divide by the [rotational symmetry number](../../../../../rotational-symmetry-number.md) $s=2$ for homonuclear [hydrogen](../../../../../hydrogen.md):

$$
\boxed{q_{\rm rot}^{\rm planar}\simeq\frac1s\sqrt{\frac{\pi T}{\theta_{\rm rot}}},\qquad s=2.}
$$

The full exact [spin isomers of hydrogen](../../../../../spin-isomers-of-hydrogen.md) count is instead the even-$m$ spatial sum plus three times the odd-$m$ sum; its high-temperature limit is $2\sqrt{\pi T/\theta_{\rm rot}}$, including the four nuclear-spin states. These conventions differ only by temperature-independent factors in this limit. All give $U_{\rm rot,m}=RT/2$ and $C_{V,m}^{\rm rot}=R/2$, consistent with one quadratic rotational degree of freedom. By comparison, the free [linear rigid rotor](../../../../../linear-rigid-rotor.md) has $q_{\rm rot}\propto T$ and $C_{V,m}^{\rm rot}=R$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [A7](../../a7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
