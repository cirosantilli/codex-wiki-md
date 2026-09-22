<h1 id="d7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take the membrane [particle flux](../../../../../particle-flux.md) density to be positive from [cytoplasm](../../../../../cytoplasm.md) into the [cell nucleus](../../../../../cell-nucleus.md). With [membrane permeability](../../../../../membrane-permeability.md) $\alpha$,

$$
j_m=\alpha(c_c-c_n)=\alpha\Delta c.
$$

For fixed compartment volumes, [conservation of mass](../../../../../mass-conservation.md) and the absence of exterior [flux](../../../../../flux.md) give

$$
V_n\frac{dc_n}{dt}=A_n\alpha\Delta c,\qquad
V_c\frac{dc_c}{dt}=-A_n\alpha\Delta c.
$$

Subtract the two [concentration](../../../../../concentration.md) derivatives:

$$
\frac{d\Delta c}{dt}=-\alpha A_n\left(\frac1{V_c}+\frac1{V_n}\right)\Delta c.
$$

This [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) has solution

$$
\boxed{\Delta c(t)=\Delta c(0)\exp\!\left[-\alpha A_n\left(\frac1{V_c}+\frac1{V_n}\right)t\right]}.
$$

Its relaxation time is $\boxed{T=V_cV_n/[\alpha A_n(V_c+V_n)]}$. Here $\alpha$ has dimensions length/time, so $\alpha A_n/V$ has dimensions inverse time. A positive initial [concentration](../../../../../concentration.md) difference decays monotonically toward zero; a negative one approaches zero from below.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [D7](../../d7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
