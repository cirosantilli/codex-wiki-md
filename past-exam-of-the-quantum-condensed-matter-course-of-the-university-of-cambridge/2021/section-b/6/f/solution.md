<h1 id="section-b/6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The positive charge per unit interface area on the n side and negative charge on the p side are

$$
Q_n=\int_0^{w/2}e\alpha x\,dx=\frac{e\alpha w^2}{8},\qquad
Q_p=-Q_n.
$$

Use the signed p-side charge $Q=Q_p$ because $V_{\rm ext}$ is the p-side voltage relative to n. Differentiating the width relation gives

$$
\frac{dw}{dV_{\rm ext}}=-\frac{w}{3(V_b-V_{\rm ext})},\qquad
C=\frac{dQ_p}{dV_{\rm ext}}
=\frac{e\alpha w^2}{12(V_b-V_{\rm ext})}.
$$

Using part (e), the positive [junction capacitance](../../../../../junction-capacitance.md) per unit area is

$$
\boxed{C=\frac{\varepsilon_s}{w}
=\left[\frac{e\alpha\varepsilon_s^2}{12(V_b-V_{\rm ext})}\right]^{1/3}.}
$$

It decreases with increasing reverse-bias magnitude as $(V_b+|V_{\rm ext}|)^{-1/3}$. Equivalently,

$$
\boxed{C^{-3}=\frac{12(V_b-V_{\rm ext})}{e\alpha\varepsilon_s^2},}
$$

so a linear $C^{-3}$ versus voltage plot diagnoses this ideal linear grading and can determine $\alpha$.

For this [linearly graded junction capacitance](../../../../../linearly-graded-junction-capacitance.md), the charge convention matters: if “stored charge” means the positive magnitude $Q_n$, then $dQ_n/dV_{\rm ext}=-\varepsilon_s/w$; the positive measured capacitance is $-dQ_n/dV_{\rm ext}=dQ_n/dV_R$ for $V_R=-V_{\rm ext}$. The total net depletion charge is zero and is not the stored terminal charge. At substantial forward bias, [minority carrier](../../../../../minority-carrier.md) storage and the failure of the sharp [depletion approximation](../../../../../depletion-approximation.md) prevent extrapolation of the apparent divergence at $V_{\rm ext}=V_b$.

## ↑ Ancestors (14)

1. [F](../f.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
