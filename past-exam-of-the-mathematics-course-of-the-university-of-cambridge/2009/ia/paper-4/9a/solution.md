<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Use signed [velocities](../../../../../velocity.md) in Skaro's [inertial frame](../../../../../inertial-frame.md); the returning velocity $w$ must be negative. For the first two rockets, the [Lorentz transformation](../../../../../lorentz-transformation.md) of infinitesimal separations is $dx=\gamma_u(dx'+u\,dt')$, $dt=\gamma_u(dt'+u\,dx'/c^2)$. Dividing with $dx'/dt'=v'$ gives the [relativistic velocity-addition formula](../../../../../velocity-addition-formula.md)

$$
\boxed{v=\frac{u+v'}{1+uv'/c^2}}.
$$

For the third rocket, its signed velocity in the second frame is $-w''$, so another application gives

$$
w=\frac{v-w''}{1-vw''/c^2},\qquad \boxed{w=\frac{u+v'-w''(1+uv'/c^2)}{1+uv'/c^2-w''(u+v')/c^2}}.
$$

Since $0<v<c$ and $0<w''<c$, the denominator $1-vw''/c^2$ is positive. The third rocket returns from positive $x$ to Skaro if and only if $w<0$, hence

$$
\boxed{w''>v=\frac{u+v'}{1+uv'/c^2}}.
$$

Equality leaves it stationary in Skaro's frame, so it never returns from $x=2L$; a smaller $w''$ leaves it travelling outward.

Let $O$ denote departure, $A$ boarding the second rocket, $B$ boarding the third, and $C$ reunion with Skaro. In coordinates $(t,x)$, their positions on the [worldline](../../../../../world-line.md) are

$$
\boxed{O=(0,0),\quad A=(L/u,L),\quad B=(L/u+L/v,2L),\quad C=(L/u+L/v-2L/w,0).}
$$

Indeed, the first two coordinate durations are $L/u$ and $L/v$, and the returning leg has duration $-2L/w>0$. Equivalently, their $(ct,x)$ coordinates are obtained by multiplying each displayed time by $c$; these are the coordinates used for the [spacetime](../../../../../spacetime.md) diagram.

<a id="9a/image-three-inertial-rocket-legs-and-reunion-in-skaro-s-frame"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-4-three-rockets.png)

**[Figure 1](#9a/image-three-inertial-rocket-legs-and-reunion-in-skaro-s-frame). Three inertial rocket legs and reunion in Skaro's frame**.

The diagram uses representative velocities satisfying the return condition; its event labels apply to the general formulas above. Skaro's elapsed time is

$$
\boxed{T=\frac Lu+\frac Lv-\frac{2L}{w}}.
$$

On a constant-velocity leg the traveller's [proper time](../../../../../proper-time.md) is $\Delta t/\gamma_V=\Delta t\sqrt{1-V^2/c^2}$, by [time dilation](../../../../../time-dilation.md). Neglecting the specified brief accelerations, Davros therefore ages by

$$
\boxed{\Delta\tau=\frac Lu\sqrt{1-\frac{u^2}{c^2}}+\frac Lv\sqrt{1-\frac{v^2}{c^2}}-\frac{2L}{w}\sqrt{1-\frac{w^2}{c^2}}.}
$$

Every contribution is positive because $w<0$. Each square-root factor is smaller than one, so $\Delta\tau<T$: Davros returns younger than a companion who remained on Skaro. The elapsed times compare the same departure and reunion events; they cannot be obtained by applying one time-dilation factor to the whole journey, whose [worldline](../../../../../world-line.md) has three different velocities.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
