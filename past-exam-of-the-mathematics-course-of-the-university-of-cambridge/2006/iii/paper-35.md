# Paper 35

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper35.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper35.pdf)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Relative to a [filtration](../../../stochastic-process.md#filtration-probability-theory) satisfying the usual conditions, a [local martingale](../../../martingale.md#local-martingale) is an [adapted](../../../stochastic-process.md#adapted-process) [càdlàg process](../../../stochastic-process.md#cadlag-process) $X$ for which there exist increasing [stopping times](../../../martingale.md#stopping-time) $S_n\uparrow\infty$ almost surely such that every stopped process $X^{S_n}_t=X_{t\wedge S_n}$ is an integrable [martingale](../../../martingale.md). Thus, for $s\le t$,

$$
\mathbb E[X_{t\wedge S_n}\mid\mathcal F_s]=X_{s\wedge S_n}.
$$

The sequence is a [localizing sequence](../../../martingale.md#localizing-sequence). A [continuous local martingale](../../../martingale.md#continuous-local-martingale) additionally has continuous sample paths. The usual definition entails integrability of the initial value; [local martingales](../../../martingale.md#local-martingale) need not be integrable at later times without stopping.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $V_t$ be the [total variation](../../../real-analysis.md#total-variation) of $X$ on $[0,t]$, and set $\tau_n=\inf\{t:V_t\ge n\}$. Adaptation and continuity of $V$ make these [stopping times](../../../martingale.md#stopping-time); [finite variation](../../../real-analysis.md#total-variation-of-a-function) on every compact interval gives $\tau_n\uparrow\infty$. The stopped process $U=X^{\tau_n}$ satisfies $|U_t|\le n$ and has [total variation](../../../real-analysis.md#total-variation) at most $n$. It is a [martingale](../../../martingale.md) by the [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion), and is [square-integrable](../../../measure-theory.md#square-integrable-function).

Fix $t$ and take deterministic partitions $0=t_0<\cdots<t_m=t$ with mesh tending to zero. The [martingale-difference orthogonality](../../../martingale.md#martingale-difference-orthogonality) of the increments gives

$$
\mathbb E[U_t^2]=\sum_j\mathbb E[(U_{t_{j+1}}-U_{t_j})^2].
$$

Pathwise, however,

$$
\sum_j(U_{t_{j+1}}-U_{t_j})^2
\le\max_j|U_{t_{j+1}}-U_{t_j}|\sum_j|U_{t_{j+1}}-U_{t_j}|
\le n\max_j|U_{t_{j+1}}-U_{t_j}|\longrightarrow0,
$$

by [uniform continuity](../../../topological-analysis.md#uniform-continuity) on $[0,t]$. These sums are bounded by $n^2$, so the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives $\mathbb E U_t^2=0$. Hence $U_t=0$ almost surely. Take all rational $t$ on a common probability-one event and use continuity to obtain $U\equiv0$. Then let $n\to\infty$. This proves the [continuous finite-variation local martingale is constant](../../../martingale.md#continuous-finite-variation-local-martingale-is-constant) result in its zero-starting form:

$$
\boxed{X_t=0\text{ for every }t\ge0\text{ almost surely}.}
$$

The proof does not assume the uniqueness of [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) that is to be established next.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For two candidates $A,C$, their difference is a continuous [adapted](../../../stochastic-process.md#adapted-process) [finite-variation process](../../../stochastic-calculus.md#finite-variation-process). It is also a [local martingale](../../../martingale.md#local-martingale), since

$$
A-C=(Y^2-C)-(Y^2-A).
$$

Apply part (b) after subtracting its initial value. Consequently

$$
\boxed{A_t-C_t=A_0-C_0\quad\text{for all }t\text{ almost surely}.}
$$

This proves the [uniqueness of an increasing square compensator](../../../stochastic-calculus.md#uniqueness-of-an-increasing-square-compensator) when the initial value is prescribed, in particular under the standard [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) normalization $A_0=C_0=0$.

The printed assertion omits that normalization and is literally false. For standard [Brownian motion](../../../brownian-motion.md) $Y$, both $A_t=t$ and $C_t=t+1$ are continuous [adapted](../../../stochastic-process.md#adapted-process) increasing processes; both $Y_t^2-t$ and $Y_t^2-t-1$ are [martingales](../../../martingale.md). Thus **uniqueness holds after fixing the initial value; otherwise it holds only up to an initial constant**.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For a [simple predictable process](../../../martingale.md#simple-predictable-process), define its [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) by

$$
(H\cdot M)_t=\sum_{k=0}^{n-1}Z_k\bigl(M_{t\wedge t_{k+1}}-M_{t\wedge t_k}\bigr).
$$

It is constant after $t_n$, so the symbol $(H\cdot M)_\infty$ means its value there. Put $\Delta_kM=M_{t_{k+1}}-M_{t_k}$. If $k<\ell$, then $Z_k\Delta_kM Z_\ell$ is $\mathcal F_{t_\ell}$-measurable, and the [conditional expectation](../../../measure-theory.md#conditional-expectation) of $\Delta_\ell M$ given that [sigma-algebra](../../../measure-theory.md#sigma-algebra) is zero. Boundedness of the coefficients and square-integrability of $M$ justify the expectations, so all cross terms vanish:

$$
\mathbb E[(H\cdot M)_\infty^2]
=\sum_k\mathbb E[Z_k^2(\Delta_kM)^2].
$$

For each diagonal term, the [martingale](../../../martingale.md) increment identity also gives

$$
\mathbb E[Z_k^2(\Delta_kM)^2]
=\mathbb E[Z_k^2(M_{t_{k+1}}^2-M_{t_k}^2)].
$$

Indeed, the omitted term $2Z_k^2M_{t_k}\Delta_kM$ has expectation zero. Apply the assumed [martingale](../../../martingale.md) property of $M^2-[M]$ to replace this difference of squares by the corresponding [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) increment. Thus

$$
\boxed{\mathbb E[(H\cdot M)_\infty^2]
=\sum_k\mathbb E[Z_k^2([M]_{t_{k+1}}-[M]_{t_k})]
=\mathbb E[(H^2\cdot[M])_\infty].}
$$

The intervals $(t_k,t_{k+1}]$ in the Lebesgue–Stieltjes integral exactly match these increments, including possible jumps of $M$.

## 2

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $M_t=\int_0^tH_s\,dB_s$ and $A_t=\int_0^tH_s^2ds=[M]_t$. The assumed path properties make $A$ continuous, strictly increasing and unbounded. Therefore $T$ is a finite [stopping time](../../../martingale.md#stopping-time) and $A_T=\sigma^2$, even though its definition uses a strict inequality.

For $u\in\mathbb R$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
E_t=\exp\left(iuM_{t\wedge T}+\frac{u^2}{2}A_{t\wedge T}\right),\qquad
dE_t=iuE_t\,dM_{t\wedge T}.
$$

Its real and imaginary parts are [local martingales](../../../martingale.md#local-martingale), and $|E_t|\le e^{u^2\sigma^2/2}$. Thus $E$ is a bounded true [martingale](../../../martingale.md). Continuity of $M$, finiteness of $T$, and [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) yield $\mathbb E E_T=1$. Rearranging gives

$$
\mathbb E e^{iuM_T}=e^{-u^2\sigma^2/2}.
$$

The [characteristic function](../../../probability-theory.md#characteristic-function) uniquely identifies the distribution, proving the [Gaussian terminal value at a deterministic bracket level](../../../martingale.md#gaussian-terminal-value-at-a-deterministic-bracket-level):

$$
\boxed{\int_0^T H_s\,dB_s\sim N(0,\sigma^2).}
$$

This proof does not use the time-change theorem that the later part asks us to prove.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) states: let $M$ be a [continuous local martingale](../../../martingale.md#continuous-local-martingale) with $M_0=0$ and $[M]_\infty=\infty$ almost surely. Set

$$
\tau_u=\inf\{t\ge0:[M]_t>u\},\qquad
\mathcal G_u=\mathcal F_{\tau_u}.
$$

Then $W_u=M_{\tau_u}$ is standard [Brownian motion](../../../brownian-motion.md) relative to $(\mathcal G_u)$ and

$$
\boxed{M_t=W_{[M]_t}.}
$$

Strict increase of the bracket is not required in the general theorem: $M$ is constant on intervals on which its bracket is constant. Continuity of $M$ is required. A nonzero initial value is handled by applying the theorem to $M-M_0$ and adding it back. If the terminal bracket is finite, the [finite-lifetime extension of the Dambis-Dubins-Schwarz theorem](../../../martingale.md#finite-lifetime-extension-of-the-dambis-dubins-schwarz-theorem) supplies the [Brownian motion](../../../brownian-motion.md) up to that bracket time and, if necessary, an independent continuation on an enlarged probability space.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use $A_t=\int_0^tH_s^2ds$ and its inverse $\tau_u$ as above. Strict increase and continuity make $u\mapsto\tau_u$ continuous, with $A_{\tau_u}=u$ and $\tau_{A_t}=t$. Thus $W_u=M_{\tau_u}$ is continuous and [adapted](../../../stochastic-process.md#adapted-process) to $\mathcal G_u=\mathcal F_{\tau_u}$, with $W_0=0$.

The essential remaining point is independence of increments, which does not follow merely from the [Gaussian](../../../probability-theory.md#normal-distribution) marginal in part (a). Fix $0\le u<v$ and $\lambda\in\mathbb R$. The complex exponential

$$
\exp\left(i\lambda M_{t\wedge\tau_v}
+\frac{\lambda^2}{2}A_{t\wedge\tau_v}\right)
$$

is bounded by $e^{\lambda^2v/2}$ in modulus, hence is a [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) [martingale](../../../martingale.md). The [optional sampling theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at the finite, possibly unbounded, times $\tau_u\le\tau_v$ gives

$$
\mathbb E\left[e^{i\lambda M_{\tau_v}+\lambda^2v/2}\mid\mathcal F_{\tau_u}\right]
=e^{i\lambda M_{\tau_u}+\lambda^2u/2}.
$$

Divide by the nonzero right-hand exponential. Then

$$
\boxed{\mathbb E[e^{i\lambda(W_v-W_u)}\mid\mathcal G_u]
=e^{-\lambda^2(v-u)/2}.}
$$

This deterministic [conditional characteristic function](../../../probability-theory.md#conditional-characteristic-function) says that $W_v-W_u$ is $N(0,v-u)$ and independent of $\mathcal G_u$. Successively conditioning proves independence of every finite family of increments. Together with continuity and the zero initial value, this proves that $W$ is [Brownian motion](../../../brownian-motion.md). The inverse-clock identity gives $W_{A_t}=M_{\tau_{A_t}}=M_t$, completing the requested special-case proof of the [Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem).

## 3

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Because $W$ is continuous and [adapted](../../../stochastic-process.md#adapted-process), the Borel function $\operatorname{sgn}(W)$ is [predictable](../../../martingale.md#predictable-process). Its value at zero is $-1$, so its square is exactly one everywhere. Consequently $A$ is a zero-starting [continuous local martingale](../../../martingale.md#continuous-local-martingale) with

$$
[A]_t=\int_0^t\operatorname{sgn}(W_s)^2ds=t.
$$

The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) therefore makes $A$ a [Brownian motion](../../../brownian-motion.md) in the same [filtration](../../../stochastic-process.md#filtration-probability-theory). Here that characterization is the deterministic-clock case of the conditional-exponential argument in question 2.

Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $V=W^2$:

$$
dV_t=2W_t\,dW_t+dt.
$$

Since $\sqrt{V_t}=|W_t|$ and $|W_t|\operatorname{sgn}(W_t)=W_t$, including at zero, substitution yields

$$
\boxed{dV_t=2\sqrt{V_t}\,dA_t+dt.}
$$

Thus $W^2$ is a [squared Bessel process](../../../brownian-motion.md#squared-bessel-process) of dimension one.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the common [filtration](../../../stochastic-process.md#filtration-probability-theory) in which the two driving processes are independent [Brownian motions](../../../brownian-motion.md) and the solutions are [adapted](../../../stochastic-process.md#adapted-process). Let $Z=X+Y$, and define [predictable](../../../martingale.md#predictable-process) bounded weights

$$
h_1=\mathbf1_{\{Z>0\}}\sqrt{X/Z}+\mathbf1_{\{Z=0\}},\qquad
h_2=\mathbf1_{\{Z>0\}}\sqrt{Y/Z},
$$

with the ratios defined only on $\{Z>0\}$. The nonnegative solutions have $X=Y=0$ when $Z=0$. Set

$$
B_t=\int_0^t h_1(s)dB_s^{(1)}+\int_0^t h_2(s)dB_s^{(2)}.
$$

Independent Brownian drivers have zero cross-variation. Since $h_1^2+h_2^2=1$ even on the zero set, $[B]_t=t$, and the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) makes $B$ a [Brownian motion](../../../brownian-motion.md). Moreover $\sqrt Z h_1=\sqrt X$ and $\sqrt Z h_2=\sqrt Y$ everywhere. Adding the two original equations therefore proves [additivity of independently driven squared Bessel processes](../../../brownian-motion.md#additivity-of-independently-driven-squared-bessel-processes):

$$
\boxed{dZ_t=2\sqrt{Z_t}\,dB_t+(\alpha+\beta)dt,\qquad \gamma=\alpha+\beta.}
$$

The unit-vector fill on $\{Z=0\}$ is essential: simply dividing by $\sqrt Z$ there would leave the Brownian construction undefined.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Localize to compact subintervals of $(0,\infty)$, so that the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) can be applied to $f(z)=\sqrt z$. Its derivatives are $f'(z)=1/(2\sqrt z)$ and $f''(z)=-1/(4z^{3/2})$, while $d[Z]_t=4Z_tdt$. Thus, before $\zeta$,

$$
\begin{aligned}
dR_t&=\frac1{2R_t}(2R_t\,dB_t+\gamma dt)
-\frac1{8R_t^3}(4R_t^2dt)\\
&=dB_t+\frac{\gamma-1}{2R_t}dt.
\end{aligned}
$$

Hence the [Bessel process](../../../brownian-motion.md#bessel-process) equation is

$$
\boxed{dR_t=dB_t+\frac{\gamma-1}{2R_t}dt,\qquad R_0=r,\quad t<\zeta.}
$$

The inverse-power drift is interpreted only while $R>0$; its boundary behaviour is justified next, not assumed in this calculation.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

[Uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law) means that, for a fixed initial value, every two [weak stochastic solutions](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) of the [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) have the same distribution as entire solution paths, even if their filtered probability spaces and driving [Brownian motions](../../../brownian-motion.md) differ. For an equation on $(0,\infty)$, initially consider the stopped path and lifetime at the boundary.

We first justify that the boundary cannot intervene when $\gamma\ge2$. For any solution of the displayed Bessel equation, let $\tau_{\varepsilon,L}$ be its first exit from $(\varepsilon,L)$, where $0<\varepsilon<r<L$. Applying Itô to $R^2$ gives

$$
\mathbb E R_{t\wedge\tau_{\varepsilon,L}}^2
=r^2+\gamma\mathbb E(t\wedge\tau_{\varepsilon,L})\le L^2.
$$

Thus the annulus exit has finite expectation and is almost surely finite. The one-dimensional generator is $\frac12\partial_{rr}+\frac{\gamma-1}{2r}\partial_r$. Its harmonic scale functions are $\log r$ for $\gamma=2$ and $r^{2-\gamma}$ for $\gamma>2$, as direct differentiation verifies. They are bounded on the stopped annulus, so optional sampling gives

$$
\mathbb P_r(\tau_\varepsilon<\tau_L)=
\begin{cases}
\dfrac{\log(L/r)}{\log(L/\varepsilon)},&\gamma=2,\\
\dfrac{r^{2-\gamma}-L^{2-\gamma}}{\varepsilon^{2-\gamma}-L^{2-\gamma}},&\gamma>2.
\end{cases}
$$

Both tend to zero as $\varepsilon\downarrow0$. A continuous path hitting zero before $\tau_L$ would hit every inner level first, so that event has probability zero. Exhausting the upper levels proves that zero is not hit at any finite time. Nor can an upper explosion occur: localization of $R^2$ gives $\mathbb P(\tau_L\le t)\le(r^2+\gamma t)/L^2\to0$. These are the [Hitting-zero classification for a Bessel process](../../../brownian-motion.md#hitting-zero-classification-for-a-bessel-process) arguments needed for the dimension-at-least-two case.

Now suppose $\gamma$ is an integer and take a $\gamma$-dimensional [Brownian motion](../../../brownian-motion.md) $U$ from any deterministic vector $u$ with $|u|=r$. For $\rho=|U|>0$, differentiation of the [Euclidean norm](../../../functional-analysis.md#euclidean-norm) gives

$$
\partial_i|u|=u_i/|u|,\qquad \Delta|u|=(\gamma-1)/|u|.
$$

Define the radial noise $\beta=\sum_i\int U_i/\rho\,dW_i$, filling the integrand by a fixed unit vector on the zero set, as in part (b). It has bracket $t$ and is a [Brownian motion](../../../brownian-motion.md). the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma), initially before a possible zero, gives

$$
d\rho_t=d\beta_t+\frac{\gamma-1}{2\rho_t}dt,\qquad \rho_0=r.
$$

The boundary argument just given makes this a global positive [weak stochastic solution](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation). The assumed [uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law) therefore identifies every solution's path law with that of $|U|$. Orthogonal invariance of [Brownian motion](../../../brownian-motion.md) makes this radial law independent of the selected point $u$ on the sphere. Consequently

$$
\boxed{(R_t)_{t\ge0}\ \stackrel{\mathrm{law}}=\ (|u+W_t|)_{t\ge0},\quad |u|=r.}
$$

This proves equality of process laws, not merely equality of one-time marginal distributions.

## 4

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $X,Y$ be two solutions with the same Brownian driver and the same initial value. Write $D=X-Y$, and take a common [Lipschitz](../../../real-analysis.md#lipschitz-continuity) constant $L$ for both coefficients. Stop when $|X|+|Y|$ reaches $n$. Before this [stopping time](../../../martingale.md#stopping-time) $\tau_n$, all difference integrands below are bounded. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
d(D^2)=2D[\sigma(X)-\sigma(Y)]\,dB
+\left([\sigma(X)-\sigma(Y)]^2+2D[b(X)-b(Y)]\right)dt.
$$

The stopped [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is a true [martingale](../../../martingale.md) on every finite horizon. [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) therefore yields

$$
\mathbb E D_{t\wedge\tau_n}^2
\le(L^2+2L)\int_0^t\mathbb E[\mathbf1_{\{s<\tau_n\}}D_s^2]ds
\le(L^2+2L)\int_0^t\mathbb E D_{s\wedge\tau_n}^2ds.
$$

Since $D_0=0$, the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) makes the left side zero. Let $n\to\infty$; the continuous global solutions are bounded on each compact time interval, so their [stopping times](../../../martingale.md#stopping-time) exhaust it. Equality first at every rational time and then by continuity gives indistinguishability. This proves **[pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) for globally [Lipschitz](../../../real-analysis.md#lipschitz-continuity) drift and diffusion coefficients**. The argument does not require the initial value to have a global second moment: after stopping, the difference is bounded and initially zero.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) with a deterministic [integrating factor](../../../differential-equation.md#integrating-factor) gives

$$
d(e^{-t}X_t)=e^{-t}dX_t-e^{-t}X_tdt=e^{-t}dB_t.
$$

Integrating from zero proves

$$
\boxed{X_t=e^t\int_0^t e^{-s}dB_s.}
$$

Both coefficients are globally [Lipschitz](../../../real-analysis.md#lipschitz-continuity), so part (a) proves that this is the pathwise unique solution. Under a measure where $B$ is a [Brownian motion](../../../brownian-motion.md), the solution is centered [Gaussian](../../../probability-theory.md#normal-distribution) with variance $e^{2t}\int_0^te^{-2s}ds=(e^{2t}-1)/2$. The positive drift sign gives an unstable linear diffusion rather than a mean-reverting one.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use $\widetilde{\mathbb P}$ for the reference measure under which $X$ is a [Brownian motion](../../../brownian-motion.md). Pathwise, $B_t=X_t-\int_0^tX_sds$. Put $h_s=X_s\mathbf1_{\{s\le T\}}$ and define

$$
Z_t=\exp\left(\int_0^{t\wedge T}X_s\,dX_s-\frac12\int_0^{t\wedge T}X_s^2ds\right).
$$

The stopped integrand has absolute value at most one. The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds on every finite horizon, so $Z$ is a density [martingale](../../../martingale.md). The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) also gives the more useful identity

$$
\boxed{Z_t=\exp\left(\frac12X_{t\wedge T}^2-\frac12(t\wedge T)
-\frac12\int_0^{t\wedge T}X_s^2ds\right)\le e^{1/2}.}
$$

Thus $Z$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) over the entire time axis, not just a true [martingale](../../../martingale.md) on each finite horizon. Under the reference measure, $\widetilde{\mathbb E}(t\wedge T)=\widetilde{\mathbb E}X_{t\wedge T}^2\le1$, so $T<\infty$ almost surely. Hence $Z_t\to Z_T>0$ and $\widetilde{\mathbb E}Z_T=1$.

Define the [probability measure](../../../probability-theory.md#probability-measure) on the original [sigma-algebra](../../../measure-theory.md#sigma-algebra) by

$$
\boxed{\frac{d\mathbb P}{d\widetilde{\mathbb P}}=Z_T.}
$$

Its restriction to $\mathcal F_t$ has density $Z_t$. The [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) states that subtracting the integrated density integrand from the reference [Brownian motion](../../../brownian-motion.md) gives a [Brownian motion](../../../brownian-motion.md) under the new measure. Therefore

$$
W_t^{\mathbb P}=X_t-\int_0^{t\wedge T}X_sds
$$

is a [Brownian motion](../../../brownian-motion.md) under $\mathbb P$, and $B_{t\wedge T}=W^{\mathbb P}_{t\wedge T}$. This is exactly the requested Brownian property until $T$. The [bounded Girsanov density for exit of an unstable linear diffusion](../../../stochastic-calculus.md#bounded-girsanov-density-for-exit-of-an-unstable-linear-diffusion) also proves global absolute continuity, so a mere collection of unspecified finite-horizon measures is unnecessary.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

At exit, continuity gives $X_T^2=1$. The preceding density identity becomes

$$
Z_T=\exp\left(\frac12-\frac T2-\frac12\int_0^T X_s^2ds\right).
$$

Since $|X_s|\le1$ before exit, $\int_0^TX_s^2ds\le T$. On $\{T\le t\}$ it follows that $Z_T\ge e^{1/2-T}\ge e^{1/2-t}$. The definition of the changed measure now yields

$$
\boxed{\mathbb P(T\le t)
=\widetilde{\mathbb E}[Z_T\mathbf1_{\{T\le t\}}]
\ge e^{1/2-t}\widetilde{\mathbb P}(T\le t).}
$$

The positive sign of the [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) in the density is what introduces the positive drift $X_tdt$; reversing that sign would give a different measure and would not prove this inequality.

## 5

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use one $d$-dimensional [Brownian motion](../../../brownian-motion.md) $W$ to couple the [diffusion processes](../../../stochastic-calculus.md#markov-diffusion)

$$
X_t^\varepsilon=x_0+\int_0^t b(X_s^\varepsilon)ds+\varepsilon W_t.
$$

The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients) supplies a unique nonexplosive [strong stochastic solution](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation). Let $x$ be the deterministic drift trajectory. Subtraction and the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) give, on every finite horizon $t$,

$$
\boxed{\sup_{s\le t}|X_s^\varepsilon-x_s|
\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|\longrightarrow0\quad\text{almost surely}.}
$$

This also follows directly from the integral equations with continuous forcing, so the coupling can be chosen simultaneously for all $\varepsilon$.

For completeness derive the needed [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) with its potential sign. For fixed $t$, apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) to

$$
Y_s=\exp\left(\int_0^s c(X_v^\varepsilon)dv\right)
 u^\varepsilon(t-s,X_s^\varepsilon),\qquad 0\le s\le t.
$$

Its drift is the exponential factor times $-u_t^\varepsilon+(\varepsilon^2\Delta/2+b\cdot\nabla)u^\varepsilon+c u^\varepsilon$, which vanishes by the [partial differential equation](../../../partial-differential-equation.md). It is a [local martingale](../../../martingale.md#local-martingale). Boundedness of $u^\varepsilon$ on the finite time slab and boundedness of $c$ make $Y$ bounded there, so it is a true [martingale](../../../martingale.md). Its endpoint expectations give

$$
u^\varepsilon(t,x_0)=\mathbb E\left[f(X_t^\varepsilon)
\exp\left(\int_0^t c(X_s^\varepsilon)ds\right)\right].
$$

The deterministic trajectory on $[0,t]$ is compact. Uniform pathwise convergence puts all sufficiently small-noise paths in a fixed compact neighbourhood of that trajectory. Continuity of $c$ therefore implies $\sup_{s\le t}|c(X_s^\varepsilon)-c(x_s)|\to0$; global [uniform continuity](../../../topological-analysis.md#uniform-continuity) of $c$ is not required. Continuity of $f$ gives convergence of the terminal factor. Finally,

$$
\left|f(X_t^\varepsilon)\exp\left(\int_0^tc(X_s^\varepsilon)ds\right)\right|
\le\|f\|_\infty e^{t\|c\|_\infty}.
$$

The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) proves the [zero-noise limit with a bounded potential](../../../stochastic-calculus.md#zero-noise-limit-with-a-bounded-potential):

$$
\boxed{u^\varepsilon(t,x_0)\longrightarrow
f(x_t)\exp\left(\int_0^t c(x_s)ds\right).}
$$

At $t=0$ this is the given initial condition. All boundedness arguments concern a fixed finite horizon; no uniform bound over infinite time is needed.

## 6

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [Markov jump process](../../../markov-process.md#markov-jump-process), considered up to its explosion time, is an [adapted](../../../stochastic-process.md#adapted-process) càdlàg piecewise-constant process whose conditional future law given $\mathcal F_t$ depends only on its current state. Describe its rates by an off-diagonal kernel $q(x,dy)$ with finite total rate $q(x,E)$. In state $x$ the [holding time](../../../markov-process.md#holding-time) has the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with this rate, followed by a destination distributed as $q(x,dy)/q(x,E)$; a zero-rate state is absorbing. Its [Markov jump-process generator](../../../markov-process.md#markov-jump-process-generator) acts by

$$
Qf(x)=\int_E[f(y)-f(x)]q(x,dy).
$$

The [Markov property](../../../markov-process.md#markov-property) must hold relative to the specified [filtration](../../../stochastic-process.md#filtration-probability-theory), not merely the natural [filtration](../../../stochastic-process.md#filtration-probability-theory): future-revealing information could change the jump compensator.

Let $\mu$ count jumps, marked by their destination states. For this [jump measure of a Markov jump process](../../../markov-process.md#jump-measure-of-a-markov-jump-process), the [predictable](../../../martingale.md#predictable-process) compensator is

$$
\nu(ds,dy)=q(X_{s-},dy)ds.
$$

The compensated random-measure theorem says that a [predictable](../../../martingale.md#predictable-process) $H(s,y)$ with $\mathbb E\int_0^t\int|H|d\nu<\infty$ gives a true [martingale](../../../martingale.md)

$$
(H*(\mu-\nu))_t=\int_{(0,t]\times E}H(s,y)(\mu-\nu)(ds,dy).
$$

The same statement holds locally when that expected integrability is obtained after localization. The compensator identity applied to $\mathbf1_A\mathbf1_{(s,t]}H$, for $A\in\mathcal F_s$, shows that each increment has zero [conditional expectation](../../../measure-theory.md#conditional-expectation). Taking $H(s,y)=f(y)-f(X_{s-})$ gives the generator [local martingale](../../../martingale.md#local-martingale) $f(X_t)-f(X_0)-\int_0^t Qf(X_s)ds$. This states the integrability conditions in the [compensated jump-measure local martingale](../../../markov-process.md#compensated-jump-measure-local-martingale) result explicitly.

For the birth-process claim first take the customary fixed initial state $X_0=i$. Write $N_t=X_t-i$, $\Lambda_t=\int_0^t\lambda(X_s)ds$ and $a=e^\theta-1$. The compensator of $N$ is $\Lambda$, whose integrand may equivalently use $X_{s-}$ because jump times have zero Lebesgue measure. A birth multiplies $e^{\theta X}$ by $e^\theta$, so the jump product rule gives

$$
\boxed{dM_t=aM_{t-}\bigl(dN_t-\lambda(X_{t-})dt\bigr),\qquad M_0=e^{\theta i}.}
$$

For an explicit localization, stop at $\tau_n=\inf\{t:X_t\ge n\}\wedge n$ with $n>i$. Up to that time the statewise rates are bounded by the maximum of the finitely many rates below $n$, the jump count is bounded, and $M$ and its compensated-integral integrand are bounded on the finite stopped horizon. The compensated-measure theorem therefore makes each stopped process a true [martingale](../../../martingale.md). The times increase to the explosion lifetime (or infinity if there is no explosion), proving **$M$ is a [local martingale](../../../martingale.md#local-martingale) on $[0,\zeta)$ for every real $\theta$**.

Now suppose $\lambda(j)\le C$ uniformly. For $C>0$, propose candidate births at the times of a rate-$C$ [Poisson process](../../../probability-theory.md#poisson-process), accepting each with probability $\lambda(X_{s-})/C$ using fresh independent uniform marks. While the state is fixed, [Poisson thinning](../../../probability-theory.md#poisson-thinning) gives a [holding time](../../../markov-process.md#holding-time) with the required [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\lambda$; accepted births have exactly the prescribed law. Thus there can be no explosion, and the true birth count $N_T$ is stochastically dominated by a [Poisson random variable](../../../discrete-probability-distribution.md#poisson-distribution) of mean $CT$. In particular,

$$
\mathbb E e^{bN_T}\le\exp\{CT(e^b-1)\}<\infty\qquad(b\ge0).
$$

The case $C=0$ is constant and immediate. For every fixed horizon $T$ and all $s\le T$, including localization times,

$$
0\le M_{s\wedge\tau_n}
\le\exp\{\theta i+\theta_+N_T+(1-e^\theta)_+CT\}.
$$

This is one integrable dominating variable for the entire stopped family. Conditional [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) removes the localization and proves

$$
\boxed{\mathbb E[M_t\mid\mathcal F_s]=M_s\quad(s\le t),}
$$

so the [exponential martingale of a pure birth process](../../../markov-process.md#exponential-martingale-of-a-pure-birth-process) is a genuine [martingale](../../../martingale.md) for uniformly bounded rates. Only [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) on each finite horizon is asserted; it need not be [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) over infinite time.

For a random initial state, the same proof requires $\mathbb E e^{\theta X_0}<\infty$. The source does not explicitly specify the initial distribution, so that qualification cannot be dropped: take constant rate one and an independent initial law $\mathbb P(X_0=n)=6/(\pi^2n^2)$. For $\theta>0$, already $\mathbb EM_0=\infty$, precluding even the integrability in the definition of a [martingale](../../../martingale.md). The fixed-initial-state interpretation above supplies the intended complete proof; bounded rates alone do not remedy an arbitrary heavy-tailed initial law.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
