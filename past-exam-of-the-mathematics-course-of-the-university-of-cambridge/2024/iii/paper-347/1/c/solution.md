<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The axisymmetric razor-thin [astrophysical disk](../../../../../../astrophysical-disk.md) equations are

$$
\partial_t\Sigma+\frac1R\partial_R(R\Sigma u_R)=0,
$$



$$
\partial_tu_R+u_R\partial_Ru_R-\frac{u_\phi^2}{R}
=-\frac1\Sigma\partial_Rp-\partial_R\Phi,
$$



$$
\partial_tu_\phi+u_R\partial_Ru_\phi+\frac{u_Ru_\phi}{R}=0,
\qquad
\nabla^2\Phi=4\pi G\Sigma(R,t)\delta(z).
$$

For the stationary background, mass and azimuthal momentum conservation are automatic, while radial force balance and the [Poisson equation](../../../../../../poisson-equation.md) give

$$
R\Omega^2=\frac1{\Sigma_0}\frac{dp_0}{dR}+\frac{d\Phi_0}{dR},
\qquad
\nabla^2\Phi_0=4\pi G\Sigma_0\delta(z).
$$

Here $dp_0/dR=0$ under the stated constant-pressure assumption.

Retaining first-order perturbations and using $c_s^2=dp/d\Sigma$ gives

$$
\partial_t\Sigma'+\frac{\Sigma_0}{R}\partial_R(Ru_R')=0,
$$



$$
\partial_tu_R'-2\Omega u_\phi'
=-\frac{c_s^2}{\Sigma_0}\partial_R\Sigma'-\partial_R\Phi',
$$



$$
\partial_tu_\phi'+\frac{\kappa^2}{2\Omega}u_R'=0,
\qquad
\nabla^2\Phi'=4\pi G\Sigma'\delta(z),
$$

where

$$
\kappa^2=4\Omega^2+2R\Omega\frac{d\Omega}{dR}
$$

is the squared [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md). In the local $|k|R\gg1$ limit, a [Fourier mode](../../../../../../fourier-mode.md) $e^{i(kR-\omega t)}$ obeys

$$
-i\omega\Sigma'+ik\Sigma_0u_R'=0,
$$



$$
-i\omega u_R'-2\Omega u_\phi'
=-ik\left(c_s^2\frac{\Sigma'}{\Sigma_0}+\Phi'\right),
$$



$$
-i\omega u_\phi'+\frac{\kappa^2}{2\Omega}u_R'=0,
\qquad
\Phi'=-\frac{2\pi G\Sigma'}{|k|}.
$$

Eliminating $\Sigma'$, $u_\phi'$, and $\Phi'$ yields the local [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{
\omega^2=\kappa^2-2\pi G\Sigma_0|k|+c_s^2k^2
}.
$$

For a [Keplerian orbit](../../../../../../kepler-orbit.md), $\Omega\propto R^{-3/2}$, so

$$
\kappa^2=4\Omega^2-3\Omega^2=\Omega^2.
$$

Instability requires $\omega^2<0$, equivalently a mode with positive imaginary frequency. Treating the right-hand side as a quadratic in $x=|k|$, its two roots are

$$
x_\pm=\frac{\pi G\Sigma_0}{c_s^2}
\left(1\pm\sqrt{1-Q^2}\right),
\qquad
Q=\frac{c_s\Omega}{\pi G\Sigma_0}.
$$

Real distinct roots, and hence an unstable interval $x_-<|k|<x_+$, exist exactly when the [Toomre stability criterion](../../../../../../toomre-s-stability-criterion.md) has $Q<1$.

With $h=c_s/\Omega$,

$$
\frac{\omega^2}{\Omega^2}
=1-\frac{2h|k|}{Q}+h^2k^2.
$$

The constant positive term is epicyclic restoration by rotation and stabilizes long wavelengths. The negative term is the razor-thin disk's self-gravity and drives collapse. The positive $k^2$ term is gas-pressure restoration and stabilizes short wavelengths. Gravitational instability can therefore survive only on an intermediate band of scales.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
