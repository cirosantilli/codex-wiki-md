# Paper 8

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_8.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_8.pdf)

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
  - [f](#1/f)
    - [Solution](#1/f/solution)
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

## 1

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $z=(x,v)$ and let $\Phi(t,s,z)$ denote the [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) from time $s$ to time $t$. The [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) satisfy [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations):

$$
\boxed{\dot X_i(t)=\partial_{v_i}H(t,X(t),V(t)),\qquad
\dot V_i(t)=-\partial_{x_i}H(t,X(t),V(t)),\qquad
(X(s),V(s))=(x,v).}
$$

The [Hamiltonian Liouville equation](../../../statistical-physics.md#hamiltonian-liouville-equation) then reduces along each curve to

$$
\frac d{dt}f(t,X(t),V(t))=h(t,X(t),V(t)).
$$

The signs and derivative variables here are those in the PDF.

The [global characteristic flow for a Hamiltonian with bounded Hessian](../../../classical-mechanics.md#global-characteristic-flow-for-a-hamiltonian-with-bounded-hessian) follows, for example, from $H\in C^2(\mathbb R\times\mathbb R^{2d})$ and, for every finite $T$,

$$
\sup_{|t|\leq T,\ z\in\mathbb R^{2d}}\|D_z^2H(t,z)\|\leq L_T<\infty,\qquad
\sup_{|t|\leq T}|\nabla_zH(t,0)|\leq A_T<\infty.
$$

Thus the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) $b=(\nabla_vH,-\nabla_xH)$ is globally [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity) in $z$ on each finite time interval and satisfies $|b(t,z)|\leq A_T+L_T|z|$. The [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem) gives local existence and uniqueness, while the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) gives, for example,

$$
|\Phi(t,s,z)|\leq (|z|+A_T|t-s|)e^{L_T|t-s|}
\qquad(|s|,|t|\leq T).
$$

This excludes finite-time escape. **There is a unique [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) for all finite forward and backward times**, and $\Phi(s,t)$ is the inverse of $\Phi(t,s)$. These sufficient conditions are deliberately stronger than necessary.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $S_t(z)=\Phi(t,0,z)$, differentiability with respect to initial data gives the variational equation

$$
Y'(t)=D_zb(t,S_t(z))Y(t),\qquad Y(0)=I_{2d},\qquad Y(t)=D_zS_t(z).
$$

The [Jacobi determinant derivative formula](../../../linear-algebra.md#jacobi-determinant-derivative-formula) gives

$$
J'(t)=\operatorname{tr}(D_zb(t,S_t(z)))J(t)
=(\operatorname{div}_zb)(t,S_t(z))J(t).
$$

The mixed derivatives in the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) cancel:

$$
\operatorname{div}_zb
=\sum_{i=1}^d\bigl(\partial_{x_i}\partial_{v_i}H
-\partial_{v_i}\partial_{x_i}H\bigr)=0.
$$

Consequently $J'(t)=0$, and $J(0)=1$ gives **preservation of [phase space](../../../classical-mechanics.md#phase-space) volume**:

$$
\boxed{\det D_zS_t(z)=1.}
$$

The same argument applies to $\Phi(t,s)$ for every starting time $s$. This is the [Liouville theorem in Hamiltonian mechanics](../../../classical-mechanics.md#liouville-s-theorem-hamiltonian). Explicit time dependence of $H$ does not affect the cancellation.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For an autonomous [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function), the [chain rule](../../../calculus.md#chain-rule) and [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) give

$$
\frac d{dt}H(X(t),V(t))
=\nabla_xH\cdot\nabla_vH-\nabla_vH\cdot\nabla_xH=0.
$$

Thus **the [energy](../../../classical-mechanics.md#energy) is constant along each characteristic**:

$$
\boxed{H(X(t),V(t))=H(x,v).}
$$

The time-independent hypothesis is implicit in the displayed expression in this subpart. For the time-dependent [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) allowed earlier, the correct [Hamiltonian energy balance](../../../classical-mechanics.md#hamiltonian-energy-balance) is instead

$$
\boxed{\frac d{dt}H(t,X(t),V(t))=\partial_tH(t,X(t),V(t)).}
$$

For example $H(t,x,v)=t+|v|^2/2$ has a unique global [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow), but its value along a curve increases at unit rate. Thus conservation cannot be claimed for arbitrary time-dependent $H$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Assume $\omega\ne0$. With $h=0$, the [method of characteristics](../../../partial-differential-equation.md#method-of-characteristics) gives $f(t,\Phi(t,0,z))=f_0(z)$. Hence

$$
\operatorname{supp}f_t=\Phi(t,0,\operatorname{supp}f_0).
$$

Let $K=\operatorname{supp}f_0$ and $E_*=\max_KH_\omega$; if $f_0=0$, the conclusion is immediate. By the [Hamiltonian energy balance](../../../classical-mechanics.md#hamiltonian-energy-balance), every image point of $K$ remains in the [energy](../../../classical-mechanics.md#energy) sublevel

$$
\mathcal K=\{(x,v):|v|^2+\omega^2|x|^2\leq2E_*\}.
$$

This is a fixed compact [ellipsoid](../../../geometry-and-topology.md#ellipsoid) in [phase space](../../../classical-mechanics.md#phase-space). Therefore **the [support](../../../function.md#support) bound is uniform in time**:

$$
\boxed{\operatorname{supp}f_t\subseteq\mathcal K,\qquad
|v|\leq\sqrt{2E_*},\quad |x|\leq\frac{\sqrt{2E_*}}{|\omega|}.}
$$

This [uniform support bound from a coercive conserved energy](../../../classical-mechanics.md#uniform-support-bound-from-a-coercive-conserved-energy) requires no explicit solution of the curves.

The nonzero-frequency qualification is necessary. At $\omega=0$ the [energy](../../../classical-mechanics.md#energy) does not control $x$, and the equation is [free transport equation](../../../partial-differential-equation.md#free-transport-equation). Choose a smooth [compactly supported](../../../function.md#compact-support) $f_0$ that is nonzero at $(x_0,v_0)$ with $v_0\ne0$. Its transported value at $(x_0+tv_0,v_0)$ stays nonzero, so the union of the supports is unbounded. Each individual [support](../../../function.md#support) is compact, but there is no fixed [compact support](../../../function.md#compact-support) for all times.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For the [isotropic harmonic oscillator flow](../../../classical-mechanics.md#isotropic-harmonic-oscillator-flow), [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) are $\dot X=V$, $\dot V=-\omega^2X$. In dimension three these are three identical uncoupled pairs. For $\omega\ne0$, put $c_t=\cos(\omega t)$, $s_t=\sin(\omega t)$. The solution from $(x,v)$ at time zero is

$$
\boxed{X(t)=c_tx+\frac{s_t}{\omega}v,\qquad
V(t)=-\omega s_tx+c_tv.}
$$

The inverse flow is obtained by replacing $t$ by $-t$:

$$
S_{-t}(x,v)=\left(c_tx-\frac{s_t}{\omega}v,\ \omega s_tx+c_tv\right).
$$

Integrating the source along the backward characteristic gives the [Duhamel formula for Hamiltonian transport](../../../statistical-physics.md#duhamel-formula-for-hamiltonian-transport):

$$
\boxed{f(t,x,v)=
f_0\!\left(c_tx-\frac{s_t}{\omega}v,\ \omega s_tx+c_tv\right)
+\int_0^t h\!\left(s,\ c_{t-s}x-\frac{s_{t-s}}{\omega}v,\
\omega s_{t-s}x+c_{t-s}v\right)\,ds.}
$$

Indeed $f(t,S_tz)=f_0(z)+\int_0^th(s,S_sz)\,ds$, and setting $z=S_{-t}(x,v)$ gives the formula. It has the prescribed initial value and differentiation along the characteristic gives the source.

The zero-frequency limit has $s_t/\omega\to t$, $\omega s_t\to0$, so $S_t(x,v)=(x+tv,v)$ and

$$
\boxed{f(t,x,v)=f_0(x-tv,v)+\int_0^th(s,x-v(t-s),v)\,ds\qquad(\omega=0).}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

For the globally invertible [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) from (a), the general characteristic formula is

$$
f(t,z)=f_0(\Phi(0,t,z))+\int_0^t h(\Phi(s,t,z))\,ds.
$$

Every $\Phi(s,t)$ preserves [Lebesgue measure](../../../measure-theory.md#lebesgue-measure), by (b). Thus composition with it is an [isometry](../../../riemannian-geometry.md#isometry) of each [Lp space](../../../measure-theory.md#lp-space). The [Minkowski integral inequality](../../../functional-analysis.md#minkowski-integral-inequality) gives

$$
\boxed{\|f(t)\|_p\leq\|f_0\|_p+t\|h\|_p.}
$$

Applying the [Minkowski inequality](../../../real-analysis.md#minkowski-inequality) also in time yields **the [finite-time Lp bound for Hamiltonian transport](../../../statistical-physics.md#finite-time-lp-bound-for-hamiltonian-transport)**:

$$
\boxed{\|f\|_{L^p([0,T]\times\mathbb R^{2d})}
\leq T^{1/p}\|f_0\|_p+
\left(\frac{T^{p+1}}{p+1}\right)^{1/p}\|h\|_p<\infty.}
$$

The smoothness assumptions allow the characteristic construction; the norm estimate itself only uses the [Lp space](../../../measure-theory.md#lp-space) data and volume preservation.

For a concrete failure on infinite time, choose $\omega=1$, $f_0=0$, and

$$
h(x,v)=e^{-(|x|^2+|v|^2)/2}=e^{-H_1(x,v)}.
$$

This is smooth, time independent and in every finite [Lp space](../../../measure-theory.md#lp-space); it is invariant under the [isotropic harmonic oscillator flow](../../../classical-mechanics.md#isotropic-harmonic-oscillator-flow). Therefore **the solution grows linearly**:

$$
\boxed{f(t,x,v)=t\,h(x,v),\qquad
\int_0^\infty\|f(t)\|_p^p\,dt
=\|h\|_p^p\int_0^\infty t^p\,dt=\infty.}
$$

This [invariant-source secular growth in Hamiltonian transport](../../../statistical-physics.md#invariant-source-secular-growth-in-hamiltonian-transport) supplies the counterexample even with zero initial data.

## 2

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Fix $t,x$. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) in the integration variable $v_*$ gives

$$
|K_tg(x,v)|^2
\leq\left(\int_{\mathbb R^d}|k(t,x,v,v_*)|^2\,dv_*\right)
\left(\int_{\mathbb R^d}|g(x,v_*)|^2\,dv_*\right).
$$

Integrate first in $v$, then in $x$. The uniform kernel hypothesis bounds the first factor after velocity integration by $C^2$, independently of $t,x$. Hence

$$
\boxed{\|K_tg\|_{L^2_{x,v}}^2\leq C^2\|g\|_{L^2_{x,v}}^2,\qquad \|K_t\|\leq C.}
$$

The [linear Boltzmann collision operator](../../../statistical-physics.md#linear-boltzmann-collision-operator) is linear by its integral definition, so this proves it is a [bounded linear operator](../../../topological-vector-space.md#continuous-linear-operator) on $L^2_{x,v}$. The estimate is the [Hilbert-Schmidt kernel bound](../../../compact-operator.md#hilbert-schmidt-kernel-bound) applied at each spatial point. The printed real-kernel square is $|k|^2$ for a complex kernel. Measurability of the coefficients is understood so that the displayed integrals are defined.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

[Free transport equation](../../../partial-differential-equation.md#free-transport-equation) is the measure-preserving shear $(x,v)\mapsto(x-vs,v)$. Its composition operator preserves the $L^2_{x,v}$ norm. Since $a\geq0$, the damping multiplier has modulus at most one:

$$
0\leq\exp\!\left(-\int_0^s a(r,x-v(s-r),v)\,dr\right)\leq1.
$$

Consequently **the [damped free-transport evolution](../../../statistical-physics.md#damped-free-transport-evolution) is contractive**:

$$
\boxed{\|F(f_0,a)(s)\|_2\leq\|f_0\|_2,\qquad
\sup_{0\leq s\leq t}\|F(f_0,a)(s)\|_2\leq\|f_0\|_2.}
$$

This needs no upper bound on $a$. Nonnegative integrals may be interpreted in the extended sense with $e^{-\infty}=0$; local integrability along characteristics additionally gives the usual continuous initial trace.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Denote the [damped free-transport evolution](../../../statistical-physics.md#damped-free-transport-evolution) from time $s$ to time $t$ by

$$
(U_a(t,s)g)(x,v)=
e^{-\int_s^t a(r,x-v(t-r),v)\,dr}g(x-v(t-s),v).
$$

By the argument in (b), $\|U_a(t,s)g\|_2\leq\|g\|_2$. The integral operator is the [Boltzmann Volterra operator](../../../statistical-physics.md#boltzmann-volterra-operator)

$$
\tau f(t)=\int_0^tU_a(t,s)K_sf(s)\,ds.
$$

The [Minkowski integral inequality](../../../functional-analysis.md#minkowski-integral-inequality) and (a) give the useful stronger pointwise bound

$$
\|\tau f(t)\|_2\leq C\int_0^t\|f(s)\|_2\,ds.
$$

Therefore **the requested estimate is**

$$
\boxed{\|\tau f(t)\|_2\leq Ct\,\sup_{0\leq s\leq t}\|f(s)\|_2.}
$$

For strongly measurable bounded $L^2$-valued $f$, these are [Bochner integrals](../../../measure-theory.md#bochner-integral); their finite norm bounds establish existence of the integrals.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

For fixed $t$, put $M_t=\sup_{0\leq s\leq t}\|f(s)\|_2$. A [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) in time strengthens the organization of the estimate in (c):

$$
\|\tau g(t)\|_2^2
\leq C^2t\int_0^t\|g(s)\|_2^2\,ds.
$$

Start with $\|\tau f(t)\|_2^2\leq C^2t^2M_t^2$. If the printed bound holds for $n-1$, then

$$
\|\tau^nf(t)\|_2^2
\leq C^2t\int_0^t
\frac{C^{2n-2}s^{2n-2}}{1\cdot3\cdots(2n-3)}M_t^2\,ds
=\frac{C^{2n}t^{2n}}{1\cdot3\cdots(2n-1)}M_t^2.
$$

Taking square roots proves **the [iterated Cauchy-Schwarz bound for a Volterra operator](../../../analysis.md#iterated-cauchy-schwarz-bound-for-a-volterra-operator)**:

$$
\boxed{\|\tau^nf(t)\|_2
\leq\frac{C^nt^n}{\sqrt{1\cdot3\cdots(2n-1)}}M_t.}
$$

There is also a [factorial bound for a Volterra iterate](../../../analysis.md#factorial-bound-for-a-volterra-iterate), obtained by iterating the unsquared integral estimate in (c):

$$
\boxed{\|\tau^nf(t)\|_2\leq\frac{C^nt^n}{n!}M_t.}
$$

Its factor $t^n/n!$ is the volume of the time-ordered simplex $0<s_n<\cdots<s_1<t$. It is stronger than the printed estimate because $\prod_{j=1}^n j^2\geq\prod_{j=1}^n(2j-1)$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Work in the [Banach space](../../../banach-space.md) $\mathcal B_T$ of bounded strongly measurable maps $[0,T]\to L^2_{x,v}$, with norm $\|g\|_{\mathcal B_T}=\sup_{0\leq t\leq T}\|g(t)\|_2$. Keeping actual representatives at every time matches the pointwise-in-time mild formulation. The [Boltzmann Volterra operator](../../../statistical-physics.md#boltzmann-volterra-operator) is bounded on this space, and the [factorial bound for a Volterra iterate](../../../analysis.md#factorial-bound-for-a-volterra-iterate) gives

$$
\|\tau^n\|_{\mathcal B_T\to\mathcal B_T}\leq\frac{(CT)^n}{n!}.
$$

Thus the [Volterra series for the linear Boltzmann equation](../../../statistical-physics.md#volterra-series-for-the-linear-boltzmann-equation) converges in [operator norm](../../../continuous-dual-space.md#operator-norm) for every finite $T$, even when $CT\geq1$. Set

$$
\boxed{f=\sum_{n=0}^\infty\tau^nF(f_0,a).}
$$

For its partial sums, $(I-\tau)\sum_{n=0}^N\tau^nF=F-\tau^{N+1}F$. The remainder tends to zero by the factorial estimate. Hence $(I-\tau)f=F$, precisely the required characteristic integral equation.

The norm bound in (b) gives **an explicit choice of the existence constant**:

$$
\boxed{\sup_{0\leq t\leq T}\|f(t)\|_2
\leq e^{CT}\|f_0\|_2,\qquad C_T=e^{CT}.}
$$

Also $f(0)=f_0$, since every term with $n\geq1$ vanishes at zero and the damping interval has length zero. This proves existence in the paper's weak, characteristic-integral sense. With merely measurable nonnegative $a$, that sense does not itself require a continuous initial trace; that trace follows under the additional local characteristic-integrability condition described in (b).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Let $f_1,f_2$ have the same initial data and satisfy the characteristic integral equation. Their difference $g=f_1-f_2$ satisfies $g=\tau g$, hence $g=\tau^ng$ for every $n$.

Fix any $T_0<T$ and let $M=\sup_{0\leq s\leq T_0}\|g(s)\|_2<\infty$. The [factorial bound for a Volterra iterate](../../../analysis.md#factorial-bound-for-a-volterra-iterate) gives

$$
\|g(t)\|_2\leq\frac{(CT_0)^n}{n!}M
\qquad(0\leq t\leq T_0).
$$

The scalar factor tends to zero, so $g(t)=0$ throughout this interval. Since $T_0<T$ is arbitrary, **the weak solution of the [linear Boltzmann equation](../../../statistical-physics.md#linear-boltzmann-equation) is unique on $[0,T)$**. The same argument gives uniqueness at $T$ whenever solutions are defined there by the integral formula.

## 3

↑ **Parent:** [Paper 8](paper-8.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For the normalized standard [Gaussian density](../../../probability-and-statistics.md#multivariate-normal-density),

$$
\nabla\gamma=-v\gamma,\qquad
\Delta\gamma=(|v|^2-d)\gamma,\qquad
\nabla\cdot(v\gamma)=(d-|v|^2)\gamma.
$$

The two terms cancel, so **the [Ornstein-Uhlenbeck Fokker-Planck equation](../../../probability-theory.md#ornstein-uhlenbeck-fokker-planck-equation) has [stationary density for a Fokker-Planck equation](../../../probability-theory.md#stationary-density-for-a-fokker-planck-equation)**

$$
\boxed{\partial_t\gamma=0,\qquad
\Delta\gamma+\nabla\cdot(v\gamma)=0.}
$$

Equivalently its [Fokker-Planck probability current](../../../probability-theory.md#fokker-planck-probability-current) $-\nabla\gamma-v\gamma$ vanishes identically. The normalization follows from the [Gaussian integral](../../../calculus.md#gaussian-integral) in each coordinate.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a smooth test function $\varphi$, [integration by parts](../../../calculus.md#integration-by-parts) gives the moment identity

$$
\frac d{dt}\int\varphi(v)f(t,v)\,dv
=\int\bigl(\Delta\varphi-v\cdot\nabla\varphi\bigr)f(t,v)\,dv.
$$

The assumed decay removes all boundary terms. Apply it to $1$, $v_i$ and $|v|^2/2$. Writing $m_i=\int v_if=M u_i$ gives the [Ornstein-Uhlenbeck moment equations](../../../probability-theory.md#ornstein-uhlenbeck-moment-equations)

$$
\boxed{M'=0,\qquad m_i'=-m_i,\qquad E'=dM-2E.}
$$

Assume $M(0)\ne0$ when using the normalized mean $u$; otherwise $u$ is undefined, while the unnormalized [momentum](../../../classical-mechanics.md#momentum) equation still holds. Since $M$ is constant, $u_i'=-u_i$. **Their solutions are**

$$
\boxed{M(t)=M_0,\qquad
u_i(t)=e^{-t}u_i(0),\qquad
E(t)=\frac{dM_0}{2}+
\left(E(0)-\frac{dM_0}{2}\right)e^{-2t}.}
$$

Thus [mass](../../../classical-mechanics.md#mass) is conserved, the [mean velocity](../../../statistical-physics.md#mean-velocity-of-a-kinetic-distribution) tends to zero, and $E(t)\to dM_0/2$. This includes the [mean velocity](../../../statistical-physics.md#mean-velocity-of-a-kinetic-distribution) conclusion omitted from the converted TeX.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In the one-dimensional unit-mass setting, put $q=f/\gamma$. Using the convention $0\log0=0$, the [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) is

$$
H(f\mid\gamma)=\int f\log(f/\gamma)\,dv=\int\gamma\,q\log q\,dv.
$$

Because $\int\gamma q=\int f=1=\int\gamma$, we can subtract $q-1$ inside the integral:

$$
\boxed{H(f\mid\gamma)=\int\gamma(v)
[q(v)\log q(v)-q(v)+1]\,dv\geq0.}
$$

This is [relative entropy nonnegativity](../../../probability-and-statistics.md#relative-entropy-nonnegativity) from the given scalar inequality. Its integrand vanishes only at $q=1$, so **zero [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) characterizes $f=\gamma$ almost everywhere**. The nonnegativity remains valid with value $+\infty$ when entropy is not finite.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For positive smooth $f$ with the stated decay, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\boxed{\int f''\log f\,dv=-\int\frac{|f'|^2}{f}\,dv}
$$

and, using unit [mass](../../../classical-mechanics.md#mass),

$$
\boxed{\int(fv)'\log f\,dv=-\int vf'\,dv=\int f\,dv=1.}
$$

For zero values of $f$, these calculations can be made with the positive unit-mass approximation $(f+\varepsilon\gamma)/(1+\varepsilon)$ and then passed to the limit whenever the quantities are finite. Positive-time solutions also have the usual Gaussian smoothing.

Since $-\log\gamma=v^2/2+\tfrac12\log(2\pi)$, [mass](../../../classical-mechanics.md#mass) conservation gives

$$
H(f_t\mid\gamma)=\int f_t\log f_t\,dv+
\frac12\int v^2f_t\,dv+\frac12\log(2\pi).
$$

The derivative of the first term is $\int\partial_tf_t\log f_t$, because $\int\partial_tf_t=0$. The two identities above and the [energy](../../../classical-mechanics.md#energy) equation in (b), with $d=M=1$, yield

$$
\frac d{dt}H(f_t\mid\gamma)
=-\int\frac{|f_t'|^2}{f_t}\,dv+1+
\left(1-\int v^2f_t\,dv\right).
$$

Now expand the [relative Fisher information](../../../probability-and-statistics.md#relative-fisher-information):

$$
I(f\mid\gamma)=\int\left|\partial_v\log(f/\gamma)\right|^2f\,dv
=\int\left(\frac{f'}f+v\right)^2f\,dv
=\int\frac{|f'|^2}{f}\,dv+\int v^2f\,dv-2,
$$

where $\int vf'=-1$. **Thus the [entropy dissipation identity for Ornstein-Uhlenbeck flow](../../../probability-theory.md#entropy-dissipation-identity-for-ornstein-uhlenbeck-flow) is**

$$
\boxed{\frac d{dt}H(f_t\mid\gamma)=-I(f_t\mid\gamma)\leq0.}
$$

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The given [relative Fisher information](../../../probability-and-statistics.md#relative-fisher-information) inequality is $I'(t)\leq-2I(t)$. Multiplying by $e^{2t}$ and integrating gives **[relative Fisher information decay under Ornstein-Uhlenbeck flow](../../../probability-and-statistics.md#relative-fisher-information-decay-under-ornstein-uhlenbeck-flow)**:

$$
\boxed{I(f_t\mid\gamma)\leq e^{-2(t-s)}I(f_s\mid\gamma)
\qquad(t\geq s\geq0).}
$$

In particular $I(t)\leq I(0)e^{-2t}$ when $I(0)$ is finite; if necessary one starts at a positive time with finite information. It follows that $I(t)\to0$.

Write $H(t)=H(f_t\mid\gamma)$. It is nonnegative and decreasing, so has a finite limit $H_\infty\geq0$ when $H(0)<\infty$. The printed integrability request concerns the product $H(t)H'(t)$. Its sign is nonpositive, and the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) gives

$$
\int_0^R|H(t)H'(t)|\,dt
=-\frac12\int_0^R(H(t)^2)'\,dt
=\frac{H(0)^2-H(R)^2}{2}.
$$

Passing to $R\to\infty$ proves **[time integrability of an entropy-dissipation product](../../../probability-theory.md#time-integrability-of-an-entropy-dissipation-product)**:

$$
\boxed{H(t)H'(t)\in L^1(0,\infty),\qquad
\|HH'\|_{L^1}=\frac{H(0)^2-H_\infty^2}{2}\leq\frac{H(0)^2}{2}.}
$$

Also $\int_0^\infty|H'|=H(0)-H_\infty\leq H(0)$. The zero value of $H_\infty$ will be used as supplied in (f); positivity and monotonicity alone only establish existence of the limit.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Use the zero entropy limit supplied in this subpart. By the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and the [entropy dissipation identity for Ornstein-Uhlenbeck flow](../../../probability-theory.md#entropy-dissipation-identity-for-ornstein-uhlenbeck-flow),

$$
H(f_t\mid\gamma)=\int_t^\infty I(f_s\mid\gamma)\,ds.
$$

Apply the [relative Fisher information](../../../probability-and-statistics.md#relative-fisher-information) decay estimate starting at time $t$:

$$
H(f_t\mid\gamma)\leq I(f_t\mid\gamma)
\int_t^\infty e^{-2(s-t)}\,ds=\frac12I(f_t\mid\gamma).
$$

Thus **the requested entropy-dissipation inequality is**

$$
\boxed{H(f_t\mid\gamma)\leq-\frac12\frac d{dt}H(f_t\mid\gamma).}
$$

It is the [Gaussian logarithmic Sobolev inequality](../../../probability-inequality.md#gaussian-logarithmic-sobolev-inequality) along this evolution. Since $H'\leq-2H$, an integrating factor gives **the [entropy convergence rate for Ornstein-Uhlenbeck flow](../../../probability-theory.md#entropy-convergence-rate-for-ornstein-uhlenbeck-flow)**:

$$
\boxed{H(f_t\mid\gamma)\leq e^{-2t}H(f_0\mid\gamma).}
$$

For finite initial entropy, $f_t$ therefore converges to the stationary [Gaussian density](../../../probability-and-statistics.md#multivariate-normal-density) in [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) at rate $2$. If desired, [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality) also converts this to the density estimate $\|f_t-\gamma\|_{L^1}\leq\sqrt{2H(f_0\mid\gamma)}e^{-t}$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
