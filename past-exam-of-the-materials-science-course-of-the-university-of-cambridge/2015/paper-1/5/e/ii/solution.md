<h1 id="5/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A physical mechanics model of wood must at least acknowledge [anisotropy](../../../../../../anisotropy.md): stiffness and creep depend on loading direction. Direction-dependent elastic elements can represent different small-strain moduli, and delayed elastic branches can approximate time-dependent [strain](../../../../../../strain.md). A linear-solid network can therefore be a local fit under specified direction, moisture and temperature, rather than a universal scalar constitutive law.

An immediate [strain](../../../../../../strain.md) followed by delayed [material creep](../../../../../../creep-deformation.md) is captured locally by a [spring](../../../../../../spring.md) plus a [Kelvin-Voigt model](../../../../../../kelvin-voigt-model.md) branch. If residual deformation remains after unloading, a [Burgers material](../../../../../../burgers-material.md) adds a free series [dashpot](../../../../../../dashpot.md) $\eta_0$. Under a constant load,

$$
\varepsilon(t)=\frac{\sigma_0}{E_0}+\frac{\sigma_0}{E_1}(1-e^{-t/\tau})+\frac{\sigma_0t}{\eta_0}.
$$

After a hold time $t_h$, the two elastic contributions recover and the dashpot retains

$$
\boxed{\varepsilon(\infty)=\frac{\sigma_0t_h}{\eta_0}}.
$$

Thus immediate recovery, delayed recovery and a residual set identify different roles for the components; an observed permanent set would rule out a purely recoverable linear-solid fit. A viscous dashpot does not itself model a yield threshold or structural damage. Strength loss, splitting, moisture-dependent response and nonlinear compression cannot be represented by one fixed linear [Kelvin-Voigt model](../../../../../../kelvin-voigt-model.md). No direction-specific measured trace is supplied, so selecting numerical parameters requires the practical data; the constitutive predictions and their limitations are the model comparison that can be made from the paper.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [5](../../../5.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the materials science course of the University of Cambridge](../../../../../split.md)
7. [Materials science course of the University of Cambridge](../../../../../../materials-science-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
