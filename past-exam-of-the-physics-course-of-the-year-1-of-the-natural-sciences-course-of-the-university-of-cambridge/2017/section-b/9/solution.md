<h1 id="section-b/9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

Use the PDF's notation $f_0$ for the source-frame pulse [frequency](../../../../frequency.md), and set $\beta=v/c$, $\gamma=(1-\beta^2)^{-1/2}$. Successive emissions occur at the same train-frame position and are separated by [proper time](../../../../proper-time.md) $1/f_0$. The [Lorentz transformation](../../../../lorentz-transformation.md) gives a station-frame emission interval $\Delta t_e=\gamma/f_0$ and displacement $v\Delta t_e$. For a receding beacon, the second pulse travels an extra distance $v\Delta t_e$, so

$$
\Delta t_r=\Delta t_e(1+\beta),\qquad \boxed{\frac f{f_0}=\frac1{\gamma(1+\beta)}=\sqrt{\frac{1-\beta}{1+\beta}}.}
$$

This derivation includes both [time dilation](../../../../time-dilation.md) and the change in light-travel time. Expanding for $\beta\ll1$ gives $f/f_0=1-\beta+O(\beta^2)$, recovering the stated nonrelativistic approximation.

Let $\lambda_0$ be the common [wavelength](../../../../wavelength.md) of the identical lights at rest. The approaching and receding [relativistic Doppler effect](../../../../relativistic-doppler-effect.md) factors give

$$
\lambda_1=\lambda_0\sqrt{\frac{1-\beta}{1+\beta}},\qquad \lambda_2=\lambda_0\sqrt{\frac{1+\beta}{1-\beta}}.
$$

Their ratio and product therefore determine the [speed](../../../../speed.md) and rest [wavelength](../../../../wavelength.md) separately:

$$
\boxed{\beta=\frac{\lambda_2-\lambda_1}{\lambda_2+\lambda_1}=\frac{636-530}{636+530}=\frac1{11},\qquad v=0.0909c,}
$$



$$
\boxed{\lambda_0=\sqrt{\lambda_1\lambda_2}=580.6\,\mathrm{nm}.}
$$

No assumption about the rest color was needed.

The last observation requires a transverse-geometry convention. The general observer-frame ray formula is

$$
\boxed{\lambda=\gamma\lambda'_3(1-\beta\cos\theta),}
$$

where $\theta$ is the angle between source [velocity](../../../../velocity.md) and photon propagation **in the platform frame at emission**. Under the usual transverse-ray interpretation, $\theta=\pi/2$, so for $\beta=0.6$ and $\gamma=1.25$,

$$
\boxed{\lambda=\gamma\lambda'_3=500\,\mathrm{nm}\quad\text{for a platform-frame transverse ray}.}
$$

This is the standard transverse redshift from [time dilation](../../../../time-dilation.md).

There is a genuine distinction between emission and reception at the instant of passing. A side-mounted source emitting perpendicularly in its own frame instead has $\cos\theta=\beta$ by [aberration of light](../../../../relativistic-aberration.md), giving $\lambda=\lambda'_3/\gamma=320\,\mathrm{nm}$. The same blue result occurs if “at the exact moment” means reception when the source's current position is at closest approach, with a small finite transverse offset. For offset $d$, reception and emission satisfy $t_r=t_e+\sqrt{v^2t_e^2+d^2}/c$. Setting $t_r=0$ gives $t_e=-\gamma d/c$ and $\cos\theta=\beta$; setting $t_e=0$ instead gives the transverse ray received at $t_r=d/c$. These limits remain different as $d\to0$.

<a id="section-b/9/image-emission-at-closest-approach-and-reception-at-closest-approach-give-different-doppler-factors"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017-doppler-geometry.png)

**[Figure 1](#section-b/9/image-emission-at-closest-approach-and-reception-at-closest-approach-give-different-doppler-factors). Emission at closest approach and reception at closest approach give different Doppler factors**.

Thus **500 nm requires the transverse ray in the platform frame**; **320 nm applies to reception at closest approach or transverse emission in the train frame**. The wording does not distinguish these event/frame choices, so merely neglecting the source-observer separation is insufficient to select between them. The reusable derivation is [transverse Doppler shift and observation time](../../../../transverse-doppler-shift-and-observation-time.md).

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Section B](../../section-b.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
