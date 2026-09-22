# Paper 337

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_337.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_337.pdf)

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
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
  - [h](#2/h)
    - [Solution](#2/h/solution)

## 1

↑ **Parent:** [Paper 337](paper-337.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The conserved [number operator](../../../quantum-mechanics.md#number-operator) is

$$
N=\int d^dx\,\Psi^\dagger\Psi=\int d^dx\,\rho.
$$

Substitution of $\Psi=\sqrt\rho e^{-i\theta}$ into the [Landau-Ginzburg theory](../../../critical-phenomenon.md#landau-ginzburg-theory) gives

$$
i\Psi^\dagger\dot\Psi=\rho\dot\theta+\frac i2\dot\rho,
\qquad
|\nabla\Psi|^2=\frac{(\nabla\rho)^2}{4\rho}+\rho(\nabla\theta)^2.
$$

The imaginary term is a [total derivative](../../../calculus.md#total-derivative), so

$$
\mathcal L=\rho\dot\theta-
\frac{(\nabla\rho)^2}{8m\rho}-
\frac{\rho}{2m}(\nabla\theta)^2-r\rho-\lambda\rho^2+\cdots.
$$

Thus $\rho$ is the [number density](../../../statistical-physics.md#number-density) and is the [canonical momentum](../../../classical-mechanics.md#canonical-momentum) conjugate to $\theta$. The [canonical commutation relation](../../../quantum-mechanics.md#canonical-commutation-relation) is $[\theta(\mathbf x),\rho(\mathbf y)]=i\delta^{(d)}(\mathbf x-\mathbf y)$. Consequently, for $\theta_0=\int d^dx\,\theta$ in volume $V$,

$$
[\theta_0,N]=iV,
\qquad
\Delta\theta_0\,\Delta N\geq\frac V2.
$$

Equivalently, the averaged phase $\bar\theta=\theta_0/V$ obeys $\Delta\bar\theta\,\Delta N\geq1/2$. This [number-phase conjugacy](../../../statistical-physics.md#number-phase-conjugacy) means that a state of sharp $N$ has no sharp phase, whereas a phase-selected state exhibiting [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) must superpose different number sectors. Such sectors become effectively degenerate in the [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Stability requires $\lambda>0$. The classical potential $r\rho+\lambda\rho^2$ has a symmetry-breaking minimum when $r<0$, at

$$
\bar\rho=-\frac r{2\lambda}>0.
$$

Writing $\rho=\bar\rho+\delta\rho$ and discarding constants and [total derivatives](../../../calculus.md#total-derivative) gives the [quadratic Lagrangian](../../../quantum-field-theory.md#quadratic-lagrangian)

$$
\mathcal L_2=\delta\rho\,\dot\theta-
\frac{(\nabla\delta\rho)^2}{8m\bar\rho}-
\lambda(\delta\rho)^2-
\frac{\bar\rho}{2m}(\nabla\theta)^2.
$$

The density fluctuation is a gapped [amplitude mode](../../../quantum-field-theory.md#higgs-mode), while the phase is the prospective [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The quadratic [path integral](../../../quantum-field-theory.md#path-integral) is

$$
Z=\int\mathcal D\theta\,\mathcal D\delta\rho\,
\exp\left(i\int dt\,d^dx\,\mathcal L_2\right).
$$

Introduce the positive spatial operator

$$
A=2\lambda-\frac{\nabla^2}{4m\bar\rho}.
$$

Completing the square in the [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) over $\delta\rho$ yields

$$
\mathcal L_{\rm eff}=
\frac12\dot\theta A^{-1}\dot\theta-
\frac{\bar\rho}{2m}(\nabla\theta)^2.
$$

The [derivative expansion](../../../quantum-field-theory.md#derivative-expansion) $A^{-1}=(2\lambda)^{-1}+O(\nabla^2)$ therefore gives

$$
\mathcal L_{\rm G}=\frac1{4\lambda}
\left[\dot\theta^2-v^2(\nabla\theta)^2\right],
\qquad
v^2=\frac{2\lambda\bar\rho}{m}=-\frac rm.
$$

This is the long-wavelength [Goldstone boson](../../../critical-phenomenon.md#goldstone-boson) action. Keeping the spatial derivative in $A$ gives $\omega^2=v^2k^2+k^4/(4m^2)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For bosonic [Matsubara frequencies](../../../quantum-field-theory.md#matsubara-frequency) $\omega_n=2\pi nT$, set $a=vk/(2\pi T)$. Applying the [residue theorem](../../../analysis.md#residue-theorem) to $\pi\coth(\pi z)/(z^2+a^2)$, whose integer poles reproduce the desired summands, gives

$$
\sum_{n\in\mathbb Z}\frac1{n^2+a^2}=\frac\pi a\coth(\pi a).
$$

It follows that

$$
T\sum_n\frac1{\omega_n^2+v^2k^2}
=\frac1{2vk}\coth\left(\frac{vk}{2T}\right).
$$

Using the area $S_{d-1}=2\pi^{d/2}/\Gamma(d/2)$ of the unit sphere, the [thermal phase fluctuation](../../../statistical-physics.md#thermal-phase-fluctuation) becomes

$$
\langle\theta^2\rangle=
\frac{S_{d-1}}{2\chi v(2\pi)^d}
\int_0^\Lambda dk\,k^{d-2}
\coth\left(\frac{vk}{2T}\right).
$$

At small $k$, $\coth(vk/(2T))\sim2T/(vk)$, so the [infrared divergence](../../../quantum-field-theory.md#infrared-divergence) is governed by $\int_0 dk\,k^{d-3}$. It diverges for $d=1,2$ and is finite for $d=3$. Therefore short-range systems cannot have true finite-temperature breaking of this continuous symmetry in one or two dimensions, in agreement with the [Mermin-Wagner theorem](../../../critical-phenomenon.md#mermin-wagner-theorem), whereas it is allowed in three dimensions. In two dimensions a [Berezinskii–Kosterlitz–Thouless transition](../../../critical-phenomenon.md#berezinskii-kosterlitz-thouless-transition) may still produce quasi-long-range order.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Subtract the zero-temperature term by using $\coth(x/2)=1+2/(e^x-1)$. In three dimensions the thermal part is

$$
\langle\theta^2\rangle_T=
\frac1{\chi v}\int\frac{d^3k}{(2\pi)^3}
\frac{1}{k}\frac1{e^{vk/T}-1}
=\frac{T^2}{12\chi v^3},
$$

where the last integral uses the [Bose-Einstein distribution](../../../statistical-physics.md#bose-einstein-distribution). Gaussian phase fluctuations reduce the [order parameter](../../../critical-phenomenon.md#order-parameter) by $\langle e^{-i\theta}\rangle=e^{-\langle\theta^2\rangle/2}$. Taking symmetry restoration to occur when the thermal variance is of order one gives

$$
T_*\sim\sqrt{12\chi v^3}.
$$

The effective action in part c has $\chi=1/(2\lambda)$, and hence $T_*\sim\sqrt{6v^3/\lambda}$. This is an order-of-magnitude estimate because near restoration the phase-only [effective field theory](../../../quantum-field-theory.md#effective-field-theory) omits large amplitude fluctuations and sensitivity to its [ultraviolet cutoff](../../../quantum-field-theory.md#ultraviolet-cutoff).

## 2

↑ **Parent:** [Paper 337](paper-337.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A ferromagnetic vacuum breaks the [special unitary group](../../../topological-group.md#special-unitary-group) $SU(2)$ to the subgroup of rotations about its magnetization, so its vacuum manifold is the [two-sphere](../../../geometry-and-topology.md#two-sphere) $S^2$. The massless field is therefore a unit vector $\mathbf n(x,t)$ with $\mathbf n^2=1$.

The only rotational scalar linear in $\dot{\mathbf n}$ that can be formed directly from $\mathbf n$ is $\mathbf n\mathbin\cdot\dot{\mathbf n}=\tfrac12\partial_t(\mathbf n^2)=0$. A local one-form $\mathbf A(\mathbf n)\mathbin\cdot\dot{\mathbf n}$ can describe the required [Berry phase](../../../quantum-mechanics.md#berry-phase), but no choice of $\mathbf A$ is globally nonsingular and strictly rotationally invariant on $S^2$. One therefore needs coordinate patches, an extension, or a redundant spinor parametrization.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In the [CP1 spinor representation](../../../statistical-physics.md#cp1-spinor-representation),

$$
n_i=z^\dagger\sigma_i z,
\qquad z^\dagger z=1,
$$

where the $\sigma_i$ are [Pauli matrices](../../../algebra.md#pauli-matrices). The transformation $z\mapsto e^{i\alpha(x,t)}z$ leaves $\mathbf n$ unchanged. For $U\in SU(2)$,

$$
U^\dagger\sigma_iU=R_{ij}\sigma_j
$$

with $R$ in the [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) $SO(3)$, so $z\mapsto Uz$ induces $n_i\mapsto R_{ij}n_j$.

A rotationally invariant first-order term is the [Ferromagnetic Wess–Zumino term](../../../statistical-physics.md#ferromagnetic-wess-zumino-term)

$$
\mathcal L_{\rm WZ}=i\kappa z^\dagger\dot z.
$$

Under the phase redundancy it changes as $\mathcal L_{\rm WZ}\mapsto\mathcal L_{\rm WZ}-\kappa\dot\alpha$. The change is a [total derivative](../../../calculus.md#total-derivative), so the action has the required invariance.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $z=(e^{-i\phi}\cos(\theta/2),\sin(\theta/2))^T$,

$$
z^\dagger\dot z=-i\cos^2\left(\frac\theta2\right)\dot\phi.
$$

Thus $i\kappa z^\dagger\dot z=(\kappa/2)(1+\cos\theta)\dot\phi$. Dropping the [total derivative](../../../calculus.md#total-derivative) $(\kappa/2)\dot\phi$ and writing $s=\kappa/2$ gives

$$
\mathcal L_{
m WZ}=s\cos\theta\,\dot\phi.
$$

The leading rotationally invariant [gradient energy](../../../critical-phenomenon.md#gradient-energy) is $(\rho_s/2)(\nabla\mathbf n)^2$, so an effective Lagrangian is

$$
\boxed{\mathcal L=s\cos\theta\,\dot\phi-
\frac{\rho_s}{2}\left[(\nabla\theta)^2+sin^2\theta(\nabla\phi)^2\right].}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Put $q=\delta\theta$, $p=\delta\phi$, so $\theta=\pi/2-q$ and $\phi=p$. The [quadratic Lagrangian](../../../quantum-field-theory.md#quadratic-lagrangian) is obtained by taking

$$
\mathcal L_2=sq\dot p-
\frac{\rho_s}{2}\left[(\nabla q)^2+(\nabla p)^2\right].
$$

The two real fluctuations form a coordinate and its [canonical momentum](../../../classical-mechanics.md#canonical-momentum) rather than two independent modes. Their [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) combine to give

$$
\ddot q+\left(\frac{\rho_s}{s}\right)^2\nabla^4q=0,
$$

and similarly for $p$. The [ferromagnetic magnon](../../../statistical-physics.md#ferromagnetic-magnon) therefore has the quadratic [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{\omega_k=\frac{\rho_s}{s}k^2.}
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

With the convention $G_R(t)=-i\Theta(t)\langle[q(t),q(0)]\rangle$, the [retarded Green function](../../../quantum-field-theory.md#retarded-green-function) is

$$
G^R_{qq}(\omega,k)=
\frac{\omega_k/s}{(\omega+i0)^2-\omega_k^2}
=\frac{\rho_sk^2/s^2}{(\omega+i0)^2-\omega_k^2}.
$$

Defining the [spectral function](../../../quantum-field-theory.md#spectral-function) by $\varrho=-2\operatorname{Im}G_R$ gives

$$
\varrho(\omega,k)=\frac\pi s
\left[\delta(\omega-\omega_k)-\delta(\omega+\omega_k)\right].
$$

Other common spectral-weight conventions differ by an overall factor.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

The [Fluctuation-dissipation theorem](../../../quantum-field-theory.md#fluctuation-dissipation-theorem) in this convention reads

$$
S(\omega,k)=\frac{\varrho(\omega,k)}{1-e^{-\omega/T}}.
$$

In the [classical limit](../../../quantum-mechanics.md#classical-limit) $|\omega|\ll T$, this becomes

$$
S(\omega,k)\simeq\frac{T}{\omega}\varrho(\omega,k)
=\frac{\pi T}{s\omega_k}
\left[\delta(\omega-\omega_k)+\delta(\omega+\omega_k)\right].
$$

The inverse temporal [Fourier transform](../../../analysis.md#fourier-transform) is therefore

$$
\boxed{C(t,k)=\int\frac{d\omega}{2\pi}e^{-i\omega t}S(\omega,k)
=\frac{T}{s\omega_k}\cos(\omega_kt)
=\frac{T}{\rho_sk^2}\cos(\omega_kt).}
$$

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

For a [damped ferromagnetic spin wave](../../../statistical-physics.md#damped-ferromagnetic-spin-wave), shifting both poles into the lower half-plane preserves [causality](../../../special-relativity.md#causality):

$$
G_R(\omega,k)=\frac{\omega_k/s}{(\omega+i\Gamma_k)^2-\omega_k^2}.
$$

Its [spectral function](../../../quantum-field-theory.md#spectral-function) is

$$
\varrho(\omega,k)=
\frac{4(\omega_k/s)\omega\Gamma_k}
{(\omega^2-\omega_k^2-\Gamma_k^2)^2+4\omega^2\Gamma_k^2}.
$$

The classical [Fluctuation-dissipation theorem](../../../quantum-field-theory.md#fluctuation-dissipation-theorem) then gives

$$
S(\omega,k)=
\frac{4T(\omega_k/s)\Gamma_k}
{(\omega^2-\omega_k^2-\Gamma_k^2)^2+4\omega^2\Gamma_k^2}.
$$

Hence the zero-frequency [static structure factor](../../../critical-phenomenon.md#static-structure-factor) is

$$
S(k)=\frac{4T\omega_k\Gamma_k}
{s(\omega_k^2+\Gamma_k^2)^2},
$$

which has the stated proportionality after absorbing the normalization $4/s$.

<h3 id="2/h">h</h3>

↑ **Parent:** [2](#2)

<h4 id="2/h/solution">Solution</h4>

↑ **Parent:** [H](#2/h)

Write $D=\rho_s/s$, so $\omega_k=Dk^2$, and take $\Gamma_k=\gamma|k|$. The small-wavenumber [static structure factor](../../../critical-phenomenon.md#static-structure-factor) behaves as

$$
S(k)\propto
\frac{TD\gamma}{|k|(\gamma^2+D^2k^2)^2}
\sim\frac{TD}{\gamma^3|k|}.
$$

The spatial [Fourier transform](../../../analysis.md#fourier-transform) of $|k|^{-1}$ in $d$ dimensions scales as $|x|^{1-d}$. Thus

$$
C(x)\sim \text{constant}\times |x|^{1-d},
$$

and in three dimensions $C(x)\sim |x|^{-2}$. Since this [two-point correlation function](../../../critical-phenomenon.md#two-point-correlation-function) tends to zero rather than to a nonzero constant at large separation, it is incompatible with true long-range ferromagnetic order and hence with [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) at this higher temperature.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
