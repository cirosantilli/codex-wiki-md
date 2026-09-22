<h1 id="5/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $t>0$, close the inverse-transform [contour](../../../../../../complex-integration-contour.md) in the upper half-plane. There $|e^{i\omega t}|\leq1$; the rational factor is $O(|\omega|^{-2})$, so the arc integral vanishes. For $\Omega>\kappa$, write $\beta=\sqrt{\Omega^2-\kappa^2}>0$. The two [simple poles](../../../../../../simple-pole.md) are $i\kappa\pm\beta$, and the [residue theorem](../../../../../../residue-theorem.md) yields

$$
\begin{aligned}
G(t)&=-i\left[\frac{e^{i\omega_+t}}{\omega_+-\omega_-}
+\frac{e^{i\omega_-t}}{\omega_--\omega_+}\right]\\
&=-i e^{-\kappa t}\frac{e^{i\beta t}-e^{-i\beta t}}{2\beta}
=\boxed{e^{-\kappa t}\frac{\sin(\beta t)}\beta}.
\end{aligned}
$$

This [causal Green function of a damped oscillator](../../../../../../causal-green-function-of-a-damped-oscillator.md) has damped oscillations with envelope $e^{-\kappa t}$ and tends to zero as $t\to\infty$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
