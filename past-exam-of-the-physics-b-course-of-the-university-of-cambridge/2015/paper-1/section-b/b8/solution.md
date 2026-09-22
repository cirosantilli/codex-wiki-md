<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

The [characteristic impedance](../../../../../characteristic-impedance.md) of a lossless [transmission line](../../../../../transmission-line.md) is the ratio of the [voltage](../../../../../voltage.md) to the current amplitude of a single forward-travelling wave. If $\mathcal L$ and $\mathcal C$ denote [inductance](../../../../../inductance.md) and [capacitance per unit length](../../../../../capacitance-per-unit-length.md), the lossless telegrapher equations give

$$
\partial_z V=-\mathcal L\partial_t I,\qquad
\partial_z I=-\mathcal C\partial_t V,
\qquad \boxed{Z=\sqrt{\mathcal L/\mathcal C}},\qquad
v_p=(\mathcal L\mathcal C)^{-1/2}.
$$

A backward wave has $I_-=-V_-/Z$ when current is positive along $+z$. Thus [characteristic impedance](../../../../../characteristic-impedance.md) is not a resistor's [electrical resistance](../../../../../electrical-resistance.md): it describes travelling-wave amplitudes and determines [impedance matching](../../../../../impedance-matching.md), power transfer and reflections. A semi-infinite line, or a line terminated by a matching load, presents that impedance at its input.

At a junction with no lumped branch, [voltage](../../../../../voltage.md) and [electric current](../../../../../electric-current.md) are continuous:

$$
V_i+V_r=V_t,\qquad \frac{V_i-V_r}{Z_1}=\frac{V_t}{Z_2}.
$$

Eliminating $V_t$ gives the voltage [reflection coefficient](../../../../../reflection-coefficient.md)

$$
\boxed{r=\frac{V_r}{V_i}=\frac{Z_2-Z_1}{Z_2+Z_1}.}
$$

For real positive $Z_1$, incident and reflected waves occupy the same line, so their power ratio is $|r|^2$.

For the slightly mismatched [coaxial cables](../../../../../coaxial-cable.md), the change in [characteristic impedance](../../../../../characteristic-impedance.md) is

$$
\Delta Z=\frac{Z_{\rm vac}}{2\pi n}\ln\!\left(1+\frac{\Delta b}b\right)
\simeq\frac{Z_{\rm vac}}{2\pi n}\frac{\Delta b}b.
$$

Consequently

$$
r\simeq\frac{\Delta Z}{2Z}=\frac1{2\ln(b/a)}\frac{\Delta b}b,\qquad
\boxed{\mathcal R\simeq\frac{1}{4\ln^2(b/a)}\left(\frac{\Delta b}b\right)^2.}
$$

The requested power limit $0.01\%=10^{-4}$ implies $|\Delta b|/b<0.02\ln(b/a)$. Since $\ln(b/a)=2\pi nZ/Z_{\rm vac}=1.918$ for the stated line, **the adjacent cables' outer radii must match within approximately $3.84\%$**. If a tolerance is quoted separately as a symmetric manufacturing range $\pm\delta b$ and arbitrary worst-case pairs can differ by $2\delta b$, the corresponding individual tolerance is approximately **$\pm1.92\%$**. The leading calculation is for small mismatches; the exact logarithmic expression gives slightly asymmetric positive and negative limits. The vacuum [wave impedance](../../../../../wave-impedance.md) used here is approximately $376.73\ \Omega$.[2022 CODATA adjustment, characteristic impedance of vacuum entry](../../../../../fundamental-physical-constants-complete-listing-by-national-institute-of-standards-and-technology-and-others.md)

A needle is a shunt [electrical resistance](../../../../../electrical-resistance.md) $R_n$, so the load seen at its location is the continuation of the line in parallel with $R_n$: $Z_L=ZR_n/(Z+R_n)$. The local voltage [reflection coefficient](../../../../../reflection-coefficient.md) and transmission amplitude are

$$
\boxed{r=-\frac{Z}{2R_n+Z}\simeq-\frac{Z}{2R_n}},\qquad t=1+r.
$$

For [periodic resistive loading of a transmission line](../../../../../periodic-resistive-loading-of-a-transmission-line.md), the reflection from the next needle travels an additional round trip $2L$ and crosses each previous needle twice. Taking the first needle as phase reference, the [single-return approximation for periodic line reflections](../../../../../single-return-approximation-for-periodic-line-reflections.md) therefore sums to

$$
R_{\rm first}=r\sum_{j=0}^\infty[t^2e^{i\phi}]^j
=\frac r{1-(1+r)^2e^{i\phi}},\qquad
\phi=2kL=\frac{4\pi\nu L}{v_p}.
$$

Here $v_p$ is the propagation [phase velocity](../../../../../phase-velocity.md) in the cable, $c/n$ for the stated nondispersive nonmagnetic filling. Squaring the amplitude gives the requested expression

$$
\boxed{\mathcal R_{\rm first}(\nu)=\left|\frac r{1-(1+r)^2e^{i\phi(\nu)}}\right|^2.}
$$

For a finite number $N$ of needles the amplitude has the additional numerator $1-[t^2e^{i\phi}]^N$. The displayed semi-infinite result assumes sufficiently many needles, no terminal reflection, and neglects intrinsic propagation loss.

For real $r<0$, write $q=t^2$. The denominator of the power coefficient is $1+q^2-2q\cos\phi$. It has constructive peaks at $\phi=2\pi j$ and minima at $\phi=(2j+1)\pi$, repeating with **frequency spacing $\Delta\nu=v_p/(2L)$**. Within this approximation,

$$
\mathcal R_{\max}=\frac1{(2+r)^2}\simeq\frac14,\qquad
\mathcal R_{\min}=\frac{r^2}{[1+(1+r)^2]^2}\simeq\frac{r^2}{4}.
$$

Weak individual shunts thus give narrow interference peaks, with phase width of order $|r|$.

The requested sum excludes paths that reflect repeatedly between different needles. It should not be read as an exact multiple-scattering result, particularly at the coherent peaks. For example the exact semi-infinite amplitude satisfies

$$
R=r+\frac{t^2e^{i\phi}R}{1-r e^{i\phi}R}.
$$

At $\phi=2\pi j$ this equation reduces to $(R+1)^2=0$: the exact ideal infinite array has unit power reflection there, rather than the first-return approximation's value near $1/4$. This does not change the requested geometric-series derivation, but identifies its physical limitation.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
