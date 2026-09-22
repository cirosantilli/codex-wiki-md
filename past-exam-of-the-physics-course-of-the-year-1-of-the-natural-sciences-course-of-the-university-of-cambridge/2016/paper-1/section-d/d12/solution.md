<h1 id="section-d/d12/solution">Solution</h1>

↑ **Parent:** [D12](../d12.md)

Comparing with the standard [wave equation](../../../../../wave-equation-split.md) gives the shallow-water [wave speed](../../../../../wave-speed.md)

$$
\boxed{c=\sqrt{gd}.}
$$

Twice differentiating the proposed [standing wave](../../../../../standing-wave.md) multiplies its spatial factors by $-k_x^2$ and $-k_y^2$, and its temporal factor by $-\omega^2$. It solves the [wave equation](../../../../../wave-equation-split.md) precisely when

$$
\boxed{\omega^2=gd(k_x^2+k_y^2).}
$$

To obtain the local [gravitational potential energy](../../../../../gravitational-energy.md), integrate through a water column of height $d+h$ and unit horizontal area:

$$
V(t)=\int_0^{d+h}\rho gz\,dz=\frac{\rho g}{2}(d+h)^2.
$$

The time averages are $\langle h\rangle=0$ and $\langle h^2\rangle=A^2\cos^2(k_xx)\cos^2(k_yy)/2$. Thus

$$
\boxed{\langle V\rangle=\frac12\rho gd^2+\frac14\rho gA^2\cos^2(k_xx)\cos^2(k_yy),\quad c_1=\frac12\rho gd^2,\quad c_2=\frac14\rho gA^2.}
$$

The constant is retained because the specified zero of [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md) is the tank bottom. This is local time-averaged [potential energy](../../../../../potential-energy.md), not the sum of [potential energy](../../../../../potential-energy.md) and [kinetic energy](../../../../../kinetic-energy.md).

The no-normal-flow wall conditions are [Neumann boundary conditions](../../../../../neumann-boundary-condition.md). Differentiating the cosine factors at the opposite walls gives

$$
\boxed{k_x=\frac{m\pi}{a},\qquad k_y=\frac{n\pi}{b},\qquad m,n=0,1,2,\ldots.}
$$

Negative integers give the same cosine modes. The formal $m=n=0$ case has $\omega=0$: it is a uniform change of the mean level, not a finite-[frequency](../../../../../frequency.md) oscillation. In a closed tank with fixed water volume even that mean-level change is excluded from the oscillatory disturbance.

Since $a<b$, the lowest finite [frequency](../../../../../frequency.md) is the mode $(m,n)=(0,1)$:

$$
\boxed{h=A\cos(\pi y/b)\cos(\omega t),\qquad \omega=\frac\pi b\sqrt{gd}.}
$$

It is uniform across the shorter direction, has opposite-sign displacement [antinodes](../../../../../antinode.md) at the two ends of the longer direction, and a displacement [node](../../../../../node-dynamical-systems.md) midway along it.

<a id="section-d/d12/image-original-mode-shapes-for-a-closed-rectangular-tank-and-an-ideal-basin-with-one-open-end"></a>
![](../../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-1-water-modes.png)

**[Figure 5](#section-d/d12/image-original-mode-shapes-for-a-closed-rectangular-tank-and-an-ideal-basin-with-one-open-end). Original mode shapes for a closed rectangular tank and an ideal basin with one open end**.

For the open-ended [Bay of Fundy](../../../../../bay-of-fundy.md) model, approximate the ocean mouth as a displacement [node](../../../../../node-dynamical-systems.md) and the closed head as an [antinode](../../../../../antinode.md). The fundamental is a [quarter-wave basin resonance](../../../../../quarter-wave-basin-resonance.md), so its [wavelength](../../../../../wavelength.md) is $4L$ and

$$
T=\frac{4L}{\sqrt{gd}},\qquad \boxed{d=\frac{16L^2}{gT^2}.}
$$

Taking a roughly $12$-hour [semidiurnal tide](../../../../../semidiurnal-tide.md) gives $d\simeq79\ \mathrm m$. Using the principal lunar period of approximately $12\ \mathrm h\ 25\ \mathrm{min}$ gives $d\simeq73\ \mathrm m$. **The idealized estimate is therefore about $7\text{–}8\times10^1\ \mathrm m$.** The lunar period is half of a roughly $24$-hour $50$-minute lunar day.[Examples M2 and S2: two lunar peaks per 24 hours 50 minutes, compared with two solar peaks per 24 hours](../../../../../about-harmonic-constituents-by-national-oceanic-and-atmospheric-administration.md)

This estimate treats the mouth as an ideal open boundary and replaces the real basin by a uniform depth. The supplied large tidal height motivates [resonance](../../../../../resonance.md); it is not enough by itself to determine damping or an amplification factor in this model.

## ↑ Ancestors (13)

1. [D12](../d12.md)
2. [Section D](../../section-d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
