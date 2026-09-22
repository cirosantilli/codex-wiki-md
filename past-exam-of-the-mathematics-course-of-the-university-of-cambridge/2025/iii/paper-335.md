# Paper 335

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_335.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_335.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
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

The [phase screen](../../../partial-differential-equation.md#phase-screen) adds the phase accumulated across its thickness, so the reduced field just after the screen is

$$
E(0,z)=e^{ik\xi w(z)}.
$$

For a zero-mean random variable $w$ with a [normal distribution](../../../probability-theory.md#normal-distribution) and variance $\sigma^2$, its [characteristic function](../../../probability-theory.md#characteristic-function) gives

$$
\boxed{\langle E(0,z)\rangle
=\exp\left(-\frac12k^2\xi^2\sigma^2\right).}
$$

The same expression is approximately valid for a non-Gaussian weak fluctuation: the [cumulant expansion](../../../probability-theory.md#cumulant-expansion) begins with $-k^2\xi^2\sigma^2/2$, while higher cumulants give higher-order corrections.

For $x>0$, every realization obeys the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation)

$$
2ikE_x+E_{zz}=0.
$$

Linearity permits ensemble averaging, so

$$
\boxed{2ik\partial_x\langle E\rangle
+\partial_z^2\langle E\rangle=0.}
$$

The initial mean is independent of $z$, hence diffraction does not change it and $\langle E(x,z)\rangle=\exp(-k^2\xi^2\sigma^2/2)$ for every $x\geq0$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let

$$
M(x;z_1,z_2)=\langle E(x,z_1)E(x,z_2)\rangle.
$$

Applying the [parabolic wave equation](../../../partial-differential-equation.md#parabolic-wave-equation) to each factor gives

$$
\boxed{2ikM_x+(\partial_{z_1}^2+\partial_{z_2}^2)M=0.}
$$

If $C(s)=\langle w(z)w(z+s)\rangle$, Gaussian averaging at the screen gives

$$
M(0;z_1,z_2)
=\boxed{\exp\{-k^2\xi^2[\sigma^2+C(z_1-z_2)]\}.}
$$

Stationarity makes this a function only of $s=z_1-z_2$. Since $\partial_{z_1}^2+\partial_{z_2}^2=2\partial_s^2$ on such functions,

$$
M_x=\frac{i}{k}M_{ss}.
$$

Writing $\widehat M_0(q)$ for the [Fourier transform](../../../analysis.md#fourier-transform) of the screen value, the solution at arbitrary range is

$$
\boxed{
M(x;s)=\frac1{2\pi}\int_{\mathbb R}
\widehat M_0(q)e^{iqs-iq^2x/k}\,dq.}
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Choose the overall phase so that the coherent mean $m=\langle E\rangle$ is real. With $E_j=m+A_j+iB_j$,

$$
I_j=|E_j|^2=m^2+2mA_j+A_j^2+B_j^2.
$$

Because the diffuse field has zero mean, keeping terms through second order gives

$$
\langle I_1I_2\rangle-\langle I\rangle^2
=4m^2\langle A_1A_2\rangle,
$$

and, at coincident points,

$$
\langle I^2\rangle-\langle I\rangle^2
=4m^2\langle A^2\rangle.
$$

The normalized spatial intensity correlation is therefore

$$
\boxed{\rho_I(z_1,z_2)
=\frac{\langle A_1A_2\rangle}{\langle A^2\rangle}.}
$$

**Thus weak-scattering intensity fluctuations measure the normalized correlation of the in-phase part of the diffuse field.**

## 2

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

With the [scattering potential](../../../inverse-problem.md#scattering-potential) $V(\mathbf r)=k_0^2(1-n^2(\mathbf r))$, the total field obeys

$$
(\nabla^2+k_0^2)\psi=V\psi.
$$

The outgoing Green function is $G_0(\mathbf r)=e^{ik_0|\mathbf r|}/(4\pi|\mathbf r|)$. The [Lippmann-Schwinger equation](../../../quantum-mechanics.md#lippmann-schwinger-equation) and the first [Born approximation](../../../quantum-theory.md#born-approximation) give

$$
\psi_s(\mathbf r)simeq
-\int_DG_0(\mathbf r-\mathbf r')V(\mathbf r')
e^{ik_0\widehat{\mathbf x}_0\cdot\mathbf r'},d\mathbf r'.
$$

For $r\to\infty$,

$$
G_0(\mathbf r-\mathbf r')
\sim\frac{e^{ik_0r}}{4\pi r}
e^{-ik_0\widehat{\mathbf r}\cdot\mathbf r'},
$$

so

$$
\boxed{
\psi_s(\mathbf r)\sim\frac{e^{ik_0r}}r
f_\infty(\widehat{\mathbf x}_0,\widehat{\mathbf r}),
\qquad
f_\infty=-\frac1{4\pi}
\int_DV(\mathbf r')e^{-i\mathbf q\cdot\mathbf r'}d\mathbf r',}
$$

where $\mathbf q=k_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)$ is the [momentum transfer](../../../quantum-mechanics.md#momentum-transfer). Thus the [far-field pattern](../../../inverse-problem.md#far-field-pattern) is $-1/(4\pi)$ times the Fourier transform of $V$ at the measured transfer vectors. If sufficiently many incident directions and frequencies supply all $\mathbf q$, the formal reconstruction is

$$
\boxed{V(\mathbf r)=-4\pi\mathcal F^{-1}
\{f_\infty(\mathbf q)\}(\mathbf r),}
$$

with constants adjusted to the chosen Fourier convention.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Use

$$
(\mathcal Fg)(\mathbf q)=\int_{\mathbb R^3}
g(\mathbf r)e^{-i\mathbf q\cdot\mathbf r}d\mathbf r,
\qquad
\mathcal F^{-1}h=\frac1{(2\pi)^3}\int h(\mathbf q)e^{i\mathbf q\cdot\mathbf r}d\mathbf q.
$$

The [adjoint operator](../../../hilbert-space.md#adjoint-operator) is consequently

$$
\boxed{\mathcal F^*=(2\pi)^3\mathcal F^{-1}.}
$$

With a unitary Fourier normalization, this is simply $\mathcal F^*=\mathcal F^{-1}$.

At fixed incident direction and wavenumber, define

$$
(TV)(\widehat{\mathbf r})
=-\frac1{4\pi}\int_D
e^{-ik_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)\cdot\mathbf r}
V(\mathbf r)d\mathbf r.
$$

Taking the complex conjugate of the kernel gives

$$
\boxed{
(T^*g)(\mathbf r)
=-\frac1{4\pi}\int_{S^2}
e^{ik_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)\cdot\mathbf r}
g(\widehat{\mathbf r})dS(\widehat{\mathbf r}),
\qquad \mathbf r\in D.}
$$

The least-squares minimizer of $\|TV-f_\infty\|^2$ satisfies the [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) $T^*TV=T^*f_\infty$. Fourier inversion on the measured transfer-vector set is exactly the corresponding Moore--Penrose reconstruction $T^\dagger f_\infty$; hence the formal solution in part (i) is the minimum-norm least-squares solution when the data are incomplete or inconsistent.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The inverse problem is ill posed for several related reasons. At one frequency and one incident direction, the data sample $\widehat V$ only on the two-dimensional Ewald surface $\mathbf q=k_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)$, so three-dimensional reconstruction is nonunique without more illuminations or prior information. Finite aperture and a bounded frequency band omit additional Fourier components and limit resolution. The forward map is compact, so its singular values tend to zero and inversion strongly amplifies measurement noise. Finally, the [Born approximation](../../../quantum-theory.md#born-approximation) neglects multiple scattering; model error becomes significant when the contrast or support is too large, while uncertainty in the incident field, measurement geometry, and domain $D$ creates further instability.

## 3

↑ **Parent:** [Paper 335](paper-335.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

A [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem) consists of bounded operators $R_\alpha:Y\to X$ and a parameter rule $\alpha=\alpha(\delta,y^\delta)$ such that, whenever $\|y^\delta-y\|\leq\delta$ and $y$ lies in the domain of $A^\dagger$,

$$
\alpha(\delta,y^\delta)\to0,
\qquad
R_{\alpha(\delta,y^\delta)}y^\delta\to A^\dagger y
$$

as $\delta\to0$. It is needed because a compact operator on an infinite-dimensional space has singular values tending to zero, so direct inversion divides noisy data by arbitrarily small numbers and is generally discontinuous.

[Tikhonov regularization](../../../inverse-problem.md#tikhonov-regularization) defines

$$
x_\alpha^\delta
=\underset{x\in X}{\operatorname{argmin}}
\left(\|Ax-y^\delta\|^2+\alpha\|x\|^2\right),
$$

and its normal equation gives

$$
\boxed{x_\alpha^\delta
=(A^*A+\alpha I)^{-1}A^*y^\delta.}
$$

For every fixed $\alpha>0$, $A^*A+\alpha I$ is bounded below by $\alpha I$, and the data-to-solution operator is bounded. Small changes in $y^\delta$ therefore produce small changes in $x_\alpha^\delta$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

A [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator) is a family $(\sigma_i,u_i,v_i)$ with $\sigma_i>0$, $\sigma_i\to0$, orthonormal $u_i\in Y$ and $v_i\in X$, and

$$
Av_i=\sigma_i u_i,
\qquad
A^*u_i=\sigma_i v_i.
$$

On each singular vector, $A^*A+\alpha I$ acts by multiplication by $\sigma_i^2+\alpha$. Hence

$$
\boxed{
x_\alpha^\delta
=\sum_{i=1}^\infty
\frac{\sigma_i}{\sigma_i^2+\alpha}
(y^\delta,u_i)v_i.}
$$

The bounded filter $\sigma/(\sigma^2+\alpha)$ replaces the unstable inverse factor $1/\sigma$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Write

$$
B=I-\frac1\alpha A^*A.
$$

The stated iteration is $x_{n+1}=Bx_n+\alpha^{-1}A^*y$, so repeated substitution and the [geometric series](../../../real-analysis.md#geometric-series) identity give

$$
x_n=B^nx_0+\frac1\alpha\sum_{j=0}^{n-1}B^jA^*y.
$$

For the singular component $v_i$, put $r_i=1-\sigma_i^2/\alpha$. Since the initial Tikhonov solution has coefficient $\sigma_i(y,u_i)/(\sigma_i^2+\alpha)$, one obtains

$$
x_n=\sum_{i=1}^\infty
\left[
r_i^n\frac{\sigma_i}{\sigma_i^2+\alpha}
+\frac{1-r_i^n}{\sigma_i}
\right](y,u_i)v_i.
$$

Therefore the requested spectral filter is

$$
\boxed{
g_{\alpha,n}(\sigma)
=\frac1\sigma\left[
1-\frac{\alpha}{\sigma^2+\alpha}
\left(1-\frac{\sigma^2}{\alpha}\right)^n
\right].}
$$

**Thus equation (3) reads $x_n=\sum_i g_{\alpha,n}(\sigma_i)(y,u_i)v_i$. Convergence of this stationary iteration requires $|1-\sigma_i^2/\alpha|<1$ on the nonzero spectrum, for example $\alpha>\|A\|^2/2$.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
