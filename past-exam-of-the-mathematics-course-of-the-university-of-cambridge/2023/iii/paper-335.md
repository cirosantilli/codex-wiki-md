# Paper 335

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_335.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_335.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [a](#1/ii/a)
      - [Solution](#1/ii/a/solution)
    - [b](#1/ii/b)
      - [Solution](#1/ii/b/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
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

## 1

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Put

$$
k=\frac{\omega}{c_0},\qquad
p=k\sin\theta_i,\qquad
q_0=k\cos\theta_i,
$$

and let $q_1=nk\cos\theta_T$ be the downward [vertical wavenumber](../../../partial-differential-equation.md#vertical-wavenumber) in the lower half-space. The given form of [Snell's law](../../../partial-differential-equation.md#snell-s-law) says

$$
q_1=q_0\sqrt{1+\alpha}.
$$

With the $e^{-i\omega t}$ convention, write the incident, reflected, and transmitted [plane waves](../../../quantum-mechanics.md#plane-wave) as

$$
\psi_i=e^{i(px-q_0z)},\qquad
\psi_r=R e^{i(px+q_0z)},\qquad
\psi_t=T e^{i(px-q_1z)}.
$$

The two [interface conditions](../../../partial-differential-equation.md#scalar-wave-interface-condition) at $z=0$ give

$$
1+R=T,
\qquad
q_0(1-R)=q_1T.
$$

Solving this [linear system](../../../linear-algebra.md#system-of-linear-equations) gives the [reflection and transmission coefficients at a scalar-wave interface](../../../partial-differential-equation.md#reflection-and-transmission-coefficients-at-a-scalar-wave-interface)

$$
\boxed{R=\frac{q_0-q_1}{q_0+q_1}
=\frac{1-\sqrt{1+\alpha}}{1+\sqrt{1+\alpha}}},
\qquad
\boxed{T=\frac{2q_0}{q_0+q_1}
=\frac{2}{1+\sqrt{1+\alpha}}}.
$$

Thus the exact fields are

$$
\boxed{\psi_0=e^{i(px-q_0z)}+R e^{i(px+q_0z)}}
\quad(z>0),
$$



$$
\boxed{\psi_1=T e^{i(px-q_1z)}}
\quad(z<0).
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/a">a</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#1/ii/a)

After separating the conserved horizontal factor as $\psi=e^{ipx}f(z)$, the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) becomes

$$
f''+q_0^2f=-\alpha q_0^2H(-z)f,
$$

where $H$ is the [Heaviside step function](../../../analysis.md#heaviside-step-function). The outgoing [Green function](../../../analysis.md#green-s-function) for $d^2/dz^2+q_0^2$ is

$$
G(z,z')=\frac{e^{iq_0|z-z'|}}{2iq_0}.
$$

The [Born approximation](../../../quantum-theory.md#born-approximation) at first order replaces $f$ on the right-hand side by the incident profile $f_i(z')=e^{-iq_0z'}$. For $z>0$ this gives

$$
f_{s,B}(z)
=-\alpha q_0^2\int_{-\infty}^{0}
\frac{e^{iq_0(z-z')}}{2iq_0}e^{-iq_0z'}\,dz'.
$$

The integral is understood with the usual outgoing-wave convergence factor. Since

$$
\int_{-\infty}^{0}e^{-2iq_0z'}\,dz'=-\frac{1}{2iq_0},
$$

we obtain

$$
f_{s,B}(z)=-\frac{\alpha}{4}e^{iq_0z}.
$$

Therefore the Born reflected field is

$$
\boxed{\psi_{r,B}(x,z)=-\frac{\alpha}{4}e^{i(px+q_0z)}}.
$$

<h4 id="1/ii/b">b</h4>

↑ **Parent:** [Ii](#1/ii)

<h5 id="1/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#1/ii/b)

The [Rytov approximation](../../../inverse-problem.md#rytov-approximation) at first order writes the total profile as $f_R=f_i e^{\chi_1}$ and identifies the first logarithmic perturbation with the Born relative field:

$$
\chi_1=\frac{f_{s,B}}{f_i}
=-\frac{\alpha}{4}e^{2iq_0z}.
$$

Hence, in the upper half-space,

$$
\boxed{
\psi_R(x,z)=e^{i(px-q_0z)}
\exp\left(-\frac{\alpha}{4}e^{2iq_0z}\right)}.
$$

Expanding the [exponential function](../../../calculus.md#exponential-function) to first order shows that its reflected component is

$$
\boxed{\psi_{r,R}^{(1)}(x,z)
=-\frac{\alpha}{4}e^{i(px+q_0z)}}.
$$

The exponentiated expression is the Rytov approximation to the total field; only its term linear in $\alpha$ is a single specular reflected [plane wave](../../../quantum-mechanics.md#plane-wave).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [Taylor expansion](../../../calculus.md#taylor-expansion) of the square root is

$$
\sqrt{1+\alpha}=1+\frac{\alpha}{2}
-\frac{\alpha^2}{8}+O(\alpha^3).
$$

Substitution into the exact [reflection coefficient](../../../partial-differential-equation.md#reflection-coefficient) gives

$$
R=\frac{1-\sqrt{1+\alpha}}
{1+\sqrt{1+\alpha}}
=-\frac{\alpha}{4}+\frac{\alpha^2}{8}
+O(\alpha^3).
$$

Consequently

$$
\boxed{
\psi_r=-\frac{\alpha}{4}e^{i(px+q_0z)}
+O(\alpha^2)}.
$$

This is exactly the reflected field furnished by both the [Born approximation](../../../quantum-theory.md#born-approximation) and the term linear in $α$ in the [Rytov approximation](../../../inverse-problem.md#rytov-approximation). Thus the exact, Born, and Rytov fields agree through first order. If the Rytov exponential is retained without re-expansion, its higher powers generate spatial harmonics $e^{i(px+(2m-1)q_0z)}$; those terms are part of the approximation and should not be confused with the exact interface's single reflected wave.

## 2

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For a slowly varying envelope $E=\psi e^{-ikx}$, the [paraxial approximation](../../../partial-differential-equation.md#paraxial-approximation) to the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) is

$$
E_x=\frac{i}{2k}E_{zz}
+\frac{ik}{2}(n^2-1)E.
$$

Because $n=1+\mu W$ and $\mu^2\ll1$, passage through a sufficiently thin [phase screen](../../../partial-differential-equation.md#phase-screen) produces

$$
E(0,z)=e^{i\phi(z)},
\qquad
\phi(z)=\frac{k}{2}\int_{-\xi}^{0}(n^2-1)\,dx
\simeq k\mu\xi W(z).
$$

Its [modulus](../../../complex-analysis.md#modulus) is one at the screen exit. Beyond the screen, $n=1$, so the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation) is $E_x=iE_{zz}/(2k)$. A [Taylor expansion](../../../calculus.md#taylor-expansion) in propagation distance gives

$$
E(x,z)=E(0,z)+\frac{ix}{2k}E_{zz}(0,z)+O(x^2).
$$

Since

$$
\frac{(e^{i\phi})_{zz}}{e^{i\phi}}
=i\phi''-(\phi')^2,
$$

we find

$$
E(x,z)=e^{i\phi(z)}
\left[1-\frac{x}{2k}\phi''(z)
-\frac{ix}{2k}(\phi'(z))^2\right]+O(x^2).
$$

It follows that

$$
\boxed{|E(x,z)|=1-\frac{x}{2k}\phi''(z)+O(x^2)},
$$

or, equivalently, $|E|^2=1-x\phi''/k+O(x^2)$. Thus random [phase curvature](../../../partial-differential-equation.md#phase-curvature) produces local focusing and defocusing: [free-space diffraction](../../../partial-differential-equation.md#free-space-diffraction) converts phase fluctuations into amplitude fluctuations immediately after the screen.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

To first order in the weak fluctuation, $n^2-1=2\mu W+O(\mu^2)$, so

$$
E_x=\frac{i}{2k}E_{zz}+ik\mu WE.
$$

For

$$
F=E_1E_2^*E_3E_4^*,
\qquad E_j=E(x,z_j),
$$

introduce the signs $s=(1,-1,1,-1)$. The [product rule](../../../calculus.md#product-rule) gives

$$
\partial_x\langle F\rangle
=\frac{i}{2k}
\left(\partial_{z_1}^2-\partial_{z_2}^2
+\partial_{z_3}^2-\partial_{z_4}^2\right)m_4
+ik\mu\sum_{j=1}^4s_j\langle W(x,z_j)F\rangle.
$$

Assume that $W$ is a zero-mean [stationary Gaussian random field](../../../stochastic-process.md#stationary-gaussian-random-field), that its longitudinal [correlation length](../../../critical-phenomenon.md#correlation-length) is short compared with the envelope's evolution scale, and that the propagation distance is long compared with that correlation length. The forward [Markov approximation](../../../stochastic-process.md#markov-approximation-for-a-random-medium) then neglects diffraction during one correlation length. Applying the [Furutsu–Novikov formula](../../../stochastic-process.md#novikov-s-theorem) closes the last average at second order in $\mu$. Define the integrated longitudinal [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field)

$$
C(\zeta)=\int_{-\infty}^{\infty}
\rho(\xi,\zeta)\,d\xi.
$$

Then

$$
\boxed{
\partial_xm_4
=\frac{i}{2k}
\left(\partial_{z_1}^2-\partial_{z_2}^2
+\partial_{z_3}^2-\partial_{z_4}^2\right)m_4
-Q_4m_4},
$$

where

$$
\boxed{
Q_4=\frac{k^2\mu^2}{2}
\sum_{i,j=1}^4s_is_jC(z_i-z_j)}.
$$

Writing $C_{ij}=C(z_i-z_j)$ and using the evenness of the covariance gives the equivalent expression

$$
Q_4=k^2\mu^2
\left(2C(0)-C_{12}+C_{13}-C_{14}
-C_{23}+C_{24}-C_{34}\right).
$$

The derivation also assumes [paraxial propagation](../../../partial-differential-equation.md#paraxial-approximation), weak scattering, sufficient regularity to interchange differentiation and [expectation](../../../probability-theory.md#expected-value), and statistical homogeneity in both coordinates. Without the short-correlation approximation, the Gaussian identity produces a nonlocal longitudinal memory integral rather than this local closed equation.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/a">a</h4>

↑ **Parent:** [Iii](#2/iii)

<h5 id="2/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/iii/a)

Substitute $m_4=e^{\Psi}$ into the given equation. The [chain rule](../../../calculus.md#chain-rule) gives

$$
\Psi_x=\frac{i}{k}
\left(\Psi_{r_1r_2}+Psi_{r_1}\Psi_{r_2}\right)-Q.
$$

The incident reduced field is the constant one, so $m_4(-\Delta x)=1$ and $\Psi(-\Delta x)=0$. During a thin-screen crossing, $\Psi=O(\Delta x)$. Its mixed-derivative contribution integrates to $O(\Delta x)$. More precisely, its contribution to $\Psi$ is $O((\Delta x)^2)$, while the product of its first derivatives contributes only at still higher order. Therefore

$$
\Psi(0,r_1,r_2)=-Q(r_1,r_2)\Delta x
+O((\Delta x)^2),
$$

and hence

$$
\boxed{
m_4(0,r_1,r_2)
=e^{-Q(r_1,r_2)\Delta x}+O((\Delta x)^2)
=1-Q(r_1,r_2)\Delta x+O((\Delta x)^2)}.
$$

<h4 id="2/iii/b">b</h4>

↑ **Parent:** [Iii](#2/iii)

<h5 id="2/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/iii/b)

In free space $Q=0$, and the fourth moment obeys

$$
\partial_xm_4=\frac{i}{k}\partial_{r_1}\partial_{r_2}m_4.
$$

For the two-dimensional [Fourier transform](../../../analysis.md#fourier-transform)

$$
\widehat m_4(x,p_1,p_2)
=\int_{\mathbb R^2}m_4(x,r_1,r_2)
e^{-i(p_1r_1+p_2r_2)}\,dr_1dr_2,
$$

the [Fourier transform of a derivative](../../../fourier-analysis.md#fourier-transform-of-a-derivative) turns this equation into the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation)

$$
\partial_x\widehat m_4
=-\frac{i}{k}p_1p_2\widehat m_4.
$$

Thus

$$
\boxed{
\widehat m_4(L,p_1,p_2)
=e^{-iLp_1p_2/k}
\widehat m_4(0,p_1,p_2)}.
$$

Using the screen-exit value from part (a), the inverse transform gives

$$
\boxed{
m_4(L,r_1,r_2)=\frac{1}{(2\pi)^2}
\int_{\mathbb R^2}e^{i(p_1r_1+p_2r_2)-iLp_1p_2/k}
\widehat{e^{-Q\Delta x}}(p_1,p_2)\,dp_1dp_2}
$$

through first order in $Δx$. Equivalently, the [free-space fourth-moment propagator](../../../partial-differential-equation.md#free-space-fourth-moment-propagator) has kernel

$$
\boxed{
m_4(L,r_1,r_2)=\frac{k}{2\pi L}
\int_{\mathbb R^2}
\exp\left[\frac{ik}{L}(r_1-s_1)(r_2-s_2)\right]
m_4(0,s_1,s_2)\,ds_1ds_2}.
$$

## 3

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Because $A$ is a real symmetric [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), the [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem) supplies an orthonormal eigenbasis $u_1,\ldots,u_n$ with

$$
0<\lambda_1\leq\cdots\leq\lambda_n.
$$

Its eigendecomposition is also its [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition). If $e=y^{(\delta)}-y$, then

$$
x^{(\delta)}-x=A^{-1}e
=\sum_{j=1}^n\frac{\langle e,u_j\rangle}{\lambda_j}u_j,
$$

so

$$
\boxed{\|x^{(\delta)}-x\|
\leq\frac{\delta}{\lambda_1}}.
$$

The operator norms satisfy $\|A\|_2=\lambda_n$ and $\|A^{-1}\|_2=1/\lambda_1$. Therefore the worst-case relative perturbation bound is

$$
\boxed{
\frac{\|x^{(\delta)}-x\|}{\|x\|}
\leq
\underbrace{\frac{\lambda_n}{\lambda_1}}_{\kappa_2(A)}
\frac{\|y^{(\delta)}-y\|}{\|y\|}}.
$$

The ratio $κ_2(A)$ is the [spectral condition number of a positive-definite matrix](../../../linear-algebra.md#spectral-condition-number-of-a-positive-definite-matrix). A large ratio means that data noise aligned with an [eigenvector](../../../linear-operator-theory.md#eigenvector) for the smallest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is strongly amplified, so the inverse problem is ill conditioned.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $(\sigma_j,u_j,v_j)$ be a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator), with

$$
Av_j=\sigma_ju_j,
\qquad
A^*u_j=\sigma_jv_j.
$$

The [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) is the generally unbounded map

$$
\boxed{
A^\dagger g
=\sum_j\frac{\langle g,u_j\rangle}{\sigma_j}v_j},
$$

defined when the [Picard criterion](../../../inverse-problem.md#picard-criterion) holds, with the component in $\ker A^*$ sent to zero. It is the [minimum-norm least-squares solution](../../../inverse-problem.md#minimum-norm-least-squares-solution) of $Af=g$.

A [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem) consists of bounded maps $R_\alpha:Y\to X$ and a parameter rule $α=α(δ,g^{(δ)})$ such that

$$
\alpha\to0,
\qquad
R_\alpha g^{(\delta)}\to A^\dagger g
$$

whenever $\|g^{(\delta)}-g\|\leq\delta$ and $g$ is in the domain of $A^\dagger$.

For [Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization), minimizing

$$
\|Af-g^{(\delta)}\|^2+\alpha\|f\|^2
$$

gives

$$
R_\alpha g^{(\delta)}
=(A^*A+\alpha I)^{-1}A^*g^{(\delta)}
=\sum_j\frac{\sigma_j}{\sigma_j^2+\alpha}
\langle g^{(\delta)},u_j\rangle v_j.
$$

The scalar [spectral filter](../../../inverse-problem.md#spectral-filter) satisfies

$$
\sup_{\sigma\geq0}\frac{\sigma}{\sigma^2+\alpha}
=\frac{1}{2\sqrt\alpha},
$$

and consequently

$$
\|R_\alpha(g^{(\delta)}-g)\|
\leq\frac{\delta}{2\sqrt\alpha}.
$$

For exact data, each filter factor $\sigma_j^2/(\sigma_j^2+\alpha)$ tends to one, so $R_\alpha g\to A^\dagger g$. Choosing

$$
\boxed{\alpha(\delta)\to0,
\qquad \frac{\delta}{\sqrt{\alpha(\delta)}}\to0}
$$

therefore makes both the approximation error and propagated data error vanish. For example, $α(δ)=δ$ is an admissible [a priori regularization parameter choice](../../../inverse-problem.md#a-priori-regularization-parameter-choice).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For the [Volterra integration operator](../../../functional-analysis.md#volterra-operator)

$$
(Af)(x)=\int_0^x f(t)\,dt,
$$

the [adjoint operator](../../../hilbert-space.md#adjoint-operator) is

$$
(A^*g)(x)=\int_x^1g(t)\,dt.
$$

Since $1/\sigma_n=(2n-1)\pi/2$, direct integration gives

$$
Au_n(x)
=\sqrt2\int_0^x\cos(t/\sigma_n)\,dt
=\sigma_n\sqrt2\sin(x/\sigma_n)
=\sigma_nv_n(x).
$$

Similarly,

$$
A^*v_n(x)
=\sqrt2\int_x^1\sin(t/\sigma_n)\,dt
=\sigma_n\sqrt2
\left(\cos(x/\sigma_n)-\cos(1/\sigma_n)\right)
=\sigma_nu_n(x),
$$

because $\cos((2n-1)\pi/2)=0$. The half-integer sine and cosine families are [orthonormal bases](../../../linear-algebra.md#orthonormal-basis) of $L^2([0,1])$, so $(\sigma_n,u_n,v_n)$ is a [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator).

The Tikhonov solution for noisy data $g^{(\delta)}$ is therefore

$$
\boxed{
f_\alpha(x)=
\sum_{n=1}^{\infty}
\frac{\sigma_n}{\sigma_n^2+\alpha}
\langle g^{(\delta)},v_n\rangle u_n(x)}.
$$

Writing out the [inner product](../../../linear-algebra.md#inner-product) and the singular functions makes this explicit:

$$
\boxed{
f_\alpha(x)=2\sum_{n=1}^{\infty}
\frac{\sigma_n}{\sigma_n^2+\alpha}
\cos\left(\frac{x}{\sigma_n}\right)
\int_0^1g^{(\delta)}(t)
\sin\left(\frac{t}{\sigma_n}\right)\,dt,
\qquad
\sigma_n=\frac{2}{(2n-1)\pi}.}
$$

The factors $\sigma_n/(\sigma_n^2+\alpha)$ suppress the unstable reciprocal growth $1/\sigma_n$ at high index.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
