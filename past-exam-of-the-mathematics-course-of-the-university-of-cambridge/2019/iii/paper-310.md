# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_310.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
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
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [perfect fluid in general relativity](../../../general-relativity.md#perfect-fluid-in-general-relativity) has [stress-energy tensor](../../../general-relativity.md#stress-energy-tensor)

$$
\boxed{T_{\mu\nu}=(\rho+P)u_\mu u_\nu+Pg_{\mu\nu}},
$$

where $u^\mu u_\mu=-1$. Besides the [metric tensor](../../../general-relativity.md#metric-tensor), one needs the [energy density](../../../statistical-physics.md#energy-density) $\rho$, the [pressure](../../../thermodynamics.md#pressure) $P$, and three independent components of the normalized [four-velocity](../../../special-relativity.md#four-velocity) $u^\mu$: **five scalar functions of spacetime in total**.

The four equations of [stress-energy conservation](../../../general-relativity.md#stress-energy-conservation), $\nabla_\mu T^{\mu\nu}=0$, split parallel and perpendicular to $u^\mu$ into

$$
\boxed{u^\mu\nabla_\mu\rho+(\rho+P)\nabla_\mu u^\mu=0},
$$



$$
\boxed{(\rho+P)u^\mu\nabla_\mu u^\alpha
+(g^{\alpha\mu}+u^\alpha u^\mu)\nabla_\mu P=0}.
$$

An [equation of state](../../../thermodynamics.md#equation-of-state), such as a [barotropic equation of state](../../../cosmology.md#barotropic-equation-of-state) $P=P(\rho)$, supplies the fifth relation needed to close the evolution.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In [cosmic time](../../../cosmology.md#cosmic-time), all three [Friedmann-Lemaître-Robertson-Walker metrics](../../../cosmology.md#friedmann-lemaitre-robertson-walker-metric) can be written

$$
ds^2=-dt^2+a^2(t)\left[d\chi^2+S_K^2(\chi)d\Omega_2^2\right],
$$

where

$$
S_K(\chi)=
\begin{cases}
\sin\chi,&K=+1\quad\hbox{closed},\\
\chi,&K=0\quad\hbox{flat},\\
\sinh\chi,&K=-1\quad\hbox{open}.
\end{cases}
$$

The closed spatial slice is a [three-sphere](../../../geometry-and-topology.md#three-sphere) of radius $a(t)$, so

$$
\boxed{V_{K=+1}=2\pi^2a^3}.
$$

The complete flat and open spatial slices are noncompact and have

$$
\boxed{V_{K=0}=V_{K=-1}=\infty}.
$$

For a homogeneous fluid in the [Spatially flat FLRW metric](../../../cosmology.md#spatially-flat-flrw-metric), the equations in part (a) reduce to the [cosmological perfect-fluid continuity equation](../../../cosmology.md#cosmological-perfect-fluid-continuity-equation)

$$
\boxed{\dot\rho+3H(\rho+P)=0},
$$

while homogeneity makes the spatial [relativistic Euler equation](../../../general-relativity.md#relativistic-euler-equation) automatic. The [Einstein field equations](../../../general-relativity.md#einstein-field-equations) give the flat [Friedmann equation](../../../cosmology.md#friedmann-equations) and [Friedmann acceleration equation](../../../cosmology.md#friedmann-acceleration-equation),

$$
\boxed{H^2=\frac{8\pi G}{3}\rho,
\qquad
\dot H=-4\pi G(\rho+P)},
$$

equivalently $\ddot a/a=-4\pi G(\rho+3P)/3$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Normalize the present [scale factor](../../../cosmology.md#scale-factor-cosmology) to $a(t_0)=1$. In a flat universe containing [radiation in cosmology](../../../cosmology.md#radiation-in-cosmology), [pressureless matter](../../../cosmology.md#pressureless-matter), and a [cosmological constant](../../../cosmology.md#cosmological-constant), the [Friedmann equation](../../../cosmology.md#friedmann-equations) is

$$
H(a)=H_0\sqrt{\Omega_{r,0}a^{-4}+\Omega_{m,0}a^{-3}+\Omega_{\Lambda,0}},
$$

where $\Omega_{r,0}+\Omega_{m,0}+\Omega_{\Lambda,0}=1$. Since $dt=da/(aH)$, the [age of an FLRW universe](../../../cosmology.md#age-of-an-flrw-universe) is

$$
\boxed{t_0=\frac1{H_0}\int_0^1
\frac{da}{a\sqrt{\Omega_{r,0}a^{-4}+\Omega_{m,0}a^{-3}+\Omega_{\Lambda,0}}}}.
$$

For a matter-only flat [Einstein-de Sitter universe](../../../large-scale-structure-of-the-universe.md#einstein-de-sitter-universe),

$$
\boxed{t_0=\frac{2}{3H_0}}.
$$

Taking the present value $H_0\simeq70\ {\rm km\,s^{-1}\,Mpc^{-1}}$, for which the [Hubble time](../../../cosmology.md#hubble-time) is $H_0^{-1}\simeq14.0\ {\rm Gyr}$, gives

$$
\boxed{t_0\simeq9.3\ {\rm Gyr}}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The identity

$$
\frac{\ddot a}{a}=H^2+\dot H=H^2(1-\epsilon)
$$

shows that [accelerating expansion](../../../cosmology.md#accelerating-expansion-of-the-universe) has $H>0$ and $\epsilon<1$, whereas [accelerated contraction](../../../cosmology.md#accelerated-contraction) has $H<0$, $\ddot a<0$, and $\epsilon>1$.

For the [monomial inflation potential](../../../cosmic-inflation.md#monomial-inflation-potential) $V=\lambda\phi^p$, the two [potential slow-roll parameters](../../../cosmic-inflation.md#potential-slow-roll-parameter) are

$$
\epsilon_V=\frac{p^2M_{\rm Pl}^2}{2\phi^2},
\qquad
\eta_V=\frac{p(p-1)M_{\rm Pl}^2}{\phi^2}.
$$

Thus $\epsilon_V<1$ requires $|\phi|>pM_{\rm Pl}/\sqrt2$, while $|\eta_V|<1$ requires $|\phi|>\sqrt{p|p-1|}\,M_{\rm Pl}$.

At $\phi_*$, the specified velocity gives kinetic energy

$$
\frac12\dot\phi_*^2=2\lambda\phi_*^p=2V(\phi_*).
$$

Hence $\rho_\phi=3V$, $P_\phi=V$, and the [first Hubble slow-roll parameter](../../../cosmic-inflation.md#first-hubble-slow-roll-parameter) is

$$
\boxed{\epsilon=\frac32\left(1+\frac{P_\phi}{\rho_\phi}\right)=2}.
$$

The universe is therefore **decelerating**, despite the flatness of the potential: the chosen initial kinetic energy violates the [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation).

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In natural units, an [energy density](../../../statistical-physics.md#energy-density) and a [pressure](../../../thermodynamics.md#pressure) have mass dimension four, while a [number density](../../../statistical-physics.md#number-density) and an [entropy density](../../../thermodynamics.md#entropy-density) have mass dimension three. Since $m$ and $T$ each have mass dimension one,

$$
\boxed{\alpha_1=4,
\quad \alpha_2=\frac32,
\quad \alpha_3=3,
\quad \alpha_4=3,
\quad \alpha_5=\frac32,
\quad \alpha_6=\frac32}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The reaction maintaining chemical equilibrium is

$$
\boxed{e^-+e^+\leftrightarrow\gamma+\gamma}.
$$

For $T<m_e$ and negligible [chemical potentials](../../../thermodynamics.md#chemical-potential), the [Electron](../../../physics.md#electron) and [Positron](../../../physics.md#positron) are dilute and obey the [nonrelativistic equilibrium number density](../../../statistical-physics.md#nonrelativistic-equilibrium-number-density). Including two spin states for each particle,

$$
n_{e^-}+n_{e^+}=4\left(\frac{m_eT}{2\pi}\right)^{3/2}e^{-m_e/T}.
$$

The [photon number density](../../../statistical-physics.md#photon-number-density) is $n_\gamma=2\zeta(3)T^3/\pi^2$, so the [electron-positron equilibrium pair abundance below the electron mass](../../../cosmology.md#electron-positron-equilibrium-pair-abundance-below-the-electron-mass) is

$$
\boxed{
\frac{n_{e^-}+n_{e^+}}{n_\gamma}
=\frac{2\pi^2}{\zeta(3)}
\left(\frac{m_e}{2\pi T}\right)^{3/2}e^{-m_e/T}}.
$$

If $n_e$ denotes only one of the charge-conjugate species, this expression is divided by two.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $Y_{\rm He}\simeq0.25$ be the present [primordial helium mass fraction](../../../cosmology.md#primordial-helium-mass-fraction). If $n_{\rm He}$ is the helium-nucleus density and $n_H$ the hydrogen-nucleus density, then

$$
n_b=n_H+4n_{\rm He},
\qquad
n_p=n_H+2n_{\rm He}.
$$

Since $Y_{\rm He}=4n_{\rm He}/n_b$,

$$
\boxed{\frac{n_p}{n_b}=1-\frac{Y_{\rm He}}2\simeq0.875}.
$$

This retains the correction from [neutrons](../../../physics.md#neutron) bound in helium. [Charge neutrality](../../../electromagnetism.md#charge-neutrality) requires one [Electron](../../../physics.md#electron) per proton, including bound electrons, so with the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) $\eta=n_b/n_\gamma\simeq6\times10^{-10}$,

$$
\boxed{\frac{n_e}{n_\gamma}
=\frac{n_p}{n_b}\eta
\simeq5.3\times10^{-10}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Pair equilibrium with negligible chemical potentials cannot continue once its predicted electron abundance falls below the residual abundance required by [charge neutrality](../../../electromagnetism.md#charge-neutrality). Put $x=m_e/T$ and equate part (b), to logarithmic accuracy, to the order-$10^{-10}$ result of part (c):

$$
x^{3/2}e^{-x}\sim10^{-10}.
$$

Taking a logarithm and retaining the numerical factor singled out in the hint gives

$$
x-\frac32\log x\simeq10\log10\simeq23.
$$

The solution is $x\simeq28$, so

$$
\boxed{T\simeq\frac{m_e}{28}\simeq1.8\times10^{-2}\ {\rm MeV}\simeq20\ {\rm keV}}.
$$

Thus the zero-chemical-potential electron-positron equilibrium description must fail before roughly $20\,\mathrm{keV}$; thereafter the small asymmetric electron population survives.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For each Fourier mode, the [cosmological Poisson equation](../../../linear-cosmological-perturbation-theory.md#cosmological-poisson-equation) gives

$$
-k^2\Phi=4\pi Ga^2\bar\rho_m\Delta_m.
$$

Because nonrelativistic matter has $\bar\rho_m\propto a^{-3}$, this implies $\Phi\propto\Delta_m/a$. Write $\Phi=C\Delta_m/a$ and use $\mathcal H=a'/a$. Direct differentiation in the stated potential equation gives

$$
\Delta_m''+\mathcal H\Delta_m'
+(\mathcal H'-\mathcal H^2)\Delta_m=0.
$$

The supplied [Friedmann equation](../../../cosmology.md#friedmann-equations) identity therefore yields

$$
\Delta_m''+\mathcal H\Delta_m'
-4\pi Ga^2\bar\rho_m\Delta_m=0.
$$

Since $d/d\tau=a\,d/dt$, this becomes the [linear growth equation](../../../linear-cosmological-density-perturbation.md#linear-growth-equation)

$$
\boxed{\ddot\Delta_m+2H\dot\Delta_m
-4\pi G\bar\rho_m\Delta_m=0}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

During [matter domination](../../../linear-cosmological-density-perturbation.md#matter-domination), $a\propto t^{2/3}$, $H=2/(3t)$, and $4\pi G\bar\rho_m=2/(3t^2)$. Substituting $\Delta_m\propto t^s$ into the [linear growth equation](../../../linear-cosmological-density-perturbation.md#linear-growth-equation) gives

$$
s(s-1)+\frac43s-\frac23=0,
$$

whose roots are $s=2/3$ and $s=-1$. Therefore

$$
\Delta_m=C_+t^{2/3}+C_-t^{-1}
=C_+a+C_-a^{-3/2}.
$$

The growing one of the [matter-dominated density-perturbation modes](../../../linear-cosmological-density-perturbation.md#matter-dominated-density-perturbation-modes) is

$$
\boxed{\Delta_m\propto a}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Increasing the [dark energy](../../../cosmology.md#dark-energy) density makes dark-energy domination begin earlier. The larger [Hubble parameter](../../../cosmology.md#hubble-parameter) strengthens the $2H\dot\Delta_m$ friction term while the clustering source $4\pi G\bar\rho_m\Delta_m$ continues to dilute, so less [large-scale structure of the universe](../../../large-scale-structure-of-the-universe.md) can grow from a fixed primordial amplitude.

Deep in cosmological-constant domination, $H\simeq H_\Lambda$ is constant and $\bar\rho_m$ is negligible. The growth equation reduces to

$$
\ddot\Delta_m+2H_\Lambda\dot\Delta_m=0,
$$

and hence

$$
\boxed{\Delta_m=C_1+C_2e^{-2H_\Lambda t}
=C_1+C_2a^{-2}}.
$$

The surviving mode is constant: **matter growth freezes**.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The background remains matter dominated, so $H=2/(3t)$ and $4\pi G\bar\rho_m=2/(3t^2)$. For the [reduced gravitational clustering strength](../../../linear-cosmological-density-perturbation.md#reduced-gravitational-clustering-strength), substitute $\Delta_m\propto t^s$ into the modified equation:

$$
s(s-1)+\frac43s-\frac23(1-f)=0.
$$

The growing root is the [matter-era growth with reduced gravitational clustering strength](../../../linear-cosmological-density-perturbation.md#matter-era-growth-with-reduced-gravitational-clustering-strength)

$$
\boxed{s(f)=\frac{-1+\sqrt{25-24f}}6}.
$$

It satisfies $0<s(f)<2/3$ for $0<f<1$. Between $t_f$ and the onset $t_\Lambda$ of dark-energy domination, standard growth supplies $(t_\Lambda/t_f)^{2/3}$ whereas the modified model supplies $(t_\Lambda/t_f)^{s(f)}$. Subsequent growth freezes in both, so

$$
\boxed{
\frac{\Delta_{m,{\rm new}}(t_0)}
{\Delta_{m,{\rm standard}}(t_0)}
\simeq
\left(\frac{t_\Lambda}{t_f}\right)^{s(f)-2/3}}.
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

A larger [cosmological constant](../../../cosmology.md#cosmological-constant) changes both the expansion history and the growth history: it alters cosmological distances, the [baryon acoustic oscillation](../../../cosmology.md#baryon-acoustic-oscillation) scale as observed in angle and redshift, and the time at which growth begins to freeze. The new interaction in part (d) leaves the background [Friedmann equation](../../../cosmology.md#friedmann-equations) unchanged but changes clustering abruptly from $t_f$ onward.

Redshift-resolved measurements of the [linear growth factor](../../../linear-cosmological-density-perturbation.md#linear-growth-factor), weak [gravitational lensing](../../../general-relativity.md#gravitational-lensing), galaxy clustering, and [cosmological distance measures](../../../cosmology.md#cosmological-distance-measure) can therefore compare geometry with growth. Equal present amplitudes do not imply equal $D(z)$, and only the higher-dark-energy model changes the distance-redshift relation. This breaks the degeneracy.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

With the symmetric Fourier normalization displayed in the question, the [creation and annihilation operators](../../../quantum-mechanics.md#creation-and-annihilation-operators) obey the [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation)

$$
\boxed{[\hat a_{\mathbf k},\hat a_{\mathbf k'}^\dagger]
=\delta^{(3)}(\mathbf k-\mathbf k')},
\qquad
[\hat a_{\mathbf k},\hat a_{\mathbf k'}]
=[\hat a_{\mathbf k}^\dagger,\hat a_{\mathbf k'}^\dagger]=0.
$$

Since $\delta\hat\phi=\hat f/a$, its vacuum [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) is

$$
\langle0|\delta\hat\phi(\tau,\mathbf x)
\delta\hat\phi(\tau,\mathbf x+\mathbf r)|0\rangle
=\int\frac{d^3k}{(2\pi)^3}
\frac{|f_k(\tau)|^2}{a^2}e^{-i\mathbf k\cdot\mathbf r}.
$$

Comparison with the definition in the question gives

$$
\Delta_{\delta\phi}^2(k,\tau)
=\frac{k^3}{2\pi^2}\frac{|f_k|^2}{a^2}.
$$

Using $|f_k|^2=(1+1/(k^2\tau^2))/(2k)$ and $a=-1/(H\tau)$,

$$
\boxed{\Delta_{\delta\phi}^2(k,\tau)
=\left(\frac H{2\pi}\right)^2(1+k^2\tau^2)}.
$$

On [superhorizon scales](../../../cosmic-inflation.md#superhorizon-scale), $k\ll aH$ or $|k\tau|\ll1$, so the [scale-invariant inflationary power spectrum](../../../cosmic-inflation.md#scale-invariant-inflationary-power-spectrum) freezes to

$$
\boxed{\Delta_{\delta\phi}^2=\left(\frac H{2\pi}\right)^2}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A perturbation $\delta\phi$ shifts the time at which the rolling inflaton reaches a fixed value by $\delta t\simeq\delta\phi/\dot\phi$. The corresponding perturbation in local expansion is $\delta N=H\delta t$, which is the [comoving curvature perturbation](../../../cosmic-inflation.md#comoving-curvature-perturbation) up to the stated sign convention:

$$
\mathcal R=\frac H{\dot\phi}\delta\phi.
$$

Therefore

$$
\Delta_{\mathcal R}^2
=\frac{H^2}{\dot\phi^2}\Delta_{\delta\phi}^2.
$$

Using $\dot\phi^2=2\epsilon H^2M_{\rm Pl}^2$ gives the [slow-roll curvature power spectrum](../../../cosmic-inflation.md#slow-roll-curvature-power-spectrum)

$$
\boxed{\Delta_{\mathcal R}^2(k)
=\frac1{2\epsilon M_{\rm Pl}^2}
\left(\frac H{2\pi}\right)^2}.
$$

For each $k$, the slowly varying quantities on the right are evaluated at [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $k=aH$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

At [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $d\log k/dN=1-\epsilon\simeq1$. Differentiating the [slow-roll curvature power spectrum](../../../cosmic-inflation.md#slow-roll-curvature-power-spectrum) and using the [Hubble slow-roll parameters](../../../cosmic-inflation.md#hubble-slow-roll-parameter) gives

$$
n_s-1=\frac{d\log\Delta_{\mathcal R}^2}{d\log k}
=-2\epsilon-\eta.
$$

The supplied relations imply

$$
\epsilon=\frac{M_{\rm Pl}^2}{2}\left(\frac{V'}V\right)^2,
\qquad
\eta=4\epsilon-2M_{\rm Pl}^2\frac{V''}V.
$$

Consequently the [scalar spectral index](../../../cosmic-inflation.md#scalar-spectral-index) is

$$
\boxed{n_s-1
=-3M_{\rm Pl}^2\left(\frac{V'}V\right)^2
+2M_{\rm Pl}^2\frac{V''}V}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For $V=\lambda\phi^4$,

$$
\epsilon_V=\frac{8M_{\rm Pl}^2}{\phi^2},
\qquad
\eta_V=\frac{12M_{\rm Pl}^2}{\phi^2}=\frac32\epsilon_V.
$$

Thus $n_s-1=-6\epsilon_V+2\eta_V=-3\epsilon_V$. Combining this with the [tensor-to-scalar ratio](../../../cosmic-inflation.md#tensor-to-scalar-ratio) $r=16\epsilon_V$ gives the [quartic-inflation tilt-tensor relation](../../../cosmic-inflation.md#quartic-inflation-tilt-tensor-relation)

$$
\boxed{n_s-1=-\frac3{16}r}.
$$

The measured tilt $n_s-1=-0.04$ would require $r\simeq0.213$, whereas $r=0.001$ predicts $n_s-1\simeq-1.88\times10^{-4}$. Therefore **quartic slow-roll inflation is inconsistent with the stated measurements**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
