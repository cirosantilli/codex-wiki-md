<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

With [Lorentz factor](../../../../../lorentz-factor.md) $\gamma=(1-v^2/c^2)^{-1/2}$, the relativistic [momentum](../../../../../momentum.md) and [four-momentum](../../../../../four-momentum.md) are

$$
p=\gamma mv,
\qquad
P^\mu=(\gamma mc,\gamma mv).
$$

The Newtonian formula $a=F/m$ fails because $p$ is not $mv$: both the magnitude and direction of $v$ affect $dp/dt$. Since

$$
\dot\gamma=\frac{\gamma^3}{c^2}v\mathbin{\cdot}a,
$$

the [relativistic force](../../../../../relativistic-force.md) is

$$
F=\frac{dp}{dt}
=m\gamma\left(a+\frac{\gamma^2}{c^2}(v\mathbin{\cdot}a)v\right).
$$

Taking the dot product with $v$ gives $F\mathbin{\cdot}v=m\gamma^3v\mathbin{\cdot}a$, and substitution yields the inverse relation

$$
\boxed{a=\frac{F}{m\gamma}-\frac{(F\mathbin{\cdot}v)v}{m\gamma c^2}}.
$$

This is the requested sum of a vector parallel to $F$ and one parallel to $v$.

In the constant [electric field](../../../../../electric-field.md), $dp/dt=qE$ and the particle starts with $p(0)=0$, so $p=qEt$. The [relativistic energy-momentum relation](../../../../../energy-momentum-relation.md) implies

$$
v=\frac{c^2p}{\sqrt{m^2c^4+c^2|p|^2}}
=\boxed{\frac{qEt/m}{\sqrt{1+q^2|E|^2t^2/(m^2c^2)}}}.
$$

**Thus the speed increases monotonically but remains [subluminal](../../../../../subluminal-speed.md), and $v$ tends to $c$ in the direction of $qE$ as $t\to\infty$.**

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
