<h1 id="section-c/c11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [free parallel RLC voltage decay](../../../../../../free-parallel-rlc-voltage-decay.md), measure $V=V_A-V_B$ and branch currents from A to B. Then

$$
I_C=C\dot V,\qquad I_R=V/R,\qquad
I_L(t)=I_L(0)+\frac1L\int_0^tV(s)\,ds.
$$

There is no external current, so [Kirchhoff's current law](../../../../../../kirchhoff-node-law.md) gives $I_C+I_R+I_L=0$. Differentiating yields

$$
\boxed{C\ddot V+\frac1R\dot V+\frac1LV=0.}
$$

For $V\propto e^{st}$ the [characteristic equation](../../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $Cs^2+s/R+1/L=0$. Its [underdamped](../../../../../../underdamping.md) roots give

$$
\boxed{\gamma=\frac1{2RC},\qquad
\omega=\sqrt{\frac1{LC}-\frac1{4R^2C^2}}.}
$$

The supplied inequality makes $\omega$ real. A real physical [voltage](../../../../../../voltage.md) has the general form $V=Ae^{-\gamma t}\cos(\omega t+\phi)$, the [real part](../../../../../../real-part.md) of the printed complex expression. A general complex-valued solution uses both roots, $e^{-\gamma t}(C_+e^{i\omega t}+C_-e^{-i\omega t})$. The [inductor](../../../../../../inductor.md)'s initial current is fixed consistently by the undifferentiated current balance; it is not an arbitrary additional voltage-mode constant.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [C11](../../c11.md)
3. [Section C](../../../section-c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2012](../../../../split.md)
6. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
