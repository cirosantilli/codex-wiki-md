<h1 id="section-b/6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the infinite system with outward drift, total [probability](../../../../../probability.md) remains one, but [probability](../../../../../probability.md) at a fixed distance from the root eventually decreases as the walker moves away. The question concerns this local decay, not a loss of total [probability](../../../../../probability.md).

The independent dimensions of the continuum coefficients are $[D]=L^2/t$ and $[C]=L/t$. The [drift-diffusion decay time](../../../../../drift-diffusion-decay-time.md) and its associated [length](../../../../../length.md) are, up to numerical factors:

$$
\ell_*\sim\frac D{|C|},\qquad
\boxed{\tau^*\sim\frac D{C^2}.}
$$

Equivalently, equating the drift distance $|C|t$ to the diffusive width of order $\sqrt{Dt}$ gives this crossover scale. Rescaling $x=(D/|C|)y$ and $t=(D/C^2)s$ removes the dimensional coefficients from the equation.

With the conventional coefficients used in the requested continuum derivation,

$$
\frac{D_0}{C^2}=\frac{\tau z^2}{2(z-2)^2},\qquad
\boxed{\tau^*\sim\tau\frac{z^2}{(z-2)^2},\quad z>2,}
$$

where the last expression suppresses the numerical factor as requested. The elementary drifted [Gaussian distribution](../../../../../normal-distribution.md) on the full line has

$$
P(x,t)=\frac1{\sqrt{4\pi Dt}}\exp\left[-\frac{(x+Ct)^2}{4Dt}\right].
$$

At fixed $x$, its exponential decay factor is $e^{-C^2t/(4D)}$, so an exponential e-folding [time](../../../../../time-in-physics.md) would conventionally be called $4D/C^2$, consistent with the same dimensional scale. The reflecting half-line changes the spatial form and algebraic prefactor. The substitution $P=e^{-Cx/(2D)}\psi$ gives $\partial_t\psi=D\partial_x^2\psi-(C^2/4D)\psi$, displaying the same exponential scale for outward drift.

For $z=2$, $C=0$ and no finite drift-induced exponential decay [time](../../../../../time-in-physics.md) exists: the [probability](../../../../../probability.md) near the root decays only algebraically. For the finite-bias, deterministic-step Gaussian envelope discussed in (b), the corresponding dimensional expression is instead $D_{\rm fixed}/C^2=2\tau(z-1)/(z-2)^2$. These continuum estimates are not exact return-probability decay rates for the lattice walk at arbitrary $z$; in particular, a [diffusion](../../../../../diffusion.md) approximation need not describe far-tail return events accurately at strong bias.

## ↑ Ancestors (14)

1. [F](../f.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
