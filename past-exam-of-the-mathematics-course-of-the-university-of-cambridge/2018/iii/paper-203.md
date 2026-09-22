# Paper 203

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_203.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_203.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [compact H-hull](../../../stochastic-process.md#compact-h-hull) is a bounded subset $A\subset\mathbb H$, closed relative to the [complex upper half-plane](../../../complex-analysis.md#upper-half-plane-complex-analysis), such that $\mathbb H\setminus A$ is a [simply connected domain](../../../complex-analysis.md#simply-connected-domain). The word compact refers to its bounded closure in $\overline{\mathbb H}$; a nonempty hull need not be a compact subset of the open half-plane.

The [Riemann mapping theorem](../../../complex-analysis.md#riemann-mapping-theorem) and normalization at infinity give a unique [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) $g_A:\mathbb H\setminus A\to\mathbb H$ with $g_A(z)-z\to0$ as $z\to\infty$. This [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) yields a [Laurent series](../../../analysis.md#laurent-series)

$$
g_A(z)=z+\frac{a_A}{z}+O(|z|^{-2}),\qquad a_A\geq0.
$$

The coefficient is the [half-plane capacity](../../../stochastic-process.md#half-plane-capacity):

$$
\boxed{\operatorname{hcap}(A)=a_A=\lim_{y\to\infty}iy\bigl(g_A(iy)-iy\bigr).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

There is a small closure issue in the printed set: the [unit disc](../../../topology.md#unit-disc) is open, so its half-disc is not relatively closed in $\mathbb H$. As written, the set is not a [compact H-hull](../../../stochastic-process.md#compact-h-hull). We compute the intended [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) after taking its relative closure in $\mathbb H$.

First remove the closed unit half-disc $K$. Its [mapping-out function of a compact H-hull](../../../stochastic-process.md#mapping-out-function-of-a-compact-h-hull) is the [Joukowski map](../../../geometry-and-topology.md#joukowski-map)

$$
g_K(z)=z+\frac1z,\qquad\operatorname{hcap}(K)=1.
$$

For $z=iy$ on the remaining portion of the vertical slit, $1<y\leq2$,

$$
g_K(iy)=i\left(y-\frac1y\right).
$$

Thus the image of the remaining slit is $(0,3i/2]$. By the [half-plane capacity of a vertical slit](../../../stochastic-process.md#half-plane-capacity-of-a-vertical-slit), its capacity is $(3/2)^2/2=9/8$. The [half-plane-capacity composition rule](../../../stochastic-process.md#half-plane-capacity-composition-rule) gives

$$
\boxed{\operatorname{hcap}(\overline A\cap\mathbb H)=1+\frac98=\frac{17}{8}.}
$$

As a direct check, composing with the slit map gives $g_A(z)=\sqrt{(z+z^{-1})^2+9/4}$, with the branch asymptotic to $z$. Its $z^{-1}$ coefficient is $17/8$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Work with a locally growing [Loewner chain](../../../stochastic-process.md#loewner-chain) started at $0$, with $A_0=\varnothing$ and the [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization) $\operatorname{hcap}(A_t)=2t$. The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) combines invariance under conformal changes of the marked domain with restarting after an initial hull has been removed.

In the half-plane this means, first, that $(r^{-1}A_{r^2t})_{t\geq0}$ has the same law as $(A_t)_{t\geq0}$ for every $r>0$. Second, conditionally on $\mathcal F_t$, the future hulls mapped by $g_t-U_t$,

$$
\widehat A_s=(g_t-U_t)(A_{t+s}\setminus A_t),\qquad s\geq0,
$$

with the usual hull closure, have the original law and are independent of $\mathcal F_t$. Their capacity is $2s$ by the [half-plane-capacity composition rule](../../../stochastic-process.md#half-plane-capacity-composition-rule). One may require the same restarting property at finite [stopping times](../../../martingale.md#stopping-time).

Equivalently, the driver has the scaling law and conditional increment law

$$
\boxed{(r^{-1}U_{r^2s})_{s\geq0}\overset{d}=(U_s)_{s\geq0},\qquad
(U_{t+s}-U_t)_{s\geq0}\mid\mathcal F_t\ \overset{d}=(U_s)_{s\geq0}\text{ independently}.}
$$

The conformal invariance clause matters: the restarting property alone would also allow a Brownian driver with deterministic drift.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) gives a continuous [Loewner driving function](../../../stochastic-process.md#loewner-driving-function), and we normalize $U_0=0$. Mapping out an initial hull transforms the future driver to $U_{t+s}-U_t$. The [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle) therefore gives [stationary increments](../../../stochastic-process.md#stationary-increments) and [independent increments](../../../stochastic-process.md#independent-increments).

Consequently $U$ is a continuous [Lévy process](../../../stochastic-process.md#levy-process). In the [Lévy–Khintchine formula](../../../stochastic-process.md#levy-khintchine-formula), continuity excludes its jump measure, so its only possible components are a deterministic linear drift and [Brownian motion](../../../brownian-motion.md):

$$
U_t=\mu t+\sigma B_t,\qquad\sigma\geq0.
$$

Conformal invariance under dilations gives $U_{r^2t}/r\overset{d}=U_t$. Comparing the [expectations](../../../probability-theory.md#expected-value) of these [Gaussian random variables](../../../probability-theory.md#gaussian-random-variable) yields $\mu rt=\mu t$ for every $r>0$, hence $\mu=0$. The Brownian term already has the required law by [Brownian scaling](../../../brownian-motion.md#brownian-scaling). Therefore the [characterization of the SLE driving function](../../../stochastic-process.md#characterization-of-the-sle-driving-function) is

$$
\boxed{U_t=\sqrt\kappa B_t\quad\text{in law},\qquad\kappa=\sigma^2\geq0.}
$$

The case $\kappa=0$ is the constant zero driver. No reflection-symmetry assumption is needed to remove the drift; scaling suffices.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The scaling rule for the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) shows that $A_t=\sqrt t\,A_1$, because $r^{-1}U_{r^2t}=a\sqrt t$. To identify the shape, rather than infer it from scaling alone, construct the inverse map explicitly. Put

$$
d=\sqrt{a^2+16},\qquad r_\pm=\frac{a\pm d}{2},\qquad
\alpha=-\frac{r_-}{d}\in(0,1).
$$

Then $r_-<0<r_+$, $r_-r_+=-4$, and $\alpha r_++(1-\alpha)r_-=0$. Define

$$
f_t(w)=(w-r_+\sqrt t)^\alpha(w-r_-\sqrt t)^{1-\alpha},
$$

using logarithms whose arguments lie in $(0,\pi)$ on $\mathbb H$. Its [Laurent series](../../../analysis.md#laurent-series) is $f_t(w)=w-2t/w+O(w^{-2})$, so it has the inverse [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity).

On the real interval $(r_-\sqrt t,r_+\sqrt t)$, the first factor has argument $\pi\alpha$ and the second has argument zero. The image therefore lies on one straight ray. Its modulus increases from zero to a maximum at $w=a\sqrt t$, and then decreases to zero. The complementary real intervals map to the negative and positive real axes. The [argument principle](../../../complex-analysis.md#argument-principle), or the usual conformal slit-map construction, shows that $f_t$ maps $\mathbb H$ conformally onto the half-plane minus that segment; the interval traverses its two sides.

The boundary walk has winding number one around every point of the half-plane off the segment: the two traversals of the slit cancel, leaving the real boundary and a large semicircle. The [argument principle](../../../complex-analysis.md#argument-principle) therefore gives exactly one preimage of each such point.

It remains to check that this is the correct [Loewner chain](../../../stochastic-process.md#loewner-chain). For $f=f_1$,

$$
\frac{f'(w)}{f(w)}=\frac{w-a}{(w-r_+)(w-r_-)}
=\frac{w-a}{w^2-aw-4}.
$$

Together with $f_t(w)=\sqrt t\,f(w/\sqrt t)$, this gives

$$
\partial_tf_t(w)=-\frac{2f_t'(w)}{w-a\sqrt t},
$$

the inverse form of the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation). Uniqueness therefore identifies its slit with $A_t$. Its endpoint is $\sqrt t\,f_1(a)$, where $f_1(a)\ne0$ lies in $\mathbb H$. This proves that the [square-root Loewner driving function generates a straight slit](../../../stochastic-process.md#square-root-loewner-driving-function-generates-a-straight-slit) and that

$$
\boxed{\bigcup_{t\geq0}A_t=\{s f_1(a):s>0\},}
$$

a straight ray from the boundary point $0$ to infinity.

## 2

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

By the [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace), chordal [SLE](../../../stochastic-process.md#schramm-loewner-evolution) is a [simple curve](../../../topology.md#simple-curve) for

$$
\boxed{0\leq\kappa\leq4.}
$$

If the convention restricts the notation to $\kappa>0$, the range is $0<\kappa\leq4$. The degenerate case $\kappa=0$ is a deterministic vertical slit and is simple as well.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

By the [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace), the trace has self-intersections but is not a [space-filling curve](../../../topology.md#space-filling-curve) for

$$
\boxed{4<\kappa<8.}
$$

The endpoint $\kappa=4$ remains simple, while $\kappa=8$ belongs to the space-filling regime.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The [Phase classification of the SLE trace](../../../stochastic-process.md#phase-classification-of-the-sle-trace) gives a [space-filling curve](../../../topology.md#space-filling-curve) precisely for

$$
\boxed{\kappa\geq8.}
$$

In particular, the critical value $\kappa=8$ is included.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Start the [Bessel process](../../../brownian-motion.md#bessel-process) at $x>0$ and let $\tau_0$ be its first hit of zero. Away from zero its [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) is

$$
dX_t=dW_t+\frac{\delta-1}{2X_t}\,dt.
$$

Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $f(x)=x^{2-\delta}$, localizing first to a compact interval in $(0,\infty)$. Its drift cancels:

$$
\frac12f''(x)+\frac{\delta-1}{2x}f'(x)
=\frac{(2-\delta)(1-\delta)}2x^{-\delta}
+\frac{(\delta-1)(2-\delta)}2x^{-\delta}=0.
$$

Thus the [Bessel power local martingale](../../../brownian-motion.md#bessel-power-local-martingale) satisfies

$$
\boxed{d(X_t^{2-\delta})=(2-\delta)X_t^{1-\delta}\,dW_t\qquad(t<\tau_0).}
$$

For $\delta=2$, this power is simply the constant one. For $\delta>2$, it is a [continuous local martingale](../../../martingale.md#continuous-local-martingale) for all time, as zero is inaccessible.

Here is a proof of that inaccessibility and of the stronger minimum assertion. For $0<r<x<R$, stop the power at $\tau_r\wedge\tau_R$. The stopped process is bounded, so the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
\mathbb P_x(\tau_r<\tau_R)
=\frac{x^{2-\delta}-R^{2-\delta}}{r^{2-\delta}-R^{2-\delta}}.
$$

Exit from the bounded interval occurs almost surely. Taking $r\downarrow0$ with $R$ fixed shows that zero cannot be hit before $R$, hence cannot be hit in finite time. Taking $R\to\infty$ instead gives

$$
\mathbb P_x(\tau_r<\infty)=\left(\frac r x\right)^{\delta-2}.
$$

If the all-time infimum were zero, every level $r>0$ below $x$ would be hit, by [continuity](../../../calculus.md#continuous-function). Letting $r\downarrow0$ proves the [all-time minimum of a transient Bessel process](../../../brownian-motion.md#all-time-minimum-of-a-transient-bessel-process) assertion:

$$
\boxed{\delta>2,\ X_0>0\quad\Longrightarrow\quad\inf_{t\geq0}X_t>0\quad\text{almost surely}.}
$$

The first claim in the printed question needs a qualification when $\delta<2$: it holds before the first hit of zero, or for the process stopped there, rather than for the usual reflecting continuation. For example, at $\delta=1$ the proposed power is $X$ itself, a [Reflected Brownian motion](../../../brownian-motion.md#reflected-brownian-motion); the [Tanaka formula](../../../stochastic-calculus.md#tanaka-s-formula) contains a nonzero [local time of a semimartingale](../../../stochastic-calculus.md#local-time-of-a-semimartingale) term, so it is not a [local martingale](../../../martingale.md#local-martingale) after reflection. A positive starting point is also needed for the negative power when $\delta>2$; an entrance process started at zero would give an infinite value at time zero.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $\kappa>0$ and $x>0$, before the boundary point is swallowed, put $X_t=(g_t(x)-U_t)/\sqrt\kappa$. The [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation) and $dU_t=\sqrt\kappa\,dB_t$ give

$$
dX_t=\frac{2}{\kappa X_t}\,dt-dB_t.
$$

Since $-B$ is again a standard [Brownian motion](../../../brownian-motion.md), this is the [Boundary-point Bessel flow for SLE](../../../stochastic-process.md#boundary-point-bessel-flow-for-sle) with

$$
\boxed{\delta=1+\frac4\kappa.}
$$

For $x<0$, it is $-X_t$ that is the nonnegative [Bessel process](../../../brownian-motion.md#bessel-process), with the same dimension; the formula without this sign convention is a signed Bessel flow.

When $0<\kappa\leq4$, one has $\delta\geq2$, and the [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process) says that $X_t$ never reaches zero. The borderline $\delta=2$ uses the [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes) $\log x$: for $0<r<x<R$,

$$
\mathbb P_x(\tau_r<\tau_R)=\frac{\log R-\log x}{\log R-\log r}\longrightarrow0\quad(r\downarrow0).
$$

Thus the critical case also cannot hit zero in finite time, though its all-time infimum is zero.

Apply the non-swallowing assertion simultaneously to all nonzero rational boundary points. The order-preserving real Loewner flow then keeps every compact real interval away from the origin in the surviving boundary. A boundary contact away from the starting point would cut off a nonempty real interval, swallowing a rational point, so the trace avoids $\mathbb R\setminus\{0\}$.

The same argument can be applied to the future after every rational time, using the [Conformal Markov property of SLE](../../../stochastic-process.md#conformal-markov-property-of-sle). If the trace revisited an earlier point, choose a rational time strictly between the two visits. In the domain with that initial segment removed, the later visit would be a contact with an old boundary point away from the current growing tip. Under the mapping-out map, such a contact cuts off a real interval and contradicts the preceding non-swallowing result. This is the usual [crosscut](../../../complex-analysis.md#crosscut) argument converting boundary non-swallowing into absence of self-intersections. Taking the countable intersection over rational restart times proves

$$
\boxed{\operatorname{SLE}_\kappa\text{ is simple for }0<\kappa\leq4.}
$$

For $\kappa=0$, the equation is deterministic and gives the simple slit $(0,2i\sqrt t]$. The division by $\sqrt\kappa$ is unnecessary in that case.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Scaling invariance of SLE](../../../stochastic-process.md#scaling-invariance-of-sle) says that $r^{-1}\gamma(r^2t)$ has the same law as $\gamma(t)$. Therefore its first time reaching height one is $r^{-2}\sigma_r$, and

$$
\mathbb P(\sigma_r<\infty)=\mathbb P(\sigma_1<\infty)=:p
$$

for every $r>0$.

To identify $p$, it suffices to look at small heights. The trace must have a point of positive imaginary part: otherwise it lies entirely on the real axis and its hull in $\mathbb H$ is empty, contradicting $\operatorname{hcap}(A_t)=2t>0$. By [continuity](../../../calculus.md#continuous-function) from $\gamma(0)=0$, any positive height attained by the trace forces it to pass through every smaller positive height.

Consequently the increasing union of events $\{\sigma_{1/n}<\infty\}$ has probability one. Each event has probability $p$, so continuity of probability gives $p=1$. This proves that [SLE reaches every positive height](../../../stochastic-process.md#sle-reaches-every-positive-height):

$$
\boxed{\mathbb P(\sigma_r<\infty)=1\qquad(r>0).}
$$

Equivalently, a positive random height supremum whose law is invariant under every dilation must be infinite almost surely. This argument uses neither [Transience of chordal SLE](../../../stochastic-process.md#transience-of-chordal-sle) nor any assertion about where the trace goes as time tends to infinity.

## 3

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

For real [test functions](../../../distribution-theory.md#test-function) $f,g\in C_c^\infty(D)$, the [Dirichlet inner product](../../../sobolev-space.md#dirichlet-inner-product) in the normalization compatible with the logarithmic Green kernel is

$$
\boxed{(f,g)_\nabla=\frac1{2\pi}\int_D\nabla f(x)\cdot\nabla g(x)\,dx.}
$$

Its norm measures gradient energy rather than the values of the functions. A [change of variables](../../../calculus.md#change-of-variables-formula) shows that this energy is invariant under planar [conformal maps](../../../geometry-and-topology.md#conformal-map): the squared derivative in the transformation of the [gradient](../../../calculus.md#gradient) cancels the area [Jacobian determinant](../../../calculus.md#jacobian-determinant).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The convention used for planar [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) theory is the [Dirichlet energy space](../../../sobolev-space.md#dirichlet-energy-space):

$$
\boxed{H_0^1(D)=\overline{C_c^\infty(D;\mathbb R)}^{\ \|\cdot\|_\nabla},\qquad
\|f\|_\nabla^2=\frac1{2\pi}\int_D|\nabla f|^2.}
$$

It is a real [Hilbert space](../../../hilbert-space.md) with the extended [Dirichlet inner product](../../../sobolev-space.md#dirichlet-inner-product). A [conformal map](../../../geometry-and-topology.md#conformal-map) from the [unit disc](../../../topology.md#unit-disc) onto $D$ identifies the two energy completions, so local representatives can be understood through the disc's zero-boundary space.

For an arbitrary unbounded domain this is the homogeneous energy completion; it should be distinguished from completion in the inhomogeneous norm $\|f\|_{L^2}+\|\nabla f\|_{L^2}$ used in another standard definition of the [zero-boundary Sobolev space](../../../sobolev-space.md#zero-boundary-sobolev-space). On bounded domains with a [Poincaré inequality](../../../sobolev-space.md#poincare-inequality), the two norms are equivalent.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(e_n)$ of the [Dirichlet energy space](../../../sobolev-space.md#dirichlet-energy-space) and independent variables $(\xi_n)$ with the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). The zero-boundary [Gaussian free field](../../../stochastic-process.md#gaussian-free-field) is the formal series

$$
\boxed{h=\sum_{n\geq1}\xi_ne_n.}
$$

Its precise energy-indexed interpretation is the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process)

$$
(h,f)_\nabla:=\sum_{n\geq1}\xi_n(e_n,f)_\nabla,\qquad f\in H_0^1(D).
$$

For every fixed $f$, this sum converges in $L^2$ of the probability space by [Parseval identity](../../../fourier-analysis.md#parseval-identity), and it is a centered [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable). For $f,g\in H_0^1(D)$,

$$
\boxed{\mathbb E[(h,f)_\nabla(h,g)_\nabla]=(f,g)_\nabla.}
$$

This [covariance](../../../variance.md#covariance) characterizes its law independently of the chosen basis. The series does not define an $H_0^1$-valued random element: $\sum_n\xi_n^2=\infty$ almost surely. It is realized as a random [distribution](../../../distribution-theory.md#distribution-mathematical-analysis), and its pairing with ordinary test functions is constructed in part (b).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The expression is a [Test-function pairing with a Gaussian free field](../../../stochastic-process.md#test-function-pairing-with-a-gaussian-free-field), rather than the pointwise integral of an ordinary random function. For a real [test function](../../../distribution-theory.md#test-function) $\phi$, take the Dirichlet solution

$$
f_\phi=-2\pi\Delta^{-1}\phi,
\qquad f_\phi(x)=\int_DG(x,y)\phi(y)\,dy,
$$

using the Green-kernel identity allowed in the original PDF. In particular, $-\Delta f_\phi=2\pi\phi$. [Integration by parts](../../../calculus.md#integration-by-parts) gives, initially for smooth compactly supported $u$ and then by [continuity](../../../calculus.md#continuous-function) in the [Dirichlet energy space](../../../sobolev-space.md#dirichlet-energy-space),

$$
(u,f_\phi)_\nabla=\frac1{2\pi}\int_D\nabla u\cdot\nabla f_\phi
=\int_Du(x)\phi(x)\,dx.
$$

The integral functional is continuous in the energy norm: pull back to the [unit disc](../../../topology.md#unit-disc), where the transformed test function has compact support, and use the [Poincaré inequality](../../../sobolev-space.md#poincare-inequality). Hence $f_\phi$ is its energy-space representer. Define

$$
\boxed{(h,\phi):=(h,f_\phi)_\nabla.}
$$

By the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process) definition, it has mean zero and [variance](../../../variance.md)

$$
\begin{aligned}
\mathbb E[(h,\phi)^2]
&=\|f_\phi\|_\nabla^2
=\int_D f_\phi(x)\phi(x)\,dx\\
&=\iint_{D\times D}\phi(x)G(x,y)\phi(y)\,dx\,dy.
\end{aligned}
$$

The logarithmic singularity is locally integrable, so this [variance](../../../variance.md) is finite for smooth compactly supported test functions. Thus

$$
\boxed{(h,\phi)\sim N\!\left(0,\iint\phi(x)G(x,y)\phi(y)\,dx\,dy\right).}
$$

The local TeX corrupted the double integral and the bracketed Green-kernel identity; the PDF supplies the identity above and does not assert an infinite [variance](../../../variance.md).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Set $F(w)=(\phi(w)-\phi(0))/w$ for $w\ne0$. The singularity is removable, with $F(0)=\phi'(0)$. Injectivity of the [conformal map](../../../geometry-and-topology.md#conformal-map) makes $F(w)\ne0$ away from zero, and conformality makes $F(0)\ne0$ as well. Since the disc is simply connected, $F$ has a [holomorphic logarithm](../../../complex-analysis.md#holomorphic-logarithm). Therefore $\psi=\log|F|$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function), including at zero, and $\psi(0)=\log|\phi'(0)|$.

The [mean value property for harmonic functions](../../../partial-differential-equation.md#mean-value-property-for-harmonic-functions) gives, for every $0<r<1$,

$$
\log|\phi'(0)|=\frac1{2\pi}\int_0^{2\pi}\log|\phi(re^{i\theta})-\phi(0)|\,d\theta-\log r.
$$

For general $D$, boundary values mean radial limits, rather than a continuous extension of $\phi$ to every point of the circle. The [boundary logarithmic mean of a univalent function](../../../complex-analysis.md#boundary-logarithmic-mean-of-a-univalent-function) justifies taking $r\uparrow1$: the [Koebe distortion theorem](../../../complex-analysis.md#koebe-distortion-theorem) bounds $|F|$ below by $|\phi'(0)|/4$, while the standard integral-mean bound for a [univalent function](../../../complex-analysis.md#univalent-function), $\sup_{r<1}\int|\phi(re^{i\theta})|^p d\theta<\infty$ for $0<p<1/2$, gives [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) of its positive logarithm. Radial limits exist almost everywhere, and passage to the integral follows. Thus, writing $dw=d\theta$ for arc length on the unit circle,

$$
\boxed{\log|\phi'(0)|=\frac1{2\pi}\int_{\partial\mathbb D}\log|\phi(w)-\phi(0)|\,dw.}
$$

The expression on the left is the logarithm of the [conformal radius](../../../geometry-and-topology.md#conformal-radius) of $D$ at $z=\phi(0)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The canonical [Dirichlet Green function](../../../analysis.md#dirichlet-green-function) on the [unit disc](../../../topology.md#unit-disc) with its pole at zero is $-\log|w|$. Conformal invariance of the planar Green kernel therefore gives

$$
G_D(z,\phi(w))=-\log|w|.
$$

Comparing with $G_D(z,y)=-\log|z-y|-G_z(y)$ yields

$$
G_z(\phi(w))=-\log|\phi(w)-\phi(0)|+\log|w|=-\psi(w).
$$

This also explains the boundary data: when $|w|=1$, the correction is $-\log|\phi(w)-z|$. The composition with $\phi^{-1}$ is harmonic by [conformal invariance of harmonicity](../../../complex-analysis.md#conformal-invariance-of-harmonicity). Its apparent singularity at $z$ is removable because the quotient defining $\psi$ extends to $\phi'(0)$.

Evaluating there proves the [regular part of the planar Dirichlet Green function](../../../analysis.md#regular-part-of-the-planar-dirichlet-green-function) formula

$$
\boxed{G_z(y)=-\psi(\phi^{-1}(y)),\qquad G_z(z)=-\log|\phi'(0)|=-\log\operatorname{crad}_D(z).}
$$

On an unbounded domain, boundary values alone need not specify a unique [harmonic function](../../../partial-differential-equation.md#harmonic-function). Here $G_z$ is the correction belonging to the canonical Dirichlet Green kernel, which fixes that ambiguity.

## 4

↑ **Parent:** [Paper 203](paper-203.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For the [Locality property of SLE](../../../stochastic-process.md#locality-property-of-sle), take a [compact H-hull](../../../stochastic-process.md#compact-h-hull) $A$ away from $0$, and map $\mathbb H\setminus A$ conformally to $\mathbb H$ by $\psi_A$, fixing $0$ and infinity and with derivative one at infinity. Up to the first contact with $A$, the image under $\psi_A$ of an $\operatorname{SLE}_6$ grown in $\mathbb H$ has the same law as $\operatorname{SLE}_6$ grown in $\mathbb H$, after the change to its own [half-plane-capacity parameterization](../../../stochastic-process.md#half-plane-capacity-parameterization). Equivalently, $\operatorname{SLE}_6$ in the smaller domain has the same initial law as the curve in the larger domain until the latter encounters the removed hull. There is no conditioning on eventual avoidance.

The [chordal restriction property](../../../stochastic-process.md#chordal-restriction-property) for $\operatorname{SLE}_{8/3}$ concerns the whole curve. Conditional on avoiding $A$, applying $\psi_A$ gives the original $\operatorname{SLE}_{8/3}$ law, modulo increasing reparameterization:

$$
\boxed{\mathcal L\bigl(\psi_A(\gamma)\mid\gamma\cap A=\varnothing\bigr)=\mathcal L(\gamma).}
$$

Its associated avoidance probability, from the [SLE eight-thirds restriction martingale](../../../stochastic-process.md#sle-eight-thirds-restriction-martingale), is

$$
\boxed{\mathbb P(\gamma\cap A=\varnothing)=\psi_A'(0)^{5/8}.}
$$

Thus locality identifies a stopped, unconditioned law, whereas restriction identifies a conditioned law of the entire curve.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Interpret the printed $A_0=0$ as the empty initial hull. Write $a(t)=\operatorname{hcap}(\widetilde A_t)$ and $F_t=\psi_t$. [Conformal maps](../../../geometry-and-topology.md#conformal-map) preserve inclusion and simple connectedness of the complementary domains, so the image sets form an increasing hull family. Boundedness of $\psi$ on bounded sets ensures that these image hulls are bounded. The [Loewner local growth property](../../../stochastic-process.md#loewner-local-growth-property) is preserved under conformal transport: after mapping out the hull at time $t$, the small new hull is transported by $F_t$ near its single boundary growth point. The [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) extends $F_t$ analytically across that point, with real positive derivative. The image diameters therefore tend to zero as the original ones do. These statements use the usual hull closures and [prime ends](../../../geometry-and-topology.md#prime-end); the initial image hull is empty.

For completeness, the infinitesimal capacity rule underlying this argument is that a shrinking hull $J$ attached near $u$, transported by a map $F$ analytic there, has

$$
\operatorname{hcap}(F(J))=F'(u)^2\operatorname{hcap}(J)+o(\operatorname{hcap}(J)).
$$

One obtains this by rescaling at $u$: the transported map tends to its linear part, and [half-plane capacity](../../../stochastic-process.md#half-plane-capacity) scales by the square of the dilation. Uniform analytic distortion near the growth point controls the error. Applying it to the mapped-out increments gives local absolute continuity of $a$ and $a'(t)=2F_t'(U_t)^2$.

The coefficient can also be read directly from the [Chordal Loewner equation](../../../stochastic-process.md#chordal-loewner-equation). The image driver is $\widetilde U_t=F_t(U_t)$. Differentiate $F_t=\widetilde g_t\circ\psi\circ g_t^{-1}$, at a fixed point $w$, to obtain

$$
\partial_tF_t(w)=\frac{a'(t)}{F_t(w)-F_t(U_t)}-\frac{2F_t'(w)}{w-U_t}.
$$

The left side is regular at $w=U_t$. On the right, the coefficient of $(w-U_t)^{-1}$ is $a'(t)/F_t'(U_t)-2F_t'(U_t)$, so it must vanish. This proves the [conformal change of half-plane capacity](../../../stochastic-process.md#conformal-change-of-half-plane-capacity) rule and its integrated version:

$$
\boxed{\operatorname{hcap}(\widetilde A_t)=\int_0^t2\bigl(\psi_s'(U_s)\bigr)^2\,ds,\qquad\widetilde A_0=\varnothing.}
$$

If the derivative at the initial boundary point is singular, the formula is interpreted by integrating from a positive time and taking the lower limit to zero; finite image capacity and kernel continuity give this limit. The duplicated incomplete normalization sentence in the TeX is absent from the PDF.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A [Brownian excursion in the upper half-plane](../../../brownian-motion.md#brownian-excursion-in-the-upper-half-plane) from $0$ to infinity is killed [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) conditioned to stay in $\mathbb H$, with its entrance law at $0$. Precisely, it is the [Doob h-transform](../../../markov-process.md#doob-h-transform) for $h(z)=\operatorname{Im}z$, obtained by starting at $i\varepsilon$ and letting $\varepsilon\downarrow0$. Equivalently,

$$
\boxed{\widehat B_t=W_t+iR_t,}
$$

where $W$ is standard [Brownian motion](../../../brownian-motion.md) and the independent process $R$ is a dimension-three [Bessel process](../../../brownian-motion.md#bessel-process) started at zero. The transformed generator is $\frac12\Delta+y^{-1}\partial_y$, which explains this representation.

First compute avoidance from an interior point $z$. Let $\tau$ be the exit time of ordinary [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) from $\mathbb H\setminus A$. The harmonic correction

$$
v(z)=\operatorname{Im}\bigl(z-g_A(z)\bigr)
$$

has boundary values $\operatorname{Im}z$ on $A$ and zero on the real axis. The [hydrodynamic normalization at infinity](../../../stochastic-process.md#hydrodynamic-normalization-at-infinity) gives $g_A(z)=z+\operatorname{hcap}(A)/z+O(|z|^{-2})$. Together with the [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions) this gives the useful bound $0\leq v\leq\sup_{a\in A}\operatorname{Im}a$. Since ordinary [Brownian motion](../../../brownian-motion.md) hits the real axis almost surely, the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) applied to this bounded [harmonic function](../../../partial-differential-equation.md#harmonic-function) gives

$$
v(z)=\mathbb E_z[\operatorname{Im}B_\tau]
=\mathbb E_z[\operatorname{Im}B_\tau\,\mathbf1_{\{B_\tau\in A\}}].
$$

The [Doob h-transform](../../../markov-process.md#doob-h-transform) weights a stopped path by its final height divided by its initial height. Applying this at the first hit of $A$, with bounded-time localization and then a limit, therefore yields

$$
\mathbb P_z^h(\tau_A<\infty)=\frac{v(z)}{\operatorname{Im}z},\qquad
\mathbb P_z^h(\tau_A=\infty)=\frac{\operatorname{Im}g_A(z)}{\operatorname{Im}z}.
$$

For the entrance law the same result follows by conditioning at a small positive time and letting that time decrease to zero: the avoidance function has the boundary limit computed next, and the excursion is initially in a neighbourhood disjoint from $A$.

Because the closure of the hull avoids $0$, the [Schwarz reflection principle](../../../complex-analysis.md#schwarz-reflection-principle) makes $g_A$ analytic in a neighbourhood of zero, with real $g_A(0)$ and positive real $g_A'(0)$. Thus

$$
\lim_{\varepsilon\downarrow0}\frac{\operatorname{Im}g_A(i\varepsilon)}{\varepsilon}=g_A'(0).
$$

In fact, the reflected Taylor expansion gives $\operatorname{Im}g_A(z)/\operatorname{Im}z=g_A'(0)+O(|z|)$ uniformly as $z\to0$ inside the half-plane, so the same limit applies to the entrance process. The map in the question is $\psi_A=g_A-g_A(0)$, so its derivative agrees with $g_A'$. We obtain the [restriction probability of a Brownian half-plane excursion](../../../brownian-motion.md#restriction-probability-of-a-brownian-half-plane-excursion):

$$
\boxed{\mathbb P\bigl[\widehat B([0,\infty))\cap A=\varnothing\bigr]=\psi_A'(0).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
