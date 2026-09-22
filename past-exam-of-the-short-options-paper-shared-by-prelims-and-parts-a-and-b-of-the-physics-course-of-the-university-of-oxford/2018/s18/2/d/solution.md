<h1 id="s18/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $E<0$, inversion of the free operator gives $G_0(x,y)=m e^{-\kappa|x-y|}/(\kappa\hbar^2)$, with $\kappa=\sqrt{-2mE}/\hbar$. The bound-state equation is $\psi=-G_0U\psi$, hence

$$
\psi(x)=-\frac m{\kappa\hbar^2}\int\!\int e^{-\kappa|x-y|}V(y,z)\psi(z)\,dy\,dz.
$$

For the separable kernel $V(y,z)=-\alpha F(y)F^*(z)$, define

$$
\boxed{C=\int_{-\infty}^{\infty}F^*(z)\psi(z)\,dz.}
$$

Then

$$
\boxed{\psi(x)=\frac{\alpha mC}{\kappa\hbar^2}\int e^{-\kappa|x-y|}F(y)\,dy.}
$$

An overall [normalization](../../../../../normalization.md) still has to be chosen after finding a permitted [energy](../../../../../energy-split.md). A nontrivial [bound state](../../../../../bound-state.md) must have $C\ne0$: if $C=0$, the potential acts as zero and a square-integrable negative-energy free solution on the whole line cannot exist. Decay or square-integrability assumptions on $F$ are needed to make these [integrals](../../../../../integral-split.md) well defined; smoothness alone would not ensure convergence.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [S18](../../../s18.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
