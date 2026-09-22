# Paper 75

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper75.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper75.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $\rho_i=\rho_n=\rho$ and $\mu=\mu_{in}=\mu_{ni}$. Use [normal modes](../../../wave-equation.md#normal-mode) proportional to $e^{i\mathbf k\cdot\mathbf x-i\omega t}$, so $\operatorname{Im}\omega<0$ means damping. The linear [displacements](../../../classical-mechanics.md#displacement) satisfy

$$
\mathbf u_i=\partial_t\boldsymbol\xi_i=-i\omega\boldsymbol\xi_i,\qquad\mathbf u_n=\partial_t\boldsymbol\xi_n=-i\omega\boldsymbol\xi_n,\qquad\mathbf k\cdot\boldsymbol\xi_i=\mathbf k\cdot\boldsymbol\xi_n=0.
$$

For a nonzero-frequency perturbation, linearizing the [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) gives

$$
\partial_t\delta\mathbf B=B_0\partial_z\partial_t\boldsymbol\xi_i,\qquad\delta\mathbf B=B_0\partial_z\boldsymbol\xi_i=ik_\parallel B_0\boldsymbol\xi_i.
$$

Project both momentum equations with $\mathsf P=I-\mathbf k\mathbf k^T/k^2$. This removes the [pressure gradients](../../../fluid-mechanics.md#pressure-gradient). The [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension) is already transverse to $\mathbf k$, and, with $a=k_\parallel v_A$, the projected equations are

$$
\ddot{\boldsymbol\xi}_i=-a^2\boldsymbol\xi_i-\mu(\dot{\boldsymbol\xi}_i-\dot{\boldsymbol\xi}_n),\qquad\ddot{\boldsymbol\xi}_n=-\mu(\dot{\boldsymbol\xi}_n-\dot{\boldsymbol\xi}_i).
$$

Here $v_A=B_0/\sqrt{4\pi\rho}$ uses the [ion](../../../chemistry.md#ion) [density](../../../fluid-mechanics.md#density), as stipulated. For either of the two independent transverse polarizations, the [equal-density ion-neutral Alfvén dispersion relation](../../../astrophysical-fluid-dynamics.md#equal-density-ion-neutral-alfven-dispersion-relation) follows from

$$
\begin{pmatrix}\omega^2-a^2+i\mu\omega&-i\mu\omega\\-i\mu\omega&\omega^2+i\mu\omega\end{pmatrix}\begin{pmatrix}\xi_i\\\xi_n\end{pmatrix}=0.
$$

Its determinant is $\omega[\omega^3+2i\mu\omega^2-a^2\omega-i\mu a^2]$. Removing the static neutral-displacement factor gives

$$
\boxed{\omega^3+2i\mu\omega^2-a^2\omega-i\mu a^2=0.}
$$

The removed factor is a time-independent neutral [displacement](../../../classical-mechanics.md#displacement) with no [velocity](../../../classical-mechanics.md#velocity) or magnetic perturbation, a relabeling of the homogeneous neutral fluid rather than a fourth physical [wave](../../../physics.md#wave). Direct elimination in the first-order system for $(u_i,u_n,\delta B)$ gives exactly the same cubic. This also handles the zero-frequency limits without introducing a displacement-label mode.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the [strong-collision ion-neutral Alfvén modes](../../../astrophysical-fluid-dynamics.md#strong-collision-ion-neutral-alfven-modes), put $a=k_\parallel v_A$ and assume $0<|a|/\mu\ll1$. Rewrite the cubic as

$$
i\mu(2\omega^2-a^2)+\omega(\omega^2-a^2)=0.
$$

The two slow roots obey $\omega=O(a)$, so the first approximation is $\omega_0^2=a^2/2$. Set $\omega=\omega_0+\delta\omega$ and retain the next order, of size $a^3$:

$$
4i\mu\omega_0\delta\omega+\omega_0(\omega_0^2-a^2)=0,\qquad4i\mu\omega_0\delta\omega-\frac{a^2\omega_0}{2}=0.
$$

Consequently

$$
\boxed{\omega_\pm=\pm\frac{k_\parallel v_A}{\sqrt2}-i\frac{k_\parallel^2v_A^2}{8\mu}+O\left(\frac{|k_\parallel v_A|^3}{\mu^2}\right).}
$$

These are weakly damped [Alfvén waves](../../../astrophysical-fluid-dynamics.md#alfven-wave). Their [phase speed](../../../wave-equation.md#phase-speed) is $v_A/\sqrt2=B_0/\sqrt{4\pi(\rho_i+\rho_n)}$, since [collisions](../../../classical-mechanics.md#collision) make the neutral mass participate in the oscillation. Their [ambipolar damping](../../../astrophysical-fluid-dynamics.md#ambipolar-damping) rate is $\Gamma_A=a^2/(8\mu)$, with $\Gamma_A/|\operatorname{Re}\omega_\pm|\ll1$.

For the remaining root, at $a=0$ the cubic is $\omega^2(\omega+2i\mu)$, so start from $\omega_{d0}=-2i\mu$. Denote the cubic by $F(\omega,a)$. Its value and derivative at this root are

$$
F(-2i\mu,a)=i\mu a^2,\qquad \left.\partial_\omega F\right|_{a=0,\,\omega=-2i\mu}=-4\mu^2.
$$

The first correction is therefore $\delta\omega_d=ia^2/(4\mu)$, giving

$$
\boxed{\omega_d=-2i\mu+i\frac{k_\parallel^2v_A^2}{4\mu}+O\left(\frac{k_\parallel^4v_A^4}{\mu^3}\right).}
$$

This branch is purely damped. Indeed, the real growth-rate polynomial for $s=-i\omega$ is $s^3+2\mu s^2+a^2s+\mu a^2$, and its simple real root near $-2\mu$ stays real for sufficiently small real $a^2$. It represents rapid decay of ion-neutral relative motion. In the $a\to0$ limit, the other two [frequencies](../../../physics.md#frequency) tend to zero; all three branches are accounted for.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The neutral [displacement](../../../classical-mechanics.md#displacement) equation gives, for each nonzero-frequency root,

$$
-i\omega\mathbf u_n=-\mu(\mathbf u_n-\mathbf u_i),\qquad\boxed{\boldsymbol\xi_i=\left(1-\frac{i\omega}{\mu}\right)\boldsymbol\xi_n,\quad\frac{\xi_n}{\xi_i}=\frac{\mu}{\mu-i\omega}.}
$$

The [vector](../../../vector-space.md#vector) [displacements](../../../classical-mechanics.md#displacement) are parallel as complex polarization [vectors](../../../vector-space.md#vector), with this scalar amplitude and phase ratio.

For the rapidly damped root, $\mu-i\omega_d=-\mu+a^2/(4\mu)+O(a^4/\mu^3)$, and hence

$$
\boxed{\frac{\xi_n}{\xi_i}=-1-\frac{a^2}{4\mu^2}+O\left(\frac{a^4}{\mu^4}\right).}
$$

The two fluids move almost equally and oppositely; [collisions](../../../classical-mechanics.md#collision) remove the counterflow at a rate close to $2\mu$.

For either weakly damped [Alfvén wave](../../../astrophysical-fluid-dynamics.md#alfven-wave), expand the ratio around unity:

$$
\boxed{\frac{\xi_n}{\xi_i}=1\pm i\frac{a}{\sqrt2\mu}+O\left(\frac{a^2}{\mu^2}\right).}
$$

Equivalently, the exact slippage relation is $\boldsymbol\xi_i-\boldsymbol\xi_n=-(i\omega/\mu)\boldsymbol\xi_n$. Thus the relative slippage has size $|a|/(\sqrt2\mu)\ll1$ and is primarily a small phase difference. The fluids almost share a common [displacement](../../../classical-mechanics.md#displacement), but [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension) acts directly on the [ions](../../../chemistry.md#ion) and drag accelerates the neutrals. This imperfect locking causes [ambipolar damping](../../../astrophysical-fluid-dynamics.md#ambipolar-damping).

The sign of the damping is also checked by the perturbation [energy](../../../classical-mechanics.md#energy) balance. With periodic or vanishing-flux boundaries,

$$
\frac{d}{dt}\int\left[\frac\rho2(|\mathbf u_i|^2+|\mathbf u_n|^2)+\frac{|\delta\mathbf B|^2}{8\pi}\right]dV=-\rho\mu\int|\mathbf u_i-\mathbf u_n|^2dV\leq0.
$$

It follows by dotting each linear momentum equation with its [velocity](../../../classical-mechanics.md#velocity) and the induction equation with $\delta\mathbf B/(4\pi)$; magnetic-tension work cancels magnetic-energy change, [pressure](../../../thermodynamics.md#pressure) contributes only boundary flux, and the two drag terms combine into the negative square. Even though spatial diffusion was neglected, ion-neutral friction still dissipates the [wave](../../../physics.md#wave) [energy](../../../classical-mechanics.md#energy).

## 2

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

At fixed [number density](../../../statistical-physics.md#number-density) $n$, the [Electron](../../../physics.md#electron) current gives

$$
\mathbf u_e=-\frac{\mathbf J}{en}=-\alpha\nabla\times\mathbf B,\qquad\alpha=\frac{c}{4\pi en},\qquad\alpha B_0=v_Ad_i.
$$

The second equality uses [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law) without [displacement current](../../../electromagnetism.md#displacement-current) and stationary [ions](../../../chemistry.md#ion). A perturbation with characteristic perpendicular [wave number](../../../wave-equation.md#wavenumber) $k_\perp$ therefore produces $\delta u_e\sim\alpha k_\perp\delta B$. Its nonlinear magnetic-advection rate is

$$
\boxed{\tau_{\mathrm{nl}}^{-1}\sim k_\perp\delta u_e\sim v_Ad_i k_\perp^2\frac{\delta B}{B_0}.}
$$

For the anisotropic [electron magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics) [wave](../../../physics.md#wave), $k\simeq k_\perp$ and $|\omega|\sim v_Ad_i|k_\parallel|k_\perp$. Equating this to the nonlinear rate by [critical balance](../../../turbulence.md#critical-balance) gives

$$
\boxed{\frac{\delta B}{B_0}\sim\frac{|k_\parallel|}{k_\perp}\sim\epsilon\ll1.}
$$

This is small-amplitude but strong [turbulence](../../../turbulence.md): a small perturbation can have order-one nonlinear distortion over one [wave](../../../physics.md#wave) period because its perpendicular gradients are much larger than its parallel gradients.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [solenoidal magnetic-field constraint](../../../electromagnetism.md#solenoidal-magnetic-field-constraint) implies

$$
\nabla_\perp\cdot\delta\mathbf B_\perp=-\partial_z\delta B_\parallel.
$$

With $\delta B/B_0=O(\epsilon)$ and $\partial_z=O(\epsilon\nabla_\perp)$, the right-hand side is $O(\epsilon^2k_\perp B_0)$. Thus the leading, order-$\epsilon$ perpendicular field is [divergence-free](../../../calculus.md#solenoidal-vector-field). On a simply connected perpendicular patch, or for the nonzero perpendicular [Fourier modes](../../../fourier-analysis.md#fourier-mode) of a periodic domain, it has a [stream function](../../../fluid-mechanics.md#stream-function). Choose its normalization by

$$
\delta B_x=-\frac{B_0}{v_A}\partial_y\Psi,\qquad\delta B_y=\frac{B_0}{v_A}\partial_x\Psi.
$$

Consequently the leading [reduced electron magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#reduced-electron-magnetohydrodynamics) representation is

$$
\boxed{\frac{\delta\mathbf B}{B_0}=\frac1{v_A}\hat{\mathbf z}\times\nabla_\perp\Psi+\hat{\mathbf z}\frac{\delta B_\parallel}{B_0}+O(\epsilon^2).}
$$

The error denotes an order-$\epsilon^2$ field relative to $B_0$. The parallel perturbation is an independent scalar and is not removed by leading perpendicular solenoidality.

For clarity, the representation is asymptotic rather than an exact decomposition of an arbitrary three-dimensional [solenoidal](../../../calculus.md#solenoidal-vector-field) field. If $\delta B_\parallel$ depends on $z$, exact solenoidality can be restored by adding $\nabla_\perp\chi$ to $\delta\mathbf B_\perp$, where $\nabla_\perp^2\chi=-\partial_z\delta B_\parallel$. Its amplitude is $O(\epsilon^2B_0)$, so it lies beyond the retained field order. A perpendicular harmonic component can be absorbed into the guide field or fixed separately by [boundary conditions](../../../differential-equation.md#boundary-condition).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put $b=\delta B_\parallel/B_0$ and $\mathbf b_\perp=\delta\mathbf B_\perp/B_0=\hat{\mathbf z}\times\nabla_\perp\Psi/v_A$. Define the two-dimensional [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) by

$$
\{f,g\}=\partial_xf\,\partial_yg-\partial_yf\,\partial_xg.
$$

Then, to the retained anisotropic order, the derivative along the perturbed [magnetic field](../../../electromagnetism.md#magnetic-field) is

$$
\boxed{\nabla_\parallel\equiv\frac{\mathbf B}{B_0}\cdot\nabla=\partial_z+\mathbf b_\perp\cdot\nabla_\perp=\partial_z+\frac1{v_A}\{\Psi,\cdot\}.}
$$

The omitted $b\partial_z$ term is smaller by $\epsilon$ than either retained term. The nonlinear field-line-bending term is of the same order as $\partial_z$, which is why it must remain.

Use $\mathbf u_e=-\alpha\nabla\times\mathbf B$ with $\alpha B_0=v_Ad_i$. The leading parallel and perpendicular [Electron](../../../physics.md#electron) [velocities](../../../classical-mechanics.md#velocity) are

$$
\boxed{\mathbf u_{e\perp}=v_Ad_i\hat{\mathbf z}\times\nabla_\perp b,\qquad u_{e\parallel}=-d_i\nabla_\perp^2\Psi.}
$$

In detail, $\nabla\times(B_0b\hat{\mathbf z})=-B_0\hat{\mathbf z}\times\nabla_\perp b$, while the parallel [curl](../../../calculus.md#curl) of $B_0\hat{\mathbf z}\times\nabla_\perp\Psi/v_A$ is $B_0\nabla_\perp^2\Psi/v_A$. The perpendicular [curl](../../../calculus.md#curl) involving $\partial_z\delta\mathbf B_\perp$ is order-smaller. Exact [Electron](../../../physics.md#electron) [incompressibility](../../../fluid-mechanics.md#incompressible-flow) follows from the [divergence](../../../calculus.md#divergence) of a [curl](../../../calculus.md#curl); its small [velocity](../../../classical-mechanics.md#velocity) correction supplies any [divergence](../../../calculus.md#divergence) omitted by this leading representation.

The [electron magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics) equation is frozen-in induction,

$$
\partial_t\mathbf B=(\mathbf B\cdot\nabla)\mathbf u_e-(\mathbf u_e\cdot\nabla)\mathbf B,
$$

because both $\mathbf B$ and $\mathbf u_e$ are [solenoidal](../../../calculus.md#solenoidal-vector-field). Keeping its leading order-$\epsilon^2$ perpendicular terms gives

$$
\partial_t\mathbf b_\perp=\partial_z\mathbf u_{e\perp}+(\mathbf b_\perp\cdot\nabla_\perp)\mathbf u_{e\perp}-(\mathbf u_{e\perp}\cdot\nabla_\perp)\mathbf b_\perp.
$$

Let $X_f=\hat{\mathbf z}\times\nabla_\perp f=(-f_y,f_x)$. Expanding the two components gives $(X_f\cdot\nabla)X_g-(X_g\cdot\nabla)X_f=X_{\{f,g\}}$. Substitution therefore reduces the perpendicular equation to

$$
\frac1{v_A}X_{\partial_t\Psi}=v_Ad_iX_{\partial_zb}+d_iX_{\{\Psi,b\}}=v_Ad_iX_{\nabla_\parallel b}.
$$

The perpendicular-constant freedom in $\Psi$ has no magnetic effect and can be fixed so that

$$
\boxed{\partial_t\Psi=v_A^2d_i\nabla_\parallel b.}
$$

The parallel induction component at the same order is

$$
\partial_tb+\mathbf u_{e\perp}\cdot\nabla_\perp b=\nabla_\parallel u_{e\parallel}.
$$

The advection term vanishes since $\mathbf u_{e\perp}\cdot\nabla_\perp b=v_Ad_i\{b,b\}=0$. Thus

$$
\boxed{\partial_tb=-d_i\nabla_\parallel\nabla_\perp^2\Psi.}
$$

Together these are both required [reduced electron magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#reduced-electron-magnetohydrodynamics) equations. Terms such as $u_{e\parallel}\partial_zb$ and $b\partial_z\mathbf u_e$ are order-$\epsilon^3$ and consistently absent.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

[Linearization](../../../algebra.md#linearization) removes the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) from $\nabla_\parallel$. For Fourier perturbations proportional to $e^{i\mathbf k\cdot\mathbf x-i\omega t}$, the two reduced equations become

$$
-i\omega\Psi=iv_A^2d_ik_\parallel b,\qquad-i\omega b=id_ik_\parallel k_\perp^2\Psi.
$$

Eliminating either amplitude gives

$$
\boxed{\omega^2=v_A^2d_i^2k_\parallel^2k_\perp^2,\qquad\omega=\pm k_\parallel v_Ad_ik_\perp.}
$$

Since $k=(k_\perp^2+k_\parallel^2)^{1/2}=k_\perp[1+O(\epsilon^2)]$, this is the specified [dispersion relation](../../../wave-equation.md#dispersion-relation) to the accuracy of the anisotropic reduction. The reduced equations cannot retain the subleading correction replacing $k_\perp$ by the full $k$.

The full [electron magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#electron-magnetohydrodynamics) equation checks that correction directly. Its [linearization](../../../algebra.md#linearization) is $\partial_t\delta\mathbf B=-\alpha B_0\partial_z\nabla\times\delta\mathbf B$. Hence

$$
-i\omega\delta\mathbf B=\alpha B_0k_\parallel\mathbf k\times\delta\mathbf B.
$$

Applying the cross-product operator twice and using $\mathbf k\cdot\delta\mathbf B=0$ gives

$$
\boxed{\omega^2=(\alpha B_0)^2k_\parallel^2k^2=v_A^2d_i^2k_\parallel^2k^2.}
$$

Thus the full model gives the stated relation exactly and the reduced model gives its leading anisotropic limit, with all signs and normalization factors consistent.

## 3

↑ **Parent:** [Paper 75](paper-75.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the [Goldreich–Sridhar turbulence](../../../turbulence.md#goldreich-sridhar-turbulence) model in its balanced form. Assume a uniform strong guide field; anisotropic fluctuations $k_\parallel\ll k_\perp$; comparable counterpropagating [Alfvén wave](../../../astrophysical-fluid-dynamics.md#alfven-wave) amplitudes; a statistically steady [inertial range](../../../turbulence.md#inertial-range) with negligible forcing and dissipation within it; transfer mainly between comparable perpendicular scales; and a scale-independent [energy](../../../classical-mechanics.md#energy) flux per unit mass $\mathcal E$. The estimate also assumes no extra scale-dependent alignment factor in the nonlinear interaction and neglects intermittency corrections.

Let $\ell_\perp$ and $\ell_\parallel$ be an eddy's perpendicular and parallel scales, and $\delta u_\ell\sim\delta B_\ell/\sqrt{4\pi\rho_0}$ its Alfvénic [velocity](../../../classical-mechanics.md#velocity) amplitude. The nonlinear interaction is supplied by the oppositely propagating [Elsässer variable](../../../astrophysical-fluid-dynamics.md#elsasser-variable), so comparable populations give

$$
\tau_{\mathrm{nl}}\sim\frac{\ell_\perp}{\delta u_\ell}.
$$

The Alfvén propagation time is $\tau_A\sim\ell_\parallel/v_A$. For strong [turbulence](../../../turbulence.md), [critical balance](../../../turbulence.md#critical-balance) makes these times comparable; the decorrelation and cascade time is therefore of order $\tau_{\mathrm{nl}}$, not a much longer time obtained by adding many weak encounters.

A constant perpendicular [energy](../../../classical-mechanics.md#energy) flux gives

$$
\mathcal E\sim\frac{\delta u_\ell^2}{\tau_{\mathrm{nl}}}\sim\frac{\delta u_\ell^3}{\ell_\perp},\qquad\boxed{\delta u_\ell\sim(\mathcal E\ell_\perp)^{1/3}.}
$$

Define the one-dimensional perpendicular [turbulent energy spectrum](../../../turbulence.md#turbulent-energy-spectrum) so that $\int E(k_\perp)\,dk_\perp$ measures fluctuation [energy](../../../classical-mechanics.md#energy) per unit mass. Locality of the spectrum then gives

$$
\delta u_\ell^2\sim\int_{1/\ell_\perp}^{\infty}E(k_\perp)dk_\perp\sim k_\perp E(k_\perp).
$$

Hence

$$
\boxed{E(k_\perp)=C\mathcal E^{2/3}k_\perp^{-5/3},}
$$

where $C$ is a dimensionless normalization constant not determined by the scaling argument. The magnetic and kinetic spectra have the same leading scaling under the assumed Alfvénic amplitude relation.

[Critical balance](../../../turbulence.md#critical-balance) also determines the scale-dependent anisotropy:

$$
\frac{\ell_\parallel}{v_A}\sim\mathcal E^{-1/3}\ell_\perp^{2/3},\qquad\boxed{k_\parallel\sim\frac{\mathcal E^{1/3}}{v_A}k_\perp^{2/3}.}
$$

Thus the eddies become relatively more elongated along the guide field at smaller perpendicular scales. The $-5/3$ exponent follows under the listed cascade assumptions; it is not established for every imbalanced or aligned [MHD](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamics) state solely by invoking [critical balance](../../../turbulence.md#critical-balance).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

At leading anisotropic order, perpendicular [Alfvénic turbulence](../../../turbulence.md#alfvenic-turbulence) evolves independently of the compressive fluctuations. The [slow modes](../../../astrophysical-fluid-dynamics.md#slow-magnetosonic-wave) and the [entropy mode](../../../astrophysical-fluid-dynamics.md#entropy-mode) are transported by that [turbulence](../../../turbulence.md). The fast magnetosonic [frequency](../../../physics.md#frequency) is of order $k_\perp(v_A^2+c_s^2)^{1/2}$, much larger than the reduced Alfvén [frequency](../../../physics.md#frequency); the low-frequency [reduced magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#reduced-magnetohydrodynamics) ordering filters out that fast-wave sector.

The passive evolution can be made explicit for a uniform ideal adiabatic [plasma](../../../physics.md#plasma-physics). Let $c_s^2=\gamma p_0/\rho_0$, $\delta=\delta\rho/\rho_0$, $b=\delta B_\parallel/B_0$, and define the normalized [entropy](../../../thermodynamics.md#entropy) perturbation

$$
s=\frac{\delta p}{p_0}-\gamma\delta.
$$

Use $D=\partial_t+\mathbf u_\perp\cdot\nabla_\perp$ and $\nabla_\parallel=\partial_z+(\delta\mathbf B_\perp/B_0)\cdot\nabla_\perp$. Perpendicular force balance makes the leading total-pressure perturbation vanish:

$$
\delta p+\rho_0v_A^2b=0.
$$

The ideal [entropy](../../../thermodynamics.md#entropy) equation gives $Ds=0$. The leading continuity and parallel-induction equations have the same compressive [divergence](../../../calculus.md#divergence) term; subtracting them gives $D(\delta-b)=-\nabla_\parallel u_\parallel$. Parallel momentum gives $Du_\parallel=-\nabla_\parallel\delta p/\rho_0$. Put

$$
r=\delta+\frac{s}{\gamma},\qquad\delta p=\rho_0c_s^2r,\qquad b=-\frac{c_s^2}{v_A^2}r.
$$

The two compressive equations therefore become

$$
Dr=-\frac{v_A^2}{v_A^2+c_s^2}\nabla_\parallel u_\parallel,\qquad Du_\parallel=-c_s^2\nabla_\parallel r.
$$

Let $c_T=v_Ac_s/(v_A^2+c_s^2)^{1/2}$ be the [tube speed](../../../astrophysical-fluid-dynamics.md#tube-speed) and $h=c_s^2r/c_T$. Then

$$
Du_\parallel=-c_T\nabla_\parallel h,\qquad Dh=-c_T\nabla_\parallel u_\parallel.
$$

Thus the [slow and entropy fluctuations in reduced magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#slow-and-entropy-fluctuations-in-reduced-magnetohydrodynamics) have characteristic amplitudes $f^\pm=u_\parallel\pm h$ obeying

$$
\boxed{Df^\pm=\mp c_T\nabla_\parallel f^\pm,\qquad Ds=0.}
$$

The two slow-wave populations propagate in opposite directions along the bent field lines while being mixed across them by $\mathbf u_\perp$. The [entropy](../../../thermodynamics.md#entropy) perturbation is carried by the fluid without a restoring-wave [frequency](../../../physics.md#frequency). A pure [entropy](../../../thermodynamics.md#entropy) perturbation has $r=b=u_\parallel=0$ and $\delta=-s/\gamma$, so its [density](../../../fluid-mechanics.md#density) variation is accompanied by a [temperature](../../../thermodynamics.md#temperature) change with no leading [pressure](../../../thermodynamics.md#pressure) variation.

The coefficients and advecting fields in these three scalar equations come from the Alfvénic cascade; the scalars do not enter the leading perpendicular Alfvén equations. They therefore develop small perpendicular scales through passive mixing. If a scalar $f$ has constant [variance](../../../variance.md) flux $\mathcal F_f$ and is mixed on the Goldreich–Sridhar time $\tau_\ell\sim\mathcal E^{-1/3}\ell_\perp^{2/3}$, then

$$
\delta f_\ell^2\sim\mathcal F_f\tau_\ell,\qquad\boxed{E_f(k_\perp)\sim\mathcal F_f\mathcal E^{-1/3}k_\perp^{-5/3}.}
$$

The flux and amplitude need not equal the Alfvénic [energy](../../../classical-mechanics.md#energy) flux. This passive-spectrum statement uses the same locality and stationary inertial-range assumptions as part (a), and ignores additional damping. If a passive mode is absent initially and is not forced, its homogeneous leading equation keeps it absent; the Alfvénic cascade does not have to generate every compressive mode.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In the ideal, leading anisotropic system, there are **five separately conserved quadratic cascade quantities**: the two oppositely propagating Alfvén populations, the two slow-wave populations, and the [entropy](../../../thermodynamics.md#entropy) fluctuation. With the amplitudes of part (b), one convenient normalization is

$$
\boxed{I_A^\pm=\int|\mathbf z_\perp^\pm|^2dV,\qquad I_S^\pm=\int(f^\pm)^2dV,\qquad I_e=\int s^2dV,}
$$

where $\mathbf z_\perp^\pm=\mathbf u_\perp\pm\delta\mathbf B_\perp/\sqrt{4\pi\rho_0}$. Constant background factors convert the [velocity](../../../classical-mechanics.md#velocity) [variances](../../../variance.md) into modal energies and the [entropy](../../../thermodynamics.md#entropy) [variance](../../../variance.md) into an entropy-related free-energy contribution. These are the [five quadratic cascade invariants of anisotropic magnetohydrodynamic turbulence](../../../astrophysical-fluid-dynamics.md#five-quadratic-cascade-invariants-of-anisotropic-magnetohydrodynamic-turbulence).

To verify conservation rather than just count polarizations, the perpendicular [Elsässer variables](../../../astrophysical-fluid-dynamics.md#elsasser-variable) obey

$$
\partial_t\mathbf z_\perp^\pm\mp v_A\partial_z\mathbf z_\perp^\pm+(\mathbf z_\perp^\mp\cdot\nabla_\perp)\mathbf z_\perp^\pm=-\nabla_\perp\Pi,\qquad\nabla_\perp\cdot\mathbf z_\perp^\pm=0.
$$

Dot each equation with $2\mathbf z_\perp^\pm$ and integrate. The propagation and nonlinear terms become surface fluxes of $|\mathbf z_\perp^\pm|^2$, and the [pressure](../../../thermodynamics.md#pressure) term becomes a surface flux because the corresponding field is [solenoidal](../../../calculus.md#solenoidal-vector-field). For periodic boundaries, or boundaries with vanishing invariant flux, all these terms vanish and $dI_A^\pm/dt=0$. Their sum is proportional to perpendicular kinetic plus [magnetic energy](../../../electromagnetism.md#magnetic-energy), while their difference is proportional to perpendicular [cross-helicity](../../../astrophysical-fluid-dynamics.md#cross-helicity); the two [Elsässer energy invariants](../../../astrophysical-fluid-dynamics.md#elsasser-energy-invariant) contain both pieces of information.

Likewise the slow-mode equations give

$$
\frac{dI_S^\pm}{dt}=-\int\mathbf u_\perp\cdot\nabla_\perp(f^\pm)^2dV\mp c_T\int\nabla_\parallel(f^\pm)^2dV=0.
$$

Here $\mathbf u_\perp$ is [divergence-free](../../../calculus.md#solenoidal-vector-field) and $\nabla_\parallel$ differentiates along the [divergence-free](../../../calculus.md#solenoidal-vector-field) [vector](../../../vector-space.md#vector) $\hat{\mathbf z}+\delta\mathbf B_\perp/B_0$, so both integrals are boundary fluxes. Finally $Ds=0$ gives $dI_e/dt=-\int\mathbf u_\perp\cdot\nabla_\perp s^2dV=0$. This proves all five quadratic [conservation laws](../../../physics.md#conservation-law) under the same boundary assumptions.

The two Alfvén cascades interact dynamically: each population strains the other and is needed for its nonlinear transfer between scales. Their integrated invariants are nevertheless conserved separately, so this interaction does not transfer one population's invariant into the other. The slow and [entropy](../../../thermodynamics.md#entropy) cascades are driven by the Alfvénic mixing and field-line motion, with no feedback on the perpendicular cascade at the retained order. Their injection rates set independent fluxes; those fluxes need not be equal, even when the resulting perpendicular spectra share the $-5/3$ scaling.

The count is a count of independent quadratic modal cascade channels. Ideal passive advection also preserves higher moments, such as $\int F(s)dV$ for arbitrary smooth $F$, and analogous integrals for the slow characteristic scalars. These are not additional quadratic modal energies. Forcing and dissipative terms make the corresponding invariants source-and-sink balances; a stationary [inertial range](../../../turbulence.md#inertial-range) conserves their flux through scales rather than their total content in a continually forced domain.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
