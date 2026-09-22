<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

In the [uniform-Earth chord oscillator](../../../../../uniform-earth-chord-oscillator.md), neglect the [mass](../../../../../mass.md) removed by the narrow tunnel and any rotation of the [Earth](../../../../../earth.md). Inside a uniform [sphere](../../../../../sphere.md), the [shell theorem](../../../../../spherical-shell-theorem.md) gives $\mathbf F=-(4\pi G\rho m/3)\mathbf r$. On the constrained chord $\mathbf r=(d,y)$, its along-tunnel component is

$$
\boxed{F_y=-m\omega_0^2y,\qquad\omega_0^2=\frac{4\pi G\rho}{3}.}
$$

The transverse component is balanced by the tunnel constraint. With release from $y_s=\sqrt{R^2-d^2}$ at rest,

$$
\ddot y+\omega_0^2y=0,\qquad \boxed{y(t)=y_s\cos\omega_0t.}
$$

The far end is $-y_s$, so **$t_{\rm transit}=\pi/\omega_0\approx2530\,\mathrm s=42.2\,\mathrm{min}$**, independent of chord offset in this ideal model. Here $\rho=5515\,\mathrm{kg\,m^{-3}}$ and $G=6.67430\times10^{-11}\,\mathrm{m^3\,kg^{-1}\,s^{-2}}$ give $\omega_0=1.24171\times10^{-3}\,\mathrm{s^{-1}}$.

With linear drag, $\ddot y+(b/m)\dot y+\omega_0^2y=0$. Inserting a [complex exponential](../../../../../complex-exponential-function.md) $e^{-(\gamma+i\omega)t}$ gives

$$
\gamma^2-\omega^2-\frac bm\gamma+\omega_0^2+i\omega(2\gamma-b/m)=0,
$$

so in the [underdamped](../../../../../underdamping.md) regime

$$
\boxed{\gamma=\frac b{2m},\qquad\omega=\sqrt{\omega_0^2-\gamma^2}.}
$$

Real physical solutions combine conjugate modes. Release from rest specifically gives $y=y_se^{-\gamma t}[\cos\omega t+(\gamma/\omega)\sin\omega t]$; a lone exponential with prefactor $y_s$ does not impose that initial [velocity](../../../../../velocity.md).

The [critical gravity-tunnel settling time](../../../../../critical-gravity-tunnel-settling-time.md) follows from critical damping, the fastest non-oscillatory release:

$$
\boxed{b_c=2m\omega_0,\qquad b_c/m=2.48342\times10^{-3}\,\mathrm{s^{-1}},\qquad
y(t)=y_s(1+\omega_0t)e^{-\omega_0t}.}
$$

Interpret the 1% tolerance relative to the initial displacement from equilibrium. With $s=\omega_0t$, $(1+s)e^{-s}=0.01$ has $s=6.63835$. Hence

$$
\boxed{t_{1\%}=6.63835/\omega_0\approx5346\,\mathrm s=89.1\,\mathrm{min}.}
$$

The equilibrium is reached only asymptotically; using a pure $e^{-\omega_0t}$ would miss the critical-damping polynomial factor and underestimate this time.

## ↑ Ancestors (13)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
