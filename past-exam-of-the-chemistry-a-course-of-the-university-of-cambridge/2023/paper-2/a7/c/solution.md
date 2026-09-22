<h1 id="a7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The definition uses a fixed reference volume, so it is a [reference-volume thermal expansion coefficient](../../../../../reference-volume-thermal-expansion-coefficient.md):

$$
\alpha=\frac{d}{dT}\frac{V(T)}{V_0}=\frac{dP_1}{dT}.
$$

Let $y=3e^{-\varepsilon/(k_BT)}$. Since

$$
\frac{dy}{dT}=\frac{\varepsilon}{k_BT^2}y,
\qquad \frac{d}{dy}\frac{y}{1+y}=\frac1{(1+y)^2},
$$

we obtain

$$
\boxed{\alpha(T)=\frac{\varepsilon}{k_BT^2}
\frac{3e^{-\varepsilon/(k_BT)}}{\left(1+3e^{-\varepsilon/(k_BT)}\right)^2}}.
$$

It is positive and has units of inverse temperature. Equivalently, $\alpha=[\varepsilon/(k_BT^2)]P_1(1-P_1)$: the response reflects changes in the thermally occupied excited population. The usual instantaneous fractional [thermal expansion coefficient](../../../../../coefficient-of-thermal-expansion.md) $V^{-1}dV/dT$ would instead equal $\alpha V_0/V$; substituting that different definition would change the answer.

<a id="a7/c/image-degeneracy-limits-the-high-temperature-volume-of-the-two-level-model"></a>
![](../../../../../past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2023/paper-2-two-level-expansion.png)

**[Figure 1](#a7/c/image-degeneracy-limits-the-high-temperature-volume-of-the-two-level-model). Degeneracy limits the high-temperature volume of the two-level model**. Original dimensionless calculation with $t=k_BT/\varepsilon$. The plotted expansion response is $(\varepsilon/k_B)\alpha$. The high-temperature volume approaches $7V_0/4$, with vanishing response at both temperature extremes.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [A7](../../a7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
