<h1 id="section-a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

There is a source error to resolve first. For a [drag coefficient](../../../../drag-coefficient.md) defined by $F_{\mathrm{drag}}=-\xi v$, the [velocity relaxation time](../../../../velocity-relaxation-time.md) is $\tau=m/\xi$. The mass and drag coefficient in the PDF's exponential are interchanged: $\xi t/m$ is dimensionless, whereas $mt/\xi$ is not. The consistent mean relaxation law is therefore $\langle v(t)\rangle=v_0e^{-t/\tau}$.

A mean relaxation law alone does not determine a [variance](../../../../variance-split.md). Use the usual thermal [Langevin equation](../../../../langevin-dynamics.md), with a bath at [temperature](../../../../temperature-split.md) $T$ and the [fluctuation-dissipation relation for a Langevin particle](../../../../fluctuation-dissipation-relation-for-a-langevin-particle.md):

$$
m\dot v=-\xi v+f(t),\qquad
\langle f(t)\rangle=0,\qquad
\langle f(t)f(t')\rangle=2\xi k_BT\,\delta(t-t').
$$

Here the calculation is for one component in [Cartesian coordinates](../../../../cartesian-coordinate-system.md). With fixed initial position and velocity, integration gives the [mean displacement](../../../../mean-displacement.md)

$$
\langle x(t)-x_0\rangle=v_0\tau(1-e^{-t/\tau}).
$$

Integrating the stochastic part of the velocity once more gives the centered displacement

$$
x(t)-\langle x(t)\rangle
=\frac1\xi\int_0^t\bigl[1-e^{-(t-s)/\tau}\bigr]f(s)\,ds.
$$

The delta correlation reduces its [variance](../../../../variance-split.md) to a single [integral](../../../../integral-split.md):

$$
\begin{aligned}
\operatorname{Var}x(t)
&=\frac{2k_BT}{\xi}\int_0^t\bigl[1-e^{-(t-s)/\tau}\bigr]^2ds\\
&=\boxed{2D\left[t-2\tau(1-e^{-t/\tau})+\frac\tau2(1-e^{-2t/\tau})\right]},
\qquad \boxed{D=\frac{k_BT}{\xi}}.
\end{aligned}
$$

This is the [integrated Ornstein-Uhlenbeck displacement](../../../../integrated-ornstein-uhlenbeck-displacement.md) for a prescribed initial velocity. Its short-time variance is $2Dt^3/(3\tau^2)+O(t^4)$; at long times it is $2Dt+O(1)$. Thus the [diffusion coefficient](../../../../diffusion-coefficient.md) is

$$
\boxed{D=\lim_{t\to\infty}\frac{\operatorname{Var}x(t)}{2t}}.
$$

If the requested mean-squared fluctuation instead refers to the conventional equilibrium [mean squared displacement](../../../../mean-squared-displacement.md), the initial velocity is also averaged over its thermal distribution, with $\langle v_0\rangle=0$ and $\langle v_0^2\rangle=k_BT/m$. Its contribution adds $D\tau(1-e^{-t/\tau})^2$, giving

$$
\boxed{\langle[x(t)-x(0)]^2\rangle_{\mathrm{eq}}=2D\left[t-\tau(1-e^{-t/\tau})\right]}.
$$

This has the ballistic limit $(k_BT/m)t^2$ and the same diffusive limit $2Dt$. For fixed nonzero $v_0$, the uncentered mean square instead equals the first boxed [variance](../../../../variance-split.md) plus $v_0^2\tau^2(1-e^{-t/\tau})^2$. In three independent spatial dimensions, the centered variances add, and the long-time result is $\langle|\mathbf r-\langle\mathbf r\rangle|^2\rangle\sim6Dt$. Stating the initial-velocity convention is necessary to distinguish these finite-time formulas.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Section A](../../section-a.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
