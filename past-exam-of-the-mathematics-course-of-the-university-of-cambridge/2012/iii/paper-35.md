# Paper 35

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_35.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_35.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
  - [d](#1/d)
    - [i](#1/d/i)
      - [Solution](#1/d/i/solution)
    - [ii](#1/d/ii)
      - [Solution](#1/d/ii/solution)
    - [iii](#1/d/iii)
      - [Solution](#1/d/iii/solution)
    - [iv](#1/d/iv)
      - [Solution](#1/d/iv/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
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
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) in which $g_t(z)=z+2t/z+O(z^{-2})$ at infinity. The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) is

$$
\boxed{\partial_tg_t(z)=\frac{2}{g_t(z)-W_t},\qquad g_0(z)=z,\qquad W_t=\sqrt\kappa\,\beta_t.}
$$

It holds up to the [Loewner swallowing time](../../../stochastic-process.md#interior-point-swallowing-time-for-a-loewner-chain) of $z$. Although $\beta$ is nowhere differentiable, it is continuous: the equation for $g$ is an ordinary integral equation with a continuous time-dependent coefficient away from its pole.

For $x\in\mathbb R\setminus\{0\}$, the same real-valued equation has a unique solution until $g_t(x)-W_t$ first reaches zero. Its solution agrees with the boundary value of the [conformal map](../../../geometry-and-topology.md#conformal-map) from the unswallowed side. One can also obtain it by [Schwarz reflection](../../../complex-analysis.md#schwarz-reflection-principle) across an unswallowed real interval. Thus

$$
\boxed{T(x)=\inf\{t:g_t(x)=W_t\}}
$$

is the [boundary-point swallowing time for a Loewner chain](../../../stochastic-process.md#boundary-point-swallowing-time-for-a-loewner-chain); it can be infinite. The collision definition agrees with membership in the closed hull. The initial point has $T(0)=0$. Swallowing a real point is not the same as visiting it: a curve can cut off an entire real interval in one step.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Before $T(x)$, the centered image satisfies the [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation)

$$
dX_t=\frac2{X_t}\,dt-\sqrt\kappa\,d\beta_t,\qquad X_0=x>0.
$$

Changing the sign of the [Brownian motion](../../../brownian-motion.md) shows that $X/\sqrt\kappa$ is a [Bessel process](../../../brownian-motion.md#bessel-process) of dimension $1+4/\kappa$. Here is a direct proof of the relevant hitting property, including finite lifetime.

Put $p=1-4/\kappa>0$. By the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), the drift of $X^p$ is

$$
pX^{p-2}\left(2+\frac\kappa2(p-1)\right)=0.
$$

Thus $X^p$ is a [local martingale](../../../martingale.md#local-martingale) and a [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes). Fix $R>x$. The nonnegative function

$$
u_R(v)=\frac{R^{2-p}v^p-v^2}{\kappa+4},\qquad 0\leq v\leq R,
$$

vanishes at both endpoints and satisfies $\mathcal Lu_R=-1$, for $\mathcal L=(\kappa/2)\partial_{vv}+(2/v)\partial_v$. Stop first on $[\epsilon,R]$, and also at a deterministic time. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives $\mathbb E(t\wedge\tau_{\epsilon,R})\leq u_R(x)$. Let $t\to\infty$ and then $\epsilon\downarrow0$. It follows that the first exit $\tau_{0,R}$ is finite almost surely, not merely that the path approaches a boundary at infinite time.

[Optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) applied to $X^p$ on this bounded interval gives

$$
\mathbb P_x(\tau_R<\tau_0)=\left(\frac{x}{R}\right)^p.
$$

On $\{\tau_0=\infty\}$ the process must therefore hit every $R>x$ before zero. Letting $R\to\infty$ makes that probability zero. Consequently

$$
\boxed{\kappa>4\ \Longrightarrow\ T(x)<\infty\quad\text{almost surely}.}
$$

At $\kappa=4$ the dimension is two; zero is not hit from a positive starting point. This endpoint must not be included in the finite-swallowing assertion.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $\lambda>0$, define $\widetilde g_t(z)=\lambda^{-1/2}g_{\lambda t}(\sqrt\lambda z)$. Differentiating the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives

$$
\partial_t\widetilde g_t(z)=\frac2{\widetilde g_t(z)-\widetilde W_t},
\qquad \widetilde W_t=\lambda^{-1/2}W_{\lambda t}.
$$

[Brownian scaling](../../../brownian-motion.md#brownian-scaling) makes $\widetilde W$ have the original driver law. The corresponding hull is $\lambda^{-1/2}K_{\lambda t}$, so

$$
\boxed{(K_{\lambda t})_{t\geq0}\overset d=(\sqrt\lambda K_t)_{t\geq0}.}
$$

The time scaling applies to the whole coupled hull process. In particular, the joint law of swallowing times satisfies $(T(cx),T(cy))\overset d=c^2(T(x),T(y))$.

Thus $F(cx,cy)=F(x,y)$. A pair $0<x<y$ is determined up to dilation by $z=y/(y-x)>1$: dilating by $(y-x)^{-1}$ turns it into $(z-1,z)$. Define $f(z)=F(z-1,z)$. Then

$$
\boxed{F(x,y)=f\!\left(\frac{y}{y-x}\right).}
$$

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Put $X_t=g_t(x)-W_t$, $Y_t=g_t(y)-W_t$ and $D_t=Y_t-X_t$. Before $T(x)$, order preservation gives $0<X_t<Y_t$ and $D_t>0$. The common noise cancels from their difference:

$$
dD_t=\left(\frac2{Y_t}-\frac2{X_t}\right)dt
=-\frac{2D_t}{X_tY_t}\,dt.
$$

Since $D$ has finite variation, applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $Z=Y/D$ gives the [SLE two-boundary-point ratio diffusion](../../../stochastic-process.md#sle-two-boundary-point-ratio-diffusion)

$$
\boxed{dZ_t=-\frac{\sqrt\kappa}{D_t}\,d\beta_t
+\frac2{D_t^2}\left(\frac1{Z_t}+\frac1{Z_t-1}\right)dt,\qquad Z_t>1.}
$$

With the strictly increasing clock $u(t)=\int_0^tD_s^{-2}ds$, the [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) yields a [Brownian motion](../../../brownian-motion.md) $B$ for which the time-changed process obeys

$$
d\widehat Z_u=\sqrt\kappa\,dB_u
+2\left(\frac1{\widehat Z_u}+\frac1{\widehat Z_u-1}\right)du.
$$

The sign of the new [Brownian motion](../../../brownian-motion.md) has absorbed the minus sign above.

The [domain Markov property of a chordal Loewner chain](../../../stochastic-process.md#domain-markov-property-of-a-chordal-loewner-chain) says that, conditionally on the past before $T(x)$, the mapped future is a fresh [SLE](../../../stochastic-process.md#schramm-loewner-evolution). Its boundary marked points are $X_t,Y_t$. Hence

$$
\mathbb P(T(x)<T(y)\mid\mathcal F_t)=F(X_t,Y_t)=f(Z_t),\qquad t<T(x).
$$

Localize, for example, where $D_t\geq1/n$, $Z_t\in[1+1/n,n]$ and $t\leq n$. On each such stopped interval this is a bounded [conditional-expectation martingale](../../../martingale.md#conditional-expectation-martingale), and therefore a genuine [martingale](../../../martingale.md). No smoothness assumption on $f$ is needed for this argument. The exit calculation below identifies it explicitly.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/i">i</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/i/solution">Solution</h5>

↑ **Parent:** [I](#1/d/i)

Differentiate once less than might seem necessary: writing $v=h'$ turns the equation into

$$
\frac{v'(z)}{v(z)}=-\frac4\kappa\left(\frac1z+\frac1{z-1}\right).
$$

Uniqueness for this first-order linear equation also covers the solution $v\equiv0$. Thus every solution has $h'(z)=C[z(z-1)]^{-4/\kappa}$. Since $4/\kappa<1$, the derivative is integrable at $1$. The specified boundary value fixes the additive constant, giving

$$
\boxed{h(z)=C\,s_\kappa(z),\qquad
s_\kappa(z)=\int_1^z[v(v-1)]^{-4/\kappa}\,dv,\qquad C>0.}
$$

The strict positivity forces $C>0$; $C=0$ gives the zero function. These are all the positive solutions. The function $s_\kappa$ is the increasing [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) for the ratio process.

<h4 id="1/d/ii">ii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/d/ii)

As $v\to\infty$, $[v(v-1)]^{-4/\kappa}\sim v^{-8/\kappa}$. Therefore

$$
s_\kappa(z)\sim
\begin{cases}
\dfrac{z^{1-8/\kappa}}{1-8/\kappa},&\kappa>8,\\
\log z,&\kappa=8.
\end{cases}
$$

Thus **every positive solution is unbounded when κ ≥ 8**, including the logarithmically divergent critical case. For $4<\kappa<8$, by contrast,

$$
S_\kappa:=s_\kappa(\infty)<\infty.
$$

For example the substitution $r=1-1/v$ identifies this normalizing constant as $B(1-4/\kappa,8/\kappa-1)$, with both [beta function](../../../complex-analysis.md#beta-function) parameters positive.

<h4 id="1/d/iii">iii</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/d/iii)

For any $C^2$ function $h$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and the ratio equation give

$$
dh(Z_t)=-\frac{\sqrt\kappa\,h'(Z_t)}{D_t}\,d\beta_t
+\frac1{D_t^2}\left[\frac\kappa2h''(Z_t)
+2\left(\frac1{Z_t}+\frac1{Z_t-1}\right)h'(Z_t)\right]dt.
$$

The bracket is zero for the functions just found. On compact localized intervals the stochastic integrand is bounded, so the stochastic integral is a [martingale](../../../martingale.md). Removing localization proves that $h(Z_t)$, on $0\leq t<T(x)$, is a [local martingale](../../../martingale.md#local-martingale). It is nonnegative because $Z_t>1$ and $C>0$.

In particular it is a [nonnegative local martingale](../../../martingale.md#nonnegative-local-martingale), hence a [supermartingale](../../../martingale.md#supermartingale) after the usual stopping and extension by its endpoint limit. This is the justification for using its maximal inequality; it is not automatically an unstopped uniformly integrable [martingale](../../../martingale.md).

<h4 id="1/d/iv">iv</h4>

↑ **Parent:** [D](#1/d)

<h5 id="1/d/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/d/iv)

The time-changed diffusion has generator $\mathcal A=(\kappa/2)\partial_{zz}+2(1/z+1/(z-1))\partial_z$. For $1<z<R$, its [boundary hitting probability from a diffusion scale function](../../../stochastic-calculus.md#boundary-hitting-probability-from-a-diffusion-scale-function) is

$$
\mathbb P_z(\tau_R<\tau_1)=\frac{s_\kappa(z)}{s_\kappa(R)}.
$$

To see this directly, stop the scale [local martingale](../../../martingale.md#local-martingale) on $[1+\epsilon,R]$ and pass to $\epsilon\downarrow0$. Exit from $(1,R)$ occurs in finite clock time: the scale density behaves as $(z-1)^{-4/\kappa}$ and the speed density as $(z-1)^{4/\kappa}$, so the usual scale-times-speed exit integral is finite at $1$. More explicitly, with $m(v)=2/(\kappa s_\kappa'(v))$ the [finite-interval diffusion exit Green kernel](../../../stochastic-calculus.md#finite-interval-diffusion-exit-green-kernel) gives

$$
\mathbb E_z\tau_{1,R}=\int_1^R
\frac{s_\kappa(z\wedge v)[s_\kappa(R)-s_\kappa(z\vee v)]}{s_\kappa(R)}\,m(v)\,dv.
$$

The equation $\mathcal A u=-1$ follows by differentiation and the derivative jump at $v=z$, so stopping the corresponding Itô identity gives this exit bound. The integrand near $1$ is $O(v-1)$; elsewhere it is bounded. At large $z$ the drift is bounded, excluding explosion at infinity in finite clock time.

Here is why these exits describe the original swallowing event. In clock time,

$$
D(u)=D(0)\exp\left(-2\int_0^u\frac{dv}{\widehat Z_v(\widehat Z_v-1)}\right).
$$

If $\widehat Z$ hits $1$ at finite $u$, its integrated [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) shows $\int_0^{\tau_1}(\widehat Z_v-1)^{-1}dv<\infty$: the Brownian term has a finite limit and both positive drift integrals must then have finite limits. Consequently $D(\tau_1)>0$, $X$ hits zero and $Y$ stays positive. This gives $T(x)<T(y)$.

Conversely $T(x)$ is finite by part (b). If its clock ends at a finite value, the diffusion must hit $1$; an interior endpoint with positive $D$ would leave $X$ positive. If the clock runs forever without hitting $1$, the standard one-dimensional scale classification gives escape to infinity whenever $S_\kappa<\infty$. This cannot represent a strict swallowing event, which has $D\to Y_{T(x)}>0$ and $Z\to1$. Hence the surviving event represents $T(x)=T(y)$. This reasoning also explains why a simultaneous collision must be treated separately rather than assigned the boundary value at $1$.

For $\kappa\geq8$, the scale is unbounded. The [maximal inequality for a nonnegative supermartingale](../../../martingale.md#maximal-inequality-for-a-nonnegative-supermartingale) gives $\mathbb P(\sup s_\kappa(\widehat Z)\geq s_\kappa(R))\leq s_\kappa(z)/s_\kappa(R)$; letting $R\to\infty$ rules out escape. Finite-interval exit then forces a hit at $1$. For $4<\kappa<8$, taking $R\to\infty$ gives

$$
\boxed{F(x,y)=1-\frac{s_\kappa(y/(y-x))}{S_\kappa},\qquad
\mathbb P(T(x)=T(y))=\frac{s_\kappa(y/(y-x))}{S_\kappa}>0.}
$$

The strict-event probability is also positive, since $0<s_\kappa(z)<S_\kappa$ for finite $z$.

For $\kappa\geq8$, first intersect the probability-one strict-order events over rational $0<a<b$. The real boundary flow gives nondecreasing swallowing times on $(0,\infty)$. For any $0<x<y$, choose rational $x<a<b<y$; then $T(x)\leq T(a)<T(b)\leq T(y)$. This proves the simultaneous assertion

$$
\boxed{\text{almost surely }T(x)<T(y)\text{ for every }0<x<y,\quad\kappa\geq8.}
$$

The range is positive points, as in the definition of $F$; reflection reverses the ordering on the negative axis. At the printed endpoint $\kappa=4$, each fixed positive point has $T=\infty$. Thus $\mathbb P(T(x)=T(y))=1$ if equality of extended times is allowed, but there is no finite simultaneous-swallowing assertion there. The preceding formulas assume $\kappa>4$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Work in the intended $\kappa\geq8$ regime. On one probability-one event, all positive points have finite swallowing times and the strict ordering from part (d) holds for all pairs. Finiteness for arbitrary points follows from finiteness for rational points and monotonicity. Reflection supplies the negative-axis version on the same event.

Fix $r>0$ and suppose the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) has not visited $r$ by $T(r)$. Its image up to this finite time is compact, so a small interval $I$ about $r$, together with a thin upper collar, is disjoint from the whole trace segment. Every point of that collar belongs to the same component of the complement at every earlier time. Thus all points in a smaller interval are disconnected from infinity at precisely the same time as $r$: before $T(r)$ none is swallowed, and at $T(r)$ all are. This contradicts strict ordering for two positive points in that interval.

Therefore $r$ is visited by time $T(r)$. It cannot be visited before its swallowing time, so the visit occurs at $T(r)$. The same deterministic argument works for every real $r<0$ by reflection, while $0$ is the starting point. Hence

$$
\boxed{\gamma[0,\infty)\supseteq\mathbb R\quad\text{almost surely},\qquad\kappa\geq8.}
$$

The threshold matters. If part (e) is read as retaining only $\kappa>4$, it is false: for $4<\kappa<8$, part (d) gives positive probability of swallowing a nonempty interval at one time, although a continuous trace can visit at most one of its points at that instant. Interior points of that swallowed boundary interval cannot subsequently be reached in capacity time: a later visit, by continuity, would make the curve stay inside an already filled hull for a time interval, contradicting strictly increasing [half-plane capacity](../../../stochastic-process.md#half-plane-capacity). Thus the preceding $\kappa\geq8$ conclusion is the necessary intended qualification.

## 2

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

At criticality, [percolation clusters](../../../bond-percolation.md#percolation-cluster) occur on every scale. Count their filled outer perimeters, discard microscopic loops through a diameter cutoff, and then pass to a [scaling limit](../../../convergence-of-random-variables.md#scaling-limit-of-a-random-curve). The cutoff gives a locally finite measure on loops of macroscopic size inside a bounded region; summing over scales gives a [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) rather than a probability distribution.

The [conformal invariance of planar percolation](../../../probability-theory.md#conformal-invariance-of-planar-percolation) makes these limiting perimeter statistics covariant under [conformal maps](../../../geometry-and-topology.md#conformal-map). Moreover, deciding whether a filled outer perimeter lies in a simply connected subdomain uses only the configuration it encloses: changing the configuration outside that subdomain does not change that perimeter. This is the restriction part of the argument. Conformal [covariance](../../../variance.md#covariance) together with this domain consistency motivates a nonzero [conformal restriction measure on simple loops](../../../brownian-motion.md#conformal-restriction-measure-on-simple-loops).

This is an informal construction principle, as requested; it does not replace the tightness, boundary-simplification and uniqueness theorems required to construct the continuum measure rigorously.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Use finite cutoff windows to avoid subtracting two infinite masses. Write $D$ for the unit disc, $D_U=\mathbf L_D\setminus\mathbf L_U$ on loops surrounding $0$, and $A(U)=\nu(D_U)$. For $0<r<1$, let $H_r=D_{rD}$. These increase to all loops in $\mathbf L_D$ surrounding $0$ as $r\downarrow0$.

On the finite-mass windows, the domain-containment events form a [pi-system](../../../measure-theory.md#pi-system). Indeed, if $U,V$ are simply connected and contain $0$, a simple loop surrounding $0$ that lies in both has its filled interior in both. It therefore lies in the component $W$ of $U\cap V$ containing $0$, which is simply connected. Thus, on the support of $\nu$,

$$
\mathbf L_U\cap\mathbf L_V=\mathbf L_W.
$$

[Inclusion-exclusion](../../../combinatorics.md#inclusion-exclusion-principle) for the finite deficits gives

$$
\nu(D_U\cap D_V)=A(U)+A(V)-A(W).
$$

Taking $V=rD$ and subtracting from $\nu(H_r)$ gives the useful recovery formula

$$
\boxed{\nu(H_r\cap\mathbf L_U)=A(W)-A(U),\qquad
W=\text{the component of }rD\cap U\text{ containing }0.}
$$

The assumed generation of the loop sigma-field by domain-containment events and the [uniqueness theorem for measures](../../../measure-theory.md#sigma-finite-uniqueness-theorem-for-measures) now determine the finite restriction to $H_r$. Increasing these windows recovers $\nu_D$; conformal transport recovers its restriction to any simply connected domain containing the marked point. If a simply connected domain omits $0$, no loop in it can surround $0$.

The argument uses finite annular deficits. This is the usual local-finiteness convention for these loop measures and is explicitly ensured by the finite logarithmic formula assumed in the continuation. Bare sigma-finiteness must not be used as permission for formal $\infty-\infty$ subtraction. This is the [recovery of a loop measure from conformal deficits](../../../brownian-motion.md#recovery-of-a-loop-measure-from-conformal-deficits).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Let $\phi_i:D\to U_i$ be the normalized maps, and put $V=\phi_1(U_2)$. A simple loop in $U_1$ has its interior there, so applying $\phi_1^{-1}$ preserves the property of surrounding $0$. There is a disjoint decomposition

$$
\mathbf L_D\setminus\mathbf L_V
=(\mathbf L_D\setminus\mathbf L_{U_1})
\ \dot\cup\ (\mathbf L_{U_1}\setminus\mathbf L_V).
$$

The conformal restriction property identifies the measure of the second set with $\nu(\mathbf L_D\setminus\mathbf L_{U_2})$. Therefore

$$
\boxed{A^\nu(\phi_1\circ\phi_2)=A^\nu(\phi_1)+A^\nu(\phi_2).}
$$

The composition fixes $0$ and has positive derivative there, so it is exactly the normalized map onto $V$. No interchange of infinite differences is needed: the argument is additivity on disjoint sets. The later logarithmic expression is consistent with this identity because $(\phi_1\circ\phi_2)'(0)=\phi_1'(0)\phi_2'(0)$.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Let $\Gamma(B)$ be the [outer boundary of a planar compact set](../../../topology.md#outer-boundary-of-a-planar-compact-set) applied to the Brownian loop. For the pinned Brownian measure here, its outer boundary is almost surely simple and surrounds its root. If $U$ is simply connected, then

$$
B\subset U\quad\Longleftrightarrow\quad\Gamma(B)\subset U.
$$

The forward implication uses the fact that filling a compact subset of a simply connected domain cannot leave that domain. For the converse, the Brownian trace is contained in the closed filled interior of its outer boundary, and that interior also lies in $U$. This is precisely why simply connected domains are used.

Let $\eta=\Gamma_*\rho$, a [pushforward measure](../../../measure-theory.md#pushforward-measure) on simple loops surrounding $0$. Its deficits are

$$
\eta(\mathbf L_D\setminus\mathbf L_U)
=\rho(B\not\subset U)
=-\log\Phi_U'(0).
$$

They agree with those of $\lambda\eta$ and $\nu_D$. The recovery argument from part (i), now with explicitly finite deficits, gives

$$
\boxed{\nu_D=\lambda\,\Gamma_*\rho.}
$$

If $\lambda=0$, the measure is zero on every cutoff window and hence zero. The rooted Brownian loop itself is not a simple loop; taking its outer boundary is essential.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Restrict $\mu$ first to loops surrounding $0$. This satisfies the pointed restriction property, so for one constant $C$,

$$
\boxed{\mu_D\big|_{E_0}=C\,\Gamma_*\rho.}
$$

A single rooted pushforward cannot equal the whole $\mu_D$: it only sees loops surrounding its root. The rest is recovered by moving that root.

For $z\in D$, choose a disc automorphism $\psi_z$ with $\psi_z(0)=z$. Conformal restriction yields

$$
\mu_D\big|_{E_z}=C\,(\psi_z\circ\Gamma)_*\rho,
$$

with the same constant. Let $(z_j)$ be a countable dense set in $D$. Every simple loop contained in $D$ surrounds one of these points. Make this cover disjoint by $P_j=E_{z_j}\setminus\bigcup_{i<j}E_{z_i}$. For a measurable event $A$ of loops in $D$,

$$
\boxed{\mu_D(A)=C\sum_j\rho\{B:\psi_{z_j}(\Gamma(B))\in A\cap P_j\}.}
$$

This explicitly relates the entire loop measure to the single-root measure without overcounting a loop once for every point in its interior. It also proves that knowledge of $\rho$, up to normalization, determines $\mu_D$. Nontriviality gives $C>0$: otherwise all countably many pointed patches would vanish. Using the usual unrooted [Brownian loop measure](../../../brownian-motion.md#brownian-loop-measure), the same construction is commonly expressed as its outer-boundary pushforward, up to a constant.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Put $a=1/4$ and $E-a=\{\gamma-a:\gamma\in E\}$. Both events consist of loops surrounding $0$; $E-a$ lies in the disc of radius $3/4$, so its loops remain in $D$. Translation invariance and the pointed representation imply

$$
C\,\rho\{\Gamma(B)\in E\}=\mu(E)=\mu(E-a)
=C\,\rho\{\Gamma(B)\in E-a\}.
$$

Since $C>0$, cancel it. Outer boundaries commute with translation, and $\Gamma(B)\in E-a$ is exactly $\Gamma(B+a)\in E$. Hence

$$
\boxed{\rho\{\Gamma(B)\in E\}=\rho\{\Gamma(B+1/4)\in E\}.}
$$

The half-disc condition ensures that translating a relevant filled Brownian trace still lies inside the original unit-disc cutoff. This proves the asserted event identity; it does not claim translation invariance of the entire measure rooted at $0$.

## 3

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $D$ be the unit disc and normalize its positive [Poisson kernel](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) at the boundary point $1$ by

$$
h(z)=\frac{1-|z|^2}{|1-z|^2},\qquad h(0)=1.
$$

It is harmonic in $D$. Let $p_D(t,z,w)$ be the killed [Brownian transition density](../../../brownian-motion.md#brownian-transition-density), for [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) with generator $\tfrac12\Delta$. The [Doob h-transform](../../../markov-process.md#doob-h-transform) has sub-Markov transition density

$$
\boxed{p_D^h(t,z,w)=p_D(t,z,w)\frac{h(w)}{h(z)}.}
$$

Its missing mass represents paths already absorbed at the distinguished boundary point. Equivalently, for a stopping time $\sigma$ before exit from a compact subdomain, its law is weighted relative to ordinary killed [Brownian motion](../../../brownian-motion.md) by $h(B_\sigma)/h(B_0)$. These stopped laws are consistent and define a diffusion up to its lifetime. Its generator is

$$
\mathcal L^hf=\frac1h\frac12\Delta(hf)=\frac12\Delta f+\nabla\log h\cdot\nabla f.
$$

This is a rigorous [Brownian motion conditioned to exit at a boundary point](../../../markov-process.md#brownian-motion-conditioned-to-exit-at-a-boundary-point), not conditioning on an event of positive probability. Exhaustion of $D$ shows that its terminal boundary limit is $1$; its lifetime is finite. For example its expected lifetime from $0$ is $\int_DG_D^{\mathrm{BM}}(0,w)h(w)\,dw$, which is finite: the Green function vanishes linearly near the smooth boundary and cancels the Poisson-kernel singularity there, while its logarithmic singularity at $0$ is integrable.

One can also condition ordinary [Brownian motion](../../../brownian-motion.md) on exiting through an arc $I_\epsilon$ about $1$, and then let its length decrease to zero. The conditional harmonic functions $\omega_D(z,I_\epsilon)/\omega_D(0,I_\epsilon)$ converge locally uniformly to $h(z)$. Thus their stopped conditional laws converge to this same diffusion. Both constructions specify the conditioning unambiguously.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Here the map direction is opposite to Question 2: write $\phi:U\to D$, with $\phi(0)=0$ and $\phi(1)=1$. The separation condition makes $U$ agree with $D$ near $1$. [Schwarz reflection](../../../complex-analysis.md#schwarz-reflection-principle) across that analytic boundary arc therefore defines the boundary derivative, whose modulus is positive.

For ordinary [Brownian motion](../../../brownian-motion.md) $W$ started at $0$, let $\sigma_U$ be its first exit from $U$. Take sufficiently short arcs $I_\epsilon$ around $1$. They are also arcs of $\partial U$. The event that $W$ stays in $U$ until its disc exit and exits in $I_\epsilon$ is exactly the event $W_{\sigma_U}\in I_\epsilon$. Therefore the conditional avoidance probability is

$$
\frac{\omega_U(0,I_\epsilon)}{\omega_D(0,I_\epsilon)}.
$$

[Conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) gives $\omega_U(0,I_\epsilon)=\omega_D(0,\phi(I_\epsilon))$. At the disc center [harmonic measure](../../../brownian-motion.md#harmonic-measure) is normalized arc length, so the ratio tends to $|\phi'(1)|$.

To justify that this limit is the avoidance probability for the point-conditioned diffusion, one may use the stopped transform directly. Its probability of reaching a smooth boundary arc at $1$ before any other boundary of $U$ is the mass at that pole in the transformed [harmonic measure](../../../brownian-motion.md#harmonic-measure). All other exit points have weights $h(w)$ and represent failure. Equivalently integrate the Poisson-kernel density at $1$ for $U$ and divide by that for $D$. This gives the boundary-density ratio above, without assuming that a full-path avoidance event is a continuity set for arbitrary weak convergence. The kernels transform by the boundary Jacobian:

$$
P_U(0,1)=P_D(\phi(0),\phi(1))\,|\phi'(1)|.
$$

Consequently

$$
\boxed{\mathbb P(B[0,\tau)\subset U)=\frac{P_U(0,1)}{P_D(0,1)}=|\Phi_U'(1)|.}
$$

There is no extra factor of $|\Phi_U'(0)|$. The starting point is fixed and the conditioning concerns boundary harmonic-measure density. In this normalization the boundary derivative is a positive real, so it may also be written $\Phi_U'(1)$. It is at most one by the probability interpretation. Given avoidance, the mapped path is the same conditioned [Brownian motion](../../../brownian-motion.md) up to conformal time change; this is [radial restriction for a conditioned Brownian path](../../../markov-process.md#radial-restriction-for-a-conditioned-brownian-path).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

One precise relation is to [radial SLE](../../../stochastic-process.md#radial-schramm-loewner-evolution) with parameter $2$. Its orientation is from the boundary point $1$ to the interior target $0$. With conformal-radius time it is defined by

$$
\partial_tg_t(z)=g_t(z)\frac{e^{i\theta_t}+g_t(z)}{e^{i\theta_t}-g_t(z)},
\qquad\theta_t=\sqrt2\,\beta_t,\qquad g_t'(0)=e^t.
$$

There is a coupling of the conditioned Brownian path $B$ with this simple radial curve $\eta$ such that, for each initial curve segment, the first point at which $B$ encounters it is its tip. More precisely, if $s_t=\inf\{s:B_s\in\eta[0,t]\}$, then $B_{s_t}=\eta(t)$. Reversing the Brownian path turns these first-hit times into the last-visit times that characterize [loop-erasure of planar Brownian motion](../../../markov-process.md#loop-erasure-of-planar-brownian-motion). Thus

$$
\boxed{\eta\text{ is a loop-erasure of the time reversal of }B,
\qquad\eta\sim\operatorname{radial\ SLE}_2(D;1\to0).}
$$

This is an existence statement for a coupling, not a pointwise equality of the two processes or a claim that a naive finite-loop deletion algorithm applies to [Brownian motion](../../../brownian-motion.md).

Here is the [martingale](../../../martingale.md) mechanism behind the coupling. Put $a_t=e^{i\theta_t}$ and

$$
Q_t(z)=\operatorname{Re}\frac{a_t+g_t(z)}{a_t-g_t(z)}.
$$

This is the positive slit-domain [Poisson kernel](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) at the tip, normalized by $Q_t(0)=1$. Writing $q_t=g_t(z)/a_t$, the radial equation gives

$$
dq_t=-i\sqrt\kappa\,q_t\,d\beta_t+
\left[q_t\frac{1+q_t}{1-q_t}-\frac\kappa2q_t\right]dt.
$$

The drift of $(1+q_t)/(1-q_t)$ is $(2-\kappa)q_t(1+q_t)/(1-q_t)^3$, so $Q_t(z)$ is a [local martingale](../../../martingale.md#local-martingale) at $\kappa=2$.

Start independent stopped $B$ and [radial SLE2](../../../stochastic-process.md#radial-sle2), and weight their joint laws, before meeting, by

$$
L(s,t)=\frac{Q_t(B_s)}{h(B_s)}.
$$

For fixed $s$ this is an [SLE](../../../stochastic-process.md#schramm-loewner-evolution) [local martingale](../../../martingale.md#local-martingale). For fixed $t$ it is a Brownian-transform [local martingale](../../../martingale.md#local-martingale), because $\mathcal L^h(Q_t/h)=(2h)^{-1}\Delta Q_t=0$. Since $L(0,t)=L(s,0)=1$, localized two-parameter weighting preserves both original marginals. For a fixed slit, the changed Brownian law is the transform by $Q_t$, so it hits that slit at the pole, its tip. Compatible stopped couplings, followed by exhaustion, give the first-hit-at-tip property. This completion is the substantive continuum coupling step. Discrete [loop-erased random walks](../../../markov-process.md#loop-erased-random-walk) and their radial-SLE2 limit give a parallel approximation picture.

For example, in this coupling avoidance by $B$ implies avoidance by $\eta$, since the radial curve is contained in the Brownian trace. The probability from part (b) therefore supplies a lower bound $|\phi'(1)|\leq\mathbb P(\eta\subset U)$. The two avoidance laws are not identical: unweighted simple radial $\operatorname{SLE}_2$ does not have the Brownian radial-restriction property. This is a way to transfer path-containment information while retaining the distinct geometry and orientation of the two random curves.

## 4

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) is a random distribution, so its purported level curve cannot be defined by evaluating its height at every point. A coupling must instead be stated using conditional means and covariances. The [SLE4 coupling with a Gaussian free field](../../../stochastic-process.md#sle4-coupling-with-a-gaussian-free-field) does exactly this.

Choose the Green-function normalization

$$
G_{\mathbb H}(z,w)=\log\left|\frac{z-\overline w}{z-w}\right|,
\qquad -\Delta_zG_{\mathbb H}(z,w)=2\pi\delta_w(z).
$$

A [Zero-boundary Gaussian free field](../../../stochastic-process.md#zero-boundary-gaussian-free-field) $H_0$ is characterized on real compactly supported smooth [test functions](../../../distribution-theory.md#test-function) by

$$
\mathbb E(H_0,\varphi)=0,\qquad
\operatorname{Cov}((H_0,\varphi),(H_0,\psi))
=\iint\varphi(z)G_{\mathbb H}(z,w)\psi(w)\,dA(z)dA(w).
$$

Equivalently its energy normalization is the [Dirichlet inner product](../../../sobolev-space.md#dirichlet-inner-product) $(2\pi)^{-1}\int\nabla f\cdot\nabla g\,dA$. This fixes the otherwise convention-dependent height constant.

Set $\lambda=\pi/2$ and

$$
m_0(z)=\lambda-\frac{2\lambda}{\pi}\arg z,
\qquad H=H_0+m_0.
$$

The field $H$ has prescribed Dirichlet values $-\lambda$ on the negative half-line and $+\lambda$ on the positive half-line. Subtracting $m_0$ recovers the zero-Dirichlet field $H_0$. It is the shifted field $H$, rather than an unshifted zero-boundary field, whose zero-height interface has ordinary chordal $\operatorname{SLE}_4$ law.

Let $\eta$ be chordal $\operatorname{SLE}_4$ from $0$ to $\infty$, with [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) $\partial_tg_t=2/(g_t-W_t)$ and $W_t=2\beta_t$. Write $D_t=\mathbb H\setminus\eta[0,t]$ and $f_t=g_t-W_t$. The coupling statement is:

$$
\boxed{\mathcal L(H\mid\eta[0,t])=
\mathcal L\bigl(H^{D_t}_0+m_t\bigr),\qquad
m_t(z)=\lambda-\frac{2\lambda}{\pi}\arg f_t(z),}
$$

where, conditionally on the curve, $H^{D_t}_0$ is an independent zero-boundary field in the slit domain. The equality is for restrictions to [test functions](../../../distribution-theory.md#test-function) in that domain, and extends to suitable stopping times. Its [covariance](../../../variance.md#covariance) is $G_{D_t}(z,w)=G_{\mathbb H}(f_t(z),f_t(w))$ by conformal invariance. The two sides of the revealed slit have heights $-\lambda$ and $+\lambda$, in the order specified by their real images under $f_t$. This is the continuum meaning of a [Gaussian free field level line](../../../stochastic-process.md#gaussian-free-field-level-line).

The fundamental calculations explain why the parameter is four. For $Z_t=f_t(z)$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
d\log Z_t=\frac{2-\kappa/2}{Z_t^2}\,dt
-\frac{\sqrt\kappa}{Z_t}\,d\beta_t.
$$

At $\kappa=4$ the drift vanishes. Thus

$$
dm_t(z)=\frac{4\lambda}{\pi}\operatorname{Im}\frac1{f_t(z)}\,d\beta_t
=2\operatorname{Im}\frac1{f_t(z)}\,d\beta_t.
$$

Each harmonic mean is a bounded [martingale](../../../martingale.md) before approaching its point. Differentiating the explicit conformally transformed Green function gives the [Loewner variation of the Dirichlet Green function](../../../stochastic-process.md#loewner-variation-of-the-dirichlet-green-function)

$$
\frac d{dt}G_{D_t}(z,w)
=-4\operatorname{Im}\frac1{f_t(z)}\operatorname{Im}\frac1{f_t(w)}.
$$

Therefore

$$
\boxed{d\langle m(z),m(w)\rangle_t=-dG_{D_t}(z,w).}
$$

In words, the variance learned from the evolving mean exactly equals the [covariance](../../../variance.md#covariance) lost when the slit is removed. For a Green kernel $cG$ the same calculation gives $\lambda=(\pi/2)\sqrt c$; using a different Green normalization changes the height constant, not the [SLE](../../../stochastic-process.md#schramm-loewner-evolution) parameter.

To construct the coupling, first sample the [SLE](../../../stochastic-process.md#schramm-loewner-evolution) curve. In the two components to its left and right, sample independent zero-boundary fields and add the corresponding constant heights. Extend these as distributions to obtain the candidate full field. The following [martingale](../../../martingale.md) identity proves its marginal law rather than merely matching its first two moments.

For a real [test function](../../../distribution-theory.md#test-function) $\varphi$, put $M_t=(m_t,\varphi)$ and

$$
V_t=\iint\varphi(z)G_{D_t}(z,w)\varphi(w)\,dA(z)dA(w).
$$

Localization permits integration of the pointwise identities. They yield $d\langle M\rangle_t=-dV_t$. Hence

$$
\mathcal Z_t=\exp\left(iM_t-\frac12V_t\right)
$$

is a complex [local martingale](../../../martingale.md#local-martingale): the $-\tfrac12dV_t$ drift cancels the $-\tfrac12d\langle M\rangle_t$ Itô correction. Since $V_t\geq0$, $|\mathcal Z_t|\leq1$, making it a true [martingale](../../../martingale.md). At the complete-curve limit, $m_t$ becomes the constant height in each component and the remaining Green kernel becomes that of those components. Thus $\mathcal Z_\infty$ is the conditional [characteristic function](../../../probability-theory.md#characteristic-function) of the sampled candidate field. Taking expectations gives

$$
\mathbb E\mathcal Z_\infty
=\exp\left(i(m_0,\varphi)-\frac12\iint\varphi G_{\mathbb H}\varphi\right).
$$

Applying this to every linear combination of [test functions](../../../distribution-theory.md#test-function) proves the entire Gaussian law, not only its [covariance](../../../variance.md#covariance). The conditional version $\mathbb E(\mathcal Z_\infty\mid\mathcal F_t)=\mathcal Z_t$ proves the displayed conditional-field statement. Exhaustion by compact test supports justifies passage across the slit and the limiting distributional extensions.

This revealed curve is a [local set of a Gaussian free field](../../../stochastic-process.md#local-set-of-a-gaussian-free-field): conditionally on it, the remaining field is a zero-boundary field plus a specified [harmonic function](../../../partial-differential-equation.md#harmonic-function). The spatial Markov property is thereby preserved at random domains, a property not available for arbitrary field-dependent sets. One can strengthen the coupling to a curve measurable from the field. The proof explores compatible interfaces in small subdomains and uses the conditional boundary heights and monotonicity to show that two such interfaces for the same field cannot separate; a countable exhaustion gives uniqueness. This supplies a rigorous replacement for the informal phrase “draw the zero contour.” It does not assert that the distribution has pointwise values.

The coupling is useful in both directions: [SLE](../../../stochastic-process.md#schramm-loewner-evolution) [martingales](../../../martingale.md) give exact conditional [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) data, while the Gaussian Markov structure explains the [SLE](../../../stochastic-process.md#schramm-loewner-evolution) domain Markov property and its distinguished parameter. **With the above normalization, the height jump is $2\lambda=\pi$, and the corresponding interface is [chordal SLE4](../../../stochastic-process.md#chordal-sle4).**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
