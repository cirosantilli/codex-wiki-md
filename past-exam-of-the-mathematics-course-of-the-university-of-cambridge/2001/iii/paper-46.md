# Paper 46

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper46.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper46.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)

## 1

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $\sigma_v^2=\langle v(0)^2\rangle$, assumed finite. The displacement is $\Delta X(t)=\int_0^t v(s)\,ds$. By [stationarity](../../../time-series.md#stationary-process), its two-time covariance is $\langle v(s)v(r)\rangle=\sigma_v^2\rho(s-r)$, with $\rho$ even for a real scalar process. Integrating over the two triangles of the square gives the [Taylor turbulent dispersion](../../../turbulence.md#taylor-turbulent-dispersion) identity

$$
\boxed{\langle\Delta X(t)^2\rangle=2\sigma_v^2\int_0^t(t-s)\rho(s)\,ds.}
$$

A sufficient condition for ordinary long-time variance growth is $\int_0^\infty|\rho(s)|\,ds<\infty$ with $\int_0^\infty\rho(s)\,ds>0$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) then gives

$$
\frac{\langle\Delta X(t)^2\rangle}{2t}\longrightarrow D,
\qquad \boxed{D=\sigma_v^2\int_0^\infty\rho(s)\,ds.}
$$

More generally the necessary asymptotic condition for a finite positive variance-based [diffusion coefficient](../../../brownian-motion.md#diffusion-coefficient) is convergence of $\sigma_v^2\int_0^t(1-s/t)\rho(s)\,ds$ to that coefficient. Absolute integrability is sufficient, not necessary. A zero integral does not give nondegenerate ordinary [diffusion](../../../thermodynamics.md#diffusion). Moreover a second-moment calculation alone does not establish a [normal distribution](../../../probability-theory.md#normal-distribution) or an entire diffusive scaling limit; those require additional probabilistic assumptions.

For the specified positive [autocorrelation](../../../time-series.md#autocorrelation), direct integration gives, when $\alpha\ne1,2$,

$$
\langle\Delta X^2\rangle=2\sigma_v^2\left[\frac{(1+t)^{2-\alpha}-1}{(1-\alpha)(2-\alpha)}-\frac t{1-\alpha}\right].
$$

Thus the [power-law velocity-correlation dispersion](../../../turbulence.md#power-law-velocity-correlation-dispersion) has the following regimes. If $\alpha>1$, the [Lagrangian integral time](../../../turbulence.md#lagrangian-integral-time) is $1/(\alpha-1)$ and **ordinary variance growth holds**, with $D=\sigma_v^2/(\alpha-1)$. At $\alpha=2$ the exact expression is $2\sigma_v^2[t-\log(1+t)]$. If $\alpha=1$,

$$
\langle\Delta X^2\rangle=2\sigma_v^2[(1+t)\log(1+t)-t]\sim2\sigma_v^2t\log t.
$$

For $0<\alpha<1$,

$$
\boxed{\langle\Delta X^2\rangle\sim\frac{2\sigma_v^2}{(1-\alpha)(2-\alpha)}t^{2-\alpha}.}
$$

The last two regimes spread faster than ordinary [diffusion](../../../thermodynamics.md#diffusion) and have no finite long-time [diffusion coefficient](../../../brownian-motion.md#diffusion-coefficient). Their slowly decaying velocity memory is responsible. At short times all these correlations instead give the ballistic law $\langle\Delta X^2\rangle\sim\sigma_v^2t^2$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Take $\kappa>0$ and initially $\omega\ne0$. Write $m_j(y,t)=\int_{\mathbb R}x^j\chi(x,y,t)\,dx$, and set $k=\pi/L$, $a=\kappa k^2$. The [advection-diffusion equation](../../../diffusion-equation.md#advection-diffusion-equation) is $\chi_t+u\chi_x=\kappa(\chi_{xx}+\chi_{yy})$. Integration by parts in the unbounded coordinate gives the [longitudinal moment hierarchy for shear transport](../../../fluid-mechanics.md#longitudinal-moment-hierarchy-for-shear-transport)

$$
\partial_t m_0=\kappa\partial_y^2m_0,\qquad
\partial_t m_1=\kappa\partial_y^2m_1+um_0,\qquad
\partial_t m_2=\kappa\partial_y^2m_2+2um_1+2\kappa m_0.
$$

All three moments obey [Neumann boundary conditions](../../../differential-equation.md#neumann-boundary-condition) at the walls. The initial values are $m_0=L$, $m_1=0$, $m_2=L^3/12$. These manipulations require finite moments and vanishing boundary terms at $x=\pm\infty$; diffusion of the compact initial distribution supplies the required decay for positive time.

The zeroth moment remains exactly $L$. Since $\sin(ky)$ is a Neumann eigenfunction, put $m_1=L g(t)\sin(ky)$. Then $g'+ag=U\cos(\omega t)$ and $g(0)=0$, giving

$$
g(t)=\frac{U}{a^2+\omega^2}[a\cos(\omega t)+\omega\sin(\omega t)-ae^{-at}].
$$

For the second moment, $2um_1=LUg\cos(\omega t)[1-\cos(2ky)]$. Thus $m_2=A(t)+B(t)\cos(2ky)$, with

$$
A'=2\kappa L+LUg\cos(\omega t),\qquad
B'+4aB=-LUg\cos(\omega t),\qquad A(0)=L^3/12,\quad B(0)=0.
$$

The equation for $B$ has positive damping and bounded forcing, so $B$ remains bounded. In the equation for $A$, the decaying term in $g$ contributes only a bounded accumulated transient. Over a complete nonzero-frequency cycle, $\langle\cos^2(\omega t)\rangle_t=1/2$ and $\langle\sin(\omega t)\cos(\omega t)\rangle_t=0$. Consequently

$$
A(t)=\left[2\kappa L+\frac{LU^2a}{2(a^2+\omega^2)}\right]t+O(1),
\qquad
\boxed{m_2(y,t)=2Ktm_0+O(1),\quad K=\kappa+\frac{U^2a}{4(a^2+\omega^2)}.}
$$

This proves [oscillating shear dispersion in an insulating channel](../../../fluid-mechanics.md#oscillating-shear-dispersion-in-an-insulating-channel), including the local-in-$y$ leading term, not just a cross-channel average. The instantaneous derivative retains bounded periodic oscillations; its cycle-averaged slope is $2Km_0$. Thus $2Ktm_0$ is the leading second moment, rather than a literal rate proportional to $t$.

The asymptotic statement holds for fixed positive [diffusivity](../../../brownian-motion.md#diffusion-coefficient) and fixed nonzero frequency, after times long compared with $a^{-1}$ and the oscillation period. If $|\omega|L^2/\kappa\ll1$, transverse [diffusion](../../../thermodynamics.md#diffusion) adjusts rapidly to the changing [shear flow](../../../fluid-mechanics.md#shear-flow), and

$$
K\simeq\kappa+\frac{U^2L^2}{4\pi^2\kappa}.
$$

This is the cycle average of the instantaneous steady-shear enhancement $U^2\cos^2(\omega t)/(2a)$. At exactly $\omega=0$, there is no cycle average: $g\to U/a$ and $K=\kappa+U^2/(2a)$. Hence the zero-frequency and long-time limits do not commute. In the intermediate range $a^{-1}\ll t\ll|\omega|^{-1}$, the shear is approximately steady at its initial amplitude and that latter enhancement is appropriate.

## 2

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $a=\Lambda T$. The [deformation gradient](../../../continuum-mechanics.md#deformation-gradient) of one interval of [shear flow](../../../fluid-mechanics.md#shear-flow) is $S(a)=\begin{pmatrix}1&a\\0&1\end{pmatrix}$. An initial unit [material line](../../../fluid-mechanics.md#material-curve) at angle $\theta$ therefore becomes $(\cos\theta+a\sin\theta,\sin\theta)$. Its orientation, including the correct quadrant, is

$$
\boxed{\theta_T=\operatorname{atan2}(\sin\theta,\cos\theta+a\sin\theta),\quad
\ell(\theta)=\sqrt{1+a\sin2\theta+a^2\sin^2\theta}.}
$$

For an unoriented line the angle is taken modulo $\pi$. If $\Lambda=0$, there is no [shear flow](../../../fluid-mechanics.md#shear-flow): every $\lambda_N=1$ and $\mu=0$. The fluctuation and maximizing calculations below concern nonzero shear.

To quantify the [renovating shear flow](../../../fluid-mechanics.md#renovating-shear-flow), use the intended isotropic model: each shear orientation is independent and uniform modulo $\pi$. Independence by itself does not specify a probability law and cannot fix the answer. Under the uniform law, conditional on every earlier deformation, the relative angle to the next shear is again uniform. Thus the logarithmic increments $\xi_n=\log\ell(\theta_n)$ are independent and identically distributed, even though the absolute orientation of the stretched [material line](../../../fluid-mechanics.md#material-curve) need not be uniform. Since $\log\lambda_N=\sum_{n=1}^N\xi_n$, only the one-step angular mean is needed.

Write $\ell^2=A+B\cos(2\theta-\delta)$, where $A=1+a^2/2$, $B=|a|\sqrt{1+a^2/4}$ and $A^2-B^2=1$. The supplied angular logarithmic integral, with parameter $B/A$, gives

$$
r(a):=\langle\xi\rangle=\frac12\log\frac{A+\sqrt{A^2-B^2}}2
=\frac12\log(1+a^2/4).
$$

Therefore **the mean logarithmic stretching rate** is

$$
\boxed{\mu=\frac{\log(1+\Lambda^2T^2/4)}{2T}
=|\Lambda|\frac{\log(1+a^2/4)}{2|a|}.}
$$

This is the [mean logarithmic stretching in an isotropic renovating shear](../../../fluid-mechanics.md#mean-logarithmic-stretching-in-an-isotropic-renovating-shear), and the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives the same almost-sure [Lyapunov exponent](../../../dynamical-systems.md#lyapunov-exponent). Taking $\Lambda>0$ without loss for this statistic puts it in the requested form $\Lambda F(\Lambda T)$.

For $b=|\Lambda|T$, $F(b)=\log(1+b^2/4)/(2b)$. At small $b$, $\mu=\Lambda^2T/8+O(\Lambda^4T^3)$; at large $b$, $\mu\sim\log(b/2)/T$, tending to zero when $T$ increases at fixed shear rate. The maximizing nonzero $b$ solves

$$
\log z=2(1-z^{-1}),\qquad z=1+b^2/4.
$$

The difference $2(1-z^{-1})-\log z$ rises from zero up to $z=2$ and then strictly decreases to $-\infty$, so there is exactly one root beyond $2$. Numerically,

$$
\boxed{|\Lambda|T\simeq3.9605826,\qquad \mu_{\max}\simeq0.2012|\Lambda|.}
$$

Very rapid renovation gives little deformation per interval and cancels the first-order mean stretch. Long intervals provide strong deformation but progressively align a [material line](../../../fluid-mechanics.md#material-curve) with the shear direction, so one interval stretches it only algebraically in $T$. Intermediate persistence combines substantial deformation with frequent reorientation, producing the finite maximum.

For the distribution, let $\gamma=\operatorname{arsinh}(|a|/2)$, so the singular stretches of $S(a)$ are $e^{\pm\gamma}$. In the right-singular-vector basis, $\ell^2=e^{2\gamma}\cos^2\varphi+e^{-2\gamma}\sin^2\varphi$. Put $q=\tanh\gamma=|a|/\sqrt{a^2+4}$. Factoring this expression and expanding its logarithm gives

$$
\xi=r(a)+\sum_{j=1}^{\infty}\frac{(-1)^{j+1}q^j}{j}\cos(2j\varphi),\qquad
v(a):=\operatorname{Var}\xi=\frac12\sum_{j=1}^{\infty}\frac{q^{2j}}{j^2}.
$$

The variance follows from angular orthogonality. These bounded independent increments imply

$$
\boxed{\frac{\log\lambda_N-Nr(a)}{\sqrt{Nv(a)}}\ \Longrightarrow\ N(0,1).}
$$

Accordingly the central part of the large-$N$ stretch distribution is approximately described by a [log-normal distribution](../../../probability-theory.md#log-normal-distribution), with density $[\lambda\sqrt{2\pi Nv}]^{-1}\exp[-(\log\lambda-Nr)^2/(2Nv)]$. This [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) is not an assertion about arbitrarily extreme tails: the exact stretch has support inside $e^{-N\gamma}\leq\lambda_N\leq e^{N\gamma}$.

For $|a|\ll1$, the [log-stretch fluctuations in an isotropic renovating shear](../../../fluid-mechanics.md#log-stretch-fluctuations-in-an-isotropic-renovating-shear) have

$$
r(a)=\frac{a^2}{8}-\frac{a^4}{64}+O(a^6),\qquad
v(a)=\frac{a^2}{8}-\frac{3a^4}{128}+O(a^6).
$$

To leading order the mean and variance of $\log\lambda_N$ both equal $Na^2/8$. Typical stretch is $\exp(Na^2/8)$, while its mean grows as $\exp(3Na^2/16)$. These moment statements can be justified directly rather than extrapolating the central Gaussian approximation: expansion of $\ell^p$ gives

$$
\langle\ell^p\rangle=1+\frac{p(p+2)}{16}a^2+O(a^4),\qquad
\boxed{\langle\lambda_N^p\rangle=\exp\left[\frac{Np(p+2)a^2}{16}+O(Na^4)\right]}
$$

for fixed $p$. In particular $\langle\lambda_N^2\rangle=(1+a^2/2)^N$ exactly. The leading small-$a$ log-normal approximation is especially precise in the many-small-renovations scaling with $Na^2$ fixed and $Na^4\to0$.

If the orientation law is not isotropic these formulas need not hold. For example, repeating a fixed shear direction gives $S(a)^N=S(Na)$, only algebraic stretch, and zero asymptotic logarithmic rate. The associated degenerate direction variables are independent, illustrating why the stated independence condition alone is insufficient to select the isotropic result.

## 3

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The unperturbed [sinusoidal cellular flow](../../../fluid-mechanics.md#sinusoidal-cellular-flow) has

$$
\mathbf u_0=(\sin x\cos y,-\cos x\sin y),\qquad
\frac{d\psi_0}{dt}=\nabla\psi_0\cdot\mathbf u_0=0.
$$

Its [stream function](../../../fluid-mechanics.md#stream-function) is a [first integral](../../../differential-equation.md#first-integral), so each trajectory lies on a level set of $\psi_0$. This planar autonomous [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) has one degree of freedom and its conserved quantity reduces motion on regular levels to a quadrature: this is its integrability. The central cell has closed [streamlines](../../../fluid-mechanics.md#streamline); the zero level is the grid of [separatrices](../../../dynamical-systems.md#separatrix).

Solving both components of $\mathbf u_0=0$ gives [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium) at $(n\pi,m\pi)$ and [center equilibria](../../../dynamical-systems.md#center-equilibrium) at $(\pi/2+n\pi,\pi/2+m\pi)$. In the specified open square, the saddles are $(0,0),(\pi,0),(0,\pi),(\pi,\pi)$ and the only interior center is $(\pi/2,\pi/2)$. Centers at the outer square's corners are on its excluded boundary.

At a saddle the [Jacobian matrix](../../../calculus.md#jacobian-matrix) is $\operatorname{diag}(s,-s)$ with $s=(-1)^{n+m}$. If $n+m$ is even, the horizontal branches are unstable and vertical branches stable; if it is odd, those roles reverse. The branches extend along $y=m\pi$ and $x=n\pi$ and connect neighboring saddles as [heteroclinic orbits](../../../dynamical-systems.md#heteroclinic-orbit). For example the bottom boundary flows from $(0,0)$ to $(\pi,0)$, the right boundary from $(\pi,0)$ to $(\pi,\pi)$, the top boundary from $(\pi,\pi)$ to $(0,\pi)$, and the left boundary returns to $(0,0)$. A connecting branch is unstable relative to its departing saddle and stable relative to its arriving saddle.

At a center the [Jacobian matrix](../../../calculus.md#jacobian-matrix) is $\begin{pmatrix}0&-s\\s&0\end{pmatrix}$, where now $s=\sin x\sin y=\pm1$. Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\pm i$. The local definite extremum of $\psi_0$ surrounds it by closed [streamlines](../../../fluid-mechanics.md#streamline), giving a neutrally stable center, not an attracting equilibrium. Central circulation is counterclockwise and adjoining cells have alternating circulation.

<a id="3/i/image-unperturbed-cellular-streamlines-four-interior-saddles-and-stable-and-unstable-branches"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-46-cellular-flow.png)

**[Figure 1](#3/i/image-unperturbed-cellular-streamlines-four-interior-saddles-and-stable-and-unstable-branches). Unperturbed cellular streamlines, four interior saddles, and stable and unstable branches**.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Use a [Poincaré map](../../../dynamical-systems.md#poincare-map) sampled once per forcing period. A hyperbolic periodic trajectory has [stable manifolds](../../../dynamical-systems.md#stable-manifold) containing parcels that approach it under forward iteration and [unstable manifolds](../../../dynamical-systems.md#unstable-manifold) containing parcels that approach it under backward iteration. In the integrable limit the relevant branches coincide along a [heteroclinic orbit](../../../dynamical-systems.md#heteroclinic-orbit) and form a barrier between neighboring cells.

A transverse crossing in the perturbed map means that this barrier has split: a parcel on the intersection belongs to both asymptotic manifolds, and adjoining branches enclose fluid lobes transported across the former boundary. Iteration stretches and folds those lobes. In the connected heteroclinic network this creates complicated intercell transport and [chaotic advection](../../../fluid-mechanics.md#chaotic-advection). The crossing is between invariant curves at the same forcing phase; it does not mean that different trajectories cross at one time in violation of uniqueness.

The [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) gives an [area-preserving map](../../../dynamical-systems.md#area-preserving-map), so lobe exchange preserves parcel area. Without [diffusion](../../../thermodynamics.md#diffusion), an advected [passive scalar](../../../fluid-mechanics.md#passive-scalar) also keeps its value on each trajectory. Therefore manifold intersections can generate fine filaments and efficient advective exchange but do not by themselves produce molecular homogenization, nor prove that every region of the flow becomes chaotic.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Put $A(t)=D\mathbf u_0(\mathbf q_0(t-t_0))$ and $\mathbf w(t)=\nabla\psi_0(\mathbf q_0(t-t_0))$. Expansion of the trajectory equation to first order gives, for either correction,

$$
\dot{\mathbf q}_1=A\mathbf q_1+\mathbf u_1(\mathbf q_0(t-t_0),t).
$$

Since the unperturbed [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) obeys $\nabla\psi_0\cdot\mathbf u_0=0$, differentiation with respect to position yields $D^2\psi_0\,\mathbf u_0+(D\mathbf u_0)^T\nabla\psi_0=0$. Along the [heteroclinic orbit](../../../dynamical-systems.md#heteroclinic-orbit) this says $\dot{\mathbf w}=-A^T\mathbf w$. Therefore the homogeneous terms cancel:

$$
\frac d{dt}(\mathbf w\cdot\mathbf q_1)
=(-A^T\mathbf w)\cdot\mathbf q_1+\mathbf w\cdot(A\mathbf q_1+\mathbf u_1)
=\mathbf w\cdot\mathbf u_1.
$$

The unperturbed orbit approaches its [hyperbolic fixed points](../../../dynamical-systems.md#hyperbolic-equilibrium-point) exponentially, so $\mathbf w\to0$ at either appropriate endpoint. The selected stable and unstable corrections remain bounded there, approaching the first-order corrections to the periodic trajectories. Their endpoint dot products consequently vanish. Integrating the stable correction forward and the unstable correction backward gives

$$
\begin{aligned}
\mathbf w(t_0)\cdot\mathbf q_1^s(t_0,t_0)&=-\int_{t_0}^\infty\mathbf w(\tau)\cdot\mathbf u_1(\mathbf q_0(\tau-t_0),\tau)\,d\tau,\\
\mathbf w(t_0)\cdot\mathbf q_1^u(t_0,t_0)&=\int_{-\infty}^{t_0}\mathbf w(\tau)\cdot\mathbf u_1(\mathbf q_0(\tau-t_0),\tau)\,d\tau.
\end{aligned}
$$

Subtracting proves the [heteroclinic Melnikov function for a periodic planar flow](../../../dynamical-systems.md#heteroclinic-melnikov-function-for-a-periodic-planar-flow):

$$
\boxed{M(\mathbf X_0,t_0)=\int_{-\infty}^{\infty}\nabla\psi_0(\mathbf q_0(\tau-t_0))\cdot\mathbf u_1(\mathbf q_0(\tau-t_0),\tau)\,d\tau.}
$$

Choose a regular point on the connection where $\nabla\psi_0\ne0$. The first-order signed normal distance between the perturbed invariant curves is $\epsilon M/|\nabla\psi_0|+O(\epsilon^2)$. If $M$ has a simple zero in the along-orbit parameter, the [implicit function theorem](../../../calculus.md#implicit-function-theorem) continues it to a zero of the actual distance for sufficiently small $\epsilon$, with nonzero derivative. The curves consequently cross transversely rather than touching tangentially.

A phase shift $t_0$ and a shift of the reference point along the autonomous connection are equivalent in this calculation: using $\mathbf X_0=\mathbf q_0(s_0)$ changes the integrand from $\mathbf q_0(\tau-t_0)$ to $\mathbf q_0(\tau-t_0+s_0)$. Thus a simple phase zero can also describe a crossing along the connection at a fixed forcing phase. These are intersections of the **perturbed** [stable manifolds](../../../dynamical-systems.md#stable-manifold) and [unstable manifolds](../../../dynamical-systems.md#unstable-manifold). The word “unperturbed” in the printed conclusion cannot be literal: those branches coincide before perturbation and have no transverse splitting.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

On $y=0$, the unperturbed trajectory satisfies $\dot x=\sin x$. Put $a_0=\log\tan(X_0/2)$. Integration with $x(0)=X_0$ gives

$$
x(s)=2\arctan e^{s+a_0},\qquad \sin x(s)=\operatorname{sech}(s+a_0),\qquad \cos x(s)=-\tanh(s+a_0).
$$

It runs from $(0,0)$ to $(\pi,0)$, so it is the appropriate [heteroclinic orbit](../../../dynamical-systems.md#heteroclinic-orbit). From the perturbed [stream function](../../../fluid-mechanics.md#stream-function),

$$
\mathbf u_1=(\cos x\sin y,-\sin x\cos y)\sin(\omega t).
$$

On the chosen connection, $\nabla\psi_0=(0,-\sin x)$; hence the scalar product in the [heteroclinic Melnikov function for a periodic planar flow](../../../dynamical-systems.md#heteroclinic-melnikov-function-for-a-periodic-planar-flow) is $\sin^2x\sin(\omega t)$. Therefore

$$
M(X_0,t_0)=\int_{-\infty}^{\infty}\operatorname{sech}^2(\tau-t_0+a_0)\sin(\omega\tau)\,d\tau.
$$

Set $s=\tau-t_0+a_0$. The odd term $\operatorname{sech}^2s\sin(\omega s)$ integrates to zero, leaving the supplied even Fourier integral multiplied by $\sin[\omega(t_0-a_0)]$. Thus

$$
\boxed{M(X_0,t_0)=\frac{\pi\omega}{\sinh(\pi\omega/2)}\sin\left[\omega\left(t_0-\log\tan\frac{X_0}{2}\right)\right].}
$$

For every fixed $\omega\ne0$ the amplitude is nonzero and the phase zeros are simple: $\partial_{t_0}M$ there is $\pm\pi\omega^2/\sinh(\pi\omega/2)\ne0$. At fixed phase, varying $X_0$ also gives simple zeros because $da_0/dX_0=1/\sin X_0$ is nonzero for $0<X_0<\pi$. The [Melnikov splitting of a periodically perturbed cellular flow](../../../fluid-mechanics.md#melnikov-splitting-of-a-periodically-perturbed-cellular-flow) therefore produces transverse manifold intersections at sufficiently small perturbation and fluid-lobe exchange between adjacent cells. The unperturbed separatrix is no longer a material transport barrier.

At high frequency the leading splitting amplitude is asymptotic to $2\pi|\omega|e^{-\pi|\omega|/2}$, so fast forcing has an exponentially weak first-order effect on this connection. This is a fixed-frequency, small-$\epsilon$ result; an exponentially small leading term need not dominate higher orders in a simultaneous high-frequency limit. At exactly $\omega=0$ the perturbation itself vanishes and $M=0$, so the nonzero-frequency conclusion does not apply. Manifold splitting demonstrates intercell [chaotic advection](../../../fluid-mechanics.md#chaotic-advection) locally, not a proof of uniform mixing or ordinary [diffusion](../../../thermodynamics.md#diffusion) throughout the entire domain.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
