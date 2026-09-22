# Paper 202

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_202.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_202.pdf)

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
    - [1](#3/a/1)
      - [Solution](#3/a/1/solution)
    - [2](#3/a/2)
      - [Solution](#3/a/2/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [1](#5/a/1)
      - [Solution](#5/a/1/solution)
    - [2](#5/a/2)
      - [Solution](#5/a/2/solution)
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
  - [d](#6/d)
    - [Solution](#6/d/solution)
  - [e](#6/e)
    - [Solution](#6/e/solution)
  - [f](#6/f)
    - [Solution](#6/f/solution)

## 1

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [L2 martingale convergence theorem](../../../martingale.md#l2-martingale-convergence-theorem) gives $M_t\to M_\infty$ in $L^2$, so

$$
\|M_\infty\|_2\leq
\left\|\sup_{t\geq0}|M_t|\right\|_2.
$$

Conversely, apply the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) on $[0,T]$:

$$
\mathbb E\sup_{t\leq T}|M_t|^2
\leq4\mathbb E|M_T|^2
\leq4\mathbb E|M_\infty|^2.
$$

[Monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) as $T\to\infty$ gives

$$
\left\|\sup_{t\geq0}|M_t|\right\|_2
\leq2\|M_\infty\|_2.
$$

**Thus the two norms are equivalent.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a [simple predictable process](../../../martingale.md#simple-predictable-process)

$$
H_s=\sum_{i=0}^{n-1}H_i\mathbf1_{(t_i,t_{i+1}]}(s),
\qquad H_i\in L^\infty(\mathcal F_{t_i}),
$$

define

$$
(H\mathbin\cdot M)_t
=\sum_{i=0}^{n-1}H_i
\bigl(M_{t\wedge t_{i+1}}-M_{t\wedge t_i}\bigr).
$$

Each summand is a bounded predictable multiple of a martingale increment, so conditional expectation proves that $H\mathbin\cdot M$ is a martingale. Orthogonality of disjoint martingale increments gives

$$
\mathbb E|(H\mathbin\cdot M)_\infty|^2
=\sum_i\mathbb E\!\left[
H_i^2(M_{t_{i+1}}-M_{t_i})^2\right]<\infty.
$$

It is therefore an $L^2$-bounded continuous martingale.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Indicators of the rectangles

$$
A\times(s,t],\qquad A\in\mathcal F_s,
$$

together with $A\times\{0\}$ generate the [predictable sigma-algebra](../../../martingale.md#predictable-sigma-algebra). Their finite linear span is precisely the set of simple processes. The monotone-class theorem therefore makes this span dense among bounded predictable functions in measure. Since $\nu$ is finite, truncation followed by bounded approximation proves density in $L^2(\mathcal P,\nu)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $\mathcal M_c^2$ be the continuous $L^2$-bounded martingales starting at zero, modulo indistinguishability, with norm $\|N\|_{\mathcal M^2}=\|N_\infty\|_2$. For a fixed $M\in\mathcal M_c^2$, define a finite measure on $\mathcal P$ by

$$
\nu_M(C)=\mathbb E\int_0^\infty\mathbf1_C(\omega,s)\,d[M]_s,
$$

and let $L^2(M)=L^2(\mathcal P,\nu_M)$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) is the isometric extension

$$
I_M:L^2(M)\longrightarrow\mathcal M_c^2,
\qquad
H\longmapsto H\mathbin\cdot M,
$$

satisfying

$$
\mathbb E|(H\mathbin\cdot M)_\infty|^2
=\mathbb E\int_0^\infty H_s^2\,d[M]_s.
$$

For the simple process in part b, orthogonality gives the sum there. Conditional on $\mathcal F_{t_i}$, the martingale identity for $M^2-[M]$ gives

$$
\mathbb E\!\left[
H_i^2(M_{t_{i+1}}-M_{t_i})^2\right]
=\mathbb E\!\left[H_i^2([M]_{t_{i+1}}-[M]_{t_i})\right].
$$

Summing proves the isometry. Part c then supplies the unique extension to all of $L^2(M)$.

## 2

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A process is [previsible](../../../martingale.md#predictable-process) when it is measurable with respect to the predictable sigma-algebra. The deterministic process $H_t=\mathbf1_{[1,\infty)}(t)$ is predictable because deterministic Borel processes are predictable, but it is not left-continuous at $t=1$ on any sample path.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Since $|Z_tY_t|\leq C Z_t$ and $Z$ is uniformly integrable, the continuous local martingale $ZY$ is locally in Doob's class and hence is a true martingale. For $A\in\mathcal F_s$ and $s\leq t$, [Bayes formula for conditional expectation](../../../probability-theory.md#bayes-formula-for-conditional-expectation) gives

$$
\widetilde{\mathbb E}[\mathbf1_A Y_t]
=\mathbb E[\mathbf1_AZ_\infty Y_t]
=\mathbb E[\mathbf1_AZ_tY_t]
=\mathbb E[\mathbf1_AZ_sY_s]
=\widetilde{\mathbb E}[\mathbf1_A Y_s].
$$

The bounded process $Y$ is integrable under $\widetilde{\mathbb P}$, so this is exactly the martingale property.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Cameron-Martin theorem](../../../brownian-motion.md#cameron-martin-theorem) on Wiener space says that the translated measure $\mathbb P_h(A)=\mathbb P(X+h\in A)$ is equivalent to Wiener measure precisely when $h$ is absolutely continuous, $h(0)=0$, and $\dot h\in L^2(\mathbb R_+)$. In that case

$$
\frac{d\mathbb P_h}{d\mathbb P}
=\exp\left(
\int_0^\infty\dot h_s\,dX_s
-\frac12\int_0^\infty\dot h_s^2\,ds\right).
$$

For such $h$, the exponential is a uniformly integrable [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential). Under the measure defined by this density, the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) makes $X_t-\int_0^t\dot h_sds=X_t-h(t)$ a Brownian motion. This identifies the translated law and proves equivalence; replacing $h$ by $-h$ gives the inverse density.

If $h$ fails the Cameron-Martin condition on some finite interval, the finite-horizon theorem gives singularity there. If it belongs locally but $\int_0^\infty\dot h_s^2ds=\infty$, the log likelihood is a Brownian motion run at that diverging energy clock minus half the clock. It tends to $-\infty$ under one measure and to $+\infty$ under the translate, producing disjoint full-measure events. Thus the measures are singular.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [Cameron-Martin theorem for a linear drift](../../../brownian-motion.md#cameron-martin-theorem-for-a-linear-drift) changes the density of Brownian paths through time $t$ by

$$
\exp\left(bB_t-\frac12b^2t\right).
$$

At the driftless hitting time $\tau_{a,0}=t$, the endpoint is $B_t=a$. Multiplying its given density by the likelihood $e^{ab-b^2t/2}$ therefore yields

$$
\boxed{a(2\pi t^3)^{-1/2}
\exp\left(-\frac{a^2}{2t}+ab-\frac12b^2t\right)
=a(2\pi t^3)^{-1/2}
\exp\left(-\frac{(a-bt)^2}{2t}\right).}
$$

## 3

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/1">1</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/1/solution">Solution</h5>

↑ **Parent:** [1](#3/a/1)

Let $\tau_n$ localize $M$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives

$$
\mathbb E M_{t\wedge\tau_n}^2
=\mathbb E[M]_{t\wedge\tau_n}
\leq\mathbb E[M]_t.
$$

Thus the stopped variables are bounded in $L^2$, and localization plus weak compactness shows that $M$ is a true martingale. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applied to $f(x)=x^2$ gives

$$
M_t^2-[M]_t=2\int_0^tM_s\,dM_s.
$$

After localization this is a martingale; the [Burkholder-Davis-Gundy inequalities](../../../martingale.md#burkholder-davis-gundy-inequalities) and $\mathbb E[M]_t<\infty$ supply the required local integrability, so it is a true martingale.

<h4 id="3/a/2">2</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/2/solution">Solution</h5>

↑ **Parent:** [2](#3/a/2)

Part 1 gives $\mathbb EM_t^2=\mathbb E[M]_t$. Hence

$$
\sup_{t\geq0}\mathbb EM_t^2
\leq\mathbb E[M]_\infty<\infty,
$$

so $M$ is $L^2$-bounded.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [martingale product identity](../../../stochastic-calculus.md#martingale-product-identity) and the Itô isometry for cross terms give

$$
\mathbb E\left[B_t\int_0^te^{B_s}\,dB_s\right]
=\mathbb E\int_0^te^{B_s}\,ds.
$$

Since $B_s\sim N(0,s)$, its [moment-generating function](../../../probability-theory.md#moment-generating-function) gives $\mathbb Ee^{B_s}=e^{s/2}$. Therefore the answer is

$$
\boxed{\int_0^te^{s/2}\,ds=2(e^{t/2}-1).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $X^x$ solve

$$
dX_s=b(X_s)\,ds+\sqrt{a(X_s)}\,dB_s,
\qquad X_0=x.
$$

The [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) is

$$
u(t,x)=\mathbb E_x\left[
f(X_t)\exp\left(\int_0^tV(X_r)\,dr\right)\right].
$$

Fix $t$ and apply the two-variable [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $F(s,y)=u(t-s,y)$ and the semimartingale vector $(s,X_s)$. Multiplying by

$$
R_s=\exp\left(\int_0^sV(X_r)\,dr\right)
$$

and using the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule), the drift of $R_sF(s,X_s)$ is

$$
R_s(-\partial_tu+Lu+Vu)(t-s,X_s)\,ds=0.
$$

The remaining stochastic integral is a true martingale because the coefficients and derivatives are bounded. Taking expectations at $s=0$ and $s=t$ gives the formula.

## 4

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $f(x)=x^2$ and the semimartingale $B$ gives

$$
B_t^2=2\int_0^tB_s\,dB_s+t.
$$

Hence

$$
X_t=-2\int_0^tB_s\,dB_s+\int_0^t(B_s^2-1)\,ds.
$$

The first term is a continuous local martingale and the second has finite variation. By uniqueness of the continuous semimartingale decomposition, $X$ could be a local martingale only if the finite-variation term were constant. Its derivative $B_s^2-1$ is not zero almost everywhere, so $X$ is not a local martingale.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Enlarge the space by an independent Brownian motion $W$ and define

$$
B_t=\int_0^t\mathbf1_{\{A_s>0\}}A_s^{-1/2}\,dX_s
+\int_0^t\mathbf1_{\{A_s=0\}}\,dW_s.
$$

The two terms have zero cross-variation and

$$
[B]_t=\int_0^t\mathbf1_{\{A_s>0\}}ds
+\int_0^t\mathbf1_{\{A_s=0\}}ds=t.
$$

The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) makes $B$ a Brownian motion. The residual $\int\mathbf1_{\{A=0\}}dX$ has zero quadratic variation and is therefore constant, so

$$
\boxed{X_t-X_0=\int_0^tA_s^{1/2}\,dB_s.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

An $L$-diffusion solves the [martingale problem](../../../stochastic-calculus.md#martingale-problem) for

$$
Lf(x)=b(x)f'(x)+\frac12\sigma(x)^2f''(x):
$$

for every $f\in C_c^2(\mathbb R)$,

$$
f(X_t)-f(X_0)-\int_0^tLf(X_s)\,ds
$$

is a local martingale. Applying this to cutoff approximations of $x$ and $x^2$ shows that

$$
M_t=X_t-X_0-\int_0^tb(X_s)\,ds
$$

is a continuous local martingale with

$$
[M]_t=\int_0^t\sigma(X_s)^2\,ds.
$$

Part b gives $M=\int|\sigma(X_s)|\,dW_s$. Changing the sign of $W$ predictably where $\sigma<0$, and filling the zero set with independent Brownian noise, produces a Brownian motion $B$ such that $M=\int\sigma(X_s)\,dB_s$. Thus

$$
\boxed{dX_t=b(X_t)\,dt+\sigma(X_t)\,dB_t.}
$$

## 5

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/1">1</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/1/solution">Solution</h5>

↑ **Parent:** [1](#5/a/1)

For every real $\lambda$, positivity of quadratic variation gives

$$
0\leq[M+\lambda N]_t
=[M]_t+2\lambda[M,N]_t+\lambda^2[N]_t.
$$

The discriminant of this quadratic is nonpositive, so

$$
|[M,N]_t|\leq\sqrt{[M]_t[N]_t}.
$$

Continuity lets the almost-sure assertion hold simultaneously for every $t$.

<h4 id="5/a/2">2</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/2/solution">Solution</h5>

↑ **Parent:** [2](#5/a/2)

For a partition $\pi$ of $[0,t]$, apply the first inequality to each increment of the covariation and then the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
\sum_{\pi}|\Delta[M,N]|
\leq\sum_\pi\sqrt{\Delta[M]\,\Delta[N]}
\leq\sqrt{[M]_t[N]_t}.
$$

Taking the supremum over partitions proves the [Kunita-Watanabe inequality](../../../stochastic-calculus.md#kunita-watanabe-inequality)

$$
\boxed{V_t([M,N])\leq\sqrt{[M]_t[N]_t}.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $\tau_n$ localize the nonnegative local martingale $M$. For $s\leq t$,

$$
\mathbb E(M_{t\wedge\tau_n}\mid\mathcal F_s)=M_{s\wedge\tau_n}.
$$

[Conditional Fatou lemma](../../../measure-theory.md#conditional-fatou-lemma) and nonnegativity give

$$
\mathbb E(M_t\mid\mathcal F_s)
\leq\liminf_nM_{s\wedge\tau_n}=M_s.
$$

**Thus $M$ is a [supermartingale](../../../martingale.md#supermartingale), recovering the general fact about a [nonnegative local martingale](../../../martingale.md#nonnegative-local-martingale).**

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

A [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) is adapted to the completed filtration of a prescribed Brownian motion $B$ on a prescribed probability space and satisfies

$$
X_t=X_0+\int_0^tb(X_s)\,ds+\int_0^t\sigma(X_s)\,dB_s
$$

almost surely. A [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) may choose the filtered probability space, Brownian motion, and adapted process as part of the solution; only the displayed integral equation and the prescribed initial law are required.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $f(t,x)=x_0e^{\sigma x+(\mu-\sigma^2/2)t}$ and the semimartingale vector $(t,B_t)$. Its derivatives give

$$
dX_t=\mu X_t\,dt+\sigma X_t\,dB_t.
$$

Therefore

$$
X_t=x_0\exp\left(\sigma B_t+
\left(\mu-\frac12\sigma^2\right)t\right).
$$

This is adapted to the given Brownian filtration and is consequently a strong solution; it is [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion).

## 6

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Approximate $h$ in $L^2[0,t]$ by deterministic step functions $h_n$. Each integral $\int h_n\,dB$ is a linear combination of independent Gaussian increments and hence is Gaussian, with mean zero and variance $\int h_n^2$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives convergence in $L^2$ to $\int h\,dB$, so characteristic functions pass to the limit. Thus

$$
\boxed{\int_0^th(s)\,dB_s
\sim N\left(0,\int_0^th(s)^2\,ds\right).}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) for $e^{\lambda t}X_t$ gives

$$
d(e^{\lambda t}X_t)=e^{\lambda t}\,dB_t.
$$

Therefore the [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process) has the explicit form

$$
\boxed{X_t=xe^{-\lambda t}
+\int_0^te^{-\lambda(t-s)}\,dB_s.}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Part a applied to the deterministic kernel gives

$$
\boxed{X_t\sim N\left(
xe^{-\lambda t},
\int_0^te^{-2\lambda(t-s)}ds\right)
=N\left(xe^{-\lambda t},
\frac{1-e^{-2\lambda t}}{2\lambda}\right).}
$$

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Every linear combination of $X_{t_1},\ldots,X_{t_n}$ is a deterministic constant plus one stochastic integral of a deterministic $L^2$ function against $B$. Part a makes every such combination Gaussian. By the linear-combination characterization of a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution), $(X_{t_1},\ldots,X_{t_n})$ is jointly Gaussian, so $X$ is a [Gaussian process](../../../stochastic-process.md#gaussian-process).

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

For $0<s<t$, only the Brownian noise accumulated through time $s$ is shared. The Itô isometry for cross terms gives

$$
\begin{aligned}
\operatorname{Cov}(X_t,X_s)
&=\int_0^se^{-\lambda(t-r)}e^{-\lambda(s-r)}\,dr\\
&=\frac{e^{-\lambda(t-s)}(1-e^{-2\lambda s})}{2\lambda}.
\end{aligned}
$$

<h3 id="6/f">f</h3>

↑ **Parent:** [6](#6)

<h4 id="6/f/solution">Solution</h4>

↑ **Parent:** [F](#6/f)

If $X_0\sim N(0,(2\lambda)^{-1})$ independently of $B$, then

$$
\operatorname{Var}(X_t)
=e^{-2\lambda t}\frac1{2\lambda}
+\frac{1-e^{-2\lambda t}}{2\lambda}
=\frac1{2\lambda}.
$$

Thus $X_t\sim N(0,(2\lambda)^{-1})$ for every $t$. For $0<s<t$, the Markov decomposition

$$
X_t=e^{-\lambda(t-s)}X_s
+\int_s^te^{-\lambda(t-r)}\,dB_r
$$

has an increment independent of $X_s$, and hence

$$
\operatorname{Cov}(X_t,X_s)
=\frac{e^{-\lambda(t-s)}}{2\lambda}.
$$

This is the stationary Ornstein-Uhlenbeck covariance.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
