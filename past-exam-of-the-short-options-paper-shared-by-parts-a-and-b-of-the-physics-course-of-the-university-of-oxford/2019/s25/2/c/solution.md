<h1 id="s25/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A linearly increasing [radiative forcing](../../../../../radiative-forcing.md) produces a fast adjustment over about four years superposed on a slow deep-ocean response over about four hundred years. Once forcing stops increasing at year 70, surface warming continues and approaches the final $3\,\mathrm K$ equilibrium. The right panel of [solution](../../../s10/2/c/solution.md) gives a model response normalized to the supplied $2\,\mathrm K$ endpoint and $3\,\mathrm K$ equilibrium.

Write $u=t-70$ after stabilization and $3-T_s=A_f e^{-u/4}+A_s e^{-u/400}$, with $A_f+A_s=1\,\mathrm K$. For a 70-year forcing ramp, the normalized step response is $1-b_f e^{-t/4}-b_s e^{-t/400}$, $b_f+b_s=1$. The ramp endpoint implies

$$
1=3\left[b_f\frac4{70}(1-e^{-70/4})+b_s\frac{400}{70}(1-e^{-70/400})\right].
$$

This gives $b_s\simeq0.322$, $A_f\simeq0.116\,\mathrm K$ and $A_s\simeq0.884\,\mathrm K$. Thus

$$
\dot T_s=\frac{A_f}{4}e^{-u/4}+\frac{A_s}{400}e^{-u/400}\simeq0.0045,\ 0.0028,\ 0.0023\,\mathrm{K\,yr^{-1}}
$$

at $u=10,15,20$ years respectively. The usual order estimate after the fast tail has largely disappeared is $\boxed{\dot T_s\sim(3-2)/400\simeq0.0025\,\mathrm{K\,yr^{-1}}}$, with a still visible fast contribution near year 10.

To hold $T_s=T_*$ fixed, the deep layer obeys $T_s-T_d\propto e^{-\gamma u/C_d}$ and the surface equation requires $F=\lambda T_*+\gamma(T_*-T_d)$. Hence $\dot F=-\gamma^2(T_*-T_d)/C_d$. Using $b_f\simeq\lambda/(\lambda+\gamma)$ gives $\gamma/\lambda\simeq0.475$ and $\gamma/C_d\simeq1/(400b_f)\simeq0.00369\,\mathrm{yr^{-1}}$. With $T_*=2\,\mathrm K$ and initial forcing $F_0=3\lambda$, the initial fractional decline is

$$
\boxed{-\frac{\dot F}{F_0}\simeq\frac{\gamma/C_d}{3}\simeq0.00123\,\mathrm{yr^{-1}}\simeq0.12\%\text{ per year}.}
$$

The rate declines slowly as the ocean contrast disappears. A coarser estimate treating the post-fast warming as an effective equilibrium change gives $0.0025/3\simeq0.08\%$ per year; distinguishing the instantaneous surface feedback from the equilibrium feedback explains that difference.

**Wording qualification:** the printed text says a “1% increase … over 70 years”. The conventional [transient climate response](../../../../../transient-climate-response.md) experiment uses $1\%$ _per year_, which nearly doubles concentration in 70 years. A literal total $1\%$ increase would not define the usual [equilibrium climate sensitivity](../../../../../equilibrium-climate-sensitivity.md) or [transient climate response](../../../../../transient-climate-response.md). The supplied $3\,\mathrm K$ and $2\,\mathrm K$ are used here as the endpoint normalizations, and a logarithmically uniform concentration growth gives the assumed linear forcing ramp.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [S25](../../../s25.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
