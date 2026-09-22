<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a single barotropic [perfect fluid in general relativity](../../../../../perfect-fluid-in-general-relativity.md), the perturbations obey $\delta P=w\,\delta\rho=w\bar\rho\delta$. This adiabatic closure is needed: constant background $P/\rho$ alone would not eliminate an independent entropy perturbation. The absence of [scalar anisotropic stress](../../../../../scalar-anisotropic-stress.md) allows the common potential used in [Newtonian gauge in cosmology](../../../../../newtonian-gauge.md).

Substituting the density constraint into the pressure equation gives the [gravitational potential evolution of a barotropic fluid](../../../../../gravitational-potential-evolution-of-a-barotropic-fluid.md)

$$
\Phi''+3(1+w)\mathcal H\Phi'
+\left[2\mathcal H'+(1+3w)\mathcal H^2\right]\Phi-w\nabla^2\Phi=0.
$$

Since $a\propto\tau^{2/(1+3w)}$, the [conformal Hubble parameter](../../../../../conformal-hubble-parameter.md) is $\mathcal H=2/[(1+3w)\tau]$. The bracket cancels identically, leaving

$$
\boxed{\Phi''+\frac{6(1+w)}{1+3w}\frac{\Phi'}\tau-w\nabla^2\Phi=0}.
$$

For a [Fourier transform](../../../../../fourier-transform.md) mode, $\nabla^2$ becomes $-k^2$.

During [radiation domination](../../../../../radiation-domination.md), $w=1/3$ and $\Phi_k''+4\Phi_k'/\tau+(k^2/3)\Phi_k=0$. Set $x=k\tau/\sqrt3$ and write $\Phi=u/x$. The resulting equation is $u_{xx}+2u_x/x+(1-2/x^2)u=0$, so the two [Spherical Bessel functions](../../../../../spherical-bessel-function.md) in the hint give

$$
\boxed{\Phi_r(k,\tau)=C(k)\frac{\sin x-x\cos x}{x^3}
+D(k)\frac{\cos x+x\sin x}{x^3}}.
$$

At $x\ll1$, the two solutions approach a constant and a mode proportional to $\tau^{-3}$. The regular [adiabatic mode](../../../../../adiabatic-mode.md), normalized to its primordial potential, is

$$
\Phi_r=3\Phi_{\rm prim}(k)\frac{\sin x-x\cos x}{x^3}
=\Phi_{\rm prim}(k)\left[1-\frac{x^2}{10}+O(x^4)\right].
$$

After entry into the [sound horizon](../../../../../sound-horizon.md), $x\gg1$, the potential oscillates at [cosmological sound speed](../../../../../cosmological-sound-speed.md) $1/\sqrt3$ with envelope $x^{-2}\propto a^{-2}$. The [Hubble radius](../../../../../hubble-radius.md) and [sound horizon](../../../../../sound-horizon.md) differ by the sound-speed factor; outside the [Hubble radius](../../../../../hubble-radius.md) the regular potential is constant, while well inside it radiation supports acoustic oscillations.

During [matter domination](../../../../../matter-domination.md), $w=0$ gives $\Phi_k''+6\Phi_k'/\tau=0$ at every wavenumber. Hence

$$
\boxed{\Phi_m(k,\tau)=A(k)+B(k)\tau^{-5}=A(k)+\widetilde B(k)a^{-5/2}}.
$$

The growing density mode has a constant potential both outside and inside the [Hubble radius](../../../../../hubble-radius.md); the other potential mode decays. Pressureless matter has zero [cosmological sound speed](../../../../../cosmological-sound-speed.md), so horizon entry does not produce the radiation acoustic decay. These formulas cover both independent solutions, while the subsequent sketches select the regular adiabatic growing mode.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
