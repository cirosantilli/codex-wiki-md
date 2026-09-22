<h1 id="section-a/a2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Distinguish reflection at the input terminal, reflection at the receiving load, and a returned signal that traverses the free-space link twice. The input [antenna](../../../../../antenna-radio.md) is initially matched, so its direct terminal reflection is zero.

In the usual weak-coupling, matched-port [two-port network](../../../../../two-port-network.md) model for the [antenna](../../../../../antenna-radio.md) pair, let the forward and reverse [wave amplitude](../../../../../wave-amplitude.md) transfer coefficients be $t_{21}$ and $t_{12}$. [Electromagnetic reciprocity](../../../../../reciprocity-electromagnetism.md) gives equal [power](../../../../../power.md) transfer factors $|t_{21}|^2=|t_{12}|^2=\mathcal F$, where $\mathcal F=(G_a\lambda/(4\pi d))^2$ from part (a). The receiving-load reflection returns [wave amplitude](../../../../../wave-amplitude.md) $t_{12}\Gamma_Lt_{21}$ to the original input port. The load-mismatch contribution to the returned [power](../../../../../power.md) is therefore

$$
\boxed{P_r^{\rm load}=P_i|\Gamma_L|^2\mathcal F^2
=P_i\left(\frac{Z_t-Z_i}{Z_t+Z_i}\right)^2
\left(\frac{G_a\lambda}{4\pi d}\right)^4.}
$$

For fixed gains and impedances this returned [power](../../../../../power.md) scales as $\lambda^4$: it contains two link traversals. By contrast, the reflected [power](../../../../../power.md) at the receiving load before that return traversal is $P_i\mathcal F|\Gamma_L|^2\propto\lambda^2$. Calling that local reflected [power](../../../../../power.md) the [power](../../../../../power.md) already back in the input line would omit one propagation loss.

The original wording does not specify an antenna scattering model. The boxed result is the load-dependent echo in an ideal matched-port link, with structural scattering and residual input coupling neglected. The actual total input return can include coherent scattering from the receiving antenna even when $\Gamma_L=0$; gains and effective areas alone do not specify that background. If “reflected back” means only the direct reflection at the stated matched transmitting antenna, its value is $0$. These meanings should not be conflated; the $\lambda^4$ result requires the two-pass echo interpretation and its stated model.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [A2](../../a2.md)
3. [Section A](../../../section-a.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
