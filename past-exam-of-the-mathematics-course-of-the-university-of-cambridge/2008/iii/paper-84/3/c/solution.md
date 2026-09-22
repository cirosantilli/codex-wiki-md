<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret absorption as irreversible capture of radioactive tracer by the formation at the stated first-order rate. With stored amount $S$ measured per the same reference pore-storage volume as $C$, [irreversible capture of an advecting tracer](../../../../../../irreversible-capture-of-an-advecting-tracer.md) gives

$$
\boxed{C_t+UC_x=D_{\rm eff}C_{xx}-\lambda C,
\qquad S_t=\lambda C.}
$$

Adding the equations conserves dissolved plus captured tracer, apart from advective and diffusive transport. A different solid-volume normalization inserts the corresponding porosity factor in $S_t$. The averaged equation has the same transverse-equilibration limitation as in part (a).

For a maintained inlet concentration $C(0,t)=C_0$, a bounded downstream stationary water profile satisfies $D_{\rm eff}C''-UC'-\lambda C=0$. Its characteristic roots are $(U\pm\Delta)/(2D_{\rm eff})$, where $\Delta=\sqrt{U^2+4\lambda D_{\rm eff}}$. Rejecting the growing root gives

$$
\boxed{C_\infty(x)=C_0 e^{-rx},
\qquad r=\frac{\Delta-U}{2D_{\rm eff}}>0.}
$$

If the inlet instead prescribes solute flux $J_0=UC-D_{\rm eff}C_x$, replace $C_0$ by $J_0/(U+D_{\rm eff}r)$. In the advection-dominated limit, $r\simeq\lambda/U$, giving an attenuation length $U/\lambda$.

The corresponding capture-rate profile is $\lambda C_\infty(x)$. There is an important qualification to the requested adsorbed profile: with a continuous source, irreversible adsorption and no solid decay or saturation, **the water concentration can be stationary but the accumulated solid concentration cannot**. At every point with positive $C_\infty$,

$$
S(x,t)=\lambda\int_0^t C(x,s)\,ds,
\qquad S(x,t)/t\longrightarrow\lambda C_0e^{-rx}.
$$

Thus the deposited amount grows asymptotically linearly with a spatially exponential rate profile. A time-independent deposit would require additional desorption, finite capacity or radioactive decay in the solid; for example $S_t=\lambda C-\gamma_sS$ would give $S_\infty=\lambda C_\infty/\gamma_s$ if $\gamma_s>0$.

If the source is the localized release in part (b), there is instead a finite final deposit and no nonzero steady water concentration. On the full line, multiply the moving Gaussian by $e^{-\lambda t}$. Integrating its governing equation over all time gives $D_{\rm eff}J''-UJ'-\lambda J=-\mathcal M\delta(x-x_0)$ for $J=\int_0^\infty C\,dt$. Continuity and the derivative jump at $x_0$ then give

$$
\boxed{S_\infty(x)=\frac{\lambda\mathcal M}{\Delta}
\exp\left[\frac{U(x-x_0)-\Delta|x-x_0|}{2D_{\rm eff}}\right],
\qquad C(x,t)\to0.}
$$

Its integral is $\mathcal M$, so all the released tracer is eventually captured in this infinite-domain model. This distinguishes the finite-pulse deposited profile from the continuously accumulating deposit under sustained injection.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
