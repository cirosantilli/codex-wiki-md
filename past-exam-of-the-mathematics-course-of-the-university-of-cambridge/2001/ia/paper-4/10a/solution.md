<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

Let $m=4\pi\rho a^3/3$ be the drop's [mass](../../../../../mass.md), with constant [mass density](../../../../../density.md) $\rho$. Its volume-growth rule gives $4\pi a^2\dot a=c\pi a^2v$, hence $\dot a=cv/4$ and $\dot m=\rho c\pi a^2v$. The incoming mist is stationary, so the [variable-mass system](../../../../../variable-mass-system.md) momentum balance is

$$
\frac d{dt}(mv)=mg-k\rho\pi a^2v^2.
$$

Expanding the [derivative](../../../../../derivative.md) and substituting the accretion rate gives the [accreting raindrop with quadratic drag](../../../../../accreting-raindrop-with-quadratic-drag.md) equations

$$
\boxed{\dot a=\frac c4v,\qquad
\dot v=g-\frac34(c+k)\frac{v^2}a.}
$$

The extra $c$ contribution is the [momentum](../../../../../momentum.md) needed to accelerate collected matter from rest; omitting it would treat the growing drop as a constant-mass particle.

Set $q=v^2/a$ and $B=7c/8+3k/4$. The [chain rule](../../../../../chain-rule.md) gives

$$
\begin{aligned}
\dot q
&=\frac{2v\dot v}a-\frac{v^2\dot a}{a^2}\\
&=\frac va\left[2g-\left(\frac74c+\frac32k\right)q\right]
=\boxed{\frac{2v}a(g-Bq)}.
\end{aligned}
$$

To justify the limiting value as well as its stability sign, use $c>0$, as appropriate to volume growth. Divide by $\dot a=cv/4$ and integrate the resulting first-order equation:

$$
\boxed{q(a)=\frac gB+\left(q(a_0)-\frac gB\right)
\left(\frac{a_0}a\right)^{7+6k/c}.}
$$

Thus $q$ remains between two positive constants, its initial value and $g/B$. Since $d\sqrt a/dt=c\sqrt q/8$, the radius is defined for all increasing time and tends to infinity. The correction vanishes, proving the [speed-radius attractor of an accreting raindrop](../../../../../speed-radius-attractor-of-an-accreting-raindrop.md):

$$
\boxed{\frac{v^2}a\longrightarrow\frac g{7c/8+3k/4},\qquad
\dot v\longrightarrow g-\frac{3(c+k)}4\frac gB
=\frac{cg}{7c+6k}<\frac g7.}
$$

The strict inequality uses $k>0$. The growing radius prevents a finite terminal [velocity](../../../../../velocity.md); instead the [acceleration](../../../../../acceleration.md) approaches this positive constant.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
