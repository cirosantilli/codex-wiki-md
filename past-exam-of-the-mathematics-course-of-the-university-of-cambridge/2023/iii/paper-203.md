# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_203.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded relatively closed set $A\subset\mathbb H$ such that $\mathbb H\setminus A$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). Its [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the unique [conformal map](../../../geometry-and-topology.md#conformal-map) $g_A:\mathbb H\setminus A\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity)

$$
g_A(z)=z+\frac a z+O(|z|^{-2}).
$$

The nonnegative coefficient $a$ is the [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) $\operatorname{hcap}(A)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $F(z)=z+z^{-1}$. On the unit semicircle, $F(e^{i\theta})=2\cos\theta$, and

$$
\left|\frac d{d\theta}F(e^{i\theta})\right|=2\sin\theta.
$$

The [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) and the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) therefore give the exit density with respect to $d\theta$:

$$
p(z,e^{i\theta})
=\frac1\pi
\frac{\operatorname{Im}F(z)}
{|F(z)-2\cos\theta|^2}\,2\sin\theta.
$$

As $z\to\infty$ in $\mathbb H$,

$$
\operatorname{Im}F(z)
=\operatorname{Im}z\left(1-\frac1{|z|^2}\right),
\qquad
|F(z)-2\cos\theta|^2
=|z|^2\bigl(1+O(|z|^{-1})\bigr),
$$

uniformly in $\theta\in[0,\pi]$. Hence

$$
\boxed{p(z,e^{i\theta})
=\frac2\pi\frac{\operatorname{Im}z}{|z|^2}
\sin\theta\bigl(1+O(|z|^{-1})\bigr).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $\sigma$ be the first time Brownian motion started outside the unit half-disc reaches its semicircular boundary. A path that reaches $A$ must first cross that semicircle. The [Strong Markov property](../../../markov-process.md#strong-markov-property) at $\sigma$ gives

$$
\mathbb E_z[\operatorname{Im}B_\tau]
=\int_0^\pi p(z,e^{i\theta})
\mathbb E_{e^{i\theta}}[\operatorname{Im}B_\tau]\,d\theta.
$$

Take $z=iy$, multiply by $y$, and let $y\to\infty$. The [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity) identifies the left side with $\operatorname{hcap}(A)$, while part b gives

$$
yp(iy,e^{i\theta})\longrightarrow\frac2\pi\sin\theta.
$$

Since the exit height is between zero and one, the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) applies and yields

$$
\boxed{\operatorname{hcap}(A)
=\frac2\pi\int_0^\pi
\mathbb E_{e^{i\theta}}[\operatorname{Im}B_\tau]
\sin\theta\,d\theta.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

Write $A_r=[-r,r]\times(0,1]$ and take $r\geq1$. By the [Brownian representation of half-plane capacity](../../../stochastic-process.md#brownian-representation-of-half-plane-capacity),

$$
\operatorname{hcap}(A_r)
=\lim_{y\to\infty}y\,
\mathbb E_{iy}[\operatorname{Im}B_\tau].
$$

On hitting $A_r$, the exit height is at most one. Moreover, $A_r$ lies in the half-disc of radius $\sqrt{r^2+1}\leq2r$. The [harmonic measure](../../../brownian-motion.md#harmonic-measure) of that semicircle as viewed from $iy$ is $O(r/y)$: mapping its exterior to $\mathbb H$ by $z\mapsto z+(2r)^2/z$ reduces the estimate to the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) on an interval of length $O(r)$. Consequently

$$
\mathbb E_{iy}[\operatorname{Im}B_\tau]\leq\frac{Cr}{y}
$$

for large $y$, and $\operatorname{hcap}(A_r)\leq Cr$. This is the [half-plane capacity of a low rectangle](../../../stochastic-process.md#half-plane-capacity-of-a-low-rectangle).

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

Let $R_r=[-r,r]\times(0,1]$ and set

$$
A_n=n^{-2}R_{n^3}
=[-n,n]\times(0,n^{-2}].
$$

The [scaling and translation of half-plane capacity](../../../stochastic-process.md#scaling-and-translation-of-half-plane-capacity) and part i give

$$
\operatorname{hcap}(A_n)
=n^{-4}\operatorname{hcap}(R_{n^3})
\leq\frac Cn\longrightarrow0.
$$

On the other hand,

$$
\operatorname{diam}(A_n)=\sqrt{4n^2+n^{-4}}\longrightarrow\infty.
$$

**Thus very long, very shallow hulls can have vanishing half-plane capacity.**

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) says that, conditionally on the curve through time $t$, mapping out the initial hull by $g_t-U_t$ turns the future into an independent [Schramm–Loewner evolution](../../../stochastic-process.md#schramm-loewner-evolution) in $(\mathbb H,0,\infty)$. More precisely,

$$
\widetilde K_s
=\bigl(g_t(K_{t+s}\setminus K_t)-U_t\bigr)^{\mathrm{fill}}
$$

has driving function $\widetilde U_s=U_{t+s}-U_t$. Since $U_t=\sqrt\kappa B_t$, the [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments) of Brownian motion give the asserted independence and equality in law.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the [Bessel process](../../../brownian-motion.md#bessel-process)

$$
dX_t=dB_t+\frac{d-1}{2X_t}dt,
$$

the [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) is $s(x)=x^{2-d}$ when $d\ne2$. If $0<\epsilon<x<R$, the [boundary hitting probability from a diffusion scale function](../../../stochastic-calculus.md#boundary-hitting-probability-from-a-diffusion-scale-function) gives

$$
\mathbb P_x(T_R<T_\epsilon)
=\frac{s(x)-s(\epsilon)}{s(R)-s(\epsilon)}.
$$

If $d<2$, then $s(0)=0$ and $s(R)\to\infty$. Letting $\epsilon\downarrow0$ and then $R\to\infty$ shows that the process cannot escape to infinity before reaching zero. The exit time from each bounded interval is finite almost surely, so $T_0<\infty$ almost surely.

If $d>2$, then $s(\epsilon)\to\infty$ in absolute value as $\epsilon\downarrow0$. Equivalently,

$$
\mathbb P_x(T_\epsilon<T_R)
=\frac{s(R)-s(x)}{s(R)-s(\epsilon)}
\longrightarrow0.
$$

**Thus the process does not hit zero. The borderline case $d=2$ has scale function $\log x$ and also does not hit zero. This is the [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process).**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

For $x>0$, the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) and $U_t=\sqrt\kappa B_t$ give

$$
dV_t^x=\frac2{V_t^x}dt-\sqrt\kappa\,dB_t.
$$

Put $D_t=V_t^r-V_t^1$. The common Brownian term cancels, so

$$
dD_t=-\frac{2D_t}{V_t^rV_t^1}dt.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applied to $Z_t=\log D_t-\log V_t^1$ gives

$$
dZ_t
=\frac{\sqrt\kappa}{V_t^1}dB_t
+\left[
\frac{\kappa-4}{2(V_t^1)^2}
-\frac2{V_t^rV_t^1}
\right]dt.
$$

Since

$$
\frac{V_t^1}{V_t^r}=\frac1{1+e^{Z_t}},
$$

the clock $q(u)=\int_0^u(V_s^1)^{-2}ds$ and its inverse $\sigma$ turn the local-martingale term into Brownian motion by the [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem). Therefore

$$
d\widetilde Z_t
=\sqrt\kappa\,dW_t
+\left(
\frac{\kappa-4}{2}
-\frac2{1+e^{\widetilde Z_t}}
\right)dt,
\qquad
\widetilde Z_0=\log(r-1).
$$

This is the [SLE boundary-point logarithmic separation diffusion](../../../stochastic-process.md#sle-boundary-point-logarithmic-separation-diffusion).

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

It is enough by [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) and reflection in the imaginary axis to treat $x=1$. Take $r=1+\epsilon$. The drift

$$
b(z)=\frac{\kappa-4}{2}-\frac2{1+e^z}
$$

tends to $(\kappa-8)/2<0$ as $z\to-\infty$. Choose $L<0$ and $a<0$ such that $b(z)\leq a$ for $z\leq L$. Before $\widetilde Z$ reaches $L$,

$$
\widetilde Z_t
\leq\log\epsilon+\sqrt\kappa W_t+at.
$$

The [infinite-horizon crossing probability for Brownian motion with negative drift](../../../brownian-motion.md#infinite-horizon-crossing-probability-for-brownian-motion-with-negative-drift) shows that this process has a finite running maximum almost surely, so

$$
\mathbb P_{\log\epsilon}(T_L<\infty)\longrightarrow0
\qquad(\epsilon\downarrow0).
$$

Order preservation for the [Loewner flow](../../../stochastic-process.md#loewner-chain) gives $\tau_1\leq\tau_{1+\epsilon}$. On $\{\tau_1<\tau_{1+\epsilon}\}$, one has $V_t^1\to0$ while $V_t^{1+\epsilon}$ remains positive, so $\widetilde Z_t\to+\infty$ and in particular $T_L<\infty$. Hence

$$
\mathbb P(\tau_1<\tau_{1+\epsilon})\longrightarrow0,
\qquad
\mathbb P(\tau_1=\tau_{1+\epsilon})\longrightarrow1.
$$

If the trace itself hit the fixed boundary point $1$, then $1$ would be the right endpoint of the swallowed interval and $\tau_1<\tau_{1+\epsilon}$ for every $\epsilon>0$. Its probability is therefore zero. Scaling and reflection prove that [SLE does not hit a fixed nonzero boundary point](../../../stochastic-process.md#sle-does-not-hit-a-fixed-nonzero-boundary-point) for every $x\in\mathbb R\setminus\{0\}$.

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace) is:

- $0<\kappa\leq4$: the trace is simple;
- $4<\kappa<8$: it has self-intersections but is not space-filling;
- $\kappa\geq8$: it is space-filling.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a real boundary point $x\ne0$, the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) says that $V_t^x/\sqrt\kappa$ is a Bessel process of dimension

$$
d=1+\frac4\kappa.
$$

When $\kappa\leq4$, one has $d\geq2$, so part 2(b), including its logarithmic $d=2$ case, shows that no fixed boundary point is swallowed.

If the trace touched the real line away from its starting point, or if a later segment crossed an earlier segment, the resulting hull would disconnect from infinity a nonempty real interval, which contains a [rational number](../../../number-theory.md#rational-number). Applying the preceding argument after every rational time and using the [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) rules this out on a countable probability-one event. Continuity of the trace then shows that no two distinct times have the same image. Thus $\operatorname{SLE}_\kappa$ is simple for $0<\kappa\leq4$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $\widehat B_t=rB_{t/r^2}$. By [Brownian scaling](../../../brownian-motion.md#brownian-scaling), $\widehat B$ is standard Brownian motion. Substituting $Y_t=rX_{t/r^2}$ into the Bessel equation gives

$$
dY_t
=d\widehat B_t+\frac{d-1}{2Y_t}dt,
\qquad
Y_0=rx.
$$

Weak uniqueness for the Bessel equation shows that $Y$ is a Bessel process of dimension $d$ started at $rx$. This is the [Scaling invariance of a Bessel process](../../../brownian-motion.md#scaling-invariance-of-a-bessel-process).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Let

$$
R=\sup\{r>0:\{z\in\mathbb H:|z|<r\}\subseteq K_1\}.
$$

By the stated fact, $R>0$ almost surely. Given $\epsilon\in(0,1)$, choose a deterministic $r_0>0$ with $\mathbb P(R\geq r_0)\geq1-\epsilon$. The [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) gives

$$
K_t\overset d=\sqrt t\,K_1,
$$

and therefore, for every $t\geq0$,

$$
\boxed{\mathbb P\!\left(
\{z\in\mathbb H:|z|<r_0\sqrt t\}\subseteq K_t
\right)\geq1-\epsilon.}
$$

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

Fix $R>0$. Part i, with $\epsilon$ arbitrarily small and $t$ sufficiently large, shows that

$$
\mathbb P\bigl(\{z\in\mathbb H:|z|<R\}\subseteq K_t
\text{ for some }t\bigr)=1.
$$

The hulls increase with time. Once this half-disc lies in $K_t$, the stated future-avoidance property gives

$$
\gamma((t,\infty))\subseteq\overline{\mathbb H}\setminus K_t
\subseteq\{z:|z|\geq R\}.
$$

Intersecting these probability-one events over positive integer $R$ proves

$$
\liminf_{t\to\infty}|\gamma(t)|=\infty
$$

almost surely. This is [Transience of chordal SLE](../../../stochastic-process.md#transience-of-chordal-sle).

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The [space of test functions](../../../distribution-theory.md#space-of-test-functions) $C_0^\infty(D)$ consists of infinitely differentiable real-valued functions whose [support of a function](../../../function.md#support) is a compact subset of $D$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Equip $C_0^\infty(D)$ with the [Dirichlet inner product](../../../sobolev-space.md#dirichlet-inner-product)

$$
(f,g)_\nabla=\frac1{2\pi}\int_D\nabla f(x)\mathbin\cdot\nabla g(x)\,dx.
$$

The [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space) $H_0^1(D)$ is its [Hilbert space completion](../../../hilbert-space.md#hilbert-space-completion) in the norm $\|f\|_\nabla=(f,f)_\nabla^{1/2}$.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The zero-boundary [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) $h$ on $D$ is the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process) over $H_0^1(D)$: for $f,g\in H_0^1(D)$, the variables $(h,f)_\nabla$ are centered jointly Gaussian and satisfy

$$
\mathbb E[(h,f)_\nabla(h,g)_\nabla]=(f,g)_\nabla.
$$

Equivalently, for an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(e_n)$ of $H_0^1(D)$ and independent standard normal variables $(\xi_n)$,

$$
h=\sum_{n\geq1}\xi_ne_n
$$

as a random [generalized function](../../../distribution-theory.md#distribution-mathematical-analysis).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For an open subdomain $U\subset D$, identify $H_0^1(U)$ with the closed subspace of $H_0^1(D)$ obtained by zero extension. Its orthogonal complement is

$$
\mathcal H_U
=\{f\in H_0^1(D):(f,g)_\nabla=0
\text{ for every }g\in H_0^1(U)\}.
$$

If $f\in\mathcal H_U$, then testing against $C_0^\infty(U)$ and integrating by parts gives $\Delta f=0$ in $U$ in the [distributional derivative](../../../distribution-theory.md#distributional-derivative) sense. The [Weyl lemma](../../../partial-differential-equation.md#weyl-lemma) therefore gives a representative harmonic on $U$.

The [orthogonal decomposition by a closed subspace](../../../hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) gives

$$
H_0^1(D)=H_0^1(U)\mathbin\oplus\mathcal H_U.
$$

Project the isonormal process defining $h$ onto these two orthogonal subspaces. The projections are jointly Gaussian and uncorrelated, hence [independent](../../../random-variable.md#independent-random-variables). The first projection is a zero-boundary Gaussian free field $h_U$ on $U$; the second is a random distribution $h^{\mathrm{har}}$ that is harmonic on $U$. Thus

$$
h=h_U+h^{\mathrm{har}},
$$

with independent summands. This proves the [Domain Markov property of the Gaussian free field](../../../stochastic-process.md#domain-markov-property-of-the-gaussian-free-field).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

The zero-Dirichlet [Green function of the Laplacian](../../../partial-differential-equation.md#green-function-of-the-laplacian) $G_D(x,y)$ is symmetric, vanishes at the boundary in the appropriate sense, is harmonic in $x$ away from $y$, and satisfies

$$
-\Delta_xG_D(x,y)=2\pi\delta_y
$$

as a [distribution](../../../distribution-theory.md#distribution-mathematical-analysis). Equivalently, for suitable $\phi$,

$$
\boxed{(-2\pi\Delta^{-1}\phi)(x)
=\int_DG_D(x,y)\phi(y)\,dy.}
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

For $\phi\in C_0^\infty(D)$, set

$$
f_\phi=-2\pi\Delta^{-1}\phi
=\int_DG_D(\mathord\cdot,y)\phi(y)\,dy
\in H_0^1(D)
$$

and define the distributional pairing by

$$
(h,\phi):=(h,f_\phi)_\nabla.
$$

It is centered Gaussian by the definition of the GFF. Integration by parts gives

$$
\begin{aligned}
\operatorname{Var}(h,\phi)
&=\|f_\phi\|_\nabla^2\\
&=\frac1{2\pi}\int_Df_\phi(-\Delta f_\phi)\,dx\\
&=\int_Df_\phi(x)\phi(x)\,dx\\
&=\iint_{D\times D}\phi(x)G_D(x,y)\phi(y)\,dx\,dy.
\end{aligned}
$$

This is the [Test-function pairing with a Gaussian free field](../../../stochastic-process.md#test-function-pairing-with-a-gaussian-free-field).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Choose an orthonormal basis $(e_n)$ of $H_0^1(D)$ and write the GFF formally as $h=\sum_n\xi_ne_n$, where the $\xi_n$ are independent standard normal variables. The [Green-kernel expansion in the Dirichlet space](../../../stochastic-process.md#green-kernel-expansion-in-the-dirichlet-space) gives

$$
\sum_{n\geq1}\left(\int_De_n(x)\rho(dx)\right)^2
=\iint_{D\times D}G_D(x,y)\rho(dx)\rho(dy)<\infty.
$$

Consequently the series

$$
(h,\rho):=\sum_{n\geq1}\xi_n\int_De_n(x)\rho(dx)
$$

converges in $L^2$. Its partial sums are centered Gaussian and their variances converge to the displayed [Green energy](../../../stochastic-process.md#green-energy). The $L^2$ limit is therefore Gaussian with mean zero and variance

$$
\iint_{D\times D}G_D(x,y)\rho(dx)\rho(dy).
$$

This constructs the [Finite-Green-energy measure pairing with a Gaussian free field](../../../stochastic-process.md#finite-green-energy-measure-pairing-with-a-gaussian-free-field) independently of the chosen orthonormal basis.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
