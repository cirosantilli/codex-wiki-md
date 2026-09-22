# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper36.pdf)

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
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take a complete, right-continuous [filtration](../../../stochastic-process.md#filtration-probability-theory) $(\mathcal F_t)$, an increasing family of sigma-algebras. Adapted means that $X_t$ is $\mathcal F_t$-measurable at each $t$; [càdlàg](../../../calculus.md#cadlag) means right-continuous with left limits. A [local martingale](../../../martingale.md#local-martingale) is an adapted [càdlàg](../../../calculus.md#cadlag) process $X$, with integrable initial value, for which there are [stopping times](../../../martingale.md#stopping-time) $\tau_n\uparrow\infty$ almost surely such that each [stopped process](../../../martingale.md#stopped-process) $X^{\tau_n}_t=X_{t\wedge\tau_n}$ is a true [martingale](../../../martingale.md). Such a sequence is a localizing sequence. A true [martingale](../../../martingale.md) is integrable at each time and satisfies $\mathbb E(X_t\mid\mathcal F_s)=X_s$ for $s\le t$.

The necessary and sufficient condition is that $X$ is a [Class DL process](../../../convergence-of-random-variables.md#class-dl-process):

$$
\boxed{X\text{ is a martingale}\ \Longleftrightarrow\ \{X_\tau:\tau\le T\text{ a stopping time}\}\text{ is uniformly integrable for every finite }T.}
$$

A family $\mathcal Z$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) if its members are integrable and $\sup_{Z\in\mathcal Z}\mathbb E(|Z|\mathbf1_{\{|Z|>K\}})\to0$ as $K\to\infty$. A [stopping time](../../../martingale.md#stopping-time) $\tau$ satisfies $\{\tau\le t\}\in\mathcal F_t$ for all $t$.

For necessity, on $[0,T]$ the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives $X_\tau=\mathbb E(X_T\mid\mathcal F_\tau)$; [conditional expectations](../../../measure-theory.md#conditional-expectation) of one integrable variable form a [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability) family. For sufficiency, $X_{t\wedge\tau_n}\to X_t$ almost surely, and [Class DL](../../../convergence-of-random-variables.md#class-dl-process) upgrades this convergence to $L^1$ on each finite horizon. Pass to the limit in $\mathbb E(X_{t\wedge\tau_n}\mid\mathcal F_s)=X_{s\wedge\tau_n}$ to obtain the [martingale](../../../martingale.md) identity. Requiring [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) of all times on the entire half-line would be stronger than necessary; [Brownian motion](../../../brownian-motion.md) is already a counterexample to that stronger requirement.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Lévy characterization of multidimensional Brownian motion](../../../brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion) says that a continuous adapted $\mathbb R^d$-valued process $Z$, with $Z_0=0$, is standard [Brownian motion](../../../brownian-motion.md) relative to the given [filtration](../../../stochastic-process.md#filtration-probability-theory) if and only if its coordinates are [local martingales](../../../martingale.md#local-martingale) and

$$
\boxed{[Z^i,Z^j]_t=\delta_{ij}t\qquad(1\le i,j\le d).}
$$

For [Brownian motion](../../../brownian-motion.md), independent centered Gaussian increments give the [martingale](../../../martingale.md) property of each coordinate and of $Z_t^iZ_t^j-\delta_{ij}t$. The defining uniqueness of [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) consequently gives the bracket condition.

Conversely, suppose the [local martingale](../../../martingale.md#local-martingale) and bracket conditions hold. For $\theta\in\mathbb R^d$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
E_t=\exp\left(i\theta\cdot Z_t+\tfrac12|\theta|^2t\right),\qquad dE_t=iE_t\,\theta\cdot dZ_t,
$$

since the bracket term cancels the time derivative. On $[0,T]$, $|E_t|\le e^{|\theta|^2T/2}$, so its real and imaginary parts are bounded [local martingales](../../../martingale.md#local-martingale) and hence true [martingales](../../../martingale.md). Thus, for $s\le t$,

$$
\mathbb E\left[e^{i\theta\cdot(Z_t-Z_s)}\mid\mathcal F_s\right]=e^{-\frac12|\theta|^2(t-s)}.
$$

This is the [characteristic function](../../../probability-theory.md#characteristic-function) of $N(0,(t-s)I_d)$ and is independent of $\mathcal F_s$. Uniqueness of [characteristic functions](../../../probability-theory.md#characteristic-function) shows that $Z_t-Z_s$ has that [Gaussian distribution](../../../probability-theory.md#normal-distribution) and is independent of the past. Iterating over ordered times gives independent Gaussian increments; together with continuous paths and $Z_0=0$, these are precisely the defining properties of standard [Brownian motion](../../../brownian-motion.md).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

First justify that the logarithm is defined at all times from one onward. For planar [Brownian motion](../../../brownian-motion.md) started at $z\ne0$, stop on exiting the annulus $\varepsilon<|x|<R$, where $\varepsilon<|z|<R$. This exit time $\rho$ is finite almost surely: the stopped identity $|B_t|^2-2t$ gives $\mathbb E(t\wedge\rho)\le R^2/2$. The function $f(x)=\log|x|$ is harmonic on the annulus, so its [stopped process](../../../martingale.md#stopped-process) is a bounded [martingale](../../../martingale.md). Optional stopping gives

$$
\mathbb P_z(\text{hit }\varepsilon\text{ before }R)=\frac{\log R-\log|z|}{\log R-\log\varepsilon}\longrightarrow0.
$$

Hitting zero before the outer circle would require hitting every inner circle first. It therefore has probability zero. Taking a countable sequence of outer radii tending to infinity proves that [planar Brownian motion avoids a fixed point](../../../brownian-motion.md#planar-brownian-motion-avoids-a-fixed-point). Since $B_1$ has a density and is nonzero almost surely, condition on $\mathcal F_1$ to apply this result to the future path.

For $x\ne0$, $\nabla f(x)=x/|x|^2$ and $\Delta f(x)=0$ in two dimensions. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) on annuli therefore gives

$$
\boxed{X_t=X_1+\int_1^t\frac{B_s}{|B_s|^2}\cdot dB_s\qquad(t\ge1).}
$$

To localize explicitly, let $\tau_n=\inf\{t\ge1:|B_t|\notin(1/n,n)\}$. These [stopping times](../../../martingale.md#stopping-time) increase to infinity almost surely: on each compact time interval the continuous path has a finite maximum and, by point avoidance, a positive minimum radius. Up to $\tau_n$, the stochastic integrand has norm at most $n$. Its stopped integral is square-integrable on every finite horizon. The initial value $\log|B_1|$ is integrable, as follows from the Rayleigh-density calculation in part d. Hence $X^{\tau_n}$ is a true [martingale](../../../martingale.md) from time one and **$X$ is a [local martingale](../../../martingale.md#local-martingale)**. This also gives its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) from time one as $\int_1^t|B_s|^{-2}\,ds$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

[Brownian scaling](../../../brownian-motion.md#brownian-scaling) gives $|B_t|\overset{d}=\sqrt t\,R$, where $R=|B_1|$ has [Rayleigh distribution](../../../continuous-probability-distribution.md#rayleigh-distribution) with density $r e^{-r^2/2}$, $r>0$. For every $p>0$,

$$
\mathbb E|\log R|^p=\int_0^\infty|\log r|^p r e^{-r^2/2}\,dr<\infty.
$$

Near zero this is bounded by $\int_0^1|\log r|^p r\,dr=\int_0^\infty u^pe^{-2u}\,du$, which is finite; near infinity the Gaussian tail dominates any logarithmic power. The inequality $|a+b|^p\le C_p(|a|^p+|b|^p)$, valid also for $0<p<1$, now yields

$$
\boxed{\mathbb E|X_t|^p<\infty\qquad(t\ge1,\ p>0).}
$$

Let $c=\mathbb E\log R$, a finite constant. The same scaling identity gives

$$
\boxed{\mathbb E X_t=\tfrac12\log t+c\longrightarrow\infty.}
$$

An integrable [martingale](../../../martingale.md) has constant expectation, so the [logarithm of planar Brownian radius](../../../martingale.md#logarithm-of-planar-brownian-radius) is a [strict local martingale](../../../martingale.md#strict-local-martingale) on $[1,\infty)$. Fixed-time integrability, even of every positive power, does not imply the stopping-time [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) required in part a.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [previsible sigma-algebra](../../../martingale.md#predictable-sigma-algebra) $\mathcal P$ on $\Omega\times[0,\infty)$ is generated by left-continuous adapted processes. Equivalently it is generated by $A\times\{0\}$ with $A\in\mathcal F_0$ and $A\times(s,t]$ with $A\in\mathcal F_s$, $0\le s<t$. A [previsible process](../../../martingale.md#predictable-process) is a process measurable for this sigma-algebra; [predictable](../../../martingale.md#predictable-process) is a synonym.

Use the zero-starting convention for $\mathcal M_c^2$: continuous [martingales](../../../martingale.md) with $M_0=0$ and $\sup_t\mathbb E M_t^2<\infty$. For such an [L2-bounded continuous martingale](../../../martingale.md#l2-bounded-continuous-martingale), the [square-integrable stochastic integrand](../../../stochastic-calculus.md#square-integrable-stochastic-integrand) space is

$$
\boxed{L^2(M)=\left\{H\text{ previsible}:\ \|H\|_{L^2(M)}^2=\mathbb E\int_0^\infty H_s^2\,d[M]_s<\infty\right\}.}
$$

Identify processes that agree almost everywhere for the [quadratic-variation measure](../../../stochastic-calculus.md#quadratic-variation-measure) $\nu_M(d\omega,ds)=\mathbb P(d\omega)\,d[M]_s$. This makes the displayed norm an actual Hilbert-space norm on equivalence classes. On a fixed horizon $[0,T]$, replace infinity by $T$; this is the same construction for continuous [martingales](../../../martingale.md) square-integrable on that horizon. Nonzero initial values may be subtracted because the integral depends only on increments.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For an elementary [previsible process](../../../martingale.md#predictable-process) $H=\sum_{j=0}^{r-1}H_j\mathbf1_{(t_j,t_{j+1}]}$, with bounded $\mathcal F_{t_j}$-measurable coefficients, define

$$
(H\cdot M)_t=\sum_j H_j\big(M_{t\wedge t_{j+1}}-M_{t\wedge t_j}\big).
$$

The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) is

$$
\boxed{\mathbb E\big[(H\cdot M)_t^2\big]=\mathbb E\int_0^t H_s^2\,d[M]_s.}
$$

More generally the squared $L^2$ distance between the integrals of $H$ and $K$ is the integral of $(H-K)^2$ on the right. The integral is a zero-starting continuous square-integrable [martingale](../../../martingale.md).

Elementary [predictable processes](../../../martingale.md#predictable-process) are dense in $L^2(M)$. Given $H$ in this space, choose elementary $H_n$ converging in its norm and define the [Itô integral](../../../stochastic-calculus.md#ito-integral) by the $L^2$ limit of $H_n\cdot M$. The isometry proves that this is independent of the approximating sequence and remains valid for the limit. The [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) bounds the expected squared path supremum of the difference by four times its terminal second moment; hence the convergence also gives a continuous [martingale](../../../martingale.md) version, with [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability).

For a [continuous local martingale](../../../martingale.md#continuous-local-martingale) $M$ and [locally bounded process](../../../stochastic-process.md#locally-bounded-process) $H$ that is [previsible](../../../martingale.md#predictable-process), choose increasing [stopping times](../../../martingale.md#stopping-time) $\tau_n\uparrow\infty$ such that $M^{\tau_n}$ is L2-bounded, $|H|\le K_n$ up to $\tau_n$, and $\tau_n\le n$. This can be done by combining localizers with first exits of $M$ from bounded intervals and the local bounds of $H$. Then $H\mathbf1_{[0,\tau_n]}$ is in the integrand space for $M^{\tau_n}$. Define the integral on each stopped interval by the preceding construction. The stopping property of elementary integrals, extended by the isometry, makes these definitions agree on overlaps. Pasting gives

$$
\boxed{H\cdot M\text{ as a continuous local martingale, defined consistently on all }[0,\tau_n].}
$$

This is a localization construction; global square integrability of the resulting process is not asserted.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For every zero-starting [continuous local martingale](../../../martingale.md#continuous-local-martingale) $M$, there is a unique, up to indistinguishability, continuous adapted increasing process $[M]$, with $[M]_0=0$, such that

$$
\boxed{M_t^2-[M]_t\text{ is a local martingale}.}
$$

This is its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation). It also satisfies, for deterministic partitions whose mesh tends to zero,

$$
[M]_t=\lim\sum_j\big(M_{t_{j+1}\wedge t}-M_{t_j\wedge t}\big)^2,
$$

with convergence uniformly on compact time intervals in probability. The theorem includes existence and finiteness on each compact interval; monotonicity is understood pathwise outside one null set.

Uniqueness follows because the difference of two candidate increasing continuous processes is both a [finite-variation process](../../../stochastic-calculus.md#finite-variation-process) and a [continuous local martingale](../../../martingale.md#continuous-local-martingale), hence is identically zero from its zero initial value. For a [continuous semimartingale](../../../stochastic-calculus.md#continuous-semimartingale) $X=X_0+M+A$, its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) is $[X]=[M]$, since continuous finite-variation terms have zero [quadratic variation](../../../stochastic-calculus.md#quadratic-variation). Polarization defines the [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) by $[M,N]=([M+N]-[M-N])/4$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The correct [quadratic variation of a stochastic integral](../../../stochastic-calculus.md#quadratic-variation-of-a-stochastic-integral) identity is

$$
\boxed{[H\cdot M]_t=\int_0^t H_s^2\,d[M]_s=(H^2\cdot[M])_t.}
$$

The brackets around the final integrator are missing in the PDF. Without them the assertion is false: for $H=1$ and $M$ [Brownian motion](../../../brownian-motion.md), the left side is $t$ while the printed right side is $B_t$.

For elementary [predictable](../../../martingale.md#predictable-process) $H$, the integral is obtained by scaling each [martingale](../../../martingale.md) increment by its known coefficient. [Quadratic variation](../../../stochastic-calculus.md#quadratic-variation) on each interval is therefore scaled by the square of that coefficient, giving the displayed formula. To pass to a general $L^2(M)$ integrand on $[0,T]$, take elementary $H_n\to H$ in the integrand norm and put $N_n=H_n\cdot M$, $N=H\cdot M$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives $\mathbb E(N_n-N)_T^2\to0$, hence $\mathbb E[N_n-N]_T\to0$. The bracket Cauchy-Schwarz bound

$$
|[N,N_n-N]_t|\le[N]_T^{1/2}[N_n-N]_T^{1/2}\qquad(t\le T)
$$

and polarization show that $[N_n]\to[N]$ uniformly in probability. On the other side, Cauchy-Schwarz for the [quadratic-variation measure](../../../stochastic-calculus.md#quadratic-variation-measure) gives

$$
\mathbb E\int_0^T|H_n^2-H^2|\,d[M]\le\|H_n-H\|_{L^2(M;T)}\big(\|H_n\|_{L^2(M;T)}+\|H\|_{L^2(M;T)}\big)\longrightarrow0.
$$

Taking limits proves the formula in the square-integrable case. Stopping and pasting as in part b proves it for locally bounded [predictable](../../../martingale.md#predictable-process) integrands and [continuous local martingales](../../../martingale.md#continuous-local-martingale).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For an elementary [previsible](../../../martingale.md#predictable-process) integrand, the integral is the increment sum $\sum_jH_j(X_{t\wedge t_{j+1}}-X_{t\wedge t_j})$. This expression uses only $H$ and $X$, so is identical under the two measures, irrespective of how the [local martingale](../../../martingale.md#local-martingale) and finite-variation parts change.

We may use the [stochastic dominated convergence theorem](../../../stochastic-calculus.md#stochastic-dominated-convergence-theorem): if bounded [predictable](../../../martingale.md#predictable-process) $H_n$ converge pointwise to $H$ under a common deterministic bound, their integrals against a [semimartingale](../../../stochastic-calculus.md#semimartingale) converge uniformly on compact intervals in probability. Also convergence in $\mathbb P$-probability implies convergence in $\mathbb Q$-probability when $\mathbb Q\ll\mathbb P$. To see the latter directly, let $D=d\mathbb Q/d\mathbb P$. For any event $E$,

$$
\mathbb Q(E)=\mathbb E_{\mathbb P}(D\mathbf1_E)\le K\mathbb P(E)+\mathbb E_{\mathbb P}(D\mathbf1_{\{D>K\}}),
$$

and let first $\mathbb P(E)\to0$, then $K\to\infty$. Apply this to events involving the supremum on a finite horizon for the uniform-in-probability statement.

Let $\mathcal C$ be the bounded [predictable](../../../martingale.md#predictable-process) integrands for which the two integral processes agree up to $\mathbb Q$-indistinguishability. It is a vector space containing elementary rectangle indicators generating the [predictable](../../../martingale.md#predictable-process) sigma-algebra. It is closed under uniformly bounded pointwise limits: stochastic [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives convergence of the integrals under each measure, and the preceding transfer makes the $\mathbb P$ limit also a $\mathbb Q$ limit. Uniqueness of limits in probability makes the two limiting integrals equal. The [functional monotone-class theorem](../../../measure-theory.md#functional-monotone-class-theorem) therefore puts every bounded [predictable](../../../martingale.md#predictable-process) integrand in $\mathcal C$.

Finally, for locally bounded $H$, stop on intervals where it has a deterministic bound. Such [stopping times](../../../martingale.md#stopping-time) tend to infinity under $\mathbb P$ and hence also under $\mathbb Q$. Apply the bounded result to the stopped integrands and use the stopping property of the integral. This proves the [stochastic integral under an absolutely continuous measure change](../../../stochastic-calculus.md#stochastic-integral-under-an-absolutely-continuous-measure-change) identity

$$
\boxed{(H\cdot X)^{\mathbb P}=(H\cdot X)^{\mathbb Q}\quad\mathbb Q\text{-indistinguishably}.}
$$

The decompositions $H\cdot M+H\cdot A$ and $H\cdot N+H\cdot B$ thus represent the same process under $\mathbb Q$, although their individual components need not agree. With only absolute continuity, equality is asserted outside a $\mathbb Q$-null set, not necessarily outside a $\mathbb P$-null set for a chosen $\mathbb Q$ version.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For [càdlàg](../../../calculus.md#cadlag) [semimartingales](../../../stochastic-calculus.md#semimartingale), the [semimartingale integration by parts](../../../stochastic-calculus.md#semimartingale-integration-by-parts) formula is

$$
\boxed{X_tY_t=X_0Y_0+\int_0^tX_{s-}\,dY_s+\int_0^tY_{s-}\,dX_s+[X,Y]_t.}
$$

For continuous processes the left limits can be replaced by the values. The bracket includes the jump products in the general formula.

For a continuous $\mathbb R^d$-valued [semimartingale](../../../stochastic-calculus.md#semimartingale) $X$ and $f\in C^2(\mathbb R^d)$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) is

$$
\boxed{f(X_t)=f(X_0)+\sum_{i=1}^d\int_0^t\partial_if(X_s)\,dX_s^i+\frac12\sum_{i,j=1}^d\int_0^t\partial_{ij}f(X_s)\,d[X^i,X^j]_s.}
$$

The formula is localized when the derivatives are unbounded; continuity of $X$ makes them bounded after stopping on compact sets.

To prove the one-dimensional formula for polynomials without assuming that formula, use induction. It is immediate for constants and $X$. Suppose

$$
d(X^k)=kX^{k-1}\,dX+\frac{k(k-1)}2X^{k-2}\,d[X].
$$

Write $X=X_0+M+A$ with $M$ a [continuous local martingale](../../../martingale.md#continuous-local-martingale) and $A$ [finite variation](../../../real-analysis.md#total-variation-of-a-function). The induction hypothesis identifies the [martingale](../../../martingale.md) part of $X^k$ as $kX^{k-1}\cdot M$. The stochastic-integral covariation identity, obtained by polarization from the quadratic-variation identity, gives

$$
d[X^k,X]=kX^{k-1}\,d[X].
$$

Apply [semimartingale integration by parts](../../../stochastic-calculus.md#semimartingale-integration-by-parts) to $X^kX$. Its first-order terms combine to $(k+1)X^k\,dX$, and its bracket terms combine to

$$
\left(\frac{k(k-1)}2+k\right)X^{k-1}\,d[X]=\frac{k(k+1)}2X^{k-1}\,d[X].
$$

This proves the induction step. Taking linear combinations proves the [polynomial Itô formula from integration by parts](../../../stochastic-calculus.md#polynomial-ito-formula-from-integration-by-parts) for every polynomial $f$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Fix a finite horizon $T$ and define $\tau_n=\inf\{s\ge0:|B_s|\ge n\}$. These [stopping times](../../../martingale.md#stopping-time) increase to infinity almost surely because continuous paths are bounded on each finite interval. Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $B_{t\wedge\tau_n}^k$, for $k\ge2$, gives

$$
B_{t\wedge\tau_n}^k=k\int_0^t\mathbf1_{\{s\le\tau_n\}}B_s^{k-1}\,dB_s+\frac{k(k-1)}2\int_0^t\mathbf1_{\{s\le\tau_n\}}B_s^{k-2}\,ds.
$$

The first integrand is bounded by $kn^{k-1}$, so its integral is square-integrable and has expectation zero. Thus

$$
\mathbb EB_{t\wedge\tau_n}^k=\frac{k(k-1)}2\mathbb E\int_0^t\mathbf1_{\{s\le\tau_n\}}B_s^{k-2}\,ds.
$$

To justify both limits explicitly, let $S_T=\sup_{s\le T}|B_s|$ and choose an integer $q>\max\{k,1\}$. The Gaussian density gives $\mathbb E|B_T|^q<\infty$ by its exponential tail. The [Doob Lp maximal inequality](../../../martingale.md#doob-lp-maximal-inequality) states

$$
\mathbb ES_T^q\le\left(\frac q{q-1}\right)^q\mathbb E|B_T|^q<\infty.
$$

Therefore $S_T^k$ and $1+S_T^{k-2}$ are integrable. The stopped terminal powers converge almost surely to $B_t^k$ and are dominated in absolute value by $S_T^k$. The integrands in the time integral converge almost surely and are bounded by $1+S_T^{k-2}$, so their integrals are dominated by $T(1+S_T^{k-2})$. [Dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) on both sides, and then Fubini justified by the same bound, give the [Brownian moment recursion](../../../brownian-motion.md#brownian-moment-recursion)

$$
\boxed{\beta_k(t)=\frac{k(k-1)}2\int_0^t\beta_{k-2}(s)\,ds\qquad(k\ge2).}
$$

This uses only finiteness of Gaussian moments, not the closed moment formula requested in the next part.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The initial values are $\beta_0(t)=1$ and $\beta_1(t)=0$. Repeatedly applying the [Brownian moment recursion](../../../brownian-motion.md#brownian-moment-recursion) to odd indices reduces them to $\beta_1$, so every odd moment vanishes. For even indices, if the formula holds at $2k-2$, then

$$
\begin{aligned}
\beta_{2k}(t)&=k(2k-1)\int_0^t\frac{(2k-2)!s^{k-1}}{2^{k-1}(k-1)!}\,ds\\
&=\frac{(2k)!}{2^kk!}t^k.
\end{aligned}
$$

The base case $k=0$ is $\beta_0=1$. Thus

$$
\boxed{\beta_{2k+1}(t)=0,\qquad\beta_{2k}(t)=\frac{(2k)!t^k}{2^kk!}\qquad(k\ge0).}
$$

Equivalently the even moments are $(2k-1)!!\,t^k$, the familiar Gaussian moment formula with [variance](../../../variance.md) $t$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Interpret the otherwise undefined $b_k(t)$ here as the moment $\beta_k(t)$ defined above. For $k=1$, the process is $B_t$, and for $k=2$ it is $B_t^2-t$; both are [martingales](../../../martingale.md).

For $k\ge3$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) and the derivative of the [Brownian moment recursion](../../../brownian-motion.md#brownian-moment-recursion) yield

$$
d\big(B_t^k-\beta_k(t)\big)=kB_t^{k-1}\,dB_t+\frac{k(k-1)}2\big(B_t^{k-2}-\beta_{k-2}(t)\big)\,dt.
$$

The [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is a true [martingale](../../../martingale.md) on finite horizons, since the required $2k-2$ moment is integrable in time. The continuous finite-variation term is not identically zero. If it were, its continuous derivative would vanish at every time, whereas at a fixed $t>0$, the nondegenerate Gaussian $B_t$ does not almost surely satisfy the polynomial equation $B_t^{k-2}=\beta_{k-2}(t)$. Uniqueness of [continuous semimartingale](../../../stochastic-calculus.md#continuous-semimartingale) decomposition therefore rules out even the [local martingale](../../../martingale.md#local-martingale) property. Hence

$$
\boxed{B_t^k-\beta_k(t)\text{ is a martingale precisely for }k=1,2.}
$$

For example $\mathbb E(B_t^3\mid\mathcal F_s)=B_s^3+3(t-s)B_s$, so merely subtracting its zero expectation cannot make the cubic power a [martingale](../../../martingale.md). The [centered Brownian powers need not be martingales](../../../brownian-motion.md#centered-brownian-powers-need-not-be-martingales) distinction is resolved by subtracting the random drift compensator $k(k-1)\int_0^tB_s^{k-2}ds/2$ instead of the deterministic mean.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) consists of a choice of probability space, [filtration](../../../stochastic-process.md#filtration-probability-theory), driving [Brownian motion](../../../brownian-motion.md) and adapted solution with the specified initial law. The driving noise and the space are part of what may be chosen.

A [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) is constructed for a prescribed [Brownian motion](../../../brownian-motion.md) and initial value, as a nonanticipating measurable functional of that data; for deterministic initial value it is adapted to the usual augmentation of the Brownian [filtration](../../../stochastic-process.md#filtration-probability-theory). No further independent randomness is required.

[Uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law) means that any two [weak solutions of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) with the same initial distribution have the same law as solution processes. [Pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) means that two solutions on the same filtered space, driven by the same [Brownian motion](../../../brownian-motion.md) and with the same initial value almost surely, are [indistinguishable](../../../stochastic-process.md#indistinguishability-of-stochastic-processes): $\mathbb P(X_t=\widetilde X_t\text{ for every }t)=1$. The latter concerns equality of paths on a common space, whereas [uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law) concerns equality of probability distributions.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $S=\|\sigma\|_\infty$, $K=\|b\|_\infty$, and write $X_t-x_0=M_t+A_t$, where $M_t=\int_0^t\sigma(X_s)\,dB_s$ and $A_t=\int_0^tb(X_s)\,ds$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) and boundedness give

$$
\mathbb E|X_t-x_0|^2\le2S^2t+2K^2t^2\longrightarrow0.
$$

Continuity and boundedness of $b$ then imply $\mathbb E b(X_s)\to b(x_0)$. Since $M$ has mean zero,

$$
\frac{\mathbb EX_t-x_0}{t}=\frac1t\int_0^t\mathbb E b(X_s)\,ds\longrightarrow b(x_0).
$$

For the [variance](../../../variance.md), $\mathbb EM_t^2=\int_0^t\mathbb E\sigma(X_s)^2\,ds$. The remaining terms satisfy

$$
\mathbb EA_t^2\le K^2t^2,\qquad |\mathbb E(M_tA_t)|\le SKt^{3/2},\qquad (\mathbb E(X_t-x_0))^2\le K^2t^2.
$$

Continuity of $\sigma$ and the initial $L^2$ convergence give $\mathbb E\sigma(X_s)^2\to\sigma(x_0)^2$. Expanding the [variance](../../../variance.md) and dividing by $t$ proves the [initial mean and variance derivatives of an Itô diffusion](../../../stochastic-calculus.md#initial-mean-and-variance-derivatives-of-an-ito-diffusion):

$$
\boxed{\left.\frac d{dt}\mathbb EX_t\right|_{0+}=b(x_0),\qquad\left.\frac d{dt}\operatorname{Var}(X_t)\right|_{0+}=\sigma(x_0)^2.}
$$

The derivatives at the initial time are right derivatives because the process is indexed by $t\ge0$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) separately to cosine and sine, using $[B]_t=t$:

$$
\boxed{dX_t=-Y_t\,dB_t-\tfrac12X_t\,dt,\qquad dY_t=X_t\,dB_t-\tfrac12Y_t\,dt.}
$$

In vector standard form $dZ_t=\sigma(Z_t)\,dB_t+b(Z_t)\,dt$, with one-dimensional driving noise and two-dimensional state, the coefficient functions are

$$
\boxed{\sigma(x,y)=\begin{pmatrix}-y\\x\end{pmatrix},\qquad b(x,y)=-\tfrac12\begin{pmatrix}x\\y\end{pmatrix}.}
$$

The original trigonometric process starts at $(1,0)$, but these coefficient functions define a [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) on all of $\mathbb R^2$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Both coefficient functions are linear, hence globally Lipschitz. Their norms are bounded by a constant times $|(x,y)|$, so they satisfy the [linear growth condition for an SDE](../../../stochastic-calculus.md#linear-growth-condition-for-an-sde). The [existence and pathwise uniqueness theorem for a stochastic differential equation](../../../stochastic-calculus.md#existence-and-pathwise-uniqueness-theorem-for-a-stochastic-differential-equation) gives a unique global [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) for every deterministic starting point $(x_0,y_0)\in\mathbb R^2$. Linear growth prevents finite-time explosion.

The theorem gives [pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness), and strong existence with [pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) gives [uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law). Thus **every initial value is permitted, and both forms of uniqueness hold**. The coefficients need not be bounded for this theorem; their global Lipschitz and linear-growth properties are sufficient.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For any initial point, rotate its vector through the Brownian angle:

$$
\boxed{X_t=x_0\cos B_t-y_0\sin B_t,\qquad Y_t=x_0\sin B_t+y_0\cos B_t.}
$$

This is a nonanticipating function of the prescribed Brownian path and has the required initial value. Equivalently, $Z_t=X_t+iY_t=(x_0+iy_0)e^{iB_t}$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives $dZ_t=iZ_t\,dB_t-Z_t\,dt/2$, whose real and imaginary parts are exactly the equations in part c. Therefore the displayed formula is the [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation), and uniqueness from part d makes it the only one.

The [Brownian rotation in the plane](../../../stochastic-calculus.md#brownian-rotation-in-the-plane) preserves radius: $X_t^2+Y_t^2=x_0^2+y_0^2$. Nonzero starting points move around their initial circle, and the origin remains fixed.

## 5

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use $M_0=0$, as implicit in the specified initial value of $Y$. First let $[M]_t=t$. The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) makes $M$ [Brownian motion](../../../brownian-motion.md) relative to the given [filtration](../../../stochastic-process.md#filtration-probability-theory). Set

$$
\varepsilon=\mathbb P(|G|>C+2)>0,\qquad G\sim N(0,1).
$$

On this event at time one, the drift has absolute size at most $C$, while $|Y_0|<1$, so $|Y_1|\ge|M_1|-|Y_0|-C>1$. Continuity forces exit by time one. Therefore

$$
\boxed{\mathbb P(T>1)\le1-\varepsilon.}
$$

The same estimate applies conditionally at each integer time without assuming anything about future drift independence. On $\{T>n\}$, $|Y_n|<1$; if $|M_{n+1}-M_n|>C+2$, the drift bound forces exit by $n+1$. That Brownian increment is independent of $\mathcal F_n$. Hence

$$
\mathbb P(T>n+1\mid\mathcal F_n)\le(1-\varepsilon)\mathbf1_{\{T>n\}},\qquad \mathbb P(T>n)\le(1-\varepsilon)^n.
$$

In particular $T<\infty$ almost surely.

For general $Q$, write $K_t=[M]_t$ and $D_t=\int_0^t A_s\,ds$. Continuity of $Q$ and monotonicity of its integral imply $Q_s\ge0$ at all times outside one null set. The drift condition gives

$$
|D_t-D_s|\le C(K_t-K_s)\qquad(s\le t).
$$

Let $\tau_u=\inf\{t:K_t>u\}$. The divergent clock makes $\tau_u$ finite for every $u$, and its continuity gives $K_{\tau_u}=u$. By the [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem), $W_u=M_{\tau_u}$ is [Brownian motion](../../../brownian-motion.md) for $\mathcal G_u=\mathcal F_{\tau_u}$. On intervals where $K$ is constant, both $M$ and $D$ are constant. Thus $d_u=D_{\tau_u}$ is a continuous adapted function of clock time satisfying $|d_v-d_u|\le C(v-u)$. The time-changed process is

$$
\widetilde Y_u=Y_{\tau_u}=Y_0+W_u+d_u.
$$

The unit-clock argument uses only this increment bound on the drift, so its first exit time $S$ obeys $\mathbb P(S>n)\le(1-\varepsilon)^n$. It is finite almost surely, and a corresponding finite ordinary time has $|Y|\ge1$. This proves the [exit with drift controlled by quadratic variation](../../../martingale.md#exit-with-drift-controlled-by-quadratic-variation) result

$$
\boxed{T<\infty\quad\text{almost surely}.}
$$

This proof needs only a nonnegative measurable bracket density, a continuous divergent integral clock, and the drift increment bound; pointwise continuity of the density is unnecessary. This observation permits the application below with measurable SDE coefficients.

For the multidimensional SDE, put $a_{ij}(x)=\sum_{k=1}^m\sigma_k^i(x)\sigma_k^j(x)$. The [generator of an SDE diffusion](../../../stochastic-calculus.md#generator-of-an-sde-diffusion) is

$$
\boxed{Lf(x)=\sum_i b_i(x)\partial_if(x)+\frac12\sum_{i,j}a_{ij}(x)\partial_{ij}f(x).}
$$

For every $f\in C_b^2(\mathbb R^d)$, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
f(X_t^x)-f(x)-\int_0^tLf(X_s^x)\,ds=\sum_k\int_0^t\nabla f(X_s^x)\cdot\sigma_k(X_s^x)\,dB_s^k.
$$

Bounded derivatives and bounded noise fields make the right side square-integrable on each finite horizon, hence a true [martingale](../../../martingale.md). This is precisely the defining test-function property of an [L-diffusion](../../../stochastic-calculus.md#diffusion-martingale-problem), in the martingale-problem sense.

Now fix $x$ and $\xi\ne0$. Its scalar projection has [martingale](../../../martingale.md) part $M_t^\xi=\sum_k\int_0^t\langle\xi,\sigma_k(X_s^x)\rangle\,dB_s^k$ and drift $\langle\xi,b(X_s^x)\rangle$. The [uniform ellipticity](../../../elliptic-boundary-value-problem.md#uniformly-elliptic-operator) assumption gives

$$
\frac{d[M^\xi]_t}{dt}=\sum_k\langle\xi,\sigma_k(X_t^x)\rangle^2\ge\lambda|\xi|^2.
$$

Let $B_*=\sup_z|b(z)|$ and take $R>|\langle\xi,x\rangle|$. Rescale the projection by $R$. Its bracket density is at least $\lambda|\xi|^2/R^2$, its absolute drift is at most $B_*|\xi|/R$, and hence that drift is at most $C_R$ times its bracket density, with $C_R=B_*R/(\lambda|\xi|)$. Its clock diverges, so the exit lemma forces it out of $(-1,1)$ in finite time. Equivalently it leaves the slab $|\langle\xi,X_t^x\rangle|<R$. Taking a countable sequence of integer $R$ tending to infinity proves the [projection unboundedness of a uniformly elliptic diffusion](../../../stochastic-calculus.md#projection-unboundedness-of-a-uniformly-elliptic-diffusion):

$$
\boxed{\sup_{t\ge0}|\langle\xi,X_t^x\rangle|=\infty\quad\text{almost surely, for each fixed }x,\ \xi\ne0.}
$$

For the final uniqueness result, let $\tau_D=\inf\{t:X_t^x\notin D\}$, with $x\in D$. Since $D$ is bounded, it lies in a finite slab; the preceding finite slab-exit time bounds $\tau_D$ from above. Thus $\tau_D<\infty$ almost surely. Continuity gives $X_{\tau_D}^x\in\partial D$.

Set $h=u-v$. It is bounded, has bounded derivatives, is zero on the boundary, and satisfies $Lh=0$ in $D$. The stopped test-function identity says $h(X_{t\wedge\tau_D}^x)$ is a [martingale](../../../martingale.md); equivalently it is a bounded [local martingale](../../../martingale.md#local-martingale), which suffices. Taking expectations and then using bounded convergence as $t\to\infty$ gives

$$
h(x)=\mathbb E_x h(X_{\tau_D})=0.
$$

Therefore the [bounded-domain harmonic uniqueness for a diffusion](../../../stochastic-calculus.md#bounded-domain-harmonic-uniqueness-for-a-diffusion) conclusion is

$$
\boxed{u=v\text{ throughout }D.}
$$

In particular the argument supplies the representation $u(x)=\mathbb E_xu(X_{\tau_D})$ and establishes uniqueness without selecting a unique diffusion law.

## 6

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [Markov jump process](../../../markov-process.md#markov-jump-process) relative to $(\mathcal F_t)$ is an adapted [càdlàg](../../../calculus.md#cadlag) process with piecewise-constant paths and finitely many jumps on each bounded time interval, whose conditional future law given $\mathcal F_t$ depends only on its current state. For a time-homogeneous process on a countable state space, write $q(x,y)\ge0$ for its transition rates and $q(x)=\sum_{y\ne x}q(x,y)<\infty$. In state $x$, the holding time is exponential of rate $q(x)$ and the next state is $y$ with probability $q(x,y)/q(x)$; a zero rate makes the state absorbing. The generator is $\mathcal Af(x)=\sum_{y\ne x}q(x,y)(f(y)-f(x))$. Nonexplosion is included here so that the process is defined at every finite time.

Here is a finite-jump, bounded-rate form of the [Kurtz fluid limit theorem](../../../queueing-theory.md#kurtz-fluid-limit-theorem). For each $N$, let $Z^N$ be a chain on a countable state space $E_N\subseteq\mathbb R^d$ with jumps $\ell/N$ at rates $N\beta_\ell(z)$, with $\ell$ in a fixed finite subset $\mathcal J\subset\mathbb R^d$. Assume the nonnegative $\beta_\ell$ are uniformly bounded, admissible jumps remain in the state space, and

$$
F(z)=\sum_{\ell\in\mathcal J}\ell\beta_\ell(z)
$$

is globally Lipschitz with constant $L$. Suppose $Z_0^N\to z_0$ in probability, and let $z$ solve $\dot z=F(z)$, $z(0)=z_0$. Then for every finite $T$,

$$
\boxed{\sup_{0\le t\le T}|Z_t^N-z(t)|\longrightarrow0\quad\text{in probability}.}
$$

Bounded total jump rates ensure nonexplosion; the globally Lipschitz drift gives a unique global ODE solution. These explicit hypotheses suffice for the population example, without needing a more general local version of the theorem.

To prove the result, compensate the jumps of this [density-dependent Markov jump process](../../../markov-process.md#density-dependent-markov-jump-process). The drift and the coordinate [martingales](../../../martingale.md) satisfy

$$
Z_t^N=Z_0^N+\int_0^tF(Z_s^N)\,ds+M_t^N,\qquad\langle M^{N,i}\rangle_t=\frac1N\int_0^t\sum_\ell\ell_i^2\beta_\ell(Z_s^N)\,ds.
$$

Here $\langle M^{N,i}\rangle$ is [predictable quadratic variation](../../../stochastic-calculus.md#predictable-quadratic-variation), not the sum of realized squared jumps. The compensation identity follows because each possible increment $\ell/N$ has intensity $N\beta_\ell$, and its squared coordinate increment contributes $\ell_i^2\beta_\ell/N$ per unit time. Bounded rates and jump sizes make these [martingales](../../../martingale.md) square-integrable.

We use the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) in the explicit form $\mathbb E\sup_{s\le T}|M_s|^2\le4\mathbb E|M_T|^2$ for a scalar square-integrable [martingale](../../../martingale.md) starting at zero. Applying it coordinatewise and setting $K=\sup_z\sum_\ell|\ell|^2\beta_\ell(z)<\infty$ gives

$$
\mathbb E\sup_{s\le T}|M_s^N|^2\le\sum_i\mathbb E\sup_{s\le T}|M_s^{N,i}|^2\le\frac{4KT}{N}.
$$

Subtract the ODE integral equation. Lipschitz continuity and [Gronwall's inequality](../../../probability-and-statistics.md#gronwall-inequality) yield

$$
\sup_{s\le T}|Z_s^N-z(s)|\le e^{LT}\left(|Z_0^N-z_0|+\sup_{s\le T}|M_s^N|\right).
$$

The first term tends to zero in probability by hypothesis, and the second by its maximal second-moment estimate. More quantitatively, for $\delta>0$,

$$
\mathbb P\left(\sup_{s\le T}|Z_s^N-z(s)|>\delta\right)\le\mathbb P\left(|Z_0^N-z_0|>\tfrac12\delta e^{-LT}\right)+\frac{16KT e^{2LT}}{N\delta^2}.
$$

This proves the stated uniform finite-horizon [fluid limit](../../../queueing-theory.md#fluid-limit).

For the cells, division replaces one cell by two and increases population by one. At population $k\le N$, the total rate is the sum of the $k$ identical cell rates, namely

$$
q_N(k,k+1)=k(1-k/N).
$$

The state $N$ is absorbing. Set $Z_t^N=\xi_t/N$; its jump is $1/N$ with rate $N\beta(z)$, where $\beta(z)=z(1-z)$ on $[0,1]$. Extending this function by zero outside $[0,1]$ makes it bounded, nonnegative and globally Lipschitz, with Lipschitz constant one. Starting from $Z_0^N=p$, or from $\lfloor pN\rfloor/N$ when integer rounding is necessary, the limiting ODE is the [logistic differential equation](../../../differential-equation.md#logistic-differential-equation)

$$
\dot z=z(1-z),\qquad z(0)=p.
$$

Separation of variables, or differentiating $z/(1-z)$, gives its solution. The [logistic cell-division process](../../../markov-process.md#logistic-cell-division-process) therefore satisfies

$$
\boxed{z(t)=\frac{pe^t}{1-p+pe^t},\qquad\sup_{s\le T}\left|\frac{\xi_s}{N}-\frac{pe^s}{1-p+pe^s}\right|\longrightarrow0\ \text{in probability for every finite }T.}
$$

Here $K\le1/4$, so the maximal [martingale](../../../martingale.md) second moment is at most $T/N$. With exact initial density $p$, the preceding pathwise bound even gives $\mathbb E\sup_{s\le T}|Z_s^N-z(s)|^2\le Te^{2T}/N$. With integer rounding, the bound $\mathbb E\sup_{s\le T}|Z_s^N-z(s)|^2\le2e^{2T}(T/N+1/N^2)$ follows from $|Z_0^N-p|\le1/N$ and $(a+b)^2\le2a^2+2b^2$. Thus the deterministic logistic curve approximates the density with fluctuations of order $N^{-1/2}$ on fixed time intervals. The convergence statement is on finite horizons; it does not interchange the limits $t\to\infty$ and $N\to\infty$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
