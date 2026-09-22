<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Printed [metric tensor](../../../../../../metric-tensor.md).** There is a genuine false premise. For the [metric tensor](../../../../../../metric-tensor.md) actually printed, introduce $T=\sinh t$. Since $dT=\cosh t\,dt$ and $T$ ranges over all real values,

$$
\boxed{ds^2=-dT^2+dx^2.}
$$

This is global two-dimensional [Minkowski spacetime](../../../../../../minkowski-spacetime.md), an example of how a [time-dependent lapse can disguise flat spacetime](../../../../../../time-dependent-lapse-can-disguise-flat-spacetime.md). A future-directed [timelike geodesic](../../../../../../timelike-geodesic.md) from the stated event, parametrized by [proper time](../../../../../../proper-time.md) $s$, has

$$
T=Es,\qquad x=ps,\qquad E^2-p^2=1,\quad E>0,
\qquad t=\operatorname{arsinh}(Es).
$$

For $p\ne0$ the spatial position is unbounded, not periodic; $t$ is strictly increasing. The curve $p=1$, $E=\sqrt2$ is an explicit counterexample. Physically these are inertial particles moving at constant Minkowski velocity $p/E$. The nonlinear original time coordinate does not create a confining force.

**Likely intended spatial lapse.** The hint instead fits the different [metric tensor](../../../../../../metric-tensor.md) $ds^2=-\cosh^2x\,dt^2+dx^2$, the unit-radius [two-dimensional anti-de Sitter spacetime](../../../../../../two-dimensional-anti-de-sitter-spacetime.md) in global static coordinates. This interpretation is not substituted silently for the printed one. For that [metric tensor](../../../../../../metric-tensor.md) the conserved energy is $E=\cosh^2x\,dt/ds$, and normalization gives

$$
\left(\frac{dx}{ds}\right)^2=\frac{E^2}{\cosh^2x}-1.
$$

Putting $y=\sinh x$ gives $\dot y^2+y^2=E^2-1$, hence an outgoing [geodesic](../../../../../../geodesic.md) from the origin has

$$
\boxed{\sinh x=\sqrt{E^2-1}\sin s,\qquad
\frac{dt}{ds}=\frac{E}{1+(E^2-1)\sin^2s}.}
$$

The supplied [integral](../../../../../../integral.md) shows that $t$ increases by $\pi$ over each proper-time half-period. Thus the spatial oscillation repeats after [proper time](../../../../../../proper-time.md) $2\pi$ and coordinate time $2\pi$, with turning points $|x|=\operatorname{arcosh}E$. It describes gravitationally confined inertial motion in AdS. On the [universal cover](../../../../../../universal-cover.md), $t$ is not identified and the worldline is not closed; identifying $t$ modulo $2\pi$ makes the [timelike geodesic](../../../../../../timelike-geodesic.md) closed. For $E=1$ the central particle stays at $x=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
