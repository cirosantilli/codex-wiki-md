<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) has $\hat H=(\dot{\hat q}^{\,2}+\omega^2\hat q^{\,2})/2$, with $\omega>0$. Using $\hat a|0\rangle=0$ and the [canonical commutation relation](../../../../../canonical-commutation-relation.md) gives

$$
E_0\equiv\langle0|\hat H|0\rangle=\frac12\left(|\dot q|^2+\omega^2|q|^2\right).
$$

For $q=re^{is}$, the [Wronskian normalization](../../../../../wronskian-normalization.md) is

$$
q\dot q^*-\dot q q^*=-2ir^2\dot s=i,
\qquad \dot s=-\frac1{2r^2}.
$$

Consequently

$$
E_0=\frac{\dot r^2}{2}+\frac1{8r^2}+\frac{\omega^2r^2}{2}
\geq\frac\omega2.
$$

Equality requires $\dot r=0$ and $r^2=1/(2\omega)$. The [minimum-energy normalized oscillator mode](../../../../../minimum-energy-normalized-oscillator-mode.md) is therefore

$$
\boxed{q(t)=\frac{e^{-i\omega t+i\alpha}}{\sqrt{2\omega}},\quad
E_0=\frac\omega2,\quad
\langle0|\hat q^\dagger\hat q|0\rangle=|q|^2=\frac1{2\omega}}.
$$

The constant phase $\alpha$ is irrelevant. This mode also solves the oscillator [equation of motion](../../../../../equation-of-motion.md); an arbitrary squeezed mode would have larger [vacuum energy](../../../../../vacuum-energy.md).

For inflation, introduce the [Mukhanov-Sasaki variable](../../../../../mukhanov-sasaki-variable.md) $v=z\mathcal R$. Since $z$ depends only on [conformal time](../../../../../conformal-time.md),

$$
z^2(\mathcal R')^2=\left(v'-\frac{z'}zv\right)^2,
\qquad z^2(\partial_i\mathcal R)^2=(\partial_iv)^2.
$$

Integrating the cross term by parts gives the canonical bulk [action](../../../../../action.md)

$$
\boxed{S=\frac12\int d\tau\,d^3x\left[(v')^2-(\nabla v)^2+\frac{z''}zv^2\right]}
$$

up to the boundary term $-\tfrac12\int d^3x\,[(z'/z)v^2]_{\rm boundary}$. The resulting [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) and its [Fourier transform](../../../../../fourier-transform.md) are

$$
v''-\nabla^2v-\frac{z''}zv=0,\qquad
\boxed{v_k''+\left(k^2-\frac{z''}z\right)v_k=0}.
$$

At leading order in the [slow-roll approximation](../../../../../slow-roll-approximation.md), retain a small positive, nearly constant $\epsilon$ in $z=a\sqrt{2\epsilon}$, while approximating $a=-1/(H\tau)$ and $H$ as constant. Then $z''/z\simeq2/\tau^2$, so

$$
v_k''+\left(k^2-\frac2{\tau^2}\right)v_k=0.
$$

Strict exact [de Sitter spacetime](../../../../../de-sitter-spacetime.md) would have $\epsilon=0$ and would not supply the nonzero curvature kinetic coefficient assumed here; the calculation is the leading quasi-de Sitter limit, not a substitution of zero into $z$.

For $-k\tau\gg1$, the expansion correction is negligible and each canonical mode is a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) of conformal frequency $k$. The [Bunch-Davies vacuum](../../../../../bunch-davies-vacuum.md) selects its positive-frequency, minimum-energy mode $e^{-ik\tau}/\sqrt{2k}$ in that early subhorizon regime. It does not minimize an instantaneous Hamiltonian after the effective squared frequency has become negative outside the horizon.

A basis of exact solutions to the leading mode equation is $e^{-ik\tau}(1-i/(k\tau))$ and its complex conjugate. Write the normalized [Bogoliubov transformation](../../../../../bogoliubov-transformation.md) combination as

$$
v_k=\frac1{\sqrt{2k}}\left[
\alpha_k e^{-ik\tau}\left(1-\frac{i}{k\tau}\right)
+\beta_k e^{ik\tau}\left(1+\frac{i}{k\tau}\right)\right],
\qquad |\alpha_k|^2-|\beta_k|^2=1.
$$

The [Bunch-Davies vacuum](../../../../../bunch-davies-vacuum.md) boundary condition sets $\beta_k=0$ and $\alpha_k=1$ up to phase. Hence

$$
\boxed{v_k(\tau)=\frac{e^{-ik\tau}}{\sqrt{2k}}\left(1-\frac{i}{k\tau}\right)}.
$$

Substitution verifies the equation, and $v_kv_k^{*\prime}-v_k'v_k^*=i$ verifies the [Wronskian normalization](../../../../../wronskian-normalization.md).

Dividing by $z$ gives the [comoving curvature perturbation](../../../../../comoving-curvature-perturbation.md) variance

$$
|\mathcal R_k(\tau)|^2
=\frac{H^2}{4\epsilon k^3}(1+k^2\tau^2),
\qquad
\boxed{P_{\mathcal R}(k)=\frac{H^2}{4\epsilon k^3}}.
$$

This is the dimensional [slow-roll curvature power spectrum](../../../../../slow-roll-curvature-power-spectrum.md) in the printed normalization, with the [reduced Planck mass](../../../../../reduced-planck-mass.md) set to one. The corresponding [dimensionless cosmological power spectrum](../../../../../dimensionless-cosmological-power-spectrum.md) is $k^3P_{\mathcal R}/(2\pi^2)=H^2/(8\pi^2\epsilon)$, which is independent of $k$ at this order. Restoring the [reduced Planck mass](../../../../../reduced-planck-mass.md) divides both power expressions by $M_{\rm Pl}^2$. Slowly varying background quantities are evaluated near each mode's horizon exit; their variation generates the small departure from exact scale invariance.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
