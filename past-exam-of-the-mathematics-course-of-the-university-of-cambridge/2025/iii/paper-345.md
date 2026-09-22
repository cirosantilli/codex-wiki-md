# Paper 345

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_345.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_345.pdf)

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
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)

## 1

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let the velocity perturbation be $(u,w)$, pressure perturbation be $p$, and density perturbation be $\rho'$ about the hydrostatic background $\hat\rho(z)$. The linearized inviscid [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) gives

$$
u_x+w_z=0,\qquad
\rho'_t+w\hat\rho_z=0,\qquad
u_t=-p_x/\rho_0,\qquad
w_t=-p_z/\rho_0-g\rho'/\rho_0.
$$

Stable stratification means $\hat\rho_z<0$, and the [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency) is

$$
\boxed{N^2=-\frac g{\rho_0}\frac{d\hat\rho}{dz}>0}.
$$

Differentiate the momentum equations to eliminate $p$, use incompressibility, and then use the density equation to eliminate $\rho'$. This yields

$$
\boxed{\left[\left(\partial_x^2+\partial_z^2\right)\partial_t^2+N^2\partial_x^2\right]w=0}.
$$

For $w\propto e^{i(kx+mz-\omega t)}$, the [internal gravity wave](../../../gravity-wave.md#internal-wave) dispersion relation is $\omega^2=N^2k^2/(k^2+m^2)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A localized monochromatic cylinder emits four narrow beams, one in each quadrant, forming a St Andrew's cross. If $\alpha$ is the beam angle to the horizontal,

$$
\boxed{\sin\alpha=\omega/N};
$$

equivalently, its angle $\theta=\pi/2-\alpha$ to the vertical obeys $\cos\theta=\omega/N$. As $\omega$ rises from zero to $N$, the beams rotate from horizontal toward vertical. For $\omega>N$ no freely propagating internal wave exists and the response is evanescent.

The wavevector and [phase velocity](../../../wave-equation.md#phase-velocity) are parallel. The dispersion relation is homogeneous of degree zero in $(k,m)$, so Euler's theorem gives $\mathbf k\mathbin{\cdot}\mathbf c_g=0$: the [group velocity](../../../wave-equation.md#group-velocity) is perpendicular to both the wavevector and phase velocity. Energy travels along the beams in the group-velocity direction.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $\mu=\tan\theta=m/k$. The incident down-right ray from $(0,s)$ has slope $-\cot\theta$ and meets the parabolic bottom $H(x)=2x^2$ at $x=x_0\in(0,1/2)$ provided

$$
\boxed{s=2x_0^2+x_0\cot\theta}.
$$

At the impact point the bottom slope is $S=H'(x_0)=4x_0$. A stationary reflection preserves frequency and tangential wavenumber $k+Sm$. For the incident wavevector $(k,m)=a(1,\mu)$ and a reflected up-left ray $(k_r,m_r)=a_r(-1,\mu)$, tangential matching gives

$$
a(1+S\mu)=a_r(S\mu-1).
$$

A positive reflected magnitude $a_r$ therefore exists exactly when $S\mu>1$. This is the supercritical-slope condition for [reflection of an internal-wave ray](../../../gravity-wave.md#reflection-of-an-internal-wave-ray) and produces a group velocity in the second quadrant.

Since $x_0<1/2$, such a point exists when

$$
\boxed{\arctan(1/2)<\theta\leq\pi/6}.
$$

For any such $\theta$, choose

$$
\frac1{4\tan\theta}<x_0<\frac12,
\qquad
\boxed{\frac{3}{8\tan^2\theta}<s<\frac12+\frac1{2\tan\theta}}.
$$

The initial ray then hits the parabola at a supercritical point and its reflected ray travels up and left, as required.

## 2

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume a hydrostatic, vertically well-mixed, inviscid shallow layer, negligible ambient horizontal velocity, and uniform channel width. Volume, mass, and horizontal momentum balances are

$$
h_t+(hu)_x=w_e-w_d,
$$



$$
(\rho_1h)_t+(\rho_1hu)_x=\rho_2w_e-\rho_1w_d,
$$



$$
(\rho_1hu)_t+\left(\rho_1hu^2+\frac12g(\rho_1-\rho_2)h^2\right)_x=-\rho_1u\,w_d.
$$

Combining the first two gives

$$
h(\rho_{1t}+u\rho_{1x})=(\rho_2-\rho_1)w_e.
$$

Detrainment removes fluid with the layer's own density and velocity, so it cancels from the corresponding material density and velocity equations; entrainment dilutes and exerts a momentum load.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Define the [reduced gravity](../../../reduced-gravity.md)

$$
g'=g\frac{\rho_1-\rho_2}{\rho_2},
$$

and use the Boussinesq limit $\rho_1\simeq\rho_2$ except in buoyancy. The balances become

$$
g'_t+ug'_x=-g'\frac{w_e}{h},
$$



$$
h_t+uh_x+hu_x=w_e-w_d,
$$



$$
u_t+uu_x+g'h_x+\frac h2g'_x=-u\frac{w_e}{h}.
$$

Thus, for $\mathbf q=(g',h,u)^T$,

$$
\boxed{
\mathbf q_t+
\begin{pmatrix}
u&0&0\\
0&u&h\\
h/2&g'&u
\end{pmatrix}\mathbf q_x
=
\begin{pmatrix}
-g'w_e/h\\
w_e-w_d\\
-uw_e/h
\end{pmatrix}},
$$

which is the required [entraining shallow-water layer](../../../reduced-gravity.md#entraining-shallow-water-layer) system.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put $c=\sqrt{g'h}$. The three real eigenvalues are

$$
\boxed{\lambda_0=u,\qquad\lambda_\pm=u\pm c},
$$

so the system is strictly hyperbolic for $g'h>0$. Along $dx/dt=u$,

$$
\boxed{\frac{D_0g'}{Dt}=-g'\frac{w_e}{h}}.
$$

Left eigenvectors for $\lambda_\pm$ are $(\pm h/(2c),\pm c/h,1)$, hence

$$
\boxed{
D_\pm u\pm\frac chD_\pm h\pm\frac h{2c}D_\pm g'
=\pm\frac ch\left(\frac{w_e}{2}-w_d\right)-u\frac{w_e}{h}},
$$

where $D_\pm=\partial_t+(u\pm c)\partial_x$.

When $w_e,w_d\to0$, reduced gravity is materially conserved. If it is initially uniform, it remains constant and the other two relations integrate to the standard [Riemann invariants](../../../compressible-flow.md#riemann-invariant)

$$
\boxed{D_\pm(u\pm2\sqrt{g'h})=0}.
$$

## 3

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Taking the curl of the Boussinesq momentum equation and using incompressibility gives the [vorticity equation](../../../physics.md#vorticity-equation)

$$
\boxed{
\partial_t\boldsymbol\omega+(\mathbf u\mathbin{\cdot}\nabla)\boldsymbol\omega
=(\boldsymbol\omega\mathbin{\cdot}\nabla)\mathbf u
+\nabla\left(\frac{\rho'}{\rho_0}\right)\times\mathbf g
+\nu\nabla^2\boldsymbol\omega}.
$$

The second term on the right is [baroclinic vorticity generation](../../../physics.md#baroclinic-vorticity-generation). It is nonzero where a horizontal density gradient crosses the vertical gravitational acceleration.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

In steady inviscid two-dimensional flow the spanwise vorticity obeys

$$
\mathbf u\mathbin{\cdot}\nabla\omega
=\left[\nabla(\rho'/\rho_0)\times\mathbf g\right]_y.
$$

Integrating this equation over the front-frame control volume converts the left side to vorticity flux through its upstream and downstream faces. For a sharp interface, the baroclinic source integrates to the circulation generated by the hydrostatic pressure jump, $g'h$. With plug flow downstream, the resulting balance is

$$
\frac12u_2^2=g'h,
\qquad
\boxed{u_2=\sqrt{2g'h}}.
$$

Volume conservation in the front frame gives $u_1H=u_2(H-h)$. The undisturbed indoor air is stationary in the laboratory, so $u_1$ is the front speed:

$$
\boxed{U_f=\frac{H-h}{H}\sqrt{2g'h}}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

With a long uniform corridor, constant depth, and negligible entrainment, the pressure head $g'h$ driving the [gravity current](../../../reduced-gravity.md#gravity-current) does not change as the nose advances. There is no growing geometric length in the local front balance, so dimensional analysis gives the constant velocity $U_f\propto\sqrt{g'h}$ after the short release transient.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The energy-conserving full-depth [lock-exchange flow](../../../reduced-gravity.md#lock-exchange-flow) is symmetric between the cold lower current and warm upper return current, so

$$
\boxed{h=H/2}.
$$

Part (b) then gives $u_2=\sqrt{g'H}$ and the laboratory front speed

$$
\boxed{U_f=\frac12\sqrt{g'H}}.
$$

During one opening, the cold current displaces the volume

$$
\boxed{V_{\rm ex}=WhU_f\,\delta t
=\frac{WH\,\delta t}{4}\sqrt{g'H}}.
$$

The same volume of warm air exits in the upper layer.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For an ideal gas in the Boussinesq limit,

$$
g'=g\frac{\hat\rho}{\rho_0}\simeq g\frac{T-T_0}{T_0}.
$$

Each opening removes $\rho_0c_pV_{\rm ex}(T-T_0)$ of heat. With $n$ openings per hour, the mean removal rate is $(n/3600)$ times this quantity. Equating it to $\dot q$ and writing $\Delta T=T-T_0$ gives

$$
\dot q=\frac n{3600}\frac{\rho_0c_pWH\delta t}{4}
\sqrt{\frac{gH}{T_0}}\,(\Delta T)^{3/2}.
$$

Therefore

$$
\boxed{
T=T_0+
\left[
\frac{14400\,\dot q}{n\rho_0c_pWH\delta t}
\sqrt{\frac{T_0}{gH}}
\right]^{2/3}}.
$$

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Mechanical mixing destroys the sharp density interface that supports efficient displacement ventilation. It entrains warm air into the incoming cold current and cold air into the outgoing current, reducing both reduced gravity and the heat removed per exchanged volume. Stopping fans or other mixing while the door is open therefore preserves the two-layer [lock-exchange flow](../../../reduced-gravity.md#lock-exchange-flow) and improves cooling efficiency.

## 4

↑ **Parent:** [Paper 345](paper-345.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) uses a constant reference density in inertia and continuity while retaining the small temperature-dependent density deficit in buoyancy. Here $(\rho_0-\rho)/\rho_0=(T-T_0)/T_0$, so the plume remains incompressible but rises under $g(T-T_0)/T_0$.

The [Batchelor entrainment hypothesis](../../../turbulent-plume.md#batchelor-entrainment-hypothesis) sets the ambient inflow speed at the exposed plume edge to $E W$, where $E$ is a dimensionless entrainment coefficient. For this one-sided [heated wall plume](../../../turbulent-plume.md#heated-wall-plume), it gives $dQ/dz=EW$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

With thermal diffusivity $\kappa_T$, temperature obeys

$$
T_t+uT_x+wT_z=\kappa_T(T_{xx}+T_{zz}).
$$

Scale $z$ with $h_0$, $x$ with $b_0=\epsilon h_0$, and $w$ with $w_0$. Continuity gives the cross-plume velocity scale $u_0\sim(b_0/h_0)w_0=\epsilon w_0$, so both advective terms scale as $w_0\Delta T/h_0$. Horizontal and vertical diffusion scale as $\kappa_T\Delta T/b_0^2$ and $\kappa_T\Delta T/h_0^2$, respectively. Their ratio is

$$
\boxed{\frac{\text{vertical diffusion}}{\text{horizontal diffusion}}=\frac{b_0^2}{h_0^2}=\epsilon^2\ll1}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For top-hat profiles, $Q=bW$, $M=bW^2$, and $\mathcal B=Q g(T-T_0)/T_0$. One-sided entrainment, vertical momentum, and the wall heat input give

$$
\boxed{Q'=E\frac MQ},\qquad
\boxed{M'=\mathcal B\frac QM}.
$$

Integrating the temperature equation across the plume gives

$$
\frac d{dz}[Q(T-T_0)]=\frac{q_0}{\rho_0c_p}.
$$

Combining this with the definition of buoyancy flux yields

$$
\boxed{\mathcal B'=\beta},
\qquad
\boxed{\beta=\frac{gq_0}{\rho_0c_pT_0}},
\qquad
\mathcal B(z)=\mathcal B_0+\beta z.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Far above the source, $\mathcal B\sim\beta z$. Suppose $Q\sim z^p$ and $M\sim z^r$. The first integral equation gives $p-1=r-p$, while the second gives $r-1=1+p-r$. Solving,

$$
\boxed{p=\frac43,\qquad r=\frac53}.
$$

Hence

$$
\boxed{Q\sim z^{4/3},\qquad M\sim z^{5/3}}.
$$

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Introduce the virtual-origin coordinate

$$
\zeta=z+z_0,\qquad z_0=\frac{\mathcal B_0}{\beta},
$$

so that $\mathcal B=\beta\zeta$. Seek $Q=A\zeta^{4/3}$ and $M=C\zeta^{5/3}$. Substitution gives

$$
A=\left(\frac{27E^2\beta}{80}\right)^{1/3},
\qquad
C=\left(\frac{27E\beta^2}{100}\right)^{1/3}.
$$

Therefore the exact similarity solution is

$$
\boxed{Q=A\zeta^{4/3}},\qquad
\boxed{M=C\zeta^{5/3}},
$$



$$
\boxed{W=\frac MQ=\left(\frac{4\beta}{5E}\right)^{1/3}\zeta^{1/3}},
\qquad
\boxed{b=\frac{Q^2}{M}=\frac{3E}{4}\zeta},
$$

and

$$
\boxed{T-T_0=\frac{T_0\mathcal B}{gQ}
=\frac{T_0\beta}{gA}\zeta^{-1/3}}.
$$

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

At the source, $\zeta=z_0=\mathcal B_0/\beta$. The initial width required to lie exactly on the similarity solution is therefore

$$
\boxed{b_0=\frac{3E}{4}z_0
=\frac{3E\mathcal B_0}{4\beta}
=\frac{3E\rho_0c_pT_0\,\mathcal B_0}{4gq_0}}.
$$

The corresponding $Q_0=A z_0^{4/3}$ and $M_0=C z_0^{5/3}$ are the compatible initial fluxes stipulated in the question.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
