# Paper 310

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_310.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_310.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
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

The [cosmological continuity equation](../../../cosmology.md#cosmological-continuity-equation) and $P_i=w_i\rho_i$ give

$$
\frac{d\rho_i}{da}+\frac{3(1+w_i)}a\rho_i=0,
\qquad
\rho_i(a)=\rho_{i,0}a^{-3(1+w_i)}.
$$

With $a_0=1$, $1+z=a^{-1}$ and

$$
\Omega_{i,0}=\frac{\rho_{i,0}}{\rho_{\rm crit,0}},
\qquad
\rho_{\rm crit,0}=\frac{3H_0^2}{8\pi G},
$$

the [Friedmann equation](../../../cosmology.md#friedmann-equations) becomes

$$
H(z)=H_0E(z),
\qquad
E(z)=\left[\sum_i\Omega_{i,0}(1+z)^{3(1+w_i)}\right]^{1/2}.
$$

Spatial curvature may be included as an effective component with $w=-1/3$ and $\Omega_{k,0}=-k/H_0^2$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Given the component parameters, solve the first-order equation

$$
\dot a=aH_0E(a^{-1}-1),
\qquad
t-t_i=\int_{a_i}^a\frac{d\widetilde a}{\widetilde aH(\widetilde a)}.
$$

A [cosmic string network](../../../cosmology.md#cosmic-string-network) has $w=-1/3$, so $\rho\propto a^{-2}$ and $H\propto a^{-1}$. Therefore $\dot a$ is constant and a string-dominated expanding universe has

$$
\boxed{a(t)\propto t}
$$

after choosing the Big Bang as $t=0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For pressureless matter, $\rho_ma^3=\rho_{m,0}$ when $a_0=1$. Set

$$
D=\frac{8\pi G\rho_{m,0}}3;
$$

then $\dot a^2=D/a-k$. Substitution of $a=A(1-\cos\theta)$ makes this identity hold when

$$
\boxed{A=\frac{D}{2k}=\frac{4\pi G\rho_{m,0}}{3k}},
\qquad
\boxed{B=\frac{A}{\sqrt k}=\frac{D}{2k^{3/2}}}.
$$

Indeed $dt/d\theta=B(1-\cos\theta)=Ba/A$, and hence

$$
t=B(\theta-\sin\theta)
$$

after setting $t=0$ at $\theta=0$. This is the [closed matter-dominated Friedmann solution](../../../cosmology.md#closed-matter-dominated-friedmann-solution).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The small-$\theta$ expansions are

$$
a=\frac A2\theta^2\left(1-\frac{\theta^2}{12}+\cdots\right),
\qquad
t=\frac B6\theta^3\left(1-\frac{\theta^2}{20}+\cdots\right).
$$

Writing $x=(6t/B)^{1/3}$ and reverting the second series gives $\theta=x(1+x^2/60+\cdots)$. Therefore

$$
\frac a{t^{2/3}}
=\boxed{\frac A2\left(\frac6B\right)^{2/3}}
\left[1-\frac1{20}\left(\frac{6t}{B}\right)^{2/3}+\cdots\right],
$$

so $C=(A/2)(6/B)^{2/3}$. The leading $a\propto t^{2/3}$ is the flat matter-dominated limit.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

During recollapse $H<0$, so nearby comoving galaxies are increasingly blueshifted rather than redshifted. Their physical separations and angular-diameter distances shrink, making them appear larger and generally brighter; in a closed geometry sufficiently old light can also produce repeated or strongly focused images.

The [cosmic microwave background](../../../cosmic-microwave-background-anisotropy.md) temperature obeys $T_\gamma\propto a^{-1}$. It therefore rises without bound as $\theta\to2\pi$, and its photons are blueshifted. Before the formal [Big Crunch](../../../cosmology.md#big-crunch), the growing temperature reionizes matter, scattering makes the universe opaque, and the idealization that old galaxies and the original last-scattering surface remain directly visible eventually fails.

## 2

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Chemical equilibrium for $e^-+p\leftrightarrow H+\gamma$ gives $\mu_e+\mu_p=\mu_H$, since $\mu_\gamma=0$. Insert the supplied nonrelativistic equilibrium densities. Neglecting $m_e/m_p$ in the translational reduced mass and using the stated degeneracy convention gives

$$
\frac{n_H}{n_en_p}
=\left(\frac{2\pi}{m_eT}\right)^{3/2}
e^{(m_e+m_p-m_H)/T}.
$$

Charge neutrality gives $n_p=n_e$, so

$$
\boxed{\frac{n_H}{n_e^2}=\left(\frac{2\pi}{m_eT}\right)^{3/2}e^{B_H/T}}.
$$

This is the hydrogen [Saha ionization equation](../../../cosmology.md#saha-ionization-equation).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Since $n_e=n_p=X_en_b$ and $n_H=(1-X_e)n_b$,

$$
\frac{1-X_e}{X_e^2}=n_b\frac{n_H}{n_e^2}.
$$

Using $n_b=\eta n_\gamma$ and $n_\gamma=2\zeta(3)T^3/\pi^2$ yields

$$
\boxed{
\frac{1-X_e}{X_e^2}
=\frac{2\zeta(3)}{\pi^2}\eta
\left(\frac{2\pi T}{m_e}\right)^{3/2}e^{B_H/T}}.
$$

[Cosmological recombination](../../../cosmology.md#recombination-cosmology) occurs far below $B_H$ because the [baryon-to-photon ratio](../../../cosmology.md#baryon-to-photon-ratio) is only about $10^{-9}$. There are roughly a billion photons per baryon, so the high-energy tail of the blackbody distribution continues to photoionize hydrogen until the exponential Boltzmann factor overcomes this enormous entropy factor.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Neglecting baryon loading, the [Sachs-Wolfe combination](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-combination) obeys a harmonic-oscillator equation with sound speed $1/\sqrt3$. [Adiabatic initial conditions](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) give a nonzero initial displacement and negligible initial velocity, hence

$$
S(k,\tau_*)=S(k,0)\cos(kr_s),
\qquad
r_s=\int_0^{\tau_*}c_s,d\tau.
$$

Projection maps $k$ approximately to $\ell/\chi_*$, and the angular power is quadratic in the transfer function, producing the observed approximate $\cos^2(kr_s)$ sequence of [acoustic peaks](../../../cosmic-microwave-background-anisotropy.md#cosmic-microwave-background-acoustic-peak). A $\sin^2$ phase would instead indicate vanishing initial displacement and nonzero initial velocity, characteristic of an isocurvature rather than adiabatic primordial mode.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Multiplying every pre-recombination density by $\lambda$ changes $H$ by $\sqrt\lambda$ and therefore shrinks the [sound horizon](../../../cosmic-microwave-background-anisotropy.md#sound-horizon) at fixed recombination epoch by $\lambda^{-1/2}$. Changing $B_H$ shifts the recombination temperature approximately as $T_{\rm rec}\propto B_H$, so $a_*\propto\mu^{-1}$. Delaying recombination with $\mu<1$ can compensate the faster expansion; schematically the acoustic scale can be retained by choosing $\mu\sqrt\lambda\simeq1$.

This can preserve the peak positions approximately because post-recombination distances are unchanged. It cannot make the entire spectrum exactly identical: the photon-diffusion scale, visibility-function width, early integrated Sachs-Wolfe effect and relative peak heights scale differently. Thus a tuned pair $(\lambda,\mu)$ creates an approximate degeneracy, with residual observables breaking it.

## 3

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

During matter domination, $a\propto t^{2/3}$, $H=2/(3t)$ and $4\pi G\bar\rho_m=2/(3t^2)$. Trying $\delta_m=t^p$ gives

$$
p(p-1)+\frac43p-\frac23=0,
$$

with roots $p=2/3,-1$. The growing [linear cosmological density perturbation](../../../linear-cosmological-density-perturbation.md) is therefore

$$
\boxed{\delta_m\propto t^{2/3}\propto a}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

After all species are nonrelativistic, each background density scales as $a^{-3}$, so

$$
f_\nu=\frac{\bar\rho_\nu}{\bar\rho_m}
=\frac{\Omega_{\nu,0}}{\Omega_{m,0}}
$$

is constant. Since $\delta\rho_i=\bar\rho_i\delta_i$,

$$
\boxed{\delta_m=(1-f_\nu)\delta_{cb}+f_\nu\delta_\nu}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

[Neutrino free streaming](../../../linear-cosmological-density-perturbation.md#neutrino-free-streaming) gives $\delta_\nu\simeq0$ on the stated scales, so $\delta_m=(1-f_\nu)\delta_{cb}$. With derivatives with respect to $N=\log a$, the growth equation becomes

$$
\delta_{cb,NN}+\frac12\delta_{cb,N}
-\frac32(1-f_\nu)\delta_{cb}=0.
$$

For $\delta_{cb}\propto a^p$,

$$
p=\frac{-1+\sqrt{25-24f_\nu}}4
=1-\frac35f_\nu+O(f_\nu^2).
$$

Hence

$$
\boxed{X(f_\nu)=1-\frac35f_\nu}
$$

to first order.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Relative to massless-neutrino growth after $z_\nu$,

$$
\frac{\delta_{cb}}{\delta_0}
=\left(\frac{a}{a_\nu}\right)^{-3f_\nu/5}
\simeq1-\frac35f_\nu\log\frac{1+z_\nu}{1+z}.
$$

The total contrast has the additional factor $1-f_\nu$. Squaring its amplitude to obtain the [cosmological density power spectrum](../../../linear-cosmological-density-perturbation.md#matter-power-spectrum) gives

$$
\boxed{
P_{f_\nu}(k,z)\simeq
\left[1-2f_\nu-\frac65f_\nu
\log\frac{1+z_\nu}{1+z}\right]P_0(k,z)}.
$$

The two terms respectively encode the unclustered neutrino fraction and the accumulated slowing of cold-matter growth.

## 4

↑ **Parent:** [Paper 310](paper-310.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Canonical quantization imposes

$$
[a_{\mathbf k},a_{\mathbf k'}^\dagger]=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k'),
\qquad [a_{\mathbf k},a_{\mathbf k'}]=[a_{\mathbf k}^\dagger,a_{\mathbf k'}^\dagger]=0.
$$

The [two-point correlation function](../../../critical-phenomenon.md#correlation-function) has mode power $P_{\delta\phi}=|f_k|^2/a^2$. After [cosmological horizon exit](../../../cosmic-inflation.md#cosmological-horizon-exit), $|k\tau|\ll1$, so

$$
|f_k|^2\simeq\frac1{2k^3\tau^2},
\qquad a^2=\frac1{H^2\tau^2}.
$$

Therefore

$$
\Delta_{\delta\phi}^2=\frac{k^3}{2\pi^2}P_{\delta\phi}
=\boxed{\left(\frac H{2\pi}\right)^2}.
$$

This is the [scale-invariant inflationary power spectrum](../../../cosmic-inflation.md#scale-invariant-inflationary-power-spectrum) of a light canonical scalar.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Linearizing the [curvaton](../../../cosmic-inflation.md#curvaton) equation and Fourier transforming gives

$$
\delta\sigma_k''+2\frac{a'}a\delta\sigma_k'
+(k^2+a^2m_\sigma^2)\delta\sigma_k=0.
$$

Writing $f_k^\sigma=a\delta\sigma_k$ yields

$$
(f_k^\sigma)''+\left(k^2+a^2m_\sigma^2-\frac{a''}{a}\right)f_k^\sigma=0.
$$

Since $m_\sigma\ll H$, the mass term is negligible and this is the equation stated. It has the same Bunch-Davies mode as the inflaton perturbation, so after horizon exit

$$
\boxed{\Delta_{\delta\sigma}^2(k)=\left(\frac H{2\pi}\right)^2}
$$

up to a small mass-induced spectral tilt.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

When $H\ll m_\sigma$ over an oscillation, the background equation reduces to

$$
\ddot{\bar\sigma}+m_\sigma^2\bar\sigma=0,
\qquad
\bar\sigma=\Sigma\cos(m_\sigma t+\varphi).
$$

Time averaging gives $\langle\dot{\bar\sigma}^2\rangle=m_\sigma^2\langle\bar\sigma^2\rangle$, hence

$$
\langle P_\sigma\rangle=0,
\qquad
\langle\rho_\sigma\rangle=\frac12m_\sigma^2\Sigma^2.
$$

The oscillating quadratic scalar is therefore [pressureless matter](../../../cosmology.md#pressureless-matter). Its continuity equation gives

$$
\boxed{\rho_\sigma\propto a^{-3}},
$$

with the slowly varying amplitude obeying $\Sigma\propto a^{-3/2}$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

After reheating, inflaton decay products are radiation with $\rho_\gamma\propto a^{-4}$, whereas the oscillating curvaton has $\rho_\sigma\propto a^{-3}$. Its fractional density therefore grows, so only the curvaton can become dynamically important at late times.

The [curvaton mechanism](../../../cosmic-inflation.md#curvaton-mechanism) can generate the observed primordial curvature perturbation even though the inflaton drives inflation. A viable pure-curvaton realization requires the field to be light during inflation, to become sufficiently important before decay, to decay into the visible sector before nucleosynthesis, and to avoid excessive residual isocurvature and primordial non-Gaussianity. If it dominates before complete decay, these conditions can be compatible with observations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
