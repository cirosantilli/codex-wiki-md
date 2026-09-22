<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hindered settling](../../../../../../hindered-settling.md) is the reduction of the particle [settling velocity](../../../../../../settling-velocity.md) by displaced-fluid backflow and interactions with other particles. In the specified model, the downward speed is $V_s$ at vanishing [concentration](../../../../../../concentration.md) and falls to zero at the maximum packing fraction $\phi_{\max}$. The [characteristic speed](../../../../../../characteristic-speed.md) of a [concentration](../../../../../../concentration.md) disturbance will differ from this individual-particle speed.

Take $z$ positive upwards. For a locally uniform horizontal suspension without diffusion or bulk fluid motion, the upward particle flux is

$$
j(\phi)=-\phi V(\phi)=-V_s\phi+\frac{V_s}{\phi_{\max}}\phi^2.
$$

Particle [volume conservation](../../../../../../volume-conservation.md) gives the [scalar conservation law](../../../../../../scalar-conservation-law.md)

$$
\boxed{\phi_t+\partial_zj(\phi)=0,\qquad
\phi_t+\left(-V_s+\frac{2V_s\phi}{\phi_{\max}}\right)\phi_z=0.}
$$

This is the [quadratic hindered-settling flux](../../../../../../quadratic-hindered-settling-flux.md). Along its [characteristic curves](../../../../../../characteristic-curve.md),

$$
\boxed{\frac{d\phi}{dt}=0,\qquad\frac{dz}{dt}=c(\phi)=-V_s+\frac{2V_s\phi}{\phi_{\max}}.}
$$

For a smooth initial profile $\phi_0(\zeta)$, the map is $z=\zeta+c(\phi_0(\zeta))t$. Its Jacobian is $1+(2V_s/\phi_{\max})\phi_0'(\zeta)t$. A [shock](../../../../../../shock-wave.md) develops where this first reaches zero: the compressive condition is $\phi_0'<0$, and

$$
t_s=-\frac{\phi_{\max}}{2V_s\min_\zeta\phi_0'(\zeta)}
$$

when the minimum is negative and no earlier boundary discontinuity is imposed. A discontinuous compressive initial state can instead contain a [shock](../../../../../../shock-wave.md) from $t=0$.

Let $z=s(t)$ separate states $\phi_L$ below the [shock](../../../../../../shock-wave.md) and $\phi_R$ above it. Integrating the [conservation law](../../../../../../conservation-law.md) across a moving thin interval gives the [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md)

$$
\dot s(\phi_R-\phi_L)=j(\phi_R)-j(\phi_L).
$$

Equivalently, the flux relative to the [shock](../../../../../../shock-wave.md) agrees on both sides. For this quadratic flux,

$$
\boxed{\dot s=-V_s+\frac{V_s}{\phi_{\max}}(\phi_L+\phi_R)
=\frac{c(\phi_L)+c(\phi_R)}2.}
$$

Since $j''=2V_s/\phi_{\max}>0$, a physical compression [shock](../../../../../../shock-wave.md) has $\phi_L>\phi_R$ and satisfies $c(\phi_L)>\dot s>c(\phi_R)$: [characteristic curves](../../../../../../characteristic-curve.md) enter it from both sides. These conditions select the [shock](../../../../../../shock-wave.md) over a nonphysical expansive discontinuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
