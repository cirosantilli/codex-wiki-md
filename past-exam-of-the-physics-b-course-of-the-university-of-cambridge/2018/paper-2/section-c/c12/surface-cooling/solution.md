<h1 id="section-c/c12/surface-cooling/solution">Solution</h1>

↑ **Parent:** [Surface cooling](../surface-cooling.md)

Replacing the fixed surface [temperature](../../../../../../temperature-split.md) by [Newton's law of cooling](../../../../../../newton-s-law-of-cooling.md) changes the [boundary condition](../../../../../../boundary-condition.md) but not the radial [derivative](../../../../../../derivative.md) in steady state. At the surface,

$$
-\kappa T'(a)=\frac{Ha}{2}=\gamma\,[T(a)-T_{\rm air}].
$$

Hence

$$
\boxed{T(a)=T_{\rm air}+\frac{Ha}{2\gamma}
=T_{\rm air}+\frac{I^2}{2\pi^2\sigma\gamma a^3}.}
$$

Here $\gamma$ is a surface [heat transfer](../../../../../../heat-transfer.md) coefficient in $\mathrm{W\,m^{-2}K^{-1}}$, unrelated to the [surface tension](../../../../../../surface-tension-split.md) symbol used in C10. An independent energy-balance check uses a length $\ell$: the electrical input $I^2\ell/(\sigma\pi a^2)$ must equal the surface loss $2\pi a\ell\gamma[T(a)-T_{\rm air}]$, which gives the same answer.

The complete [temperature](../../../../../../temperature-split.md) profile is

$$
T(\rho)=T_{\rm air}+\frac{Ha}{2\gamma}+\frac{H(a^2-\rho^2)}{4\kappa}.
$$

[Thermal conductivity](../../../../../../thermal-conductivity.md) controls the internal gradient, but cancels from the surface-temperature rise because all generated [power](../../../../../../power.md) must eventually cross the prescribed surface. This assumes positive constant $\gamma$, uniform [electrical conductivity](../../../../../../electrical-conductivity.md) and negligible end or additional radiative losses; temperature-dependent material properties could make the heating and boundary problem nonlinear.

## ↑ Ancestors (15)

1. [Surface cooling](../surface-cooling.md)
2. [C12](../../c12.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
