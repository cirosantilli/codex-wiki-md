<h1 id="section-b/b7/solution">Solution</h1>

↑ **Parent:** [B7](../b7.md)

For a uniform taut sheet in the small-displacement approximation, the two-dimensional [wave equation](../../../../../wave-equation-split.md) is

$$
\partial_t^2\psi=v^2(\partial_x^2\psi+\partial_y^2\psi).
$$

Seek a harmonic solution $Y(y)e^{i\omega t-ik_xx}$. The clamped edges impose [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) $Y(0)=Y(b)=0$. Hence $Y''+k_y^2Y=0$ has nontrivial solutions only for

$$
Y=A\sin(n\pi y/b),\qquad k_y=n\pi/b,\quad n=1,2,\ldots.
$$

Taking the real part gives the stated sinusoidal transverse profile. There is no nonzero $n=0$ mode satisfying both clamped boundaries.

Substitution gives the [dispersion relation](../../../../../dispersion-relation-split.md)

$$
\boxed{\omega_n^2=v^2\left[k_x^2+(n\pi/b)^2\right].}
$$

The three branches have cutoffs $\omega_{c,n}=n\pi v/b$ at $k_x=0$ and approach $\omega=v|k_x|$ at large $|k_x|$. Only frequencies above a branch's cutoff give traveling [waves](../../../../../wave-split.md) along an infinitely long guide; below it, the axial dependence is evanescent. For a forward propagating mode,

$$
\boxed{v_{p,n}=\frac{\omega}{k_x}
=\frac{v}{\sqrt{1-(nv/(2bf))^2}},\qquad
v_{g,n}=\frac{d\omega}{dk_x}=\frac{v^2}{v_{p,n}}.}
$$

The [phase velocity](../../../../../phase-velocity.md) exceeds $v$, while the [group velocity](../../../../../group-velocity.md) is smaller: the carrier phase speed is not the signal speed.

Here the first two cutoff frequencies are $50$ and $100\ {\rm Hz}$, so both modes propagate at $200\ {\rm Hz}$. With $\omega=400\pi\ {\rm s^{-1}}$,

$$
\boxed{
\begin{array}{c|cc}
n&k_x\ ({\rm m^{-1}})&v_p\ ({\rm m\,s^{-1}})\\
1&10\pi\sqrt{15}=121.673&40/\sqrt{15}=10.328\\
2&20\pi\sqrt3=108.828&20/\sqrt3=11.547
\end{array}}
$$

Each transverse mode independently acquires its axial phase. The second mode first changes sign relative to the first when $(k_1-k_2)x_1=\pi$, giving

$$
\boxed{x_1=\frac{\pi}{10\pi\sqrt{15}-20\pi\sqrt3}
=\frac{1}{10(\sqrt{15}-2\sqrt3)}
\simeq0.2446\ {\rm m}.}
$$

At that distance a common temporal phase is $\phi=-k_1x_1$ modulo $2\pi$; the second term is negative relative to the first for every $y$ and every time, not just at one selected instant.

In an optical fibre, different guided modes have different [group velocities](../../../../../group-velocity.md), so an input pulse becomes a sum of differently delayed pulses. This [intermodal dispersion](../../../../../intermodal-dispersion.md) broadens pulses and can make adjacent digital symbols overlap. A [single-mode optical fiber](../../../../../single-mode-optical-fiber.md) removes this particular mode-delay mechanism; a [graded-index optical fiber](../../../../../graded-index-optical-fiber.md) can reduce it in a multimode design. Single-mode propagation still permits wavelength-dependent group delay, so it does not remove every kind of [optical dispersion](../../../../../dispersion-optics.md).

## ↑ Ancestors (14)

1. [B7](../b7.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
