<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

In Cartesian coordinates the [magnetic field](../../../../../magnetic-field.md) is $(bx,by,-2bz)$. Its [divergence](../../../../../divergence.md) is $b+b-2b=0$, and all components of its [curl](../../../../../curl.md) vanish. Thus it satisfies the static vacuum magnetic equations $\nabla\cdot\mathbf B=0$ and $\nabla\times\mathbf B=0$, with no [electric current](../../../../../electric-current.md) in the region.

Fix clockwise orientation as viewed from above, looking down the positive $z$-axis. Its positive area normal is $-\mathbf e_z$. The loop's external [magnetic flux](../../../../../magnetic-flux.md) is therefore

$$
\boxed{\Phi_B=2\pi ba^2z=Kz,\qquad K=2\pi ba^2.}
$$

With the opposite normal its flux has the opposite sign. On the circle $\mathbf B=ba\mathbf e_r-2bz\mathbf e_z$ and clockwise line element is $d\boldsymbol\ell=-a\mathbf e_\varphi d\varphi$. The [Lorentz force](../../../../../lorentz-force.md) element is

$$
I\,d\boldsymbol\ell\times\mathbf B=Iba^2\mathbf e_z\,d\varphi+2Ibaz\mathbf e_r\,d\varphi.
$$

The radial terms cancel around the circle, so

$$
\boxed{\mathbf F_B=KI\mathbf e_z.}
$$

This fixes the current/flux/force signs together.

Neglect [self-inductance](../../../../../self-inductance.md) initially, so [Faraday's law](../../../../../faraday-s-law-of-induction.md) and [Ohm's law](../../../../../ohm-s-law.md) give $RI=-K\dot z$. Including gravity then gives

$$
\boxed{m\ddot z=-mg-\frac{K^2}{R}\dot z.}
$$

For $R>0$ and $K\ne0$, the terminal solution is $z=z_0-vt$ with

$$
\boxed{v=\frac{mgR}{K^2}=\frac{mgR}{4\pi^2b^2a^4}.}
$$

The general [velocity](../../../../../velocity.md) relaxes exponentially to $-v$ on time scale $mR/K^2$. In the terminal state $I=Kv/R$, and the Joule-heating rate is

$$
I^2R=\frac{K^2v^2}{R}=mgv=-\frac{d}{dt}(mgz).
$$

Thus all the lost [gravitational potential energy](../../../../../gravitational-energy.md) becomes resistive heat when kinetic [energy](../../../../../energy.md) is constant.

Within the zero-inductance approximation $v\to0$ as $R\to0$; finite-speed motion would require an unbounded current. This limit is singular, so it is important to describe the physical ideal-conductor limit separately. With finite [self-inductance](../../../../../self-inductance.md) $\mathcal L$, the circuit equation is $\mathcal L\dot I+RI=-K\dot z$. At $R=0$, total linked flux $\mathcal LI+Kz$ is conserved and there is no [Joule heating](../../../../../joule-heating.md). If $I=0$ initially at $z_0$, then

$$
I=-\frac K{\mathcal L}(z-z_0),\qquad
m\ddot z=-mg-\frac{K^2}{\mathcal L}(z-z_0).
$$

This [lossless limit of magnetic loop braking](../../../../../lossless-limit-of-magnetic-loop-braking.md) has undamped oscillations about $z_0-mg\mathcal L/K^2$, with magnetic [energy](../../../../../energy.md) storing and returning mechanical [energy](../../../../../energy.md). It has no generic dissipative terminal descent. Thus the vanishing terminal speed is the formal resistive-model limit, not a justification for dropping inductance in a perfectly conducting moving loop.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
