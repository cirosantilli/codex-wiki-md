# Paper 39

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper39.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper39.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded relatively closed subset $K$ of $\mathbb H$ with [simply connected](../../../algebraic-topology.md#simply-connected-space) complement, considered together with its compact [closure](../../../topology.md#closure-topology) in $\overline{\mathbb H}$. Its unique [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) has [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity)

$$
g_K:\mathbb H\setminus K\longrightarrow\mathbb H,
\qquad g_K(z)=z+\frac{a_K}{z}+O(z^{-2})\quad(z\to\infty).
$$

The nonnegative coefficient $a_K$ is its [half-plane capacity](../../../stochastic-process.md#half-plane-capacity). Thus the [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) here gives $g_t(z)=z+2t/z+O(z^{-2})$. Strict increase means $K_s\subsetneq K_t$ whenever $s<t$; the strictly increasing capacity already excludes equality.

The [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) means that the new growth becomes small after removing the old [compact H-hull](../../../stochastic-process.md#compact-h-hull). More precisely set $K_{t,t+h}=\overline{g_t(K_{t+h}\setminus K_t)}$, taking the [closure](../../../topology.md#closure-topology) from the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). On each bounded time interval, the diameters of these image [compact H-hulls](../../../stochastic-process.md#compact-h-hull) tend uniformly to zero as $h\downarrow0$. Equivalently the new growth can be separated from infinity by [crosscuts](../../../complex-analysis.md#crosscut) of vanishing diameter in the mapped domain. It is this single-point local growth, together with capacity continuity, that gives a continuous real [Loewner driver](../../../stochastic-process.md#loewner-driving-function).

The [Loewner transform](../../../stochastic-process.md#loewner-driving-function) $\xi_t$ is the limiting point at which this mapped growth occurs:

$$
\boxed{\xi_t=\lim_{h\downarrow0}g_t(z_h),\qquad z_h\in(K_{t+h}\setminus K_t)\cap\mathbb H.}
$$

The limit is independent of the chosen new-growth points. The [Loewner correspondence theorem](../../../stochastic-process.md#loewner-correspondence-theorem) says that the resulting [mapping-out functions](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) satisfy

$$
\partial_tg_t(z)=\frac{2}{g_t(z)-\xi_t},\qquad g_0(z)=z.
$$

Conversely, given a continuous real $\xi$, solve this [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) until the maximal lifetime $T_z$ of each $z\in\mathbb H$. The surviving set $H_t=\{z:T_z>t\}$ is mapped conformally onto $\mathbb H$ by $g_t$; its complement, with the appropriate [boundary](../../../topology.md#boundary-of-a-set) [closure](../../../topology.md#closure-topology), is $K_t$. The [Laurent coefficient](../../../analysis.md#laurent-coefficient) is $2t$, and the composition law reconstructs the local growth. A continuous [Loewner driver](../../../stochastic-process.md#loewner-driving-function) always determines the [compact H-hulls](../../../stochastic-process.md#compact-h-hull); generation by a continuous [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) is an additional property, not a conclusion for every continuous [Loewner driver](../../../stochastic-process.md#loewner-driving-function).

A chordal [SLE](../../../stochastic-process.md#schramm-loewner-evolution) [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) with parameter $\kappa\geq0$ is the continuous curve associated with the [Loewner driver](../../../stochastic-process.md#loewner-driving-function) $\xi_t=\sqrt\kappa B_t$, where $B$ is standard real [Brownian motion](../../../brownian-motion.md) started at zero. It starts at zero, its [compact H-hull](../../../stochastic-process.md#compact-h-hull) at time $t$ is the curve's past with all pockets cut off from infinity filled, and

$$
\gamma(t)=\lim_{y\downarrow0}g_t^{-1}(\xi_t+iy).
$$

The capacity clock has $\operatorname{hcap}(K_t)=2t$. For $\kappa=0$ this gives the vertical slit $\gamma(t)=2i\sqrt t$.

To prove [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle), fix $r>0$ and put

$$
\widehat K_t=r^{-1}K_{r^2t},\qquad
\widehat g_t(z)=r^{-1}g_{r^2t}(rz),\qquad
\widehat\xi_t=r^{-1}\xi_{r^2t}.
$$

The [Laurent series](../../../analysis.md#laurent-series) of $\widehat g_t$ has coefficient $2t$, and direct differentiation gives

$$
\partial_t\widehat g_t(z)=\frac2{\widehat g_t(z)-\widehat\xi_t}.
$$

[Brownian scaling](../../../brownian-motion.md#brownian-scaling) says $(r^{-1}B_{r^2t})_{t\geq0}$ has the same law as $B$. The [Loewner drivers](../../../stochastic-process.md#loewner-driving-function) therefore agree in law, and uniqueness of the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives equality in law of the maps, [compact H-hulls](../../../stochastic-process.md#compact-h-hull), and continuous [Loewner traces](../../../stochastic-process.md#trace-of-a-loewner-chain):

$$
\boxed{(r^{-1}\gamma(r^2t))_{t\geq0}\overset d=(\gamma(t))_{t\geq0}.}
$$

This identifies the time change $t\mapsto r^2t$ as well as the spatial scaling.

For a [simply connected](../../../algebraic-topology.md#simply-connected-space) [Jordan domain](../../../topology.md#jordan-domain) $D$ with distinct marked [boundary](../../../topology.md#boundary-of-a-set) points, choose a [conformal bijection](../../../complex-analysis.md#biholomorphism) $f:\mathbb H\to D$ taking zero to the initial point and infinity to the target, and use $f(\gamma)$ as an unparameterized curve. The [Caratheodory boundary extension theorem](../../../complex-analysis.md#caratheodory-boundary-extension-theorem) supplies the [boundary](../../../topology.md#boundary-of-a-set) values of $f$. Any second such map is $f\circ(z\mapsto rz)$ for $r>0$, because the automorphisms of $\mathbb H$ fixing zero and infinity are positive dilations. The [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) just proved makes the two image laws identical, up to the corresponding deterministic change of capacity clock. Thus this defines [SLE](../../../stochastic-process.md#schramm-loewner-evolution) consistently in marked [Jordan domains](../../../topology.md#jordan-domain). The assumed $|\gamma(t)|\to\infty$ and the continuous [boundary](../../../topology.md#boundary-of-a-set) extension give $f(\gamma(t))\to f(\infty)$, the specified target. The law is conformally natural and does not impose a distinguished [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) on an arbitrary domain.

## 2

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $\xi_t=\sqrt\kappa B_t$ and $0<\kappa<4$. We use these precise [Bessel process](../../../brownian-motion.md#bessel-process) facts, which the question permits: for [dimension](../../../vector-space.md#dimension-vector-space) $\delta>2$ a process started at $r>0$ exists for all time, never reaches zero, and has a strictly positive all-time minimum. More quantitatively,

$$
\mathbb P_r\left(\inf_{t\geq0}R_t\leq\varepsilon\right)
=(\varepsilon/r)^{\delta-2},\qquad0<\varepsilon<r.
$$

No assertion about [SLE](../../../stochastic-process.md#schramm-loewner-evolution) simplicity or transience is being assumed.

For a real point $x>0$ before its Loewner lifetime, set $Z_t^x=g_t(x)-\xi_t$. Its equation is

$$
dZ_t^x=\frac2{Z_t^x}dt-\sqrt\kappa\,dB_t.
$$

Thus $Z^x/\sqrt\kappa$ is a [Bessel process](../../../brownian-motion.md#bessel-process) of [dimension](../../../vector-space.md#dimension-vector-space) $1+4/\kappa>2$. For each rational $x>0$ it stays positive on every finite interval, almost surely. These countably many events hold together. They cover every real $y>0$ as well: choose rational $0<x<y$ and observe that the noise cancels in the difference,

$$
g_t(y)-g_t(x)=(y-x)\exp\left(-2\int_0^t\frac{ds}{Z_s^yZ_s^x}\right)>0.
$$

Consequently $Z^y$ cannot reach zero while $Z^x$ remains positive. The negative side has the identical argument with the reflected [Brownian motion](../../../brownian-motion.md).

This excludes [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) contact with every real point other than zero, rather than just with each fixed rational point. On any finite interval a positive gap at a real point stays bounded away from zero. Continuous dependence of the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) then solves it on a complex neighborhood of that point, and the analytic flow extends the map conformally across a real interval there. Its real [derivative](../../../calculus.md#derivative) is $\exp(-2\int_0^t(Z_s^x)^{-2}ds)>0$, and its image stays away from the driving point. The [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) tip therefore cannot be there. We have proved $\gamma[0,\infty)\cap\mathbb R\subseteq\{0\}$.

Now use [Brownian motion](../../../brownian-motion.md) independent increments to restart at every deterministic rational time $s>0$. The centered future maps have [Loewner driver](../../../stochastic-process.md#loewner-driving-function) $\xi_{s+t}-\xi_s$ and therefore the original [SLE](../../../stochastic-process.md#schramm-loewner-evolution) law, independently of the past. Its [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) stays in $\mathbb H\cup\{0\}$ by the preceding argument. The inverse map $g_s^{-1}$ extends continuously to the real [boundary](../../../topology.md#boundary-of-a-set) for a continuous trace-generated [compact H-hull](../../../stochastic-process.md#compact-h-hull): the finite [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) gives a locally connected [boundary](../../../topology.md#boundary-of-a-set), and the [Caratheodory boundary extension theorem](../../../complex-analysis.md#caratheodory-boundary-extension-theorem) applies. Its value at $\xi_s$ is $\gamma(s)$. Thus the future in the original plane can meet $K_s\cup\mathbb R$ only at $\gamma(s)$. All these restart conclusions hold simultaneously for rational $s$.

Suppose $\gamma(u)=\gamma(v)$ with $u<v$. The [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) cannot be constant throughout $(u,v)$, since its [compact H-hull](../../../stochastic-process.md#compact-h-hull) capacity increases strictly. By continuity there is a rational $s\in(u,v)$ with $\gamma(s)\ne\gamma(u)$. But $\gamma(v)=\gamma(u)$ lies in $K_s\cup\mathbb R$, contradicting the restart conclusion at $s$. This also excludes any return to the starting point. Hence **the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) is simple and lies in the open [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) at every positive time**.

For transience, first strengthen the [boundary](../../../topology.md#boundary-of-a-set) conclusion to avoidance of the [closure](../../../topology.md#closure-topology) at each fixed real point. Fix $x>0$ and $0<r<x/4$. If the now-simple curve first enters the closed half-disc of radius $r$ about $x$ at time $\sigma$, join its tip to $x$ by the segment inside that disc. Before $\sigma$ the segment misses the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain). Together with the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) and the real interval from zero to $x$, it bounds a pocket whose [boundary](../../../topology.md#boundary-of-a-set) includes the positive side of the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) and $[0,x/2]$. A [Brownian motion](../../../brownian-motion.md) path from high on the imaginary axis reaching that [boundary](../../../topology.md#boundary-of-a-set) arc must enter the pocket through the segment. The [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) bounds its [harmonic measure](../../../brownian-motion.md#harmonic-measure) by the chance of hitting the entire half-disc.

The [boundary](../../../topology.md#boundary-of-a-set) arc maps under $g_\sigma$ to $[\xi_\sigma,g_\sigma(x/2)]$. Its [harmonic measure](../../../brownian-motion.md#harmonic-measure) from $iY$, as $Y\to\infty$, is

$$
\frac{g_\sigma(x/2)-\xi_\sigma}{\pi Y}+o(Y^{-1}).
$$

The half-disc maps out by $z\mapsto z+r^2/(z-x)$; its semicircle becomes an interval of length $4r$. Its [harmonic measure](../../../brownian-motion.md#harmonic-measure) has asymptotic $4r/(\pi Y)$. Comparing and letting $Y\to\infty$ yields

$$
g_\sigma(x/2)-\xi_\sigma\leq4r.
$$

But $m_x=\inf_{t\geq0}(g_t(x/2)-\xi_t)>0$ by the [all-time minimum of a transient Bessel process](../../../brownian-motion.md#all-time-minimum-of-a-transient-bessel-process) fact. The curve cannot enter any such disc with $4r<m_x$. Therefore it stays a strictly positive distance from $x$ for all time. Reflection proves the same for fixed $x<0$. This is the [boundary approach forces a small SLE Bessel gap](../../../stochastic-process.md#boundary-approach-forces-a-small-sle-bessel-gap) argument; the [crosscut](../../../complex-analysis.md#crosscut) comparison is also described in [the boundary-closure lemma in the primary SLE paper](https://arxiv.org/pdf/math/0106036).

Map out the simple initial slit at time one. The starting point zero has two distinct real [prime end](../../../geometry-and-topology.md#prime-end) images $b_-,b_+$ under $g_1$, lying on opposite sides of $\xi_1$. Conditionally on the initial slit, the image future is a fresh independent [SLE](../../../stochastic-process.md#schramm-loewner-evolution) translated by $\xi_1$. The just-proved fixed-point [closure](../../../topology.md#closure-topology) avoidance applies to each of $b_--\xi_1$ and $b_+-\xi_1$. Therefore neither $b_-$ nor $b_+$ lies in the [closure](../../../topology.md#closure-topology) of the mapped future. If a sequence of future [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) points approached zero in the original domain, their images would approach one of these two [prime ends](../../../geometry-and-topology.md#prime-end). This is impossible. Thus

$$
R_1:=\inf_{t\geq1}|\gamma(t)|>0\quad\text{almost surely}.
$$

Finally [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) gives $R_T:=\inf_{t\geq T}|\gamma(t)|\overset d=\sqrt T R_1$. For every fixed $R>0$,

$$
\mathbb P(R_T\leq R)=\mathbb P(R_1\leq R/\sqrt T)\longrightarrow0.
$$

The events of returning to the closed radius-$R$ disc after time $T$ decrease as $T$ increases. Continuity of probability on decreasing events implies that the probability of returns at arbitrarily late times is zero. Taking the countable intersection over positive integer $R$ proves

$$
\boxed{\gamma\text{ is simple and }|\gamma(t)|\longrightarrow\infty\quad\text{almost surely}.}
$$

This proves actual eventual escape, not merely unboundedness of the growing [compact H-hulls](../../../stochastic-process.md#compact-h-hull).

## 3

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Each marginal is a [Bessel process](../../../brownian-motion.md#bessel-process) of [dimension](../../../vector-space.md#dimension-vector-space) $\delta=1+2a\in(1,2)$, but finite lifetime can also be proved directly. Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) before $X$ reaches zero:

$$
\log X_t=\log x+\int_0^tX_s^{-1}\,dB_s+
\left(a-\frac12\right)\int_0^tX_s^{-2}\,ds.
$$

With clock $u(t)=\int_0^tX_s^{-2}ds$, the [Itô integral](../../../stochastic-calculus.md#ito-integral) is a [Brownian motion](../../../brownian-motion.md) $W_u$. The inverse clock satisfies

$$
X_{t(u)}=x e^{W_u-(1/2-a)u},\qquad
 t(u)=x^2\int_0^u e^{2W_v-(1-2a)v}\,dv.
$$

The clock runs through all $u\geq0$ up to the maximal lifetime: a finite terminal clock would leave $X$ at a finite positive limit, allowing continuation, or, at an infinite physical lifetime, would make its clock grow at a positive rate, a contradiction. There is no finite-time explosion to infinity; for example $dX_t^2=2X_t\,dB_t+(1+2a)dt$ and localization bounds the probability of reaching arbitrarily large levels on a fixed time interval. Since $W_u/u\to0$ almost surely and $1-2a>0$, the last exponential integral has finite limit, while $X_{t(u)}\to0$. Therefore

$$
\boxed{\zeta=x^2\int_0^\infty e^{2W_v-(1-2a)v}\,dv<\infty\quad\text{almost surely}.}
$$

The same argument applies to $Y$, whose noise $-B$ is also [Brownian motion](../../../brownian-motion.md), so its lifetime is finite too. No [independence](../../../random-variable.md#independent-random-variables) between the two lifetimes is being claimed.

Set $S=X+Y$ and $U=Y/S$ before $T=\zeta\wedge\tau$. [Brownian motion](../../../brownian-motion.md) terms cancel in the sum:

$$
dS_t=a\left(\frac1{X_t}+\frac1{Y_t}\right)dt,
\qquad S_t\geq x+y>0.
$$

Thus simultaneous extinction is impossible. At the finite first lifetime, precisely one coordinate is zero and the other remains positive. Because $S$ has finite variation, differentiating the ratio gives

$$
dU_t=-\frac1{S_t}\,dB_t
+\frac{a(1-2U_t)}{S_t^2U_t(1-U_t)}dt.
$$

After clock change $v=\int_0^tS_s^{-2}ds$, its generator is

$$
\mathcal L=\frac12\frac{d^2}{du^2}
+\frac{a(1-2u)}{u(1-u)}\frac d{du}.
$$

A [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) $H$ solves $\mathcal LH=0$, so

$$
\frac{H''}{H'}=-2a\frac{1-2u}{u(1-u)},\qquad
H'(u)=C u^{-2a}(1-u)^{-2a}.
$$

Both endpoint singularities are integrable since $a<1/2$. Normalize $H(0)=0,H(1)=1$ to obtain

$$
H(u)=\frac{\displaystyle\int_0^u v^{-2a}(1-v)^{-2a}dv}
{\displaystyle\int_0^1 v^{-2a}(1-v)^{-2a}dv}.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) makes $H(U_{t\wedge T})$ a bounded [martingale](../../../martingale.md), first by localization away from the endpoints and then by [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem). Its terminal value is one on $\{\zeta<\tau\}$, when $U_T=1$, and zero on the opposite event, when $U_T=0$. [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) therefore proves the [oppositely driven Bessel exit probability](../../../brownian-motion.md#oppositely-driven-bessel-exit-probability)

$$
\boxed{\mathbb P(\zeta<\tau)=
\frac1{\mathrm B(1-2a,1-2a)}\int_0^{y/(x+y)}\frac{du}{u^{2a}(1-u)^{2a}},
\qquad c_a=\frac{\Gamma(2-4a)}{\Gamma(1-2a)^2}.}
$$

Here $\mathrm B$ is the [beta function](../../../complex-analysis.md#beta-function) and $\Gamma$ is the [Gamma function](../../../complex-analysis.md#gamma-function).

**The integral printed in the question is incorrect for general $a$.** Its first exponent is $2-4a$, whereas the two coupled equations give $2a$. At $a=1/4$, which lies in the allowed interval, its integral from zero diverges for every positive upper limit; no finite normalizing constant gives a probability. Moreover exchanging $X$ and $Y$ while changing $B$ to $-B$ shows that at $x=y$ the probability must be $1/2$. The corrected symmetric integral has this value for every $a\in(0,1/2)$, whereas the printed asymmetric normalized integral generally does not. For $a>1/4$, even when the printed integral converges, its [derivative](../../../calculus.md#derivative) density $H_{\mathrm{print}}'(u)\propto u^{-(2-4a)}(1-u)^{-2a}$ satisfies

$$
\frac{\mathcal LH_{\mathrm{print}}}{H_{\mathrm{print}}'}=\frac{3a-1}{u},
$$

so it is harmonic for the required exit problem only at $a=1/3$. The two exponents agree exactly at that value.

To relate that value to [percolation](../../../probability-theory.md#percolation-theory), write the two [SLE](../../../stochastic-process.md#schramm-loewner-evolution) [boundary](../../../topology.md#boundary-of-a-set) gaps as $g_t(x)-\xi_t$ and $\xi_t-g_t(-y)$. In Brownian-time units $s=\kappa t$, they have the displayed coupled equations with $a=2/\kappa$, after reversing the [Brownian motion](../../../brownian-motion.md) sign. Hence $a=1/3$ corresponds to $\kappa=6$. The event is that the positive marked point $x$ is swallowed before the negative marked point $-y$.

For a quadrilateral with [boundary](../../../topology.md#boundary-of-a-set) points in the order $(-y,0,x,\infty)$, its conformal [cross-ratio](../../../group-theory.md#cross-ratio) coordinate is $u=y/(x+y)$. In the critical [percolation](../../../probability-theory.md#percolation-theory) exploration, wire the arcs $(-y,0)$ and $(x,\infty)$ blue and the other two arcs yellow. Exploration from zero, stopped when one of the two marked sides is swallowed, detects a blue crossing between those two blue arcs exactly in the event just computed. The continuum exploration has the SLE6 law; its [Locality property of SLE](../../../stochastic-process.md#locality-property-of-sle) lets one stop the ordinary chordal exploration before the distant [boundary](../../../topology.md#boundary-of-a-set) colors affect it. Thus the crossing probability is

$$
\boxed{\frac{\Gamma(2/3)}{\Gamma(1/3)^2}\int_0^{y/(x+y)}[u(1-u)]^{-2/3}du,}
$$

the [Cardy boundary crossing formula](../../../stochastic-process.md#cardy-boundary-crossing-formula). This is the rigorous scaling-limit formula for critical [site percolation](../../../site-percolation.md) on the triangular lattice; applying it to other critical planar models requires the corresponding universality assumption. At this [percolation](../../../probability-theory.md#percolation-theory) value of $a$, the printed integral is already the correct one.

## 4

↑ **Parent:** [Paper 39](paper-39.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work in the [prime end](../../../geometry-and-topology.md#prime-end) [closure](../../../topology.md#closure-topology) of the marked domain, so that its two conformal [boundary](../../../topology.md#boundary-of-a-set) points are distinct even if their physical [boundary](../../../topology.md#boundary-of-a-set) representatives coincide. A [chordal filling](../../../stochastic-process.md#chordal-filling) is a closed connected set joining those points, meeting the conformal [boundary](../../../topology.md#boundary-of-a-set) nowhere else, and full relative to the two [boundary](../../../topology.md#boundary-of-a-set) arcs between them: complementary pockets that do not reach either [boundary](../../../topology.md#boundary-of-a-set) arc have been added. In the normalized [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), its two complementary sides are [simply connected](../../../algebraic-topology.md#simply-connected-space) and abut the negative and positive real axes. For a proper boundary-to-boundary curve, [chordal filling](../../../stochastic-process.md#chordal-filling) means adjoining all such trapped pockets to its range. Independent curves are combined by taking their union and then applying this same [chordal filling](../../../stochastic-process.md#chordal-filling) operation.

An admissible marked subdomain $V\subset U$ contains neighborhoods of the two marked [boundary](../../../topology.md#boundary-of-a-set) points and has a [simply connected](../../../algebraic-topology.md#simply-connected-space) component joining them. The restriction property says that, conditional on the random [chordal filling](../../../stochastic-process.md#chordal-filling) $K$ being contained in $V$, its law is the [chordal filling](../../../stochastic-process.md#chordal-filling) law for $(V,z_0,z_1)$. Equivalently, mapping the conditional [chordal filling](../../../stochastic-process.md#chordal-filling) conformally back to $(U,z_0,z_1)$ recovers the original law. The contained-set events are understood away from the shared marked endpoints.

By transporting the family under [conformal maps](../../../geometry-and-topology.md#conformal-map), it suffices to work in $(\mathbb H,0,\infty)$. Let $A$ be an admissible [compact H-hull](../../../stochastic-process.md#compact-h-hull) whose [closure](../../../topology.md#closure-topology) avoids zero, and normalize

$$
\Phi_A:\mathbb H\setminus A\longrightarrow\mathbb H,
\qquad\Phi_A(0)=0,\quad\Phi_A'(\infty)=1.
$$

In terms of the single normalized measure $\mu$, restriction is precisely

$$
\boxed{\mathcal L(\Phi_A(K)\mid K\cap A=\varnothing)=\mu.}
$$

The [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) extends $\Phi_A$ analytically near zero, with $\Phi_A'(0)>0$, so the stated conditioning events have positive probability for the two laws considered below. This is the [chordal restriction property](../../../stochastic-process.md#chordal-restriction-property) for filled sets. An unbounded marked subdomain can be approximated by such compact-hull removals; [conformal maps](../../../geometry-and-topology.md#conformal-map) transport the formulation to general domains.

We need a determination principle for filled sets, since a probability of one avoidance event alone would not establish equality of laws. Choose countably many thin polygonal [compact H-hulls](../../../stochastic-process.md#compact-h-hull) with rational data, attached to real [boundary](../../../topology.md#boundary-of-a-set) intervals away from zero. For each [chordal filling](../../../stochastic-process.md#chordal-filling), every point of its complement has a path within one of the two complementary sides to the appropriate real [boundary](../../../topology.md#boundary-of-a-set) interval. A sufficiently thin tube along such a path avoids the [chordal filling](../../../stochastic-process.md#chordal-filling) and contains a neighborhood of that point. Hence the union of interiors of all avoided test tubes is exactly the complement.

Their joint avoidance probabilities are also determined by single-hull probabilities. For a finite union of test [compact H-hulls](../../../stochastic-process.md#compact-h-hull), either the union separates zero from infinity, in which case a connected [chordal filling](../../../stochastic-process.md#chordal-filling) cannot avoid it, or its unbounded complementary component contains both marked endpoints. In the latter case fill the union's bounded pockets to get an admissible [compact H-hull](../../../stochastic-process.md#compact-h-hull) $C$. A connected set joining zero to infinity and avoiding the union cannot enter one of these separated pockets, so it avoids $C$ as well. Thus joint avoidance is either impossible or is the avoidance event for $C$. The [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) gives every finite joint [probability distribution](../../../probability-theory.md#probability-distribution) of the tube-avoidance indicators, and these indicators determine the random complement and [chordal filling](../../../stochastic-process.md#chordal-filling). This proves [avoidance probabilities determine a chordal filling law](../../../stochastic-process.md#avoidance-probabilities-determine-a-chordal-filling-law).

In the given avoidance formulas, the argument of the conformal map must be the retained open domain, rather than the random closed filling. We express that domain as $\mathbb H\setminus A$ to keep the two objects distinct. The formulas then imply for the two filled processes

$$
p_\gamma(A)=\Phi_A'(0)^{5/8},\qquad p_E(A)=\Phi_A'(0).
$$

The [chordal filling](../../../stochastic-process.md#chordal-filling) operation does not change avoidance of an admissible [compact H-hull](../../../stochastic-process.md#compact-h-hull): every piece of that [compact H-hull](../../../stochastic-process.md#compact-h-hull) is attached to the real [boundary](../../../topology.md#boundary-of-a-set) away from the endpoints, and so cannot be inside a trapped pocket while its generating curve avoids the [compact H-hull](../../../stochastic-process.md#compact-h-hull). These laws are conformally invariant as unparameterized [chordal filling](../../../stochastic-process.md#chordal-filling) laws. For [SLE](../../../stochastic-process.md#schramm-loewner-evolution) this follows from Question 1; for the [Brownian half-plane excursion](../../../brownian-motion.md#brownian-excursion-in-the-upper-half-plane), [Brownian scaling](../../../brownian-motion.md#brownian-scaling) of its independent one- and three-dimensional coordinates shows that its unparameterized law is unchanged by positive dilations, and mapping the [Brownian half-plane excursion](../../../brownian-motion.md#brownian-excursion-in-the-upper-half-plane) to another marked domain gives the conformally natural law. [Conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) describes the corresponding change of time, which does not alter the [chordal filling](../../../stochastic-process.md#chordal-filling).

Here is the conditional-law calculation for either exponent $\alpha\in\{5/8,1\}$. For another admissible [compact H-hull](../../../stochastic-process.md#compact-h-hull) $B$ in the image [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), set

$$
C=A\cup\Phi_A^{-1}(B),\qquad\Phi_C=\Phi_B\circ\Phi_A.
$$

The complement of $C$ is mapped to $\mathbb H$ by this composition, so $C$ is again admissible; both maps fix zero and have [derivative](../../../calculus.md#derivative) one at infinity. The chain rule gives $\Phi_C'(0)=\Phi_B'(0)\Phi_A'(0)$. Therefore

$$
\begin{aligned}
\mathbb P(\Phi_A(K)\cap B=\varnothing\mid K\cap A=\varnothing)
&=\frac{\mathbb P(K\cap C=\varnothing)}{\mathbb P(K\cap A=\varnothing)}\\
&=\frac{\Phi_C'(0)^\alpha}{\Phi_A'(0)^\alpha}
=\Phi_B'(0)^\alpha.
\end{aligned}
$$

These are exactly the original [chordal filling](../../../stochastic-process.md#chordal-filling)'s avoidance probabilities for every $B$. The determination principle proves equality of the conditional image law with the original law. Hence **both generated [chordal fillings](../../../stochastic-process.md#chordal-filling) have restriction**, with exponents $5/8$ and $1$ respectively. This is a complete implication from the two allowed avoidance formulas; the restriction conclusion was not assumed.

For independent [chordal fillings](../../../stochastic-process.md#chordal-filling), avoidance of $A$ by their filled union is equivalent to avoidance by every component. [Independence](../../../random-variable.md#independent-random-variables) multiplies the probabilities, and thus adds their [restriction exponents of a chordal filling](../../../stochastic-process.md#restriction-exponent-of-a-chordal-filling). Consequently

$$
\mathbb P(\overline\gamma^{\otimes8}\cap A=\varnothing)
=\bigl(\Phi_A'(0)^{5/8}\bigr)^8
=\Phi_A'(0)^5
=\bigl(\Phi_A'(0)\bigr)^5
=\mathbb P(\overline E^{\otimes5}\cap A=\varnothing).
$$

The determination principle applies once more, giving

$$
\boxed{\mathcal L(\overline\gamma^{\otimes8})=\mathcal L(\overline E^{\otimes5}).}
$$

The equality concerns the filled, unparameterized closed sets. The numerical reason is $8\cdot(5/8)=5\cdot1=5$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
