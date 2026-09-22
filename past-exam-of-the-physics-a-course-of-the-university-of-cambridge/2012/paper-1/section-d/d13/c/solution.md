<h1 id="section-d/d13/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Current conservation at A, with the [capacitor](../../../../../../capacitor.md) $C_1$ connected from A to the output as verified in the PDF, gives

$$
\frac{V_{\rm in}-V_A}{R_1}
=\frac{V_A-V_B}{R_2}+sC_1(V_A-V_{\rm out}).
$$

Substitute $V_A=(1+sR_2C_2)V_B$ and $V_{\rm out}=KV_B$:

$$
\frac{V_{\rm in}}{V_B}
=1+s[C_1R_1(1-K)+C_2(R_1+R_2)]+s^2R_1R_2C_1C_2.
$$

Therefore, at $s=i\omega$,

$$
\boxed{\frac{V_{\rm out}}{V_{\rm in}}
=\frac K{1-\omega^2R_1R_2C_1C_2+i\omega[C_1R_1(1-K)+C_2(R_1+R_2)]}}.
$$

This algebraic [transfer function](../../../../../../transfer-function.md) alone does not establish that transients decay; the [pole](../../../../../../pole.md) check in the parent solution is necessary for the requested numerical choice.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D13](../../d13.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
