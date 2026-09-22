# Paper 84

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper84.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper84.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [a](#2/iii/a)
      - [Solution](#2/iii/a/solution)
    - [b](#2/iii/b)
      - [Solution](#2/iii/b/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 84](paper-84.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Treat $\psi$ and its [complex conjugate](../../../complex-analysis.md#complex-conjugate) as independent variables in the [functional derivative](../../../calculus-of-variations.md#functional-derivative). Integrating the gradient variation by parts, with vanishing boundary terms, gives

$$
\delta E=\int\left[-\frac{\hbar^2}{2m}\nabla^2\psi
+V_0|\psi|^2\psi+W_0|\psi|^4\psi\right]\delta\psi^*\,d\mathbf x
+\text{complex conjugate}.
$$

The factors follow from $\partial_{\psi^*}|\psi|^4=2|\psi|^2\psi$ and $\partial_{\psi^*}|\psi|^6=3|\psi|^4\psi$. Thus the [cubic-quintic Gross–Pitaevskii equation](../../../statistical-physics.md#cubic-quintic-gross-pitaevskii-equation) is

$$
\boxed{i\hbar\partial_t\psi=-\frac{\hbar^2}{2m}\nabla^2\psi
+V_0|\psi|^2\psi+W_0|\psi|^4\psi}.
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

At fixed particle number $N_p=\int|\psi|^2d\mathbf x$, an equilibrium [wavefunction](../../../quantum-mechanics.md#wave-function) is a constrained critical point of the [energy functional](../../../calculus-of-variations.md#energy-functional). Introduce the [chemical potential](../../../thermodynamics.md#chemical-potential) $\mu$ as the [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) for $N_p$, and impose $\delta(E-\mu N_p)=0$. The resulting stationary [cubic-quintic Gross–Pitaevskii equation](../../../statistical-physics.md#cubic-quintic-gross-pitaevskii-equation) is

$$
\boxed{-\frac{\hbar^2}{2m}\nabla^2\psi_0
+\left(V_0|\psi_0|^2+W_0|\psi_0|^4\right)\psi_0=\mu\psi_0}.
$$

The time-dependent equilibrium has $\psi(\mathbf x,t)=e^{-i\mu t/\hbar}\psi_0(\mathbf x)$, so its [number density](../../../statistical-physics.md#number-density) is stationary even though its [quantum phase](../../../quantum-mechanics.md#quantum-phase) changes uniformly. The specified particle number fixes $\mu$ together with the boundary conditions. In an infinite uniform bulk, particle number is understood through a finite volume or a prescribed bulk density.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For a nonzero uniform [wavefunction](../../../quantum-mechanics.md#wave-function), the [Laplacian](../../../calculus.md#laplacian) vanishes. Dividing the stationary [cubic-quintic Gross–Pitaevskii equation](../../../statistical-physics.md#cubic-quintic-gross-pitaevskii-equation) by $\psi_0$ yields

$$
\boxed{\mu=V_0n_0+W_0n_0^2}.
$$

Equivalently, the interaction energy density is $e(n)=V_0n^2/2+W_0n^3/3$ and its derivative $e'(n_0)$ is the [chemical potential](../../../thermodynamics.md#chemical-potential). Positive local [compressibility](../../../thermodynamics.md#compressibility) requires $\mu'(n_0)=V_0+2W_0n_0>0$. This stability condition is distinct from the sign of $\mu$ itself.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

For the displayed scaling, assume $\mu>0$ and $n_0>0$. Set

$$
\psi_0(\mathbf x)=\sqrt{n_0}\,\widetilde\psi(\widetilde{\mathbf x}),\qquad
\mathbf x=\ell\widetilde{\mathbf x},\qquad
\boxed{\ell=\frac{\hbar}{\sqrt{2m\mu}}}.
$$

Substituting in the stationary [cubic-quintic Gross–Pitaevskii equation](../../../statistical-physics.md#cubic-quintic-gross-pitaevskii-equation) and dividing by $\mu\sqrt{n_0}$ gives

$$
\widetilde\nabla^2\widetilde\psi+
\left(1-\alpha|\widetilde\psi|^2-\beta|\widetilde\psi|^4\right)\widetilde\psi=0,
\qquad
\boxed{\alpha=\frac{V_0n_0}{\mu},\quad\beta=\frac{W_0n_0^2}{\mu}}.
$$

The uniform-state relation proves $\alpha+\beta=1$, so the real bulk amplitude is one; its constant [quantum phase](../../../quantum-mechanics.md#quantum-phase) can be chosen to make $\widetilde\psi\to1$ in the zero-winding sector. The unit of distance $\ell$ is the kinetic-to-chemical-potential scale, reducing to the stated [healing length](../../../statistical-physics.md#healing-length) convention for purely repulsive two-body coupling.

The positive-$\mu$ assumption is necessary for the printed sign convention. If $\mu<0$, the real length is $\hbar/\sqrt{2m|\mu|}$, and the dimensionless linear term is $-1$, with interaction coefficients divided by $|\mu|$; the displayed equation with linear term $+1$ does not follow. At $\mu=0$ this scaling is undefined. These are limitations of this particular nondimensionalization, not a claim that all cubic-quintic bulk states have positive [chemical potential](../../../thermodynamics.md#chemical-potential).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

A straight [quantum vortex](../../../critical-phenomenon.md#quantum-vortex) with integer [winding number](../../../complex-analysis.md#winding-number) $\mathcal N$ has $\widetilde\psi=R(r)e^{i\mathcal N\theta}$, independent of $z$. Here $r$ is measured in the unit of distance from the preceding part. The polar [Laplacian](../../../calculus.md#laplacian) supplies the centrifugal term, giving

$$
\boxed{R''+\frac{R'}r-\frac{\mathcal N^2}{r^2}R
+(1-\alpha R^2-\beta R^4)R=0}.
$$

For $\mathcal N\ne0$, regularity requires $R\sim c r^{|\mathcal N|}$ near the axis; the bulk condition is $R\to1$. The full [wavefunction](../../../quantum-mechanics.md#wave-function) tends to $e^{i\mathcal N\theta}$ rather than one. This is the [constant far-field phase excludes net vortex winding](../../../critical-phenomenon.md#constant-far-field-phase-excludes-net-vortex-winding) distinction: the equation remains applicable to a vortex, but the nonwinding boundary condition must be interpreted as an amplitude condition.

Let $F(R)=R-\alpha R^3-\beta R^5$. Since $\alpha+\beta=1$, one has $F(1)=0$ and $F'(1)=1-3\alpha-5\beta=-2(1+\beta)$. Insert $R=1-p/r^2+\cdots$. Its derivative terms start at order $r^{-4}$, while

$$
-\frac{\mathcal N^2R}{r^2}=-\frac{\mathcal N^2}{r^2}+O(r^{-4}),\qquad
F(R)=\frac{2(1+\beta)p}{r^2}+O(r^{-4}).
$$

Cancellation of the order-$r^{-2}$ terms proves the [cubic-quintic quantum vortex tail](../../../critical-phenomenon.md#cubic-quintic-quantum-vortex-tail)

$$
\boxed{R(r)=1-\frac{\mathcal N^2}{2(1+\beta)r^2}+O(r^{-3}),\qquad
p=\frac{\mathcal N^2}{2(1+\beta)}}.
$$

For a stable nondegenerate bulk state in this scaling, $1+\beta=n_0(V_0+2W_0n_0)/\mu>0$. At $\beta=-1$ the amplitude restoring derivative vanishes, and an inverse-square perturbation cannot cancel the centrifugal term, so the stated expansion fails. For zero winding the uniform solution has $p=0$.

## 2

↑ **Parent:** [Paper 84](paper-84.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

To first order, $|1+u+iv|^2=1+2u$ and $(1-|\psi|^2)\psi=-2u$. Equating real and imaginary parts of the [Gross–Pitaevskii equation](../../../statistical-physics.md#gross-pitaevskii-equation) therefore gives

$$
\boxed{2v_t=\nabla^2u-2u,\qquad -2u_t=\nabla^2v}.
$$

Differentiate the second equation in time and use the first to eliminate $v$:

$$
\boxed{u_{tt}=\frac12\nabla^2u-\frac14\nabla^4u}.
$$

For a [Fourier mode](../../../fourier-analysis.md#fourier-mode) with $k=|\mathbf k|$, the [dispersion relation](../../../wave-equation.md#dispersion-relation) is

$$
-\omega^2=-\frac{k^2}{2}-\frac{k^4}{4},\qquad
\boxed{\omega_\pm(k)=\pm\frac{k}{2}\sqrt{k^2+2}}.
$$

This is the normalized [Bogoliubov spectrum](../../../statistical-physics.md#bogoliubov-quasiparticle-dispersion). At small [wavenumber](../../../wave-equation.md#wavenumber) the positive branch has sound speed $\lim_{k\to0}\omega_+(k)/k=1/\sqrt2$; at large [wavenumber](../../../wave-equation.md#wavenumber) it approaches the free-particle quadratic dispersion. The linear frequencies are real, confirming stability of the repulsive uniform bulk.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Introduce the translating coordinate $Z=z-Ut$ and put $\psi(\mathbf x,t)=\Psi(x,y,Z)$. Then $\psi_t=-U\Psi_Z$. Substitution in the [Gross–Pitaevskii equation](../../../statistical-physics.md#gross-pitaevskii-equation) gives the stationary [Gross–Pitaevskii solitary wave](../../../statistical-physics.md#gross-pitaevskii-solitary-wave) equation

$$
\boxed{\nabla^2\Psi+(1-|\Psi|^2)\Psi-2iU\partial_Z\Psi=0}.
$$

The complex bulk field is fixed by $\Psi\to1$ far from the localized disturbance. Spatial derivatives in this equation are taken in the translating frame. There is no additional uniform temporal phase here because the normalization has already made the background $\psi=1$ stationary.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/a">a</h4>

↑ **Parent:** [Iii](#2/iii)

<h5 id="2/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/iii/a)

Use decaying variations with the same complex bulk field one, so that [integration by parts](../../../calculus.md#integration-by-parts) produces no variation boundary term. The [functional derivatives](../../../calculus-of-variations.md#functional-derivative) of energy and [renormalized momentum of a condensate](../../../statistical-physics.md#renormalized-momentum-of-a-condensate) are

$$
\frac{\delta E}{\delta\psi^*}=-\frac12\left[\nabla^2\psi+(1-|\psi|^2)\psi\right],\qquad
\frac{\delta p}{\delta\psi^*}=-i\partial_z\psi.
$$

For the second identity, variation of the two momentum terms and integration of the $\partial_z\delta\psi^*$ term each supply $(2i)^{-1}\psi_z$, so together they give $-i\psi_z$. It follows that

$$
\frac{\delta(E-Up)}{\delta\psi^*}=
-\frac12\left[\nabla^2\psi+(1-|\psi|^2)\psi\right]+iU\psi_z=0
$$

is exactly the stationary [Gross–Pitaevskii solitary wave](../../../statistical-physics.md#gross-pitaevskii-solitary-wave) equation. Thus each solitary wave is a constrained energy critical point with multiplier $U$.

Let $s$ parametrize a differentiable family of these waves. Apply the critical-point identity to the variation $\partial_s\psi$, keeping the multiplier fixed at its value for that member of the family. Including the [complex conjugate](../../../complex-analysis.md#complex-conjugate) variation gives

$$
\frac{dE}{ds}-U(s)\frac{dp}{ds}=0.
$$

Hence the [energy–momentum slope of a solitary wave](../../../statistical-physics.md#energy-momentum-slope-of-a-solitary-wave) is

$$
\boxed{\frac{dE}{dp}=U}
$$

wherever $dp/ds\ne0$. At a momentum turning point the parametrized identity $dE/ds=U\,dp/ds$ remains the correct statement; a globally single-valued energy as a function of momentum is not needed. Differentiating $E-U(s)p$ as a composite function would include an extra $-pU'$ term, so that composite derivative must not be set to zero.

<h4 id="2/iii/b">b</h4>

↑ **Parent:** [Iii](#2/iii)

<h5 id="2/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/iii/b)

Split the solitary-wave energy into longitudinal, transverse and interaction contributions,

$$
E=E_z+E_\perp+E_{\rm pot},\quad
E_z=\frac12\int|\psi_z|^2dV,\quad
E_\perp=\frac12\int(|\psi_x|^2+|\psi_y|^2)dV.
$$

Consider the longitudinal dilation $\psi_\lambda(x,y,z)=\psi(x,y,\lambda z)$ for $\lambda>0$. Changing variables to $Z=\lambda z$ gives

$$
E[\psi_\lambda]=\lambda E_z+\lambda^{-1}(E_\perp+E_{\rm pot}).
$$

The [renormalized momentum of a condensate](../../../statistical-physics.md#renormalized-momentum-of-a-condensate) is unchanged: its single $z$ derivative contributes $\lambda$, cancelling the measure factor $\lambda^{-1}$. Since the wave is a critical point of $E-Up$, differentiating this admissible scaling variation at $\lambda=1$ gives

$$
0=E_z-E_\perp-E_{\rm pot}.
$$

Therefore the [longitudinal scaling identity for a condensate solitary wave](../../../statistical-physics.md#longitudinal-scaling-identity-for-a-condensate-solitary-wave) yields

$$
\boxed{E=2E_z=\int|\partial_z\psi|^2dV}.
$$

This directional [Pohozaev identity](../../../nonlinear-analysis.md#pohozaev-identity) assumes the finite energy and sufficient decay to justify the dilation variation; it can equivalently be obtained with cutoffs followed by a limit. It is an identity for solitary-wave critical points, not for arbitrary localized fields.

## 3

↑ **Parent:** [Paper 84](paper-84.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Write $g=V_0$ for the effective coupling and keep $N$ for the number obtained by the stated two-dimensional normalization. A repulsive interaction, $g>0$, permits the [Thomas–Fermi approximation for a condensate](../../../statistical-physics.md#thomas-fermi-approximation-for-a-condensate): density-gradient [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is small compared with the trapping and interaction terms over most of the cloud. The stationary [Gross–Pitaevskii equation](../../../statistical-physics.md#gross-pitaevskii-equation) then gives

$$
\boxed{\psi(\mathbf x,t)\simeq e^{-i\mu t/\hbar}\sqrt{n_{\rm TF}(r)},\qquad
n_{\rm TF}(r)=\frac{\mu-\tfrac12m\omega^2r^2}{g}\quad(0\le r<R)}
$$

and $n_{\rm TF}=0$ outside the cloud, up to the narrow edge region. Here

$$
R^2=\frac{2\mu}{m\omega^2},\qquad n_c=\frac\mu g.
$$

Normalize the parabolic [number density](../../../statistical-physics.md#number-density) directly:

$$
N=\frac{2\pi}{g}\int_0^R\left(\mu-\frac12m\omega^2r^2\right)r\,dr
=\frac{\pi\mu^2}{gm\omega^2}=\frac{\pi n_cR^2}{2}.
$$

Consequently the [two-dimensional Thomas–Fermi condensate](../../../statistical-physics.md#two-dimensional-thomas-fermi-condensate) parameters are

$$
\boxed{\mu=\sqrt{\frac{Ngm\omega^2}{\pi}},\qquad
R=\sqrt{\frac{2\mu}{m\omega^2}},\qquad n_c=\frac\mu g}.
$$

With $a_{\rm ho}=\sqrt{\hbar/(m\omega)}$ and central [healing length](../../../statistical-physics.md#healing-length) $\xi=\hbar/\sqrt{2m\mu}$, the bulk approximation requires

$$
\boxed{\mu\gg\hbar\omega\quad\Longleftrightarrow\quad
\frac{Ngm}{\pi\hbar^2}\gg1}.
$$

Indeed $R/\xi=2\mu/(\hbar\omega)\gg1$. In the coupling convention printed in the paper, formal substitution of $g=4\pi\hbar^2a/m$ gives

$$
\boxed{\mu=2\hbar\omega\sqrt{Na},\qquad
R=2a_{\rm ho}(Na)^{1/4},\qquad Na\gg1}.
$$

This is the requested relationship in that convention; $\omega$ sets the physical size and [chemical potential](../../../thermodynamics.md#chemical-potential), while the interaction-strength ratio to $\hbar\omega$ is independent of $\omega$.

There is a dimensional convention to make explicit. A physical three-dimensional [scattering length](../../../quantum-mechanics.md#scattering-length-from-a-partial-wave-s-matrix) $a$ makes $4\pi\hbar^2a/m$ a three-dimensional contact coupling, whereas a genuinely two-dimensional particle-number normalization requires coupling units of energy times area. For an axial factor $\chi(z)$ normalized to one, the [effective two-dimensional contact coupling](../../../statistical-physics.md#effective-two-dimensional-contact-coupling) is $g_{2D}=(4\pi\hbar^2a/m)\int|\chi|^4dz$. For a Gaussian of width $a_z$ this is $4\pi\hbar^2a/(m\sqrt{2\pi}a_z)$, and the physical TF condition becomes $Na/a_z\gg1$ up to numerical constants. Alternatively the printed coupling can be retained if $N$ is a line density. The paper supplies no axial scale, so its $Na$ expressions require that effective-unit or line-density convention; the formulas in terms of $g$ above are unambiguous. The approximation fails inside vortex cores and at the cloud edge, and it is not a repulsive TF ground-state construction for $g\le0$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Use the central [number density](../../../statistical-physics.md#number-density) $n_c$, radius $R$ and central [healing length](../../../statistical-physics.md#healing-length) $\xi$ from the preceding part. The vortex energy means the excess over the no-vortex ground state at fixed particle number. Choose an intermediate matching radius $\xi\ll L\ll R$. Inside $L$, the trapped [number density](../../../statistical-physics.md#number-density) differs little from $n_c$, so the resolved uniform vortex core gives

$$
\Delta E_{\rm inner}\simeq\frac{\pi n_c\hbar^2}{m}
\left[\log\frac L\xi+L_{01}\right].
$$

Outside the core, the singly quantized [superfluid velocity](../../../statistical-physics.md#superfluid-velocity) is $u_\theta=\hbar/(mr)$. Its leading flow [kinetic energy](../../../classical-mechanics.md#kinetic-energy) in the parabolic background is therefore

$$
\begin{aligned}
\Delta E_{\rm outer}
&\simeq\frac12\int_L^R m n_{\rm TF}(r)u_\theta^2\,2\pi r\,dr\\
&=\frac{\pi n_c\hbar^2}{m}\int_L^R\left(1-\frac{r^2}{R^2}\right)\frac{dr}{r}\\
&=\frac{\pi n_c\hbar^2}{m}\left[\log\frac RL-\frac12+\frac{L^2}{2R^2}\right].
\end{aligned}
$$

Adding the regions cancels the arbitrary matching radius. Sending $L/R\to0$ while $\xi/L\to0$ gives the [matched vortex energy in a parabolic condensate](../../../critical-phenomenon.md#matched-vortex-energy-in-a-parabolic-condensate)

$$
\boxed{\Delta E_1\simeq\frac{\pi n_c\hbar^2}{m}
\left[\log\frac R\xi+L_{01}-\frac12\right]
=\frac{2N\hbar^2}{mR^2}\left[\log\frac R\xi+L_{01}-\frac12\right]}.
$$

The $-1/2$ comes from the decrease of background [number density](../../../statistical-physics.md#number-density) away from the centre. It would be missed by treating the whole trap as uniform. To this accuracy, using the unperturbed TF density in the outer region is appropriate at fixed $N$: the first variation of trapping plus interaction energy is $\mu\,\delta N$ and therefore vanishes after the small normalization adjustment. The resolved core energy supplies the finite core correction $L_{01}$, while remaining cloud-edge and density-relaxation corrections vanish in the small-core TF limit. This is an asymptotic energy estimate, not an exact formula at finite $R/\xi$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For an axisymmetric centred unit [quantum vortex](../../../critical-phenomenon.md#quantum-vortex), write $\psi=f(r)e^{i\theta}$, including its radial density depletion in $f$. The axial [angular momentum](../../../classical-mechanics.md#angular-momentum) operator is $\widehat L_z=-i\hbar\partial_\theta$, so every particle in this single-winding state has eigenvalue $\hbar$. Hence

$$
\boxed{L_z=\int\psi^*(-i\hbar\partial_\theta)\psi\,d^2x
=\hbar\int|\psi|^2d^2x=N\hbar}.
$$

This is exact at the specified particle number and does not require neglecting the core or using the parabolic TF profile.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Let $\mathcal N\in\mathbb Z$ be the vortex [winding number](../../../complex-analysis.md#winding-number), distinct from the particle number $N$. Outside its core, the [superfluid velocity](../../../statistical-physics.md#superfluid-velocity) is $u_\theta=\hbar\mathcal N/(mr)$. The outer flow energy is therefore multiplied by $\mathcal N^2$, while the resolved core contribution contains the appropriate constant $L_{0|\mathcal N|}$. The same matching integration gives

$$
\boxed{\Delta E_{\mathcal N}\simeq
\frac{\pi n_c\hbar^2}{m}\mathcal N^2
\left[\log\frac R\xi+L_{0|\mathcal N|}-\frac12\right]}.
$$

The core equation depends on $\mathcal N^2$, so reversing circulation leaves this energy unchanged. On the other hand, $-i\hbar\partial_\theta[f(r)e^{i\mathcal N\theta}]=\hbar\mathcal N f(r)e^{i\mathcal N\theta}$, giving the exact result

$$
\boxed{L_z=N\hbar\mathcal N}.
$$

Negative winding reverses [angular momentum](../../../classical-mechanics.md#angular-momentum); zero winding has zero excess vortex energy and zero angular momentum. The energy approximation applies to each fixed nonzero winding in the TF limit. More generally its core radius, of order $|\mathcal N|\xi$, must be much smaller than $R$ so that a matching interval exists. It is not valid uniformly for arbitrary growing $|\mathcal N|$ at fixed cloud size. The leading quadratic energy cost also explains why multiply quantized vortices can lower their energy by separating into singly quantized vortices; this energy comparison does not by itself establish a particular dynamical splitting rate.

## 4

↑ **Parent:** [Paper 84](paper-84.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Here equilibrium means a time-independent [number density](../../../statistical-physics.md#number-density) and current, with a common temporal [quantum phase](../../../quantum-mechanics.md#quantum-phase). Write $\psi(\mathbf x,t)=e^{-i\mu t/\hbar}\Psi(\mathbf x)$ with real $\mu$, since an imaginary temporal frequency would change the density. The stationary pumped [Gross–Pitaevskii equation](../../../statistical-physics.md#gross-pitaevskii-equation) is

$$
\boxed{\mu\Psi=-\frac{\hbar^2}{2m}\nabla^2\Psi
+V_0|\Psi|^2\Psi+i(\gamma-\Gamma|\Psi|^2)\Psi}.
$$

The [chemical potential](../../../thermodynamics.md#chemical-potential) is the common phase-rotation frequency times $\hbar$; this open system has no conserved particle-number constraint fixing it as in the conservative problem. Local gain and loss need not cancel separately in an inhomogeneous equilibrium, because a stationary [condensate number current](../../../statistical-physics.md#condensate-number-current) can transport particles between gain and loss regions.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Define the physical [velocity potential](../../../fluid-mechanics.md#velocity-potential) by $\psi=\sqrt n\exp(im\phi/\hbar)$, so the [superfluid velocity](../../../statistical-physics.md#superfluid-velocity) is $\mathbf v=\nabla\phi$. The [condensate number current](../../../statistical-physics.md#condensate-number-current) is

$$
\mathbf j=\frac\hbar m\operatorname{Im}(\psi^*\nabla\psi)=n\nabla\phi.
$$

Multiplying the pumped [Gross–Pitaevskii equation](../../../statistical-physics.md#gross-pitaevskii-equation) by $\psi^*$ and subtracting its [complex conjugate](../../../complex-analysis.md#complex-conjugate) gives the density equation. Equivalently, substituting the amplitude and phase and equating imaginary parts yields

$$
\boxed{n_t+\nabla\cdot(n\nabla\phi)=\frac2\hbar(\gamma-\Gamma n)n}.
$$

Equating real parts gives the other [gain-loss Madelung equations](../../../statistical-physics.md#gain-loss-madelung-equations) relation,

$$
\boxed{m\phi_t+\frac m2|\nabla\phi|^2+V_0n
-\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt n}{\sqrt n}=0}.
$$

The last term is the [quantum potential](../../../quantum-theory.md#quantum-potential), retained wherever $n>0$. Taking a [gradient](../../../calculus.md#gradient) gives the equivalent velocity equation

$$
 m[\mathbf v_t+(\mathbf v\cdot\nabla)\mathbf v]
=-\nabla\left(V_0n-\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt n}{\sqrt n}\right)
$$

in an irrotational region. In equilibrium $n_t=0$ and $\phi(\mathbf x,t)=\Phi(\mathbf x)-\mu t/m$, so

$$
\boxed{\nabla\cdot(n\nabla\Phi)=\frac{2n}{\hbar}(\gamma-\Gamma n)},\qquad
\mu=\frac m2|\nabla\Phi|^2+V_0n-
\frac{\hbar^2}{2m}\frac{\nabla^2\sqrt n}{\sqrt n}.
$$

This convention distinguishes the physical [velocity potential](../../../fluid-mechanics.md#velocity-potential) from the dimensionless [quantum phase](../../../quantum-mechanics.md#quantum-phase) $m\phi/\hbar$; using the latter instead would change the divergence prefactor.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

For a positive uniform [number density](../../../statistical-physics.md#number-density) $n_*$ and constant [superfluid velocity](../../../statistical-physics.md#superfluid-velocity) $v\widehat{\mathbf x}$, current divergence vanishes. The stationary density equation therefore imposes $(\gamma-\Gamma n_*)n_*=0$, giving $n_*=\gamma/\Gamma$. The [quantum potential](../../../quantum-theory.md#quantum-potential) vanishes, so the phase equation sets $\mu=mv^2/2+V_0\gamma/\Gamma$. Thus the [uniform-current pumped polariton condensate](../../../statistical-physics.md#uniform-current-pumped-polariton-condensate) is

$$
\boxed{\psi(\mathbf x,t)=\sqrt{\frac\gamma\Gamma}
\exp\left[\frac{i}{\hbar}\left(mvx-
\left(\frac{mv^2}{2}+V_0\frac\gamma\Gamma\right)t\right)\right]}.
$$

Direct substitution verifies the equation: the kinetic term gives $mv^2/2$, the interaction gives $V_0\gamma/\Gamma$, and the gain-loss term is zero. A constant overall phase is arbitrary.

With the stated $\gamma,\Gamma>0$, this nonzero plane wave exists for any real $v$ and real interaction coefficient $V_0$ when $\mu$ is determined by the solution. If a particular real [chemical potential](../../../thermodynamics.md#chemical-potential) is prescribed instead, the existence condition is

$$
\boxed{\mu\ge V_0\frac\gamma\Gamma,\qquad
v=\pm\sqrt{\frac2m\left(\mu-V_0\frac\gamma\Gamma\right)}}.
$$

Equality gives the uniform condensate at rest. A nonzero density generally requires $\gamma/\Gamma>0$; a zero nonlinear-loss coefficient with positive pumping would not allow this nonzero stationary balance. The vacuum is a separate zero solution, unstable to small perturbations for positive pump.

Existence should not be confused with stability. For completeness, linearize in the comoving frame with $\psi=\psi_*[1+u+iw]$, and let $\epsilon_k=\hbar^2k^2/(2m)$. The linear real-amplitude and phase equations give

$$
\begin{pmatrix}\dot u\\\dot w\end{pmatrix}
=\frac1\hbar\begin{pmatrix}-2\gamma&\epsilon_k\\
-(\epsilon_k+2V_0n_*)&0\end{pmatrix}
\begin{pmatrix}u\\w\end{pmatrix},
$$

so

$$
\lambda(\lambda+2\gamma/\hbar)
+\epsilon_k(\epsilon_k+2V_0n_*)/\hbar^2=0.
$$

For $V_0\ge0$ both [growth rates](../../../wave-equation.md#growth-rate) have nonpositive real parts, including the neutral uniform-phase mode. For $V_0<0$, sufficiently small nonzero $k$ makes the constant term negative, so one [growth rate](../../../wave-equation.md#growth-rate) is positive: the plane wave still exists but is unstable in an infinite system. Uniform drift adds only a Doppler phase to these [growth rates](../../../wave-equation.md#growth-rate) in this model.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Let $N=\int_S n\,dS$ be the particle number per unit axial length, and consider the axially homogeneous equilibrium implicit in a cross-sectional description. Integrating the stationary [gain-loss Madelung equations](../../../statistical-physics.md#gain-loss-madelung-equations) over $S$ and applying the [divergence theorem](../../../calculus.md#divergence-theorem) gives

$$
\oint_{\partial S}n\nabla_\perp\Phi\cdot\boldsymbol\nu\,dl
=\frac2\hbar\left(\gamma N-\Gamma\int_S n^2\,dS\right).
$$

The wall condition $n=0$ means the lateral [condensate number current](../../../statistical-physics.md#condensate-number-current) vanishes. This is also directly apparent from $\mathbf j=(\hbar/m)\operatorname{Im}(\Psi^*\nabla\Psi)$ for a regular Dirichlet wavefunction, without assigning a phase at its zeros. Consequently the [cylindrical pump-loss balance](../../../statistical-physics.md#cylindrical-pump-loss-balance) is

$$
\boxed{\int_S n^2\,dS=qN,\qquad q=\frac\gamma\Gamma}.
$$

Integrated particle creation equals integrated nonlinear loss; there is no assumption that $n=q$ pointwise. In fact the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives $N^2\le|S|\int_Sn^2=|S|qN$, so a nonzero equilibrium obeys $N\le q|S|$.

The axial condition is needed for a slice-by-slice statement. More generally, put $J(z)=\int_S n\partial_z\Phi\,dS$. Lateral no-flux and stationary density give

$$
J'(z)=\frac2\hbar\left[\gamma N(z)-\Gamma\int_S n^2\,dS\right],\qquad
\int_S n^2\,dS=\frac\gamma\Gamma N(z)-\frac\hbar{2\Gamma}J'(z).
$$

Thus the requested equality also holds whenever the integrated axial current is constant. If axially inhomogeneous equilibria with nonzero axial flux divergence are allowed, the lateral boundary condition alone proves this more general balance, rather than the stated equality at every cross-section.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
