<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Schechter function](../../../../../schechter-function.md) has logarithmic slope $\alpha\simeq-1$ for $M\ll M_*$ and an exponential cutoff for $M\gg M_*$. Thus a log-log plot is approximately a straight line of slope $-1$ at low mass and bends sharply downward near $M_*$.

For a collisionless self-gravitating system, define the inertia tensor

$$
I_{ij}=\int\rho x_ix_j\,dV.
$$

Two time derivatives, the collisionless Boltzmann equation, and integration by parts give the [tensor virial theorem](../../../../../tensor-virial-theorem.md)

$$
\frac12\ddot I_{ij}=2K_{ij}+W_{ij},
$$

where

$$
K_{ij}=\frac12\int\rho\langle v_iv_j\rangle\,dV,
\qquad
W_{ij}=-\int\rho x_i\partial_j\Phi\,dV.
$$

For an isolated steady state, or a long-time average of a bounded system, $\ddot I_{ij}=0$ and surface terms vanish, so

$$
\boxed{2K_{ij}+W_{ij}=0}.
$$

Taking the trace gives $2K+W=0$. Therefore

$$
\boxed{E=K+W=-K=\frac W2}.
$$

Introduce the [gravitational radius](../../../../../gravitational-radius.md) by $W=-GM^2/R$. Virial equilibrium gives

$$
\boxed{
E_I=-\frac12M_I\langle v_I^2\rangle
=-\frac{GM_I^2}{2R_I}
}.
$$

Assume dissipationless accretion, negligible escaping mass, no external work, and final re-virialization. The accreted systems bring

$$
E_A=-\frac12M_A\langle v_A^2\rangle.
$$

With $\eta=M_A/M_I$ and $\epsilon=\langle v_A^2\rangle/\langle v_I^2\rangle$,

$$
\boxed{
E_F=E_I+E_A
=-\frac12M_I\langle v_I^2\rangle(1+\epsilon\eta)
}.
$$

Since $M_F=M_I(1+\eta)$ and $E_F=-M_F\langle v_F^2\rangle/2$,

$$
\boxed{
\frac{\langle v_F^2\rangle}{\langle v_I^2\rangle}
=\frac{1+\eta\epsilon}{1+\eta}
}.
$$

Using $E=-GM^2/(2R)$ also gives

$$
\boxed{
\frac{R_F}{R_I}
=\frac{(1+\eta)^2}{1+\eta\epsilon}
}.
$$

Many [minor galaxy mergers](../../../../../minor-galaxy-merger.md) have dynamically cold accreted material, $\epsilon\ll1$. If they double the mass, $\eta=1$, then $R_F/R_I\simeq4$, and

$$
\frac{\bar\rho_F}{\bar\rho_I}
=\frac{M_F/M_I}{(R_F/R_I)^3}
=\frac2{4^3}=\frac1{32}.
$$

The steep low-mass side of the [Schechter function](../../../../../schechter-function.md) supplies many small satellites. Repeated [dry galaxy mergers](../../../../../dry-galaxy-merger.md) can therefore add stars mainly at large radius, increasing size much faster than mass and lowering [mean density](../../../../../density.md). This explains how compact, dense redshift-two galaxies can evolve into larger present-day [elliptical galaxies](../../../../../elliptical-galaxy.md) without requiring comparable in-situ [star formation](../../../../../star-formation.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
