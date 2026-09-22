<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At latitude $\theta_0$, resolve the planetary angular velocity as

$$
\boldsymbol\Omega=(0,\Omega\cos\theta_0,
\Omega\sin\theta_0).
$$

For velocity $(u,v,w)$, the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) is

$$
2\boldsymbol\Omega\times\mathbf u
=2\Omega
\left(
w\cos\theta_0-v\sin\theta_0,
u\sin\theta_0,
-u\cos\theta_0
\right).
$$

The [traditional approximation](../../../../../../traditional-approximation-geophysical-fluid-dynamics.md) drops the terms involving the horizontal rotation component $\Omega\cos\theta_0$. The retained horizontal force is therefore

$$
f\widehat{\mathbf z}\times\mathbf u_h,
\qquad
f=2\Omega\sin\theta_0.
$$

Its direct velocity-scale requirement is

$$
W\cos\theta_0\ll U\sin\theta_0.
$$

For an [incompressible flow](../../../../../../incompressible-flow.md), $W/U=O(H/L)$, so a sufficient condition is

$$
\boxed{\frac HL|\cot\theta_0|\ll1},
$$

together with the small aspect ratio that makes [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) the leading vertical momentum balance. The approximation consequently becomes delicate near the equator.

The [beta plane](../../../../../../beta-plane.md) is the local [Taylor expansion](../../../../../../taylor-expansion.md)

$$
f(y)=2\Omega\sin(\theta_0+y/a)
=f_0+\beta y+O\!\left(\Omega L^2/a^2\right),
$$

where

$$
f_0=2\Omega\sin\theta_0,
\qquad
\beta=\frac{2\Omega\cos\theta_0}{a},
$$

and $a$ is the planetary radius. It requires a local Cartesian region,

$$
\boxed{L/a\ll1},
$$

and $H/a\ll1$. Away from the equator, treating the variation as a perturbation of an [f-plane](../../../../../../f-plane.md) also requires $\beta L/|f_0|\ll1$; near the equator one instead retains the linear term as the leading Coriolis parameter.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
