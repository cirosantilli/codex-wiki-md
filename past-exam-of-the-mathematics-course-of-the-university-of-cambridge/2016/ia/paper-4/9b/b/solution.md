<h1 id="9b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now $m$ denotes the instantaneous [rest mass](../../../../../../invariant-mass.md) of the rocket, including its fuel and stored [internal energy](../../../../../../internal-energy.md), and $v$ is measured in a fixed [inertial frame](../../../../../../inertial-frame.md). Assume the exhaust is expelled backwards with speed $0<u<c$ in the rocket's instantaneous rest frame. By the [relativistic velocity-addition formula](../../../../../../velocity-addition-formula.md), material emitted at time $\tau$ has inertial velocity

$$
w(\tau)=\frac{v(\tau)-u}{1-u v(\tau)/c^2}.
$$

It coasts at this velocity after emission.

The crucial change is that the expelled material's rest mass is not simply $-dm$: some of the rocket's [rest energy](../../../../../../rest-energy.md) becomes exhaust motion. Instead, use [conservation of relativistic energy](../../../../../../conservation-of-relativistic-energy.md). Put $q(t)=m(t)\gamma(t)$, so the rocket's energy is $c^2q(t)$. The exhaust emitted during $d\tau$ carries energy $-c^2q'(\tau)d\tau$. For material moving at velocity $w$, the [relativistic energy-momentum relation](../../../../../../energy-momentum-relation.md) gives momentum $wE/c^2$, since $E=\gamma_{\rm ex}\mu c^2$ and $p=\gamma_{\rm ex}\mu w$. Hence the modified total [momentum](../../../../../../momentum.md) is

$$
P(t)=q(t)v(t)-\int_0^t w(\tau)q'(\tau)\,d\tau.
$$

Meanwhile the total relativistic energy is $c^2[q(t)-\int_0^tq'(\tau)d\tau]=c^2q(0)$. These expressions consistently account for both [energy](../../../../../../energy.md) and [momentum](../../../../../../momentum.md) of the expelled material.

Differentiate the momentum formula. The [momentum conservation](../../../../../../momentum-conservation.md) law gives

$$
\boxed{\frac{d(m\gamma v)}{dt}
=\frac{v-u}{1-uv/c^2}\frac{d(m\gamma)}{dt}}.
$$

To simplify it, use

$$
qv'+(v-w)q'=0,\qquad
v-w=\frac{u}{\gamma^2(1-uv/c^2)},\qquad
q'=\gamma m'+m\gamma^3\frac{vv'}{c^2}.
$$

Multiplying by $\gamma^2(1-uv/c^2)$, the equation becomes

$$
m\gamma^3(1-uv/c^2)v'
+u\gamma m'+um\gamma^3vv'/c^2=0.
$$

The two terms containing $uv/c^2$ cancel. Dividing by $\gamma>0$ proves **the [relativistic rocket equation](../../../../../../relativistic-rocket-equation.md)**

$$
\boxed{m\gamma^2v'+um'=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9B](../../9b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
