<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At times long compared with the encounter time at depth $H$, the fixed depth $H$ is negligible relative to the growing diffusion lengths. Salt obeys the [diffusion equation](../../../../../../diffusion-equation-split.md) with diffusivity $D$. With

$$
\eta_s=\frac{z}{2\sqrt{Dt}},
\qquad
\eta_s(h)=\frac{\lambda}{\epsilon},
\qquad
\epsilon=\sqrt{\frac D\kappa},
$$

the self-similar concentration profile in the liquid is

$$
\boxed{
C(z,t)=C_0+(C_i-C_0)
\frac{\operatorname{erfc}\eta_s}
{\operatorname{erfc}(\lambda/\epsilon)}}.
$$

It has $C(h,t)=C_i$ and tends to $C_0$ in the far field.

Because the solid contains no salt, conservation of solute at the moving boundary requires the rejected solute flux from [Fick's first law](../../../../../../fick-s-first-law.md) to equal the rate at which the interface sweeps up salt:

$$
\boxed{C_i\dot h=-D C_z(h^+,t)}.
$$

Substituting the similarity profile gives

$$
\lambda C_i
=
(C_i-C_0)
\frac{\epsilon e^{-(\lambda/\epsilon)^2}}
{\sqrt{\pi}\operatorname{erfc}(\lambda/\epsilon)}.
$$

This relation determines $C_i$ if $\lambda$ is already known. More generally it must be solved together with the thermal [Stefan condition](../../../../../../stefan-condition.md) and the interfacial phase-equilibrium relation $T_i=-mC_i$ from the [liquidus](../../../../../../liquidus.md). For $\epsilon\ll1$, salt occupies a much thinner boundary layer than heat and $C_i$ can be much larger than $C_0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
