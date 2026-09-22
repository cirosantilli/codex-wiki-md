# Twin paradox with finite acceleration

↑ **Parent:** [Twin paradox](twin-paradox.md)

An instantaneous reversal is an idealization. A real traveller changes [velocity](velocity.md) over a finite time, follows a smooth [world line](world-line.md), and has finite [proper acceleration](proper-acceleration.md). [Special relativity](special-relativity-split.md) still calculates the elapsed [proper time](proper-time.md) using the home [inertial frame](inertial-frame.md) and the same [integral](integral.md); [general relativity](general-relativity-split.md) is not needed merely because the traveller accelerates in otherwise flat [spacetime](spacetime.md). The [clock hypothesis](clock-hypothesis.md) identifies an ideal clock's reading with this geometric [proper time](proper-time.md).

One explicit smooth trip between the same $O$ and $R$ starts and ends at rest in the home [inertial frame](inertial-frame.md). Choose

$$
v(t)=v_{\max}\sin\left(\frac{2\pi t}{T}\right),\qquad
x_T(t)=\frac{v_{\max}T}{2\pi}\left[1-\cos\left(\frac{2\pi t}{T}\right)\right],
\qquad 0\leq t\leq T.
$$

Its [velocity](velocity.md) reverses continuously at $T/2$, and its [proper acceleration](proper-acceleration.md) is bounded because $v_{\max}<c$ and $dv/dt$ is finite. With $v_{\max}=0.6c$ and $T=10\,\mathrm{yr}$, [numerical integration](numerical-integration.md) gives

$$
\Delta\tau_T=\int_0^{10\,\mathrm{yr}}\sqrt{1-0.36\sin^2\left(\frac{2\pi t}{10\,\mathrm{yr}}\right)}\,dt
\simeq9.028\,\mathrm{yr}.
$$

This comparison fixes the reunion [spacetime events](event-relativity.md) and maximum [speed](speed.md), not the turnaround distance: the smooth trip reaches $v_{\max}T/\pi\simeq1.910$ light-years, whereas the ideal trip reaches $3$ light-years. The smooth traveller spends less time at high [speed](speed.md) and therefore accumulates more [proper time](proper-time.md) than the ideal traveller, while still accumulating less than the home clock.

<a id="image-signed-velocity-and-accumulated-proper-time-for-ideal-and-smooth-trips-with-the-same-ten-year-reunion-and-maximum-speed-0-6c-their-turnaround-distances-differ"></a>
![](twin-paradox-smooth-speed-proper-time.png)

**[Figure 3](#image-signed-velocity-and-accumulated-proper-time-for-ideal-and-smooth-trips-with-the-same-ten-year-reunion-and-maximum-speed-0-6c-their-turnaround-distances-differ). Signed velocity and accumulated proper time for ideal and smooth trips with the same ten-year reunion and maximum speed 0.6c; their turnaround distances differ**.

For a sufficiently short smooth reversal replacing the corner, the [proper time](proper-time.md) approaches the piecewise inertial result. A reversal interval of home duration $\delta t$ contributes between zero and $\delta t$ to the clock reading; shrinking that interval cannot create a finite extra loss concentrated at the corner. The finite difference survives in the long coasting legs. Keeping the same reversal manoeuvre while lengthening those legs changes the age difference. Conversely, two travellers following mirrored paths with the same [speed](speed.md) history accumulate equal [proper times](proper-time.md), even though both accelerate. Thus [acceleration](acceleration.md) distinguishes paths and enables reunion here, but an amount of [acceleration](acceleration.md) alone does not determine the age difference.

The changing simultaneity assignment also becomes continuous. At a traveller [spacetime event](event-relativity.md) $(t,x(t))$ with instantaneous [velocity](velocity.md) $v(t)$, the momentarily comoving [inertial frame](inertial-frame.md) assigns home time $t_H=t-v(t)x(t)/c^2$. Differentiating gives

$$
\frac{dt_H}{dt}=1-\frac{v(t)^2}{c^2}-\frac{x(t)}{c^2}\frac{dv}{dt}.
$$

During the reversal at positive $x$, the last term advances the assigned home time rapidly. It describes the traveller's changing [relativity of simultaneity](relativity-of-simultaneity.md), not a locally measured alteration of the home clock's ticking.

**Table of contents**

- [Clock hypothesis](clock-hypothesis.md)

## ↑ Ancestors (7)

1. [Twin paradox](twin-paradox.md)
2. [Time dilation](time-dilation.md)
3. [Lorentz factor](lorentz-factor.md)
4. [Special relativity](special-relativity-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
