# Paper 1

↑ **Parent:** [2014](../2014.md)

[Original public PDF, physical pages 320–326; examination dated 15 January 2014](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=320)

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
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Measure both angles from the downward vertical, as in the source diagram. With upward $y$, the cylinder centres are

$$
\mathbf R=(2a\sin\theta,-2a\cos\theta),\qquad
\mathbf r=\mathbf R+(a\sin\phi,-a\cos\phi).
$$

The large hoop has central inertia $4Ma^2$ and [angular velocity](../../rigid-body-dynamics.md#angular-velocity) $\dot\theta$, while the small hoop has no spin in this part. [Translation](../../geometry-and-topology.md#translation-geometry) and [rotation](../../riemannian-geometry.md#rotation-mathematics) therefore give

$$
T=\frac12Ma^2[12\dot\theta^2+\dot\phi^2+
4\cos(\theta-\phi)\dot\theta\dot\phi],
\qquad V=-Mga(4\cos\theta+\cos\phi).
$$

Thus $L=T-V$. Counting each angle and [velocity](../../classical-mechanics.md#velocity) as first order, replacing the cosine in the [velocity](../../classical-mechanics.md#velocity) product by one changes only fourth-order terms. Expanding the potential and dropping its constant gives

$$
\boxed{L_2=\frac12Ma^2(12\dot\theta^2+\dot\phi^2+4\dot\theta\dot\phi)
-\frac12Mga(4\theta^2+\phi^2).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Euler-Lagrange equations](../../analysis.md#euler-lagrange-equation) from the quadratic [Lagrangian](../../calculus-of-variations.md#lagrangian) are

$$
12\ddot\theta+2\ddot\phi+\frac{4g}{a}\theta=0,
\qquad2\ddot\theta+\ddot\phi+\frac ga\phi=0.
$$

For a [normal mode](../../wave-equation.md#normal-mode) proportional to $e^{i\omega t}$, let $\lambda=\omega^2a/g$. Nonzero amplitudes require

$$
\det\begin{pmatrix}4-12\lambda&-2\lambda\\-2\lambda&1-\lambda\end{pmatrix}
=4-16\lambda+8\lambda^2=0.
$$

Hence

$$
\boxed{\omega_\pm^2=\frac ga\left(1\pm\frac1{\sqrt2}\right).}
$$

The corresponding amplitude ratios are $\Phi/\Theta=2\lambda/(1-\lambda)$. The lower-frequency mode has **$\Phi/\Theta=2(\sqrt2-1)$**, with the angles in phase; the higher-frequency mode has **$\Phi/\Theta=-2(1+\sqrt2)$**, with opposite signs. The small hoop's spin remains zero in both modes.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $\psi$ be the small hoop's absolute spin angle with the same angular sign convention. Equating the two contact-point velocities cancels the large hoop centre's [translation](../../geometry-and-topology.md#translation-geometry). The remaining tangential equality is

$$
a\dot\phi+a\dot\psi=2a\dot\theta,
\qquad\boxed{\dot\psi=2\dot\theta-\dot\phi.}
$$

This [rolling constraint inside a moving circular track](../../rigid-body-dynamics.md#rolling-constraint-inside-a-moving-circular-track) adds small-hoop rotational [energy](../../energy.md) $Ma^2(2\dot\theta-\dot\phi)^2/2$. At quadratic order its cross term cancels the translational cross term in part a. The potential is unchanged, so

$$
\boxed{L_2=\frac12Ma^2(16\dot\theta^2+2\dot\phi^2)
-\frac12Mga(4\theta^2+\phi^2).}
$$

Static friction enforces rolling; ideal no-slip contact dissipates no [energy](../../energy.md).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The new kinetic matrix is diagonal, giving

$$
\ddot\theta+\frac{g}{4a}\theta=0,
\qquad\ddot\phi+\frac{g}{2a}\phi=0,
\qquad
\boxed{\omega_1^2=\frac g{4a},\quad\omega_2^2=\frac g{2a}.}
$$

For the first mode, $\phi=0$: the line between the centres stays vertical, both centres translate together, and $\dot\psi=2\dot\theta$. For the second, $\theta=0$: the outer hoop stays still while the inner hoop rolls within it, with $\dot\psi=-\dot\phi$. These coordinate motions are independent only at the retained quadratic order.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Choose electric scalar potential $\Phi=-Ex$ and the [symmetric gauge](../../quantum-theory.md#symmetric-gauge) $\mathbf A=B(-y,x,0)/2$, whose curl is $B\hat{\mathbf z}$. [Minimal coupling](../../quantum-theory.md#minimal-coupling) gives $L=m\dot{\mathbf r}^{\,2}/2-k\mathbf r^2/2+q\mathbf A\cdot\dot{\mathbf r}-q\Phi$. Since $x=\rho\cos\theta$ and $x\dot y-y\dot x=\rho^2\dot\theta$,

$$
\boxed{L=\frac m2(\dot\rho^2+\rho^2\dot\theta^2)-\frac k2\rho^2
+qE\rho\cos\theta+\frac{qB}{2}\rho^2\dot\theta.}
$$

The magnetic term is [velocity](../../classical-mechanics.md#velocity) dependent; it is not an ordinary position-only potential.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [canonical momenta](../../hamiltonian-mechanics.md#canonical-momentum) are

$$
\boxed{p_\rho=m\dot\rho,\qquad
p_\theta=m\rho^2\dot\theta+\frac{qB}{2}\rho^2.}
$$

Taking the [Legendre transform](../../convex-optimization.md#convex-conjugate) gives

$$
\boxed{H=\frac{p_\rho^2}{2m}
+\frac1{2m}\left(\frac{p_\theta}{\rho}-\frac{qB\rho}{2}\right)^2
+\frac{k\rho^2}{2}-qE\rho\cos\theta.}
$$

Its four [Hamilton equations](../../hamiltonian-mechanics.md#hamilton-s-equations), in a polar chart with $\rho>0$, are

$$
\dot\rho=\frac{p_\rho}{m},\quad
\dot\theta=\frac{p_\theta}{m\rho^2}-\frac{qB}{2m},
$$



$$
\dot p_\rho=\frac{p_\theta^2}{m\rho^3}
-\frac{q^2B^2\rho}{4m}-k\rho+qE\cos\theta,
\qquad\dot p_\theta=-qE\rho\sin\theta.
$$

Canonical [angular momentum](../../momentum.md#angular-momentum) includes the vector-potential contribution and is not simply mechanical [angular momentum](../../momentum.md#angular-momentum).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Direct variation of the [Lagrangian](../../calculus-of-variations.md#lagrangian) gives

$$
m\ddot\rho-m\rho\dot\theta^2+k\rho-qE\cos\theta-qB\rho\dot\theta=0,
$$



$$
m\rho^2\ddot\theta+2m\rho\dot\rho\dot\theta
+qB\rho\dot\rho+qE\rho\sin\theta=0.
$$

For a static configuration, $k\rho=qE\cos\theta$ and $qE\rho\sin\theta=0$. Since $qE>0$ and the radius is positive,

$$
\boxed{\rho_0=qE/k,\qquad\theta_0=0\pmod{2\pi}.}
$$

The magnetic force vanishes at rest and does not shift this equilibrium. In canonical variables it has $p_\rho=0$ but $p_\theta=qB\rho_0^2/2$, rather than zero canonical [angular momentum](../../momentum.md#angular-momentum).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Substitution of the proposed sine and cosine displacements into either linearized equation gives $m\omega^2+qB\omega-k=0$. Thus

$$
\boxed{\omega_{1,2}=-\frac{qB}{2m}
\left[1\mp\sqrt{1+\frac{4mk}{q^2B^2}}\right].}
$$

These are signed angular frequencies, not two positive [frequency](../../wave.md#frequency) magnitudes. To first order, with $\varepsilon\ll\rho_0$,

$$
x=\rho_0+\varepsilon\cos\omega t+O(\varepsilon^2/\rho_0),
\qquad y=\varepsilon\sin\omega t+O(\varepsilon^2/\rho_0).
$$

The orbit is therefore a **circle of radius $\varepsilon$ about $(\rho_0,0)$** at this order. The positive root runs counterclockwise; the negative root runs clockwise and has the larger magnitude. A positive charge in $B\hat{\mathbf z}$ alone circles clockwise. Here the spring permits an additional counterclockwise mode by providing inward force against its magnetic force.

<a id="2/d/image-opposite-handed-circular-modes-about-the-shifted-spring-equilibrium"></a>
![](../../past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2014/paper-1-tp1-circular-modes.png)

**[Figure 1](#2/d/image-opposite-handed-circular-modes-about-the-shifted-spring-equilibrium). Opposite-handed circular modes about the shifted spring equilibrium**.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a regular [Lagrangian](../../calculus-of-variations.md#lagrangian) define $p_i=\partial L/\partial\dot q_i$ and $H=\sum_i p_i\dot q_i-L$. Its differential is

$$
dH=\sum_i\dot q_i\,dp_i-\sum_i\frac{\partial L}{\partial q_i}\,dq_i
-\frac{\partial L}{\partial t}\,dt.
$$

The [velocity](../../classical-mechanics.md#velocity) differentials cancel. Using $\partial L/\partial q_i=\dot p_i$ and comparing independent coefficients gives

$$
\boxed{\dot q_i=H_{p_i},\quad\dot p_i=-H_{q_i},\quad H_t=-L_t.}
$$

The last equality concerns explicit partial derivatives in their respective natural variables; it does not assert that total time derivatives are always negatives.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The assumed relation makes the old and new actions differ by the endpoint term $G(t_f)-G(t_i)$. Fixed endpoint values of both coordinate sets make its variation zero. Therefore stationarity of the old [action](../../lagrangian-mechanics.md#action) is equivalent to stationarity of

$$
\int\left(\sum_iP_i\dot Q_i-\mathcal H(Q,P,t)\right)dt.
$$

Varying independent $Q_i,P_i$ and integrating $P_i\delta\dot Q_i$ by parts gives

$$
\delta S=\int\sum_i[(\dot Q_i-\mathcal H_{P_i})\delta P_i
-(\dot P_i+\mathcal H_{Q_i})\delta Q_i]dt.
$$

Both coefficients vanish: **the new variables satisfy [Hamilton's equations](../../hamiltonian-mechanics.md#hamilton-s-equations)**, so a locally invertible transformation with this [action](../../lagrangian-mechanics.md#action) identity is canonical.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

When the Hamiltonians agree, exactness of the one-form gives

$$
\sum_i p_i\,dq_i-\sum_iP_i\,dQ_i=dG,
\qquad L-\mathcal L=\frac{dG}{dt}.
$$

The [action](../../lagrangian-mechanics.md#action) argument of part b then proves canonicity. Equivalently, exterior differentiation preserves the symplectic two-form. For a time-dependent transformation, **the [exact differential](../../differential-form.md#exact-differential) must supply the full [action](../../lagrangian-mechanics.md#action) identity**; a fixed-time check alone would not establish that the new [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) equals the old one without a time-dependent correction.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The general [action](../../lagrangian-mechanics.md#action) identity is

$$
dG=\sum_i p_i\,dq_i-\sum_iP_i\,dQ_i+(\mathcal H-H)dt.
$$

Treating $q,Q,t$ as independent and comparing coefficients gives

$$
\boxed{p_i=G_{q_i},\qquad P_i=-G_{Q_i},\qquad
\mathcal H=H+G_t.}
$$

Choose a [complete integral of the Hamilton-Jacobi equation](../../hamiltonian-mechanics.md#complete-integral-of-the-hamilton-jacobi-equation),

$$
\boxed{G_t+H(q,G_q,t)=0.}
$$

Then $\mathcal H=0$, and [Hamilton's equations](../../hamiltonian-mechanics.md#hamilton-s-equations) become $\dot Q_i=\dot P_i=0$. Completeness and local invertibility are needed: a solution with too few independent parameters cannot generate an arbitrary trajectory.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Separating $G=W(q)-\beta t$ gives $[W'(q)]^2/(2m)+m\omega^2q^2/2=\beta$. On the positive-momentum branch choose

$$
G=\int_0^q\sqrt{2m\left(\beta-\frac12m\omega^2s^2\right)}\,ds-\beta t.
$$

With $Q=\beta$ and $A=\sqrt{2\beta/(m\omega^2)}$, differentiation with respect to $Q$ gives

$$
P=-G_\beta=t-\int_0^q\frac{m\,ds}
{\sqrt{2m(\beta-m\omega^2s^2/2)}}
=t-\frac1\omega\arcsin(q/A).
$$

Since $P=\gamma$ is constant,

$$
\boxed{q=A\sin[\omega(t-\gamma)].}
$$

The displayed integral is a local positive-$p$ branch. Continuing the trajectory through turning points switches [momentum](../../momentum.md) branches and extends the sine solution over the complete orbit. $\beta$ is the oscillator [energy](../../energy.md), and $\gamma$ fixes its time phase.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use metric signature $(+,-,-,-)$ and units $\hbar=c=1$. Varying $\phi^*$ and $\phi$ independently gives

$$
\boxed{(\Box+m^2)\phi=0,\qquad(\Box+m^2)\phi^*=0.}
$$

In the divergence of the stated current, the products of first derivatives cancel, leaving

$$
\partial_\mu j^\mu=iq(\phi^*\Box\phi-\phi\Box\phi^*)=0.
$$

The two identical [mass](../../classical-mechanics.md#mass) terms cancel on the field equations.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

An infinitesimal constant phase change has $\delta\phi=-iq\alpha\phi$ and $\delta\phi^*=iq\alpha\phi^*$. Both the [derivative](../../calculus.md#derivative) product and the [mass](../../classical-mechanics.md#mass) term are invariant. [Noether's theorem](../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry) gives, per unit $\alpha$,

$$
j^\mu=(\partial^\mu\phi^*)(-iq\phi)
+(\partial^\mu\phi)(iq\phi^*)
=iq(\phi^*\partial^\mu\phi-\phi\partial^\mu\phi^*).
$$

Thus **the global phase symmetry supplies the conserved current in part a**.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The derivatives needed for varying $A_\nu$ are

$$
\frac{\partial\hat{\mathcal L}}{\partial(\partial_\mu A_\nu)}=-F^{\mu\nu},
\qquad
\frac{\partial\hat{\mathcal L}}{\partial A_\nu}
=-iq(\phi^*D^\nu\phi-\phi\bar D^\nu\phi^*)=-J^\nu.
$$

Therefore the electromagnetic [Euler-Lagrange equation](../../analysis.md#euler-lagrange-equation) is

$$
\boxed{\partial_\mu F^{\mu\nu}=J^\nu,\qquad
J^\mu=iq(\phi^*D^\mu\phi-\phi\bar D^\mu\phi^*).}
$$

Antisymmetry of $F$ and commutation of derivatives imply $\partial_\nu\partial_\mu F^{\mu\nu}=0$, hence $\partial_\nu J^\nu=0$. In ordinary derivatives, $J^\mu=j^\mu-2q^2A^\mu|\phi|^2$; the interaction contribution must not be omitted.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Under the combined local transformation,

$$
D'_\mu\phi'=(\partial_\mu+iqA_\mu+iq\partial_\mu\alpha)
(e^{-iq\alpha}\phi)=e^{-iq\alpha}D_\mu\phi.
$$

The [derivative](../../calculus.md#derivative) of the phase cancels the added gauge potential. The conjugate [derivative](../../calculus.md#derivative) gains the opposite phase, so their product and $|\phi|^2$ are invariant. Also

$$
F'_{\mu\nu}=F_{\mu\nu}+\partial_\mu\partial_\nu\alpha
-\partial_\nu\partial_\mu\alpha=F_{\mu\nu}.
$$

**Every term of the interacting [Lagrangian](../../calculus-of-variations.md#lagrangian) is therefore invariant.**

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The local [gauge symmetry](../../relativistic-quantum-field.md#gauge-invariance) contains the constant-phase subgroup. For constant $\alpha$, $\delta A_\mu=0$, and [Noether's theorem](../../calculus-of-variations.md#noether-conserved-quantity-for-a-mechanical-point-symmetry) applied to the matter fields gives

$$
\frac{j_{\rm N}^\mu}{\alpha}
=(\bar D^\mu\phi^*)(-iq\phi)+(D^\mu\phi)(iq\phi^*)=J^\mu.
$$

Thus $\partial_\mu J^\mu=0$ on the matter field equations. More explicitly, allowing $\alpha(x)$ in the matter variation while holding $A$ fixed gives $\delta\mathcal L=J^\mu\partial_\mu\alpha$. On shell it also equals $\partial_\mu(\alpha J^\mu)$, so equality for arbitrary $\alpha$ implies conservation. In the full gauge transformation, varying $A$ cancels the $J^\mu\partial_\mu\alpha$ term; this is the related Noether second-theorem identity, not a new independent charge for every gauge function.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For the supplied [Lagrangian](../../calculus-of-variations.md#lagrangian), variation with respect to $\phi^*$ uses

$$
\frac{\partial\mathcal L}{\partial(\partial_\mu\phi^*)}
=\partial^\mu\phi+ieA^\mu\phi,
\qquad
\frac{\partial\mathcal L}{\partial\phi^*}
=-m^2\phi-ieA_\mu\partial^\mu\phi+f.
$$

Thus $\Box\phi+2ieA^\mu\partial_\mu\phi+ie(\partial_\mu A^\mu)\phi+m^2\phi=f$. In the [Lorenz gauge](../../relativistic-electromagnetism.md#lorenz-gauge-condition),

$$
\boxed{(\Box+2ieA^\mu\partial_\mu+m^2)\phi=f(t).}
$$

For real external fields and driving, the conjugate equation has $-2ieA^\mu\partial_\mu$ acting on $\phi^*$. The supplied model has no $e^2A^2|\phi|^2$ term; one must not insert such a term from a different minimally coupled [Lagrangian](../../calculus-of-variations.md#lagrangian).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

First fix the source at the spatial origin. [Fourier transform](../../fourier-transform.md) replaces $\partial_t$ by $-i\omega$ and $\nabla$ by $i\mathbf k$ in the free term. Multiplication by a static background becomes a [momentum](../../momentum.md) convolution; the [derivative](../../calculus.md#derivative) in $A\cdot\partial G$ acts on the [Green function](../../green-s-function.md), so it carries the internal [momentum](../../momentum.md) $\mathbf k'$. Consequently

$$
\boxed{(k^2+m^2-\omega^2)G(\mathbf k;\omega)
+2e\int\frac{d^3k'}{(2\pi)^3}
[\omega A^0(\mathbf k-\mathbf k')-\mathbf A(\mathbf k-\mathbf k')\cdot\mathbf k']
G(\mathbf k';\omega)=1.}
$$

The transformed point source supplies the right-hand side one. The signs follow from $A^\mu\partial_\mu=A^0\partial_t+\mathbf A\cdot\nabla$ in these conventions.

**Source-position qualification.** For a nonuniform $A(\mathbf r)$, the general [Green function](../../green-s-function.md) is not [translation](../../geometry-and-topology.md#translation-geometry) invariant. In the printed basis $e^{i\mathbf k\cdot(\mathbf r-\mathbf r')}$, its coefficient must also depend on $\mathbf r'$, and the convolution contains an extra factor $e^{i(\mathbf k-\mathbf k')\cdot\mathbf r'}$. The displayed source equation is valid for $\mathbf r'=0$, or with the background itself expressed in coordinates centred on that source. Equivalently, a general spatial Fourier [Green function](../../green-s-function.md) has two [momentum](../../momentum.md) arguments and a momentum-delta-function source. Staticity alone permits the time-difference transform, not a general position-difference-only transform.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The delta function in the artificial constant potential collapses the convolution. Put $b=e\gamma$ and $K^2=k^2+m^2$. Then

$$
\boxed{G(\mathbf k;\omega)=\frac1{-\omega^2+2ib\omega+K^2},
\qquad\omega_\pm=ib\pm\sqrt{K^2-b^2}.}
$$

Inverse [Fourier transform](../../fourier-transform.md) gives the stated real-frequency integral with exponential $e^{-i\omega(t-t')}$. For $K^2>b^2$, the [poles](../../isolated-singularity.md#pole) have opposite real parts and common imaginary part $b$. For $0<K^2<b^2$, both are imaginary, at $i[b\pm\sqrt{b^2-K^2}]$. They remain in the upper half-plane if $b>0$, or the lower half-plane if $b<0$. At equality they merge into a **second-order [pole](../../isolated-singularity.md#pole) at $ib$**. For $K^2=0$ one [pole](../../isolated-singularity.md#pole) reaches the real axis, requiring a prescription.

<a id="5/c/image-pole-motion-above-at-and-below-the-repeated-pole-threshold-shown-for-positive-e-gamma"></a>
![](../../past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2014/paper-1-tp1-poles.png)

**[Figure 2](#5/c/image-pole-motion-above-at-and-below-the-repeated-pole-threshold-shown-for-positive-e-gamma). Pole motion above, at and below the repeated-pole threshold; shown for positive e gamma**.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Let $\tau=t-t'$ and $\Omega=\sqrt{K^2-b^2}>0$. Because $|e^{-i(u+iv)\tau}|=e^{v\tau}$, close below for $\tau>0$ and above for $\tau<0$. The lower closure is clockwise. The two [residues](../../analysis.md#residue) sum to $i e^{b\tau}\sin(\Omega\tau)/\Omega$. Hence, for nonzero $b$,

$$
\boxed{G(\tau)=
\begin{cases}
-e^{b\tau}\sin(\Omega\tau)H(-\tau)/\Omega,&b>0,\\
 e^{b\tau}\sin(\Omega\tau)H(\tau)/\Omega,&b<0.
\end{cases}}
$$

In particular, **the printed sign with $e\gamma>0$ gives zero for $t>t'$ and an [advanced Green function](../../green-s-function.md#advanced-green-function) for $t<t'$**. Reversing that sign puts the [poles](../../isolated-singularity.md#pole) below and gives a [retarded Green function](../../quantum-field-theory.md#retarded-green-function). Both solutions have the unit [derivative](../../calculus.md#derivative) jump required by $(\partial_\tau^2-2b\partial_\tau+K^2)G=\delta(\tau)$. If $b=0$, the bare integral has real-axis [poles](../../isolated-singularity.md#pole) and requires an additional contour prescription; a unique retarded or advanced answer cannot be inferred without one.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

At mean-field level, positive gradient stiffness favours a spatially uniform [order parameter](../../critical-phenomenon.md#order-parameter). Writing $r=|\phi|$, minimization of $f=ar^2+r^4/2$ gives

$$
\boxed{\phi=0\quad(a\ge0),\qquad
\phi=\sqrt{-a}\,e^{i\delta}\quad(a<0),}
$$

with arbitrary constant $\delta$. The minimized density is zero above the transition and $-a^2/2$ below it. The [order parameter](../../critical-phenomenon.md#order-parameter) vanishes continuously as $(-a)^{1/2}$; the first [derivative](../../calculus.md#derivative) of the minimized free [energy](../../energy.md) is continuous while the second changes. This is the continuous mean-field transition.

The broken symmetry is **[global U(1) symmetry](../../scalar-field-theory.md#global-u-1-symmetry)**, not merely the Ising sign symmetry. Selecting one ordered phase breaks this continuous symmetry and leaves a soft phase direction. These are minima of the supplied [Landau free energy](../../critical-phenomenon.md#landau-free-energy), not an exact finite-temperature long-range-order claim in one dimension: phase fluctuations invalidate that inference for a short-range one-dimensional system.[§4.2.3, continuous symmetry, phase fluctuations and the Mermin-Wagner theorem](../../physics-bibliography.md#statistical-field-theory-by-david-tong)

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Take the ordered phase selected by a small positive real field, so $\phi$ is real and positive before sending $B\to0^+$. Stationarity gives $2a\phi+2\phi^3=B$. Differentiation yields $\chi=(2a+6\phi^2)^{-1}$. Therefore

$$
\boxed{\chi=\frac1{2a}\quad(a>0),\qquad
\chi_{\parallel}=\frac1{4|a|}\quad(a<0).}
$$

Both have mean-field [critical exponent](../../critical-phenomenon.md#critical-exponent) one, with a factor-of-two amplitude difference. The below-transition result is the longitudinal response of a selected pure phase. The transverse phase direction is soft, so a transverse zero-field response is singular; an unselected phase average is not the same susceptibility. At $a=0$, $\phi=(B/2)^{1/3}$ and the linear susceptibility diverges.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Set $r=\phi_0$ and $A_k=a+ck^2+k^4$. The trial density is $A_kr^2+r^4/2$. At fixed $k$, its minimum is $r=0$ if $A_k\ge0$ and $r^2=-A_k$ otherwise, with density $-A_k^2/2$. Minimizing $A_k$ uses

$$
\frac{dA_k}{dk}=2k(c+2k^2)=0.
$$

For $c\ge0$, $k=0$ minimizes the quadratic coefficient. For $c<0$, the minima are at $k=\pm\sqrt{-c/2}$ and have $A_k=a-c^2/4$. Thus

$$
\boxed{
\begin{array}{c|c|c}
\text{ordered region}&k&\phi_0^2\\\hline
c\ge0,\ a<0&0&-a\\
c<0,\ a<c^2/4&\pm\sqrt{-c/2}&c^2/4-a
\end{array}}
$$

Everywhere else the minimum is $\phi=0$; at the transition boundary the ordered amplitude tends to zero. The zero-field minimum is respectively $-a^2/2$ or $-(a-c^2/4)^2/2$ in the two ordered regions. For $c<0$ the helical solution is lower than a uniform ordered extremum whenever the latter exists, and lower than the disordered state whenever its amplitude is nonzero. The assumed positive-amplitude ansatz must allow its zero-amplitude boundary to describe disorder.

**The phase $\delta$ remains arbitrary** because the functional has [global U(1) symmetry](../../scalar-field-theory.md#global-u-1-symmetry). At nonzero $k$, a [translation](../../geometry-and-topology.md#translation-geometry) shifts that phase; separate [translation](../../geometry-and-topology.md#translation-geometry) and phase operations retain a combined unbroken subgroup. The two signs of $k$ also select opposite handedness. The meeting point of the uniform, modulated and disordered mean-field regions is the [Lifshitz point](../../critical-phenomenon.md#lifshitz-point) $(a,c)=(0,0)$.

<a id="6/c/image-uniform-helical-and-disordered-minima-of-the-specified-complex-landau-free-energy"></a>
![](../../past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2014/paper-1-tp1-landau-phases.png)

**[Figure 3](#6/c/image-uniform-helical-and-disordered-minima-of-the-specified-complex-landau-free-energy). Uniform, helical and disordered minima of the specified complex Landau free energy**.

## ↑ Ancestors (12)

1. [2014](../2014.md)
2. [Past exam of the theoretical physics I course of the University of Cambridge](../../past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge.md)
3. [Theoretical Physics I course of the University of Cambridge](../../university-of-cambridge.md#theoretical-physics-i-course-of-the-university-of-cambridge)
4. [Theoretical Physics course of the University of Cambridge](../../university-of-cambridge.md#theoretical-physics-course-of-the-university-of-cambridge)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
8. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
9. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
10. [University of Cambridge](../../university-of-cambridge.md)
11. [List of universities](../../README.md#list-of-universities)
12. [Codex Wiki](../../README.md)
