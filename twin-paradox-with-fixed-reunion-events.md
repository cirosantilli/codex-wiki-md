# Twin paradox with fixed reunion events

↑ **Parent:** [Twin paradox](twin-paradox.md)

Work in [Minkowski spacetime](minkowski-spacetime.md), neglect [gravity](gravity.md), and choose the stay-at-home clock's [inertial frame](inertial-frame.md). Let departure be $O=(t,x)=(0,0)$ and reunion be $R=(T,0)$. The home clock follows $x_H(t)=0$. A traveller moves outward with [velocity](velocity.md) $+v$ and returns with [velocity](velocity.md) $-v$, where $0<v<c$ and $c$ is the [speed of light](speed-of-light.md). The ideal [world line](world-line.md) has a sharp turnaround at $P=(T/2,vT/2)$:

$$
x_T(t)=
\begin{cases}
vt,&0\leq t\leq T/2,\\
v(T-t),&T/2\leq t\leq T.
\end{cases}
$$

Each straight leg lies in an [inertial frame](inertial-frame.md), but no single traveller [inertial frame](inertial-frame.md) covers both legs.

For any differentiable [timelike curve](timelike-curve.md) in this home [inertial frame](inertial-frame.md), its clock accumulates [proper time](proper-time.md) through the [integral](integral.md)

$$
\Delta\tau=\int_0^T\sqrt{1-\frac{v(t)^2}{c^2}}\,dt.
$$

Apply it separately to the traveller's two legs. With the [Lorentz factor](lorentz-factor.md) $\gamma=(1-v^2/c^2)^{-1/2}$,

$$
\Delta\tau_H=T,\qquad
\Delta\tau_T=\frac{T}{\gamma},\qquad
\Delta\tau_H-\Delta\tau_T=T\left(1-\frac1\gamma\right).
$$

For $v=0.6c$ and $T=10\,\mathrm{yr}$, the [Lorentz factor](lorentz-factor.md) is $\gamma=1.25$. The turnaround is $3$ light-years away at home time $5\,\mathrm{yr}$. The traveller records $4\,\mathrm{yr}$ outward and $4\,\mathrm{yr}$ returning: the reunited clocks read $10\,\mathrm{yr}$ and $8\,\mathrm{yr}$. These are illustrative model values, not experimental measurements.

<a id="image-fixed-departure-and-reunion-events-a-0-6c-traveller-records-eight-years-while-the-inertial-home-clock-records-ten-turnaround-simultaneity-slices-meet-the-home-world-line-at-3-2-and-6-8-years"></a>
![](twin-paradox-reunion-spacetime.png)

**[Figure 2](#image-fixed-departure-and-reunion-events-a-0-6c-traveller-records-eight-years-while-the-inertial-home-clock-records-ten-turnaround-simultaneity-slices-meet-the-home-world-line-at-3-2-and-6-8-years). Fixed departure and reunion events: a 0.6c traveller records eight years while the inertial home clock records ten; turnaround simultaneity slices meet the home world line at 3.2 and 6.8 years**.

The same [integral](integral.md) gives a short geometric explanation: $\sqrt{1-v(t)^2/c^2}\leq1$, so every such competing [timelike curve](timelike-curve.md) between these fixed [spacetime events](event-relativity.md) has $\Delta\tau\leq T$. Equality requires zero [velocity](velocity.md) throughout, apart from sets of zero duration. Thus the straight home [world line](world-line.md) maximizes [proper time](proper-time.md) in this [Minkowski spacetime](minkowski-spacetime.md) problem. This statement concerns fixed endpoints and an inertial home clock; in a [gravitational field](gravitational-field.md), compare paths using the appropriate [metric tensor](metric-tensor.md).

## ↑ Ancestors (7)

1. [Twin paradox](twin-paradox.md)
2. [Time dilation](time-dilation.md)
3. [Lorentz factor](lorentz-factor.md)
4. [Special relativity](special-relativity-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
