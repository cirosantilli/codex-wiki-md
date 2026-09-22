# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper29.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Set $h_n=2^{-n}$ and $t_n=h_n\lceil t/h_n\rceil$. Replace the last sampled value $X_{t_n}$ by $X_t$, and call the resulting absolute-increment sum $W_n(t)$. This is a sum over a genuine [partition of an interval](../../../real-analysis.md#partition-of-an-interval) of $[0,t]$, and

$$
|V_t^{n,|\cdot|}-W_n(t)|\le |X_{t_n}-X_t|\longrightarrow0
$$

by right continuity. This is the [dyadic approximation of total variation](../../../real-analysis.md#dyadic-approximation-of-total-variation). Let $V(t)$ be the [total variation of a function](../../../real-analysis.md#total-variation-of-a-function) $X$ on $[0,t]$, allowing $+\infty$. Every $W_n(t)$ is at most $V(t)$. Conversely, take any finite [partition of an interval](../../../real-analysis.md#partition-of-an-interval) of $[0,t]$. Approximate its interior points from the right by dyadic grid points, retaining the endpoint $t$. For large $n$ these approximating points remain distinct, and right continuity makes their absolute-increment sum converge to that of the original partition. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) makes $W_n(t)$ at least this selected sum. Taking the [supremum](../../../real-analysis.md#supremum) over all partitions proves

$$
\boxed{\lim_{n\to\infty}V_t^{n,|\cdot|}=V(t),\quad V(t)=\operatorname{Var}_{[0,t]}X\in[0,\infty].}
$$

The limit is the total-variation function; for locally finite variation it is the [total-variation process](../../../stochastic-calculus.md#total-variation-process).

There is a missing hypothesis in the assertion about being [càdlàg](../../../calculus.md#cadlag). A general [càdlàg function](../../../calculus.md#cadlag) can have infinite [total variation of a function](../../../real-analysis.md#total-variation-of-a-function) arbitrarily close to zero. For example,

$$
X_0=0,\qquad X_s=s\sin(1/s)\quad(s>0)
$$

is continuous. At the successive points $s_j=(\pi/2+j\pi)^{-1}$ its values alternate in sign with magnitude $s_j$. The variation along these points dominates a divergent harmonic series. Thus $V(t)=\infty$ for every $t>0$, but $V(0)=0$, so even extended-valued right continuity fails at zero.

The correct [càdlàg](../../../calculus.md#cadlag) conclusion holds when $X$ has [finite variation](../../../real-analysis.md#total-variation-of-a-function) on every compact interval. Indeed $V$ is then finite and nondecreasing, so it has finite left limits. To prove right continuity at $t$, fix $s>t$ and choose a partition of $[t,s]$ whose sum is within $\varepsilon$ of its variation. If $u>t$ lies before the first interior partition point, changing the first endpoint from $t$ to $u$ changes that sum by at most $|X_u-X_t|$. Additivity of [total variation of a function](../../../real-analysis.md#total-variation-of-a-function) therefore gives

$$
0\le V(u)-V(t)\le\varepsilon+|X_u-X_t|.
$$

Let $u\downarrow t$ and then $\varepsilon\downarrow0$. This proves right continuity. This proves [càdlàg regularity of finite total variation](../../../stochastic-calculus.md#cadlag-regularity-of-finite-total-variation). Under that qualification, the jump formula is

$$
\boxed{\Delta V_t=|\Delta X_t|=|X_t-X_{t-}|\qquad(t>0).}
$$

If the variation is infinite, a difference of two infinite variation values is not a defined jump.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Fix $T<\infty$. By [uniform continuity](../../../topological-analysis.md#uniform-continuity) of each path of the [continuous local martingale](../../../martingale.md#continuous-local-martingale) on $[0,T+1]$, its modulus

$$
\eta_n=\sup_{\substack{u,v\in[0,T+1]\\|u-v|\le h_n}}|X_u-X_v|
$$

tends to zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). For every $s\le T$, comparison of powers of each increment gives

$$
V_s^{n,|\cdot|^p}\le\eta_n^{p-2}V_T^{n,|\cdot|^2}.
$$

The squared-increment sum converges in [probability](../../../probability-theory.md#probability) to $[X]_T$, by the dyadic definition of [quadratic variation](../../../stochastic-calculus.md#quadratic-variation). Including the last full grid interval instead of the last partial interval changes that sum by a quantity bounded by $2\eta_n^2$, so the ceiling convention has the same limit. In particular these squared-increment sums are bounded in [probability](../../../probability-theory.md#probability).

Since $p-2>0$, a quantity tending to zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) multiplied by a family bounded in [probability](../../../probability-theory.md#probability) tends to zero in [probability](../../../probability-theory.md#probability). Hence

$$
\boxed{\sup_{s\le T}V_s^{n,|\cdot|^p}\xrightarrow{\mathbb P}0\quad\text{for every }T<\infty.}
$$

This is [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability), and proves the superquadratic case of [dyadic power variation of a continuous local martingale](../../../stochastic-calculus.md#dyadic-power-variation-of-a-continuous-local-martingale).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix the specified time $t$. With the path modulus $\eta_n$ on $[0,t+1]$ as above, comparison of increment powers now gives

$$
V_t^{n,|\cdot|^2}\le\eta_n^{2-p}V_t^{n,|\cdot|^p}.
$$

The hypothesis makes the second factor eventually bounded [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), while the first tends to zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) because $2-p>0$. Thus the squared-increment sums tend to zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). They also converge in [probability](../../../probability-theory.md#probability) to the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $[X]_t$, so uniqueness of the limit in [probability](../../../probability-theory.md#probability) implies $[X]_t=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence).

The [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) is nondecreasing, hence it vanishes throughout $[0,t]$. To see explicitly that the [continuous local martingale](../../../martingale.md#continuous-local-martingale) must then be constant, localize it to square-integrable stopped [martingales](../../../martingale.md). The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives

$$
\mathbb E\bigl|X_{s\wedge\sigma_N}-X_0\bigr|^2
=\mathbb E[X]_{s\wedge\sigma_N}=0\qquad(s\le t).
$$

Remove the localization, apply the conclusion at every rational $s\le t$, and use continuity. Since $X_0=0$, this proves

$$
\boxed{\mathbb P(X_s=0\text{ for every }s\in[0,t])=1.}
$$

Thus $X$ is indistinguishable from the zero process on that interval. This is the subquadratic case of [dyadic power variation of a continuous local martingale](../../../stochastic-calculus.md#dyadic-power-variation-of-a-continuous-local-martingale).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

No [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) argument is needed. For deterministic $u<v$, the [martingale](../../../martingale.md) property and square integrability give

$$
\mathbb E(X_vX_u)=\mathbb E\bigl[X_u\mathbb E(X_v\mid\mathcal F_u)\bigr]=\mathbb E X_u^2.
$$

Consequently

$$
\mathbb E(X_v-X_u)^2=\mathbb E X_v^2-\mathbb E X_u^2.
$$

Apply this identity separately to each consecutive grid increment. The second moments telescope, giving

$$
\boxed{\mathbb E V_t^{n,|\cdot|^2}=\mathbb E X_{t_n}^2-\mathbb E X_0^2
\le\sup_{s\ge0}\mathbb E X_s^2-\mathbb E X_0^2<\infty.}
$$

This uniform bound follows directly from [martingale-difference orthogonality](../../../martingale.md#martingale-difference-orthogonality), including the final interval specified by the ceiling.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The gradient bound makes $f$ a [Lipschitz function](../../../real-analysis.md#lipschitz-continuity), with $|f(x)|\le|f(0)|+K\lVert x\rVert$, so its value at a [Gaussian random variable](../../../probability-theory.md#gaussian-random-variable) is integrable and square integrable. The future [Brownian increment](../../../brownian-motion.md#brownian-increment) $X_1-X_t$ is independent of $\mathcal F_t$ and has distribution $N(0,(1-t)I_d)$. Conditioning on the current location therefore gives

$$
\boxed{M_t=\mathbb E[f(X_t+(X_1-X_t))\mid\mathcal F_t]=P_{1-t}f(X_t).}
$$

This is the [Markov property](../../../markov-process.md#markov-property) expressed through the [Brownian transition semigroup](../../../brownian-motion.md#brownian-transition-semigroup). In particular $M_0=\mu$ and $M_1=f(X_1)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $u(t,x)=P_{1-t}f(x)$ for $t<1$. Differentiating the [Brownian transition semigroup](../../../brownian-motion.md#brownian-transition-semigroup) in the spatial variables is justified by the bounded gradient and gives

$$
\partial_i u(t,x)=P_{1-t}(\partial_i f)(x).
$$

The [heat equation](../../../diffusion-equation.md#heat-equation) for this [semigroup](../../../algebra.md#semigroup) is the backward equation $\partial_tu+\tfrac12\Delta u=0$. Applying the multidimensional [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) yields

$$
du(t,X_t)=\left(\partial_tu+\tfrac12\Delta u\right)(t,X_t)\,dt
+\sum_{i=1}^d\partial_i u(t,X_t)\,dX_t^i.
$$

The finite-variation term vanishes. Thus

$$
\boxed{dM_t=\sum_{i=1}^d P_{1-t}(\partial_i f)(X_t)\,dX_t^i.}
$$

Initially this calculation holds on $[0,1-\varepsilon]$. The vector of [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) coefficients has norm at most $K$, so the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) lets the integrals extend to time one. Also $P_{1-t}f(X_t)\to f(X_1)$ in $L^2$ by the [Lipschitz function](../../../real-analysis.md#lipschitz-continuity) bound and continuity of [Brownian motion](../../../brownian-motion.md). The same representation therefore holds on the entire interval.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $g_t=P_{1-t}(\nabla f)(X_t)$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) for the conditional average gives

$$
\lVert g_t\rVert\le P_{1-t}(\lVert\nabla f\rVert)(X_t)\le K.
$$

The independent coordinate [Brownian motions](../../../brownian-motion.md) have zero cross-variation, so the [quadratic variation of a stochastic integral](../../../stochastic-calculus.md#quadratic-variation-of-a-stochastic-integral) gives

$$
\boxed{[M]_1=\int_0^1\lVert g_t\rVert^2\,dt\le K^2.}
$$

The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) says that a [continuous local martingale](../../../martingale.md#continuous-local-martingale) $N$ starting at zero whose [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) diverges admits a [Brownian motion](../../../brownian-motion.md) $B$, with the inverse-clock filtration, such that $N_t=B_{[N]_t}$. If the total clock is finite, one may enlarge the probability space and append independent [Brownian motion](../../../brownian-motion.md) after the clock terminates. This gives the same identity up to the original lifetime.

Apply this theorem to $N=M-M_0$. The clock bound implies the event inclusion

$$
\{|M_1-M_0|>r\}\subseteq\left\{\sup_{0\le s\le K^2}|B_s|>r\right\}.
$$

The latter event is contained in the union of the upper and lower crossing events. Symmetry of [Brownian motion](../../../brownian-motion.md) gives

$$
\boxed{\mathbb P(|M_1-M_0|>r)\le2\mathbb P\left(\sup_{0\le s\le K^2}B_s>r\right).}
$$

This uses only an event inclusion; independence between the [Brownian motion](../../../brownian-motion.md) and its random clock is neither assumed nor needed.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) and [Brownian scaling](../../../brownian-motion.md#brownian-scaling) give

$$
\mathbb P\left(\sup_{s\le K^2}B_s>r\right)
=2\mathbb P(B_{K^2}>r)=2\mathbb P(Z>r/K),
$$

where $Z$ has the standard [normal distribution](../../../probability-theory.md#normal-distribution). Combine part (c) with the allowed [Gaussian tail bound](../../../probability-and-statistics.md#gaussian-tail-bound) to obtain

$$
\boxed{\mathbb P(|f(X)-\mu|>r)\le4\exp\left(-\frac{r^2}{2K^2}\right).}
$$

This is the [Brownian martingale proof of Gaussian concentration](../../../stochastic-process.md#brownian-martingale-proof-of-gaussian-concentration). It proves the intended [Gaussian concentration inequality](../../../stochastic-process.md#gaussian-concentration-inequality). The denominator printed in the initial bound is $2K$, whereas the gradient hypothesis and part (c) give $2K^2$. The stronger printed bound is false in general. For a concrete counterexample, take $d=1$, $K=2$, and $f(x)=2x$. At $r=10$,

$$
\mathbb P(|f(Z)|>10)=2\mathbb P(Z>5)
>\frac{2}{\sqrt{2\pi}}e^{-18}>4e^{-25},
$$

where the first strict inequality follows by integrating the decreasing normal density over $[5,6]$. The rightmost term is the printed bound. Thus the square on $K$ is a necessary source correction, rather than a change of proof technique.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use the following form of the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem). If $W$ is [Brownian motion](../../../brownian-motion.md), $\vartheta$ is predictable, and

$$
Z_t=\exp\left(\int_0^t\vartheta_s\,dW_s-\frac12\int_0^t\vartheta_s^2\,ds\right)
$$

is a [uniformly integrable martingale](../../../martingale.md#uniformly-integrable-martingale) with $Z_0=1$, then the [probability measure](../../../probability-theory.md#probability-measure) with terminal density $Z_\infty$ makes $W_t-\int_0^t\vartheta_s\,ds$ a [Brownian motion](../../../brownian-motion.md). The analogous finite-horizon statement uses the terminal density at that horizon.

Here take $W_t=X_t-x$ and $\vartheta_s=\mathbf1_{\{s<\tau\}}/X_s$. Before $\tau$, $X_s\in[\varepsilon,M]$, so the [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is well-defined. The assumed uniform integrability of the stopped [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) gives

$$
\mathbb E_{\mathbb W_x}Z_\tau=1,\qquad
Z_{t\wedge\tau}=\mathbb E_{\mathbb W_x}(Z_\tau\mid\mathcal F_t).
$$

Thus the proposed weighting really defines a [probability measure](../../../probability-theory.md#probability-measure), and the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) gives the [Brownian motion](../../../brownian-motion.md)

$$
B_t=X_t-x-\int_0^{t\wedge\tau}\frac{ds}{X_s}
$$

under that measure. In particular

$$
\boxed{X_t=x+B_t+\int_0^t\frac{ds}{X_s}\qquad(0\le t\le\tau).}
$$

All calculations are first made on this compact stopped interval. The integral involving $1/X$ is naturally defined on $[0,T_0)$; at $T_0$ its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) may diverge. The density will have a zero limiting extension there, as established below, rather than a finite stochastic logarithm at the hitting time.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $w\ne0$ in $\mathbb R^3$, the radial function $r(w)=\lVert w\rVert$ has

$$
\partial_i r=\frac{w_i}{r},\qquad
\partial_{ij}r=\frac{\delta_{ij}}{r}-\frac{w_iw_j}{r^3},\qquad
\Delta r=\frac2r.
$$

The multidimensional [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), initially stopped away from zero, gives

$$
dR_t=\sum_{i=1}^3\frac{W_t^i}{R_t}\,dW_t^i+\frac{dt}{R_t}.
$$

The martingale term has [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $dt$, since $\sum_i(W_t^i/R_t)^2=1$. The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) says that a continuous [local martingale](../../../martingale.md#local-martingale) starting at zero with [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $t$ is a standard [Brownian motion](../../../brownian-motion.md). Consequently the radial equation is

$$
\boxed{dR_t=dB_t+\frac{dt}{R_t}.}
$$

On $[\varepsilon,M]$ the drift $1/r$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). Extend it to a bounded globally [Lipschitz function](../../../real-analysis.md#lipschitz-continuity) on the real line. The standard existence and pathwise uniqueness theorem for [stochastic differential equations](../../../stochastic-calculus.md#stochastic-differential-equation) with globally Lipschitz coefficients applies to this extension, and gives uniqueness in law up to the first exit from $[\varepsilon,M]$. Both this radial process and the process in part (a) solve the same equation from $x$. Thus

$$
\boxed{\mathcal L(R_{\cdot\wedge\tau_R})
=\mathcal L_{\mathbb Q^{M,\varepsilon}}(X_{\cdot\wedge\tau_X}),}
$$

where each exit time is computed from its own coordinate path.

For completeness, the radial equation is valid globally: the [three-dimensional Bessel process](../../../brownian-motion.md#three-dimensional-bessel-process) does not hit zero. Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $1/R$ on the annulus. Its drift is zero, and the stopped process is a bounded [martingale](../../../martingale.md). At the first exit,

$$
\frac1x=\frac1\varepsilon\mathbb P(T_\varepsilon<T_M)
+\frac1M\mathbb P(T_M<T_\varepsilon),
$$

so

$$
\mathbb P(T_\varepsilon<T_M)=\frac{\varepsilon(M-x)}{x(M-\varepsilon)}\longrightarrow0.
$$

The exit time is finite because one coordinate of the underlying [Brownian motion](../../../brownian-motion.md) reaches $M$ in finite time. Letting $\varepsilon\downarrow0$ and then considering arbitrarily large $M$ proves that zero is never reached. The radial martingale therefore has [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $t$ on the whole time axis, completing the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) argument.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Under [Wiener measure](../../../brownian-motion.md#wiener-measure), $dX_t=dW_t$ and

$$
[M]_t=\int_0^t\frac{ds}{X_s^2}\qquad(t\le\tau).
$$

The definition of the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) gives

$$
d\log Z_t=\frac{dX_t}{X_t}-\frac{dt}{2X_t^2}.
$$

On the other hand, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applied to the logarithm gives precisely

$$
d\log X_t=\frac{dX_t}{X_t}-\frac{dt}{2X_t^2}.
$$

Their initial values differ by $\log x$, so

$$
\boxed{\log Z_t=\log X_t-\log x,\qquad Z_t=X_t/x\quad(t\le\tau),}
$$

[almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) under [Wiener measure](../../../brownian-motion.md#wiener-measure). In particular,

$$
Z_\tau=\frac Mx\mathbf1_{\{T_M<T_\varepsilon\}}
+\frac\varepsilon x\mathbf1_{\{T_\varepsilon<T_M\}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write $\tau_\varepsilon=T_\varepsilon\wedge T_M$. The stopped [Bessel process](../../../brownian-motion.md#bessel-process) has the same law as the weighted stopped [Brownian motion](../../../brownian-motion.md), so for every bounded measurable functional $F$ of a continuous path,

$$
\mathbb E F(R^{\tau_\varepsilon})
=\mathbb E_{\mathbb W_x}\left[F(X^{\tau_\varepsilon})
\left(\frac Mx\mathbf1_{\{T_M<T_\varepsilon\}}
+\frac\varepsilon x\mathbf1_{\{T_\varepsilon<T_M\}}\right)\right].
$$

The [Bessel process](../../../brownian-motion.md#bessel-process) hits $M$ in finite time and never hits zero. Its minimum before that hitting time is strictly positive. Thus for sufficiently small $\varepsilon$, depending on the path, its stopped path $R^{\tau_\varepsilon}$ equals $R^{T_M}$ exactly. Under [Wiener measure](../../../brownian-motion.md#wiener-measure), the events $\{T_M<T_\varepsilon\}$ increase to $\{T_M<T_0\}$, and on that event the stopped paths eventually equal $X^{T_M}$. The remaining term is bounded by $\varepsilon\lVert F\rVert_\infty/x$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) therefore yields the precise limiting identity

$$
\boxed{\mathbb E F(R^{T_M})
=\frac Mx\mathbb E_{\mathbb W_x}\left[
\mathbf1_{\{T_M<T_0\}}F(X^{T_M})\right].}
$$

The bounded stopped [martingale](../../../martingale.md) $X_{t\wedge T_0\wedge T_M}$ gives

$$
x=\mathbb E X_{T_0\wedge T_M}=M\mathbb W_x(T_M<T_0),
\qquad \mathbb W_x(T_M<T_0)=x/M.
$$

Hence the limiting identity says

$$
\boxed{\mathcal L(R^{T_M})
=\mathcal L_{\mathbb W_x}(X^{T_M}\mid T_M<T_0).}
$$

This establishes [Brownian conditioning by a stopped Bessel density](../../../stochastic-calculus.md#brownian-conditioning-by-a-stopped-bessel-density).

The displayed density in the question requires a stopping convention. On the full, unstopped path space, the probability measure

$$
\frac{d\widetilde{\mathbb Q}^{M}}{d\mathbb W_x}
=\frac Mx\mathbf1_{\{T_M<T_0\}}
$$

is well-defined, but its paths continue as [Brownian motion](../../../brownian-motion.md) after $T_M$. Its pushforward by the stopping map $\omega\mapsto\omega(\cdot\wedge T_M(\omega))$ is the law $\mathbb Q^M$ of the stopped [Bessel process](../../../brownian-motion.md#bessel-process). Equivalently, if $\mathbb W_x^{0,M}$ denotes the law of [Brownian motion](../../../brownian-motion.md) stopped at $T_0\wedge T_M$, then the actual stopped laws satisfy

$$
\boxed{\frac{d\mathbb Q^M}{d\mathbb W_x^{0,M}}
=\frac Mx\mathbf1_{\{\text{exit at }M\}}.}
$$

Literal absolute continuity of the stopped law with respect to unstopped [Wiener measure](../../../brownian-motion.md#wiener-measure) is false: paths that become permanently constant at $M$ have probability one for the stopped law and zero under [Wiener measure](../../../brownian-motion.md#wiener-measure). The same density is also valid on the stopped sigma-algebra of the original coordinate space. Thus the corrected stopped-law formulation proves the intended conclusion without equating these different full-path measures.

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion) is a time-change statement. If $\phi:D\to D'$ is a conformal bijection of planar domains and $B$ is [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started in $D$, let $\tau_D$ be its exit time and define

$$
A_t=\int_0^{t\wedge\tau_D}|\phi'(B_s)|^2\,ds.
$$

Before exit this clock is strictly increasing. Its inverse $C_u$ makes $\phi(B_{C_u})$ a [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $\phi(B_0)$, up to its transformed lifetime $A_{\tau_D}$. The image of the stopped trajectory is therefore invariant in law after this change of time. A holomorphic map with nonzero derivative gives the corresponding local statement even without global injectivity.

Here is the proof. Write $\phi=u+iv$ and $B=(B^1,B^2)$. The real and imaginary parts are harmonic. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) therefore gives the two [continuous local martingales](../../../martingale.md#continuous-local-martingale)

$$
u(B_t)-u(B_0)=\int_0^t\nabla u(B_s)\cdot dB_s,
\qquad
v(B_t)-v(B_0)=\int_0^t\nabla v(B_s)\cdot dB_s,
$$

stopped on compact subsets of $D$. The [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) imply

$$
|\nabla u|^2=|\nabla v|^2=|\phi'|^2,
\qquad\nabla u\cdot\nabla v=0.
$$

Thus both coordinate [quadratic variations](../../../stochastic-calculus.md#quadratic-variation) equal $A_t$ and their [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) is zero. After inverse time change, the covariance matrix of the two [continuous local martingales](../../../martingale.md#continuous-local-martingale) is $uI_2$. The multidimensional [Lévy characterization of multidimensional Brownian motion](../../../brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion) states that a continuous vector [local martingale](../../../martingale.md#local-martingale) starting at zero with this covariance matrix is standard vector [Brownian motion](../../../brownian-motion.md). Apply it after subtracting $\phi(B_0)$, and exhaust $D$ by compact subsets. This proves the theorem, with killing at the transformed exit lifetime. The clock is the [conformal Brownian clock](../../../brownian-motion.md#conformal-brownian-clock); omitting it would generally give an incorrect speed.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The exponential map is a conformal bijection from the strip

$$
\mathcal S=\{z:-\alpha<\operatorname{Im}z<\beta\}
$$

to the wedge containing the starting point $1$. The restriction $\alpha+\beta<2\pi$ makes it injective. A [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) $U+iV$ started at zero in this strip maps, after the [conformal Brownian clock](../../../brownian-motion.md#conformal-brownian-clock), to the required [Brownian motion](../../../brownian-motion.md) in the wedge.

Let $\sigma$ be the first time $V$ exits $(-\alpha,\beta)$. It is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and $V_{t\wedge\sigma}$ is a bounded [martingale](../../../martingale.md). The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
0=\mathbb E V_\sigma
=\beta p-\alpha(1-p),
\qquad p=\mathbb P(V_\sigma=\beta).
$$

The strip exit maps to the corresponding bounding ray. The exponential clock is finite at $\sigma$, because its integrand is continuous on the compact time interval $[0,\sigma]$. Thus it does not remove or reverse the exit event. We obtain

$$
\boxed{\mathbb P(S_\beta<S_{-\alpha})=\frac{\alpha}{\alpha+\beta}.}
$$

This is the [Brownian wedge-exit probability](../../../brownian-motion.md#brownian-wedge-exit-probability) obtained directly from the strip, using [conformal invariance of planar Brownian motion](../../../brownian-motion.md#conformal-invariance-of-planar-brownian-motion).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Put $L_r=\theta_{T_r}$. The hitting times $T_r$ are finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) by [recurrence of planar Brownian motion](../../../brownian-motion.md#recurrence-of-planar-brownian-motion), and increase with $r$. At $T_r$, the position is $e^{-r}e^{iL_r}$. By the [Strong Markov property](../../../markov-process.md#strong-markov-property), [Brownian scaling](../../../brownian-motion.md#brownian-scaling), and [rotational invariance of planar Brownian motion](../../../brownian-motion.md#rotational-invariance-of-planar-brownian-motion), the future process

$$
\widehat B_u=e^r e^{-iL_r}B_{T_r+e^{-2r}u}
$$

is a standard [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion) started at $1$, independent of $\mathcal F_{T_r}$. The random rotation does not change its conditional law, since that law is rotationally invariant.

The first time this rescaled process reaches radius $e^{-h}$ corresponds to the original time $T_{r+h}$. Its continuous argument starts at zero and equals the increment of the original winding angle. Hence

$$
\boxed{L_{r+h}-L_r\ \text{is independent of }\mathcal F_{T_r}
\text{ and has the law of }L_h.}
$$

For any ordered finite collection of levels, apply this assertion successively. Earlier winding values are measurable at the current hitting time, so all increments are independent and their laws depend only on the level differences. This proves the [Lévy process](../../../stochastic-process.md#levy-process) property of [winding at logarithmic radial passage levels](../../../brownian-motion.md#winding-at-logarithmic-radial-passage-levels).

One can also verify stochastic continuity and identify this process. The logarithmic-radius and argument martingales have the common clock

$$
H_t=\int_0^t|B_s|^{-2}\,ds.
$$

The same [Cauchy-Riemann equations](../../../analysis.md#cauchy-riemann-equations) calculation as in part (a), applied locally to the logarithm and joined along the continuous argument, gives independent [Brownian motions](../../../brownian-motion.md) $U,V$ such that $\log R_t=U_{H_t}$ and $\theta_t=V_{H_t}$. This clock diverges: if it had a finite limit, convergence of martingales with finite total [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) would make $\log R_t$ converge to a finite value, forcing the clock integral itself to diverge.

Thus, with $\eta_r=\inf\{u:U_u=-r\}$, we have $L_r=V_{\eta_r}$. The [Brownian first-passage Laplace transform](../../../markov-process.md#brownian-first-passage-laplace-transform) is $\mathbb E e^{-q\eta_r}=e^{-r\sqrt{2q}}$. It follows either from the [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion) stopped at $\eta_r\wedge n$, or from the one-dimensional exit equation. Conditioning on the independent process $U$ gives

$$
\boxed{\mathbb E e^{i\lambda L_r}=\mathbb E e^{-\lambda^2\eta_r/2}=e^{-r|\lambda|}.}
$$

So this is a symmetric [Cauchy process](../../../stochastic-process.md#cauchy-process), with level parameter $r$. The formula implies stochastic continuity at zero and, by stationary increments, everywhere. Under the usual definition requiring [càdlàg](../../../calculus.md#cadlag) paths, use the right-continuous passage clock $\eta_r^+=\inf\{u:U_u<-r\}$. It agrees with $\eta_r$ for each fixed level [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and $V_{\eta_r^+}$ is the [càdlàg](../../../calculus.md#cadlag) modification. This distinction concerns simultaneous passage levels and does not alter any increment law.

## 5

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A left-continuous [adapted process](../../../stochastic-process.md#adapted-process) is a [predictable process](../../../martingale.md#predictable-process). Define the elementary predictable approximation

$$
H_s^{(n)}=H_{kh_n}\quad\text{for }kh_n<s\le(k+1)h_n,
\qquad h_n=2^{-n}.
$$

At every $s>0$, its sample time approaches $s$ from the left, including when $s$ is itself a grid point. Thus $H_s^{(n)}\to H_s$ pathwise by left continuity.

Use the [continuous semimartingale decomposition](../../../stochastic-calculus.md#continuous-semimartingale-decomposition) $X=X_0+M+A$, with $M$ a [continuous local martingale](../../../martingale.md#continuous-local-martingale) and $A$ a continuous [finite-variation process](../../../stochastic-calculus.md#finite-variation-process). Localize so that on a fixed horizon $T$, the integrands are bounded by a deterministic constant, $[M]_T$ is bounded, and the [total-variation process](../../../stochastic-calculus.md#total-variation-process) of $A$ at $T$ is bounded. This is possible using local boundedness and the finite pathwise clock and variation.

For the finite-variation integral, the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives

$$
\sup_{t\le T}\left|\int_0^t(H_s^{(n)}-H_s)\,dA_s\right|
\le\int_0^T|H_s^{(n)}-H_s|\,d|A|_s\longrightarrow0
$$

[almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). For the martingale integral, the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) and the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) give

$$
\mathbb E\sup_{t\le T}\left|\int_0^t(H_s^{(n)}-H_s)\,dM_s\right|^2
\le4\mathbb E\int_0^T|H_s^{(n)}-H_s|^2\,d[M]_s\longrightarrow0.
$$

Here the localized bounds justify dominated convergence also in expectation. Remove localization to conclude that the full elementary integrals converge in [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability) to $\int H\,dX$.

The sum of completed intervals differs from the full elementary integral at time $t$ by

$$
H_{h_n\lfloor t/h_n\rfloor}
\left(X_t-X_{h_n\lfloor t/h_n\rfloor}\right).
$$

Its maximum on $[0,T]$ tends to zero [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), by the local bound on $H$ and [uniform continuity](../../../topological-analysis.md#uniform-continuity) of $X$. Therefore

$$
\boxed{\sum_{k=0}^{\lfloor t/h_n\rfloor-1}H_{kh_n}
(X_{(k+1)h_n}-X_{kh_n})
\xrightarrow{\mathrm{u.c.p.}}\int_0^tH_s\,dX_s.}
$$

This proves [left-endpoint approximation of a continuous semimartingale integral](../../../stochastic-calculus.md#left-endpoint-approximation-of-a-continuous-semimartingale-integral), including the unfinished interval convention.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Define the [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) of two [continuous semimartingales](../../../stochastic-calculus.md#continuous-semimartingale) by polarization:

$$
[X,Y]_t=\frac14\bigl([X+Y]_t-[X-Y]_t\bigr).
$$

The available [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) convergence theorem and the [polarization identity](../../../linear-algebra.md#polarization-identity) imply that the sums of products of simultaneous grid increments converge in [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability) to $[X,Y]$. The [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) is a continuous finite-variation process, vanishing at time zero.

For a grid ending at $t_n=h_n\lfloor t/h_n\rfloor$, the elementary algebraic identity

$$
X_{(k+1)h_n}Y_{(k+1)h_n}-X_{kh_n}Y_{kh_n}
=X_{kh_n}\Delta_kY+Y_{kh_n}\Delta_kX+\Delta_kX\Delta_kY
$$

telescopes. The first two sums converge by part (a), with the continuous processes $X,Y$ as integrands; continuous paths are left-continuous and locally bounded. The last sum converges to the [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) by the preceding polarization argument. Finally, $X_{t_n}Y_{t_n}\to X_tY_t$ locally uniformly by continuity. Hence

$$
\boxed{X_tY_t=X_0Y_0+\int_0^tX_s\,dY_s+\int_0^tY_s\,dX_s+[X,Y]_t.}
$$

This is the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule), or stochastic [integration by parts](../../../calculus.md#integration-by-parts). Uniqueness of the limit in [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability), followed by continuity, makes the identity hold simultaneously for all $t$ outside one null set. The proof used finite-grid algebra, part (a), and the permitted [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) theorem; it did not use the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma).

## 6

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Use the local convention for the [martingale problem](../../../stochastic-calculus.md#martingale-problem), which is appropriate for arbitrary measurable coefficients. A continuous [adapted process](../../../stochastic-process.md#adapted-process) $X$ solves $\mathbf M(a,b)$ if the coefficient integrals are locally finite and, for every $f\in C_c^\infty(\mathbb R)$,

$$
N_t^f=f(X_t)-f(X_0)-\int_0^t
\left(\frac12a(X_s)f''(X_s)+b(X_s)f'(X_s)\right)ds
$$

is a [local martingale](../../../martingale.md#local-martingale). Here locally finite means $\int_0^T(|a(X_s)|+|b(X_s)|)ds<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) for each $T<\infty$. Suitable localization upgrades the identities to true [martingale](../../../martingale.md) identities. With bounded coefficients and bounded test derivatives, this distinction disappears on finite horizons.

A [Markov diffusion](../../../stochastic-calculus.md#markov-diffusion) generated by $L$ is a time-homogeneous [Markov process](../../../markov-process.md) with continuous paths whose [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) on the stated test domain is $L$. Its transition operators satisfy the generator limit, and [Dynkin formula](../../../stochastic-process.md#dynkin-s-formula) gives precisely the preceding [martingale problem](../../../stochastic-calculus.md#martingale-problem) identities. Some terminology uses [L-diffusion](../../../stochastic-calculus.md#diffusion-martingale-problem) for the test-function identities alone; the Markov property is an additional assertion unless uniqueness supplies it.

Suppose now $a=\sigma^2>0$. Use smooth compactly supported functions agreeing with $x$ and $x^2$ on $[-R,R]$, and stop before exiting this interval. Removing these stops shows that

$$
N_t=X_t-X_0-\int_0^tb(X_s)ds
$$

is a [continuous local martingale](../../../martingale.md#continuous-local-martingale). Consequently $X$ is a [continuous semimartingale](../../../stochastic-calculus.md#continuous-semimartingale). The [martingale problem](../../../stochastic-calculus.md#martingale-problem) applied to the second cutoff function says that

$$
X_t^2-X_0^2-\int_0^t\bigl(a(X_s)+2X_sb(X_s)\bigr)ds
$$

is a [local martingale](../../../martingale.md#local-martingale). The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) for $X^2$ also says that

$$
X_t^2-X_0^2-2\int_0^tX_sb(X_s)ds-[N]_t
$$

is a [local martingale](../../../martingale.md#local-martingale). Subtracting, the continuous finite-variation process $[N]_t-\int_0^ta(X_s)ds$ is a [local martingale](../../../martingale.md#local-martingale) and starts at zero. The theorem that a [continuous finite-variation local martingale is constant](../../../martingale.md#continuous-finite-variation-local-martingale-is-constant) gives

$$
[N]_t=\int_0^t\sigma^2(X_s)ds.
$$

Define

$$
B_t=\int_0^t\frac1{\sigma(X_s)}\,dN_s.
$$

The integrand is predictable and is stochastically integrable, since its integral against the bracket is exactly $t$. Thus $B$ is a [continuous local martingale](../../../martingale.md#continuous-local-martingale) with $B_0=0$ and $[B]_t=t$. The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) states that these conditions make $B$ a [Brownian motion](../../../brownian-motion.md) relative to the given filtration. Associativity of [stochastic integrals](../../../stochastic-calculus.md#stochastic-integral) recovers $N=\int\sigma(X)\,dB$, and therefore

$$
\boxed{dX_t=b(X_t)dt+\sigma(X_t)dB_t.}
$$

The original process is a [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation), with its driving [Brownian motion](../../../brownian-motion.md) constructed on the original space.

Conversely, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applied to any weak solution with locally integrable coefficients gives the [martingale problem](../../../stochastic-calculus.md#martingale-problem) identities. A [Markov diffusion](../../../stochastic-calculus.md#markov-diffusion) with generator $L$ gives them by [Dynkin formula](../../../stochastic-process.md#dynkin-s-formula). A [well-posed martingale problem](../../../stochastic-calculus.md#well-posed-martingale-problem), with the usual measurable path-space setup, identifies a unique family of diffusion laws and yields the [Strong Markov property](../../../markov-process.md#strong-markov-property). Without uniqueness, the test-function identities alone do not assert that every chosen solution is Markov. This specifies both the equivalence with weak equations and the role of uniqueness in identifying a diffusion.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Set $u_0=\alpha/\beta$ and use the accelerated grid time $j/n$. At population $k=nu_0+\sqrt n\,x$, the fluctuation increment is $h_n=n^{-1/2}$, $-h_n$, or zero. Its first and second conditional moments, multiplied by $n$, are

$$
b_n(x)=n\mathbb E(\Delta X^n\mid x)
=\sqrt n\,(p_k-q_k)=-\alpha x-\frac\beta{\sqrt n}x^2,
$$



$$
a_n(x)=n\mathbb E((\Delta X^n)^2\mid x)
=p_k+q_k=\frac{2\alpha^2}{\beta}
+\frac{3\alpha}{\sqrt n}x+\frac\beta n x^2.
$$

Thus $b_n\to b(x)=-\alpha x$ and $a_n\to a=2\alpha^2/\beta$, uniformly on every compact set. The centered conditional variance has the same limit, since the squared conditional mean contributes only $b_n(x)^2/n$.

Here is the [diffusion approximation theorem](../../../stochastic-calculus.md#diffusion-approximation-theorem) being applied. For Markov chains sampled with time step $1/n$, suppose the first and second conditional increment moments multiplied by $n$ converge uniformly on compact sets to continuous coefficients $b,a$; the large-jump conditional second moments satisfy the local Lindeberg condition; the initial laws converge; compact containment holds on finite time intervals; and the limiting [martingale problem](../../../stochastic-calculus.md#martingale-problem) is well-posed and nonexplosive. Then the interpolated chains converge weakly, uniformly on finite time intervals, to that problem's continuous solution. The step versions converge in the [Skorokhod J1 topology](../../../convergence-of-random-variables.md#skorokhod-j1-topology). Local moment bounds supply the stopped-process tightness, and the limiting test-function identities identify every subsequential limit by the [martingale problem](../../../stochastic-calculus.md#martingale-problem).

We verify the global condition rather than assume it. Before the stopping rule is triggered, $p_k+q_k\le1$, and $k\ge0$ implies $x\ge-u_0\sqrt n$. Therefore

$$
xb_n(x)=-x^2\left(\alpha+\frac\beta{\sqrt n}x\right)\le0.
$$

For the [Lyapunov function](../../../dynamical-systems.md#lyapunov-function) $V(x)=x^2$, the exact one-step generator is consequently

$$
G_nV(x)=2xb_n(x)+a_n(x)\le1.
$$

After stopping, the process is constant. Applying the elementary stopped [supermartingale](../../../martingale.md#supermartingale) inequality for $V(X_{j/n}^n)-j/n$, and stopping also on first reaching $|X^n|\ge L$, gives

$$
\boxed{\mathbb P\left(\sup_{t\le1}|X^n_{t\wedge\tau_n}|\ge L\right)
\le\frac{(X_0^n)^2+1}{L^2}.}
$$

This is [compact containment](../../../convergence-of-random-variables.md#compact-containment). At zero population we use the natural absorbing convention $p_0=q_0=0$; the same calculation is valid there.

The invalid-probability threshold is at the positive root

$$
u_* =\frac{\sqrt{\alpha^2+4\beta}-\alpha}{2\beta}
\quad\text{of}\quad\alpha u+\beta u^2=1.
$$

Because $2\alpha^2<\beta$, we have $u_*>u_0$. The corresponding fluctuation level $\sqrt n(u_*-u_0)$ tends to infinity, so the stopping rule changes none of the compact-set moment limits. The initial fluctuation satisfies $|X_0^n|\le n^{-1/2}$ and hence tends to zero. All jumps have magnitude at most $n^{-1/2}$, so the Lindeberg condition is immediate. The limiting equation has globally Lipschitz coefficients and is well-posed and nonexplosive. The theorem therefore gives

$$
\boxed{dX_t=-\alpha X_tdt+\alpha\sqrt{\frac2\beta}\,dB_t,
\qquad X_0=0.}
$$

This is the [Ornstein-Uhlenbeck fluctuation limit at a stable population equilibrium](../../../markov-process.md#ornstein-uhlenbeck-fluctuation-limit-at-a-stable-population-equilibrium). The limiting [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process) has explicit solution

$$
X_t=\alpha\sqrt{\frac2\beta}\int_0^te^{-\alpha(t-s)}dB_s,
\qquad \operatorname{Var}(X_t)=\frac\alpha\beta(1-e^{-2\alpha t}).
$$

The PDF samples the linearly interpolated population at $\lfloor nt\rfloor$, so its displayed process is actually the step version. Using $nt$ instead gives the continuous interpolation; their uniform distance is at most $n^{-1/2}$. Both therefore have the asserted continuous diffusion limit, with the step version interpreted in [Skorokhod J1 topology](../../../convergence-of-random-variables.md#skorokhod-j1-topology).

Finally, if $\tau_n\le1$, the stopped fluctuation reaches a value greater than $\sqrt n(u_*-u_0)$. The preceding [Lyapunov function](../../../dynamical-systems.md#lyapunov-function) bound gives directly

$$
\boxed{\mathbb P(\tau_n\le1)
\le\frac{(X_0^n)^2+1}{n(u_*-u_0)^2}\longrightarrow0.}
$$

This also shows explicitly why the artificial stopping rule is asymptotically irrelevant.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
