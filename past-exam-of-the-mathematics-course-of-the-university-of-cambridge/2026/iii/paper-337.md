# Paper 337

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20337.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20337.pdf)

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
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
  - [vii](#1/vii)
    - [Solution](#1/vii/solution)
  - [viii](#1/viii)
    - [Solution](#1/viii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)

## 1

↑ **Parent:** [Paper 337](paper-337.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The defining integral for the [retarded Green function](../../../quantum-field-theory.md#retarded-green-function) has support only at $t\geq0$. If $\omega=\omega_R+i\omega_I$ with $\omega_I>0$, then $e^{i\omega t}=e^{i\omega_Rt}e^{-\omega_It}$ supplies exponential damping. Under the usual tempered-growth condition on the thermal commutator, the integral and all its $\omega$ derivatives converge locally uniformly. Therefore

$$
\boxed{G_R(\omega)\ \text{is analytic for }\operatorname{Im}\omega>0}.
$$

This is the frequency-space expression of causality.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $H|a\rangle=E_a|a\rangle$, $p_a=e^{-E_a/T}$, and take $A$ Hermitian. Inserting energy eigenstates gives

$$
\operatorname{Im}G_R(\omega)
=-\pi\sum_{a,b}
(p_a-p_b)|A_{ab}|^2
\delta(\omega-E_b+E_a).
$$

On the support of the delta function, $E_b-E_a=\omega$ and

$$
p_a-p_b=p_a(1-e^{-\omega/T}).
$$

This has the same sign as $\omega$. Every remaining factor is nonnegative, hence

$$
\boxed{\omega\,\operatorname{Im}G_R(\omega)\leq0}.
$$

This thermal spectral-positivity statement also shows that $\operatorname{Im}G_R$ is odd after pairing $a,b$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

A [path integral](../../../quantum-field-theory.md#path-integral) is obtained by slicing an evolution operator into short time intervals and inserting complete sets of field eigenstates between successive factors. An operator inserted at a later slice therefore appears to the left of one inserted at an earlier slice. Summing over the intermediate fields preserves this ordering, so real-time path integrals generate time-ordered correlators and Euclidean thermal path integrals generate [imaginary-time-ordered correlation functions](../../../quantum-field-theory.md#imaginary-time-ordered-correlation-function).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Let $\beta=1/T$ and $A(\tau)=e^{H\tau}Ae^{-H\tau}$. For $0<\tau<\beta$, cyclicity of the trace gives

$$
\operatorname{Tr}\!\left(e^{-\beta H}A(\tau)A(0)\right)
=\operatorname{Tr}\!\left(e^{-\beta H}A(0)A(\tau-\beta)\right).
$$

This is the bosonic [Kubo--Martin--Schwinger condition](../../../quantum-field-theory.md#kubo-martin-schwinger-condition). It identifies the two time orderings across the end of the thermal interval, so

$$
\boxed{C(\tau+\beta)=C(\tau)}.
$$

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Periodicity on the interval $0\leq\tau<\beta$ gives the bosonic [Matsubara frequencies](../../../quantum-field-theory.md#matsubara-frequency)

$$
\boxed{\omega_n=2\pi nT,\qquad n\in\mathbb Z}.
$$

The Fourier coefficients are

$$
\boxed{
G(i\omega_n)=
\int_0^\beta d\tau\,
e^{i\omega_n\tau}C(\tau)}.
$$

The notation emphasizes that these data lie at imaginary real-time frequencies $i\omega_n$.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

The energy-eigenstate expansion of $C(\tau)$ for $0<\tau<\beta$ is

$$
C(\tau)=\sum_{a,b}
p_a e^{-(E_b-E_a)\tau}|A_{ab}|^2.
$$

Fourier integration and $e^{i\omega_n\beta}=1$ give

$$
G(i\omega_n)
=\sum_{a,b}
\frac{p_a-p_b}{E_b-E_a-i\omega_n}|A_{ab}|^2.
$$

Comparing this with the spectral expression in part ii yields the [spectral representation of a thermal correlation function](../../../quantum-field-theory.md#spectral-representation-of-a-thermal-correlation-function)

$$
\boxed{
G(i\omega_n)
=-\int_{-\infty}^{\infty}
\frac{d\Omega}{\pi}\,
\frac{\operatorname{Im}G_R(\Omega)}
{\Omega-i\omega_n}}.
$$

<h3 id="1/vii">vii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#1/vii)

The [Drude response](../../../quantum-field-theory.md#drude-response)

$$
G_R(\omega)=\frac{\sigma_0}{1-i\omega t_0}
$$

has a pole at $\omega=-i/t_0$. Analyticity in the upper half plane therefore requires

$$
\boxed{t_0>0}.
$$

For real frequency,

$$
\operatorname{Im}G_R(\omega)
=\frac{\sigma_0\omega t_0}{1+\omega^2t_0^2}.
$$

The sign condition from part ii then requires

$$
\boxed{\sigma_0t_0\leq0},
$$

so with a nonzero causal relaxation time the convention used in this question has $\sigma_0<0$. In conventions where the physical conductivity is defined with an additional minus sign, its static value is positive. The parameter $t_0$ is the relaxation time: after forcing is removed, the corresponding current or response decays as $e^{-t/t_0}$.

<h3 id="1/viii">viii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/viii/solution">Solution</h4>

↑ **Parent:** [Viii](#1/viii)

The spectral density is

$$
\operatorname{Im}G_R(\Omega)
=\frac{\sigma_0\Omega t_0}
{1+\Omega^2t_0^2}.
$$

Substitution into the spectral representation, closing the contour in the half plane selected by the sign of $\omega_n$, gives

$$
\boxed{
G(i\omega_n)
=-\frac{\sigma_0}{1+|\omega_n|t_0}}.
$$

In particular $G(0)=-\sigma_0\geq0$ under the sign convention established in part vii. The absolute value is required because a bosonic Hermitian-operator Matsubara correlator is even in $\omega_n$.

## 2

↑ **Parent:** [Paper 337](paper-337.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

In the long-wavelength $O(N)$ description of an antiferromagnet, $v$ is the [antiferromagnetic spin wave](../../../statistical-physics.md#antiferromagnetic-spin-wave) velocity and $g$ controls the stiffness or strength of quantum fluctuations. The field $\lambda$ is an auxiliary [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) enforcing the fixed-length constraint on the order parameter. At the translation-invariant saddle, $i\lambda=m^2$ shifts every propagator denominator and $m$ is the excitation gap, which explains the name [gap equation](../../../quantum-field-theory.md#gap-equation).

The [Large-N expansion](../../../quantum-field-theory.md#large-n-expansion) makes fluctuations of the auxiliary field relatively small. Its leading saddle-point condition is then self-consistent and becomes the displayed gap equation.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

As $T\to0$, the Matsubara sum becomes $\int d\omega/(2\pi)$. Put $p_0=\omega/v$ and $M=m/v$. The factors of $v$ cancel from both sides, leaving

$$
\frac1g
=\int^\Lambda\frac{d^4p}{(2\pi)^4}
\frac1{p^2+M^2}.
$$

Using four-dimensional spherical coordinates,

$$
\begin{aligned}
\frac1g
&=\frac{2\pi^2}{(2\pi)^4}
\int_0^\Lambda\frac{p^3\,dp}{p^2+M^2}\\
&=\boxed{
\frac1{16\pi^2}
\left[
\Lambda^2-M^2
\log\left(1+\frac{\Lambda^2}{M^2}\right)
\right]}.
\end{aligned}
$$

At the onset of [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking), the symmetric-phase gap closes. Thus

$$
\boxed{
\frac1{g_c}=\frac{\Lambda^2}{16\pi^2}},
\qquad
\boxed{
g_c=\frac{16\pi^2}{\Lambda^2}}.
$$

For $g<g_c$ the constraint is instead satisfied by an ordered condensate; a positive symmetric gap exists for $g>g_c$.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

Subtracting the critical equation from the massive equation gives

$$
\boxed{
\frac1{g_c}-\frac1g
=\frac{M^2}{16\pi^2}
\log\left(1+\frac{\Lambda^2}{M^2}\right)},
\qquad M=\frac mv.
$$

As $g\downarrow g_c$ from above,

$$
\frac{g-g_c}{g_c^2}
\sim
\frac{M^2}{16\pi^2}
\log\frac{\Lambda^2}{M^2}.
$$

Therefore, up to constants inside the slowly varying logarithm,

$$
\boxed{
m\sim
4\pi v
\left[
\frac{g-g_c}
{g_c^2\log(1/(g-g_c))}
\right]^{1/2}}.
$$

The square-root mean-field power is modified by a logarithm. It is therefore not a pure quantum-critical power law; this is an [upper-critical-dimension logarithmic correction](../../../quantum-field-theory.md#upper-critical-dimension-logarithmic-correction).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The first term is a gauge choice for the [Spin coherent-state Berry phase](../../../statistical-physics.md#spin-coherent-state-berry-phase). For a closed spin trajectory, changing the surface used to evaluate the solid angle changes the action by

$$
\Delta S_B=4\pi S.
$$

The path-integral phase $e^{iS_B}$ must be independent of that choice, so

$$
e^{i4\pi S}=1.
$$

Hence

$$
\boxed{2S\in\mathbb Z},
$$

and the spin is integer or half-integer.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Write $\theta=\pi/2-\vartheta$ and $\phi=\varphi$. To quadratic order,

$$
\cos\theta=\vartheta+O(\vartheta^3),
\qquad
\sin^2\theta=1+O(\vartheta^2).
$$

After dropping the total derivative $S\varphi_t$, the quadratic Lagrangian density is

$$
\boxed{
\mathcal L_2
=S\vartheta\varphi_t
-u(\vartheta_x^2+\varphi_x^2)
-K\vartheta^2}.
$$

Its Euler--Lagrange equations are

$$
S\varphi_t+2u\vartheta_{xx}-2K\vartheta=0,
\qquad
-S\vartheta_t+2u\varphi_{xx}=0.
$$

For modes proportional to $e^{i(kx-\omega t)}$, nontrivial amplitudes require

$$
\boxed{
\omega^2(k)
=\frac{4uk^2(uk^2+K)}{S^2}}.
$$

Thus

$$
\boxed{
\omega\sim\frac{2\sqrt{uK}}S|k|}
\quad(k\to0),
\qquad
\boxed{
\omega\sim\frac{2u}{S}k^2}
\quad(|k|\to\infty).
$$

At short wavelength the anisotropy is negligible and the quadratic dispersion is that of a conventional [ferromagnetic magnon](../../../statistical-physics.md#ferromagnetic-magnon). At long wavelength, [easy-plane anisotropy](../../../statistical-physics.md#easy-plane-anisotropy) makes the out-of-plane fluctuation the conjugate density of the in-plane phase; eliminating it produces the linear Goldstone sound mode characteristic of a [superfluid](../../../statistical-physics.md#superfluid).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
