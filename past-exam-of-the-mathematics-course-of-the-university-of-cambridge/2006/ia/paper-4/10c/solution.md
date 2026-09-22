<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

Take rightward velocities as positive just before the right-wall collision. The incoming particle velocity is $v$ and the wall velocity is $-V$. Their total momentum divided by total mass gives the [centre of mass](../../../../../center-of-mass.md) velocity

$$
\boxed{v_{\mathrm{cm}}=\frac{mv-MV}{m+M}.}
$$

In an [elastic collision](../../../../../elastic-collision.md), relative velocity reverses, so the particle's signed outgoing velocity is $v_{\mathrm{out}}=2v_{\mathrm{cm}}-v$. For $M>m$ it is negative, and its speed is

$$
\boxed{v'=\frac{(M-m)v+2MV}{M+m}.}
$$

Consequently the exact change in speed is

$$
v'-v=\frac{2(MV-mv)}{M+m}
=2V-\frac{2m}{M+m}(v+V).
$$

For $m/M\to0$ with $v,V$ fixed, this proves the requested leading increment $v'-v\simeq2V$. Reflection gives the same increment at the left wall.

This approximation is not uniform when $v/V$ is allowed to become arbitrarily large. To neglect recoil relative to the increment $2V$ requires

$$
\frac mM\frac vV\ll1.
$$

The inequalities $m\ll M$ and $v\gg V$ alone do not imply it: for example, $m/M=10^{-3}$ and $v/V=10^3$ give an exact zero speed increment. The subsequent slowly moving-wall approximation therefore uses the consistent joint range $1\ll v/V\ll M/m$, or treats the walls as effectively prescribed massive reflectors. The assumed slow change of wall speed over many impacts embodies the same negligible-recoil requirement.

Within this approximation, the separation derivative is the right-wall velocity minus the left-wall velocity:

$$
\dot\ell=-2V,\qquad \Delta\ell\simeq-2V\Delta t.
$$

For a time window containing many crossings but little separation change, $\ell/v\ll\Delta t\ll\ell/V$, the flight time between successive wall collisions is approximately $\ell/v$. Thus their number and the cumulative speed change are

$$
N_{\mathrm{coll}}\simeq\frac{v\Delta t}{\ell},\qquad
\Delta v\simeq2V N_{\mathrm{coll}}
=\frac{2Vv\Delta t}{\ell}
=-\frac{\Delta\ell}{\ell}v.
$$

Passing to the averaged differential equation gives

$$
\frac{\dot v}{v}=-\frac{\dot\ell}{\ell},\qquad
\frac d{dt}\log(v\ell)\simeq0.
$$

Hence the [particle-speed invariant between slowly approaching walls](../../../../../particle-speed-invariant-between-slowly-approaching-walls.md) is

$$
\boxed{v(t)\ell(t)\simeq v(t_0)\ell(t_0),\qquad v\propto\ell^{-1}.}
$$

It is an [adiabatic invariant](../../../../../adiabatic-invariant.md) for the rapid elastic bouncing motion while the separation and wall velocities vary slowly on the flight-time scale.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
