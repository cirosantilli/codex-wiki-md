# Paper 27

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_27.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_27.pdf)

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
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the [intrinsic boundary of a simply connected domain](../../../geometry-and-topology.md#intrinsic-boundary-of-a-simply-connected-domain), so different approaches to the two sides of a slit remain distinct. The [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) $g_K$ extends as a [homeomorphism](../../../topology.md#homeomorphism) from this intrinsic compactification to that of the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). Set $T=T(H)$. The imaginary coordinate of [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) hits zero in finite time almost surely, and $T$ is no larger than that time. Thus $T<\infty$ and continuity gives a finite Euclidean exit point.

By [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion), $g_K(B_t)$ is a [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), run with clock

$$
A(t)=\int_0^t|g_K'(B_s)|^2\,ds.
$$

The terminal clock cannot be infinite: that would make the transformed Brownian motion stay in the upper half-plane forever. It cannot stop while the transformed path is in the interior either, since continuity of $g_K^{-1}$ would then put the original exit point inside $H$. Hence the terminal clock is precisely the transformed [Brownian exit time](../../../brownian-motion.md#brownian-exit-time). The transformed path converges to a real boundary point, and applying the extended inverse proves **almost sure convergence to a point of the intrinsic boundary**.

Write $g_K(x+iy)=u+iv$, and let $E=g_K(S)\cap\mathbb R$. The point at infinity has zero [harmonic measure](../../../brownian-motion.md#harmonic-measure). [Conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) and the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) give

$$
\mathbb P_{x+iy}(\widehat B_T\in S)
=\int_E\frac{v}{\pi((t-u)^2+v^2)}\,dt.
$$

The [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) gives $g_K(z)=z+O(1/z)$, so along the specified approach $v/y\to1$ and $u/y\to0$. For each fixed real $t$,

$$
\frac{yv}{(t-u)^2+v^2}\longrightarrow1,
\qquad
0\le\frac{yv}{(t-u)^2+v^2}\le\frac yv.
$$

If $\operatorname{Leb}(E)<\infty$, [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) applies because $y/v$ is eventually bounded. If $\operatorname{Leb}(E)=\infty$, [Fatou's lemma](../../../measure-theory.md#fatou-s-lemma) makes the limit infinite. This proves the [harmonic-measure asymptotic at infinity](../../../brownian-motion.md#harmonic-measure-asymptotic-at-infinity)

$$
\boxed{\lim_{y\to\infty,\ x/y\to0}
\pi y\,\mathbb P_{x+iy}(\widehat B_T\in S)
=\operatorname{Leb}(g_K(S)),}
$$

with the equality understood in the extended nonnegative reals.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The capacity in this question is [harmonic capacity from infinity in the upper half-plane](../../../brownian-motion.md#harmonic-capacity-from-infinity-in-the-upper-half-plane), which has units of length; it is distinct from [half-plane capacity](../../../stochastic-process.md#half-plane-capacity), which has units of length squared.

Here is a proof of existence that also works with irregular real attachments. The function

$$
u(z)=\mathbb P_z(B_{T(H)}\in K)
$$

is bounded and [harmonic](../../../partial-differential-equation.md#harmonic-function) on $H$, by the [Strong Markov property](../../../markov-process.md#strong-markov-property) and the mean-value characterization of [harmonic functions](../../../partial-differential-equation.md#harmonic-function). Therefore $u\circ g_K^{-1}$ is a bounded [harmonic function](../../../partial-differential-equation.md#harmonic-function) on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), with a [Poisson kernel](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) representation

$$
u(g_K^{-1}(w))
=\int_{\mathbb R}\frac{\operatorname{Im}w}
{\pi|t-w|^2}\,f(t)\,dt,\qquad 0\le f\le1.
$$

The boundary function $f$ vanishes outside a bounded interval. Indeed, far enough along either real ray the original domain contains a half-disc neighbourhood, and $g_K$ extends there; the probability of hitting the bounded hull before the real boundary tends to zero as the starting point approaches that ray. Applying the same dominated-limit calculation as in part (i) yields

$$
\boxed{\operatorname{cap}(K)=\int_{\mathbb R}f(t)\,dt<\infty.}
$$

When the intrinsic boundary pieces landing on the hull are identified, $f$ is their indicator almost everywhere and this is the length of their image under $g_K$. For ordinary finite slit hulls this is exactly the image of $\delta H\setminus H_0$, since real attachment endpoints have zero [harmonic measure](../../../brownian-motion.md#harmonic-measure). The Poisson representation avoids requiring that boundary identification in the general existence argument.

If $K\subset K'$, couple the two exit events using the same [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion), stopped at its first hit of the real axis. Any path that hits $K$ before the real axis also hits $K'$ before the real axis. Consequently

$$
\mathbb P_{iy}(B_{T(\mathbb H\setminus K)}\in K)
\le
\mathbb P_{iy}(B_{T(\mathbb H\setminus K')}\in K'),
$$

and taking the limits proves **monotonicity of this capacity**.

For a half-disc of radius $r$ centred at $b\in\mathbb R$, the [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is

$$
g(z)=b+(z-b)+\frac{r^2}{z-b}.
$$

Its semicircular boundary maps onto $[b-2r,b+2r]$, of length $4r$. Hence its [harmonic capacity from infinity in the upper half-plane](../../../brownian-motion.md#harmonic-capacity-from-infinity-in-the-upper-half-plane) is $4r$. With

$$
\operatorname{rad}(K)=\inf\{r>0:K\subset\{z:|z-b|\le r\}
\text{ for some }b\in\mathbb R\},
$$

enclose $K$ in such a half-disc and use monotonicity. Letting the enclosing radius decrease to the infimum proves

$$
\boxed{\operatorname{cap}(K)\le4\operatorname{rad}(K).}
$$

The same conclusion holds if radius is instead measured about a specified real centre.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

**As printed, the lower bound needs a connectedness hypothesis.** This illustrates that [radius gives no positive lower bound for disconnected harmonic hull capacity](../../../brownian-motion.md#radius-gives-no-positive-lower-bound-for-disconnected-harmonic-hull-capacity). A [compact H-hull](../../../stochastic-process.md#compact-h-hull) need not have connected closure. To see the obstruction, take $0<\varepsilon<1/12$, set $c=\sqrt{1-\varepsilon^2}$, and use three disjoint vertical slits,

$$
K_\varepsilon=(0,i\varepsilon]\cup(c,c+i\varepsilon]
\cup(-c,-c+i\varepsilon].
$$

Their complement in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain): the three slits attach to the real boundary, and create no interior holes. Symmetry shows that the smallest enclosing half-disc is centred at zero and has radius one. More explicitly, any real centre $b$ has maximum distance to the two outer tips at least $\sqrt{c^2+\varepsilon^2}=1$, while the unit half-disc contains every slit. Also $0\in\overline K_\varepsilon$ and $c+i\varepsilon$ has modulus one.

For a vertical slit of height $\varepsilon$, the [mapping-out function of a vertical slit](../../../stochastic-process.md#mapping-out-function-of-a-vertical-slit) maps its two faces onto an interval of length $2\varepsilon$, so its [harmonic capacity from infinity in the upper half-plane](../../../brownian-motion.md#harmonic-capacity-from-infinity-in-the-upper-half-plane) is $2\varepsilon$. [Subadditivity of harmonic hull capacity](../../../brownian-motion.md#subadditivity-of-harmonic-hull-capacity), from the union bound for the Brownian hitting events, gives

$$
\boxed{\operatorname{cap}(K_\varepsilon)\le6\varepsilon<\frac12.}
$$

Thus the requested conclusion does not follow from the printed assumptions.

The intended [reflection lower bound for harmonic hull capacity](../../../brownian-motion.md#reflection-lower-bound-for-harmonic-hull-capacity) works when the closure is a connected continuum joining the two specified points, as for a slit hull. Reflect in the vertical line through $x$, using $\rho(z)=2x-\bar z$. The reflected continuum joins $2x$ to $x+iy$. Together the original and reflected continua form a barrier between infinity and the segment $I$ together with the real interval between $0$ and $2x$. One can first verify this separation for polygonal simple arcs, then use decreasing connected neighbourhoods of the continuum. Hence, for Brownian motion started at $x+iY$, $Y$ large, reaching $I$ or the real interval $J$ between $0$ and $x$ requires a hit of the original or reflected barrier. Reflection symmetry and the union bound give

$$
\mathbb P_{x+iY}\bigl(B_{T(\mathbb H\setminus I)}\in I\cup J\bigr)
\le2\,\mathbb P_{x+iY}(B_{T(H)}\in\overline K).
$$

For the connected slit setting, the real attachment endpoints have zero [harmonic measure](../../../brownian-motion.md#harmonic-measure), so the last event may be written with $K$.

For $y>0$, use the branch of the square root fixed by [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity):

$$
g_I(z)=x+\sqrt{(z-x)^2+y^2}.
$$

The two slit faces together have image length $2y$. The interval $J$ has image length $\sqrt{x^2+y^2}-y=1-y$, by the square-root formula on the appropriate real side. Thus the image length of $I\cup J$ is $1+y$. Multiply the probability inequality by $\pi Y$ and use part (i); the allowed starting approach includes $x+iY$. We obtain

$$
\boxed{\operatorname{cap}(K)\ge\frac{1+y}{2}\ge\frac12}
$$

under the stated connected-barrier interpretation. If $y=0$, the model slit is empty and $J$ has length $|x|=1$, giving the same lower bound by the real-interval argument. The connectedness repair is essential, as the explicit three-slit counterexample demonstrates.

## 2

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Use the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) with [Loewner driving function](../../../stochastic-process.md#loewner-driving-function) $\xi_t=\sqrt\kappa W_t$, and set $Z_t=g_t(z)-\xi_t=X_t+iY_t$. Before the [Loewner swallowing time](../../../stochastic-process.md#interior-point-swallowing-time-for-a-loewner-chain),

$$
dZ_t=\frac2{Z_t}\,dt-\sqrt\kappa\,dW_t.
$$

The upper-half-plane branch of the logarithm has imaginary part $h_t$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
d\log Z_t=\frac{4-\kappa}{2Z_t^2}\,dt
-\frac{\sqrt\kappa}{Z_t}\,dW_t,
$$

and therefore the [SLE angle process](../../../stochastic-process.md#sle-angle-process) satisfies

$$
\boxed{dh_t=(\kappa-4)\frac{X_tY_t}{|Z_t|^4}\,dt
+\sqrt\kappa\,\frac{Y_t}{|Z_t|^2}\,dW_t.}
$$

At $\kappa=4$ the drift vanishes. Since $0<h_t<\pi$, the stopped [local martingale](../../../martingale.md#local-martingale) is a true bounded [martingale](../../../martingale.md), and the [SLE4 angle martingale](../../../stochastic-process.md#sle4-angle-martingale) is global for each fixed point almost surely, using [fixed-interior-point avoidance of SLE4](../../../stochastic-process.md#fixed-interior-point-avoidance-of-sle4) for the simple parameter-four [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain).

Conversely, take $\kappa>0$. If this [semimartingale](../../../stochastic-calculus.md#semimartingale) were a [local martingale](../../../martingale.md#local-martingale), uniqueness of its finite-variation decomposition would force $(\kappa-4)X_tY_t=0$ throughout every compact interval before swallowing. Because $Y_t>0$, for $\kappa\ne4$ this would force $X_t$ to be identically zero on such an interval. Its Brownian component has [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $\kappa t$, which makes that impossible. Thus **for positive $\kappa$, the martingale parameter is exactly four**.

If the degenerate value $\kappa=0$ is admitted, there is one exception to a fixed-point reading of the assertion: for $z$ on the positive imaginary axis the deterministic flow stays on that axis until swallowing, and $h_t=\pi/2$ is constant. For all starting points simultaneously, the unique parameter giving the martingale property is still four.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For a simple [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain), the domain mapped by $g_t$ is $D_t=\mathbb H\setminus\gamma[0,t]$. For a non-simple [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain), use instead the unbounded component $D_t=\mathbb H\setminus K_t$; the map $g_t$ is not defined on swallowed bounded components. This is the necessary domain interpretation when $\kappa>4$.

The function $\operatorname{Im}\log(g_t(z)-\xi_t)$ is [harmonic](../../../partial-differential-equation.md#harmonic-function) in $D_t$ because the logarithm is [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point) on the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis). Let $S_t^-$ and $S_t^+$ be the intrinsic boundary sets mapped to $(-\infty,\xi_t)$ and $(\xi_t,\infty)$ respectively. The [Dirichlet problem](../../../analysis.md#dirichlet-problem) has boundary data

$$
\boxed{h_t=\pi\text{ on }S_t^-,
\qquad h_t=0\text{ on }S_t^+.}
$$

For a simple [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) these are the left bank of the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) together with the negative real boundary, and the right bank together with the positive real boundary. Left and right refer to the orientation from the starting point towards the tip. The tip and infinity correspond to discontinuities of the data; no unique limit is imposed there. They have zero [harmonic measure](../../../brownian-motion.md#harmonic-measure).

More precisely, the bounded solution is

$$
h_t(z)=\pi\,\omega_{D_t}(z,S_t^-),
$$

by the [Poisson kernel for the upper half-plane](../../../partial-differential-equation.md#poisson-kernel-for-the-upper-half-plane) and [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion). This establishes the boundary values in the intrinsic sense and uniqueness among bounded solutions of the [Dirichlet problem](../../../analysis.md#dirichlet-problem), without treating the two banks as one Euclidean boundary point.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For parameter four, the [SLE4 angle martingale](../../../stochastic-process.md#sle4-angle-martingale) is bounded, so the [Continuous-time martingale convergence theorem](../../../martingale.md#continuous-time-martingale-convergence-theorem) gives an almost sure limit. The imaginary part of the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) gives

$$
\frac{d}{dt}Y_t=-\frac{2Y_t}{X_t^2+Y_t^2},
\qquad
\frac{d}{dt}Y_t^2=-4\sin^2h_t.
$$

For a point off the full simple [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) the flow exists at every finite time. If the limiting angle lay strictly between $0$ and $\pi$, the last derivative would eventually be bounded above by a strictly negative constant. That would make $Y_t^2$ negative, a contradiction. Hence **the terminal angle is either zero or $\pi$**.

The simple transient chordal [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) from $0$ to infinity splits the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) into a left component $D^-$, adjacent to the negative real boundary, and a right component $D^+$, adjacent to the positive real boundary. The [Dirichlet boundary values of the SLE angle process](../../../stochastic-process.md#dirichlet-boundary-values-of-the-sle-angle-process) identify which terminal value occurs. Indeed, run an independent [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) from $z$ until it first hits the full [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) or the real axis. This time is finite. The Brownian path up to that time is bounded, and [Transience of chordal SLE](../../../stochastic-process.md#transience-of-chordal-sle) ensures that any [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) point it meets belongs to a finite initial segment. Thus its exit side for the truncated domains eventually agrees with its exit side for the full component. In $D^-$ every such exit is through the left bank or negative real boundary; in $D^+$ every exit is through the right bank or positive real boundary. [Dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) in the harmonic-measure representation therefore gives

$$
\boxed{F(z)=
\begin{cases}
\pi,&z\in D^-,\\
0,&z\in D^+.
\end{cases}}
$$

This is a random side indicator, not the deterministic value $\arg z$. Uniform integrability also gives $\mathbb E[F(z)]=\arg z$, so the [SLE4 left-passage probability](../../../stochastic-process.md#sle4-left-passage-probability) is

$$
\boxed{\mathbb P(z\in D^-)=\frac{\arg z}{\pi}.}
$$

## 3

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The complex form of the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation), driven by a continuous real [Loewner driving function](../../../stochastic-process.md#loewner-driving-function), is

$$
\boxed{\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},
\qquad g_0(z)=z.}
$$

For $z\in\mathbb C\setminus\{\xi_0\}$ this is an [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) up to its maximal lifetime, when the solution reaches the driving singularity. The coefficients respect complex conjugation, so the lower-half-plane flow is the conjugate of the upper-half-plane flow. On surviving real points it is the real boundary flow. The [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) and factor two correspond to [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) $\operatorname{hcap}(K_t)=2t$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Assume $\kappa>0$ and $x\ne0$, since the initial driving point does not admit the displayed ordinary boundary flow. The sign of the driver in this part is negative, so

$$
d\bigl(g_t(x\sqrt\kappa)-\xi_t\bigr)
=\frac2{g_t(x\sqrt\kappa)-\xi_t}\,dt+\sqrt\kappa\,dW_t.
$$

After division by $\sqrt\kappa$, the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) is

$$
\boxed{dX_t=dW_t+\frac a{X_t}\,dt,\qquad
X_0=x,\qquad a=\frac2\kappa.}
$$

For $x>0$ this is a [Bessel process](../../../brownian-motion.md#bessel-process) of dimension $\delta=1+2a$. For $x<0$, $-X_t$ obeys the same equation driven by $-W_t$ until hitting zero. It suffices to treat a positive initial value.

The [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) is $\mathcal Lf=\tfrac12f''+(a/u)f'$. An increasing [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) is

$$
s(u)=
\begin{cases}
u^{1-2a}/(1-2a),&a\ne1/2,\\
\log u,&a=1/2.
\end{cases}
$$

It satisfies $\mathcal Ls=0$. For $0<\varepsilon<x<b$, [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives the [boundary hitting probability from a diffusion scale function](../../../stochastic-calculus.md#boundary-hitting-probability-from-a-diffusion-scale-function)

$$
\mathbb P_x(\tau_\varepsilon<\tau_b)
=\frac{s(b)-s(x)}{s(b)-s(\varepsilon)}.
$$

When $a<1/2$, put $\beta=1-2a>0$. The inner boundary is reached in finite time: the nonnegative function

$$
v(u)=\frac{b^{2-\beta}u^\beta-u^2}{1+2a}
$$

vanishes at $0,b$ and satisfies $\mathcal Lv=-1$. Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) before exiting $(\varepsilon,b)$ gives $\mathbb E(\tau_\varepsilon\wedge\tau_b)\le v(x)$. As $\varepsilon\downarrow0$, these times increase to a finite limiting exit time almost surely. Thus the scale limit is an actual hitting event, not just asymptotic approach to zero, and

$$
\mathbb P_x(\tau_0<\tau_b)=1-(x/b)^\beta.
$$

Let $b\uparrow\infty$ to obtain $\mathbb P_x(\tau_0<\infty)=1$.

If $a>1/2$, then $s(\varepsilon)\to-\infty$, and the same formula makes the probability of hitting zero before any fixed $b$ equal to zero. A finite-time hit would occur before reaching some integer upper level, because the stopped path is continuous and bounded on a finite interval. Taking the countable union over those levels proves that no hit occurs. At $a=1/2$, $s(u)=\log u$ gives the same conclusion. Therefore

$$
\boxed{\tau_0<\infty\text{ a.s. if }a<\tfrac12;\qquad
\tau_0=\infty\text{ a.s. if }a\ge\tfrac12.}
$$

The source's $x=0$ case must be excluded: zero is then already the initial value, and the displayed singular flow is undefined.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace) has its simple range

$$
\boxed{0\le\kappa\le4,}
$$

with $\kappa=0$ the deterministic vertical slit. For positive $\kappa$, the dividing parameter is precisely $\delta=1+4/\kappa=2$ in the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle).

Here is the reason this diffusion threshold controls simplicity. For $\kappa\le4$, no nonzero real boundary point is swallowed. It suffices to check rational boundary points: a first meeting with either nonzero real half-axis would close a boundary crosscut and swallow a nonempty real interval, including a rational point. Thus the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) stays in the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) apart from its starting point. By the [domain Markov property of a chordal Loewner chain](../../../stochastic-process.md#domain-markov-property-of-a-chordal-loewner-chain), after any fixed rational time $s$ the future mapped and centred [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) has the same boundary-avoidance property.

Suppose two [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) times $r<r'$ had the same image. Positive [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) growth rules out constancy on a nonempty time interval, so continuity supplies a rational $s\in(r,r')$ with $\gamma_s\ne\gamma_r$. In the mapped future, the point at $r'$ is either in the open upper half-plane or at the starting boundary point $0$; it cannot lie at another real point. The first case puts $\gamma_{r'}$ inside the surviving domain at $s$, whereas $\gamma_r$ lies on the past [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain). The second gives $\gamma_{r'}=\gamma_s$, also contradicting the choice of $s$. Boundary continuity of the inverse [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) makes these identifications valid. This proves that the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) has no repeated points.

For $\kappa>4$, part (ii) makes a fixed positive real point have finite swallowing time, so the [SLE boundary swallowing criterion](../../../stochastic-process.md#sle-boundary-swallowing-criterion) ensures that the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) hits the positive real axis. In fact [positive boundary-interval hitting probability for SLE above parameter four](../../../stochastic-process.md#positive-boundary-interval-hitting-probability-for-sle-above-parameter-four) holds: any interval $J\subset(0,\infty)$ has positive hitting probability. To prove this, cover the positive axis by countably many dilates of $J$. If $J$ had zero hitting probability, [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) would give zero probability for every dilate, contradicting the almost sure hit of the positive axis. Reflection gives the same conclusion for negative intervals.

At a fixed positive time, if the past [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) already repeats a point there is nothing to prove. Otherwise, boundary continuity of the inverse [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) supplies a nonempty real interval, away from the current driving point, mapped back into the earlier [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) in the open upper half-plane. Such an interval exists because positive capacity growth creates a genuine [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) boundary in the interior; choose an accessible boundary point away from the tip and then a small interval around its preimage. Conditional on the past, the [domain Markov property of a chordal Loewner chain](../../../stochastic-process.md#domain-markov-property-of-a-chordal-loewner-chain) gives a future centred SLE. With positive conditional probability its [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) hits this interval, by the preceding boundary-interval argument. Mapping back then gives a visit to the earlier [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain). Thus a repeated point occurs by some finite time with positive probability.

Finally let $E_t$ be the event of a repeated point by time $t$. [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) makes $\mathbb P(E_t)$ the same for every $t>0$. The positive finite-time probability just proved makes this common value positive. Hence $\bigcap_nE_{1/n}$ also has positive probability. This event belongs to the Brownian germ sigma-field; the [Blumenthal zero-one law](../../../brownian-motion.md#blumenthal-zero-one-law) forces its probability to be one. Consequently **the [Loewner trace](../../../stochastic-process.md#trace-of-a-loewner-chain) is not simple almost surely for every $\kappa>4$**. At $\kappa=4$, the logarithmic scale function gives non-hitting of zero, so equality belongs to the simple range.

## 4

↑ **Parent:** [Paper 27](paper-27.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded relatively closed subset $K$ of the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis) such that $\mathbb H\setminus K$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). This does not require its closure to be connected. Its [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the unique [conformal map](../../../geometry-and-topology.md#conformal-map) $g_K:\mathbb H\setminus K\to\mathbb H$ with [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity),

$$
g_K(z)=z+\frac{a_K}{z}+O(|z|^{-2}).
$$

The [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) is

$$
\boxed{\operatorname{hcap}(K)=a_K
=\lim_{z\to\infty}z\bigl(g_K(z)-z\bigr)\ge0.}
$$

The coefficient is zero exactly for the empty hull.

In terms of the least radius of a real-centred enclosing half-disc, the [sharp displacement bound for a compact H-hull](../../../stochastic-process.md#sharp-displacement-bound-for-a-compact-h-hull), also called the continuity estimate, is

$$
\boxed{|g_K(z)-z|\le3\operatorname{rad}(K),
\qquad z\in\mathbb H\setminus K.}
$$

The [differentiability estimate for a mapping-out function](../../../stochastic-process.md#differentiability-estimate-for-a-mapping-out-function) is a uniform small-hull expansion: there is an absolute constant $C$ such that if $K\subset\{z:|z-\xi|\le r\}$ with $\xi\in\mathbb R$, then

$$
\boxed{\left|g_K(z)-z-\frac{\operatorname{hcap}(K)}{z-\xi}\right|
\le \frac{Cr\,\operatorname{hcap}(K)}{|z-\xi|^2},
\qquad |z-\xi|>2r.}
$$

These are statements of the two requested estimates. The second is not merely a bound for $g_K'$: it controls the first-order change of a [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) when a small hull is removed.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Take increasing to mean strict growth on every nonempty time interval; otherwise a constant family has no uniquely determined driving point. The [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) imposed below guarantees strict growth. For $s<t$, define the increment hull in the mapped domain by

$$
K_{s,t}=\mathbb H\setminus g_s(\mathbb H\setminus K_t).
$$

This definition includes filling and boundary conventions automatically. Its [mapping-out function](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is $g_{s,t}=g_t\circ g_s^{-1}$. The [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) means

$$
\boxed{\sup_{0\le t\le T}\operatorname{rad}(K_{t,t+h})
\longrightarrow0\quad(h\downarrow0)}
$$

for every finite $T$ within the parameter range. Equivalently, the mapped increments have uniformly vanishing diameter on compact time intervals.

For fixed $t$, the nonempty compact Euclidean closures $\overline K_{t,t+h}$ are nested as $h$ decreases. Their diameters tend to zero, so their intersection is a singleton. Its point lies on the real axis: the imaginary part of any point in a hull is at most its enclosing radius. Define the [Loewner transform](../../../stochastic-process.md#loewner-driving-function) by

$$
\boxed{\{\xi_t\}=\bigcap_{h>0}\overline K_{t,t+h}.}
$$

Since $\xi_t$ lies in each closure, every point of $K_{t,t+h}$ is at distance at most $2\operatorname{rad}(K_{t,t+h})$ from it.

To prove continuity, choose $z\in K_{t+2h}\setminus K_{t+h}$ and write $w=g_t(z)$, $w'=g_{t+h}(z)$. Then $w\in K_{t,t+2h}$, $w'\in K_{t+h,t+2h}$ and $w'=g_{t,t+h}(w)$. The continuity estimate from part (i) gives

$$
\begin{aligned}
|\xi_{t+h}-\xi_t|
&\le|\xi_t-w|+|w-w'|+|w'-\xi_{t+h}|\\
&\le2\operatorname{rad}(K_{t,t+2h})
+3\operatorname{rad}(K_{t,t+h})
+2\operatorname{rad}(K_{t+h,t+2h}).
\end{aligned}
$$

The right-hand side tends to zero uniformly on compact time intervals. Applying the same inequality with the earlier time as the base proves left continuity as well. Thus **the Loewner transform is continuous**.

Now impose $\operatorname{hcap}(K_t)=2t$. The [half-plane-capacity composition rule](../../../stochastic-process.md#half-plane-capacity-composition-rule) follows by composing Laurent expansions at infinity and gives

$$
\operatorname{hcap}(K_{s,t})=2(t-s).
$$

For a point not yet swallowed, put $z_s=g_s(z)$ and $r_{s,t}=2\operatorname{rad}(K_{s,t})$. The increment is contained in the half-disc of radius $r_{s,t}$ centred at $\xi_s$. The continuity estimate first proves continuity of $s\mapsto g_s(z)$: its increment is bounded by $3\operatorname{rad}(K_{s,t})$. The [differentiability estimate for a mapping-out function](../../../stochastic-process.md#differentiability-estimate-for-a-mapping-out-function) then gives, when $t-s$ is small enough,

$$
g_t(z)-g_s(z)
=\frac{2(t-s)}{g_s(z)-\xi_s}
+O\!\left(\frac{r_{s,t}(t-s)}{|g_s(z)-\xi_s|^2}\right).
$$

On a compact interval before swallowing the denominator stays away from zero. Divide by $t-s$ and let $t\downarrow s$. The local-growth property makes the error tend to zero. The analogous backward quotient has the same limit, using continuity of $g_s(z)$ and $\xi_s$. Thus the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) follows:

$$
\boxed{\partial_tg_t(z)=\frac2{g_t(z)-\xi_t},\qquad g_0(z)=z.}
$$

The initial value follows from $\operatorname{hcap}(K_0)=0$, hence $K_0=\varnothing$. Without the capacity parameterization, the same argument gives $dg_t(z)=d\,\operatorname{hcap}(K_t)/(g_t(z)-\xi_t)$, interpreted with the capacity clock.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
