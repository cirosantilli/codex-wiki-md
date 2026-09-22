# Paper 202

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_202.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_202.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
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
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
  - [f](#4/f)
    - [Solution](#4/f/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
    - [iii](#5/c/iii)
      - [Solution](#5/c/iii/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The integrand $\operatorname{sign}(\beta_s)$ is a bounded [previsible process](../../../martingale.md#predictable-process), so $B$ is a [continuous local martingale](../../../martingale.md#continuous-local-martingale). The [quadratic variation of a stochastic integral](../../../stochastic-calculus.md#quadratic-variation-of-a-stochastic-integral) is

$$
[B]_t=\int_0^t\operatorname{sign}(\beta_s)^2ds=t,
$$

because the [Brownian zero set](../../../brownian-motion.md#brownian-zero-set) has zero [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Since $B_0=0$, the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) shows that $B$ is a standard [Brownian motion](../../../brownian-motion.md).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Both variables are centered. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) in its bilinear form gives

$$
\operatorname{Cov}(B_t,\beta_t)=\mathbb E\!\left[\left(\int_0^t\operatorname{sign}(\beta_s)d\beta_s\right)\left(\int_0^t1\,d\beta_s\right)\right]=\int_0^t\mathbb E[\operatorname{sign}(\beta_s)]ds=0,
$$

where the last equality follows because a centered [Gaussian distribution](../../../probability-theory.md#normal-distribution) is a [symmetric probability distribution](../../../probability-theory.md#symmetric-probability-distribution). Thus $B_t$ and $\beta_t$ are [uncorrelated random variables](../../../variance.md#uncorrelated-random-variables).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

They are not independent. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives $\beta_t^2=t+2\int_0^t\beta_s\,d\beta_s$, and the bilinear [Itô isometry](../../../stochastic-calculus.md#ito-isometry) therefore gives

$$
\mathbb E[B_t\beta_t^2]=2\int_0^t\mathbb E[\operatorname{sign}(\beta_s)\beta_s]ds=2\int_0^t\mathbb E|\beta_s|ds=\frac43\sqrt{\frac2\pi}\,t^{3/2}>0.
$$

If $B_t$ and $\beta_t$ were [independent random variables](../../../random-variable.md#independent-random-variables), then $B_t$ would also be independent of the [measurable function](../../../measure-theory.md#measurable-function) $\beta_t^2$, and centeredness would instead give $\mathbb E[B_t\beta_t^2]=\mathbb E[B_t]\mathbb E[\beta_t^2]=0$. This contradiction disproves independence.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) states that if $M$ is a [continuous local martingale](../../../martingale.md#continuous-local-martingale) with $M_0=0$ and $[M]_\infty=\infty$, then, for

$$
\tau_s=\inf\{t\geq0:[M]_t>s\},
$$

the process $W_s=M_{\tau_s}$ is a standard [Brownian motion](../../../brownian-motion.md) and $M_t=W_{[M]_t}$. If $[M]_\infty<\infty$, one obtains the same representation after enlarging the [probability space](../../../probability-theory.md#probability-space) and continuing $W$ independently beyond $[M]_\infty$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Set $M_t=\int_0^tH_s\,dB_s$. Its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) is $[M]_t=\int_0^tH_s^2ds$, which is continuous and tends to infinity almost surely by assumption. The stated [stopping time](../../../martingale.md#stopping-time) is the inverse clock at level one, so $[M]_\tau=1$. The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) gives

$$
\boxed{\int_0^\tau H_s\,dB_s=M_\tau=W_{[M]_\tau}=W_1\sim N(0,1).}
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

**False.** The [Brownian motion produced by the Dambis-Dubins-Schwarz theorem need not be independent of its clock](../../../martingale.md#brownian-motion-produced-by-the-dambis-dubins-schwarz-theorem-need-not-be-independent-of-its-clock). Let $W$ be a standard [Brownian motion](../../../brownian-motion.md) and set

$$
M_t=\int_0^tW_s\,dW_s=\frac12(W_t^2-t),
\qquad
[M]_t=\int_0^tW_s^2ds.
$$

If the Brownian motion $B$ in $M_t=B_{[M]_t}$ were independent of the whole [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) process, then conditioning on $[M]$ would give $\mathbb E[M_t[M]_t]=\mathbb E[B_{[M]_t}[M]_t]=0$. Instead, the fourth-moment formula for a [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) gives $\operatorname{Cov}(W_t^2,W_s^2)=2s^2$ for $s\leq t$, and hence

$$
\mathbb E[M_t[M]_t]=\frac12\int_0^t\operatorname{Cov}(W_t^2,W_s^2)ds=\int_0^ts^2ds=\frac{t^3}{3}>0.
$$

**Thus $B$ and $[M]$ are dependent.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Because independent [Brownian motions](../../../brownian-motion.md) have zero [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation), the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) gives

$$
d(B_t^1B_t^2)=B_t^1\,dB_t^2+B_t^2\,dB_t^1.
$$

After integration, the random variable in the question is $B_t^1B_t^2$. Writing $B_t^j=\sqrt t\,Z_j$ for independent standard [Gaussian random variables](../../../probability-theory.md#gaussian-random-variable) $Z_1,Z_2$, its distribution is

$$
tZ_1Z_2,
$$

the scaled [product of two independent standard normal random variables](../../../probability-theory.md#product-of-two-independent-standard-normal-random-variables).

## 2

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [càdlàg process](../../../stochastic-process.md#cadlag-process) $A$ is a [finite-variation process](../../../stochastic-calculus.md#finite-variation-process) when, almost surely, for every $T<\infty$,

$$
\sup_\pi\sum_{k}|A_{t_{k+1}}-A_{t_k}|<\infty,
$$

where the [supremum](../../../real-analysis.md#supremum) is over every finite [partition of an interval](../../../real-analysis.md#partition-of-an-interval) $0=t_0<\cdots<t_n=T$.

[Uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability) of $X^n$ to $X$ means that, for every $T<\infty$ and $\varepsilon>0$,

$$
\boxed{\mathbb P\!\left(\sup_{0\leq t\leq T}|X_t^n-X_t|>\varepsilon\right)\longrightarrow0.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Apply the [realized absolute covariation](../../../stochastic-calculus.md#realized-absolute-covariation) theorem to each dyadic [partition of an interval](../../../real-analysis.md#partition-of-an-interval). More explicitly, use the continuous increasing clock $C=[M]+[N]$ and the [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem) to write

$$
a=\frac{d[M]}{dC},\qquad b=\frac{d[N]}{dC},\qquad c=\frac{d[M,N]}{dC}.
$$

For each time, let $(U,V)$ have the centered [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) with covariance matrix $\left(\begin{smallmatrix}a&c\\c&b\end{smallmatrix}\right)$, and define

$$
\widetilde V_t=\int_0^t\mathbb E|UV|\,dC.
$$

This process is continuous and increasing. To prove convergence, localize $M,N$, represent the pair as [stochastic integrals](../../../stochastic-calculus.md#stochastic-integral) against a two-dimensional [Brownian motion](../../../brownian-motion.md), and approximate the integrands in $L^2(dC)$ by bounded step [previsible processes](../../../martingale.md#predictable-process). For step integrands, the result is the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) applied on each block to independent [Gaussian random variables](../../../probability-theory.md#gaussian-random-variable). The [Burkholder-Davis-Gundy inequality](../../../martingale.md#burkholder-davis-gundy-inequalities) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) make the error uniform on each compact interval in probability. Consequently

$$
\widetilde V^n\longrightarrow\widetilde V
$$

in the sense of [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

With the notation from part (i), the [total-variation process](../../../stochastic-calculus.md#total-variation-process) of $[M,N]$ is

$$
V_t=\int_0^t|c|\,dC.
$$

For the centered [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) $(U,V)$ used there, $c=\mathbb E[UV]$. The [integral triangle inequality](../../../topological-analysis.md#integral-triangle-inequality) gives

$$
|c|=|\mathbb E[UV]|\leq\mathbb E|UV|.
$$

Integrating this pointwise inequality against $dC$ proves $V_t\leq\widetilde V_t$ for every $t\geq0$.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The [Kunita-Watanabe inequality](../../../stochastic-calculus.md#kunita-watanabe-inequality) applied to the [continuous local martingales](../../../martingale.md#continuous-local-martingale) $M,N$ gives directly

$$
V_t([M,N])\leq[M]_t^{1/2}[N]_t^{1/2}.
$$

Equivalently, with the clock and densities from part (i), positivity of the covariance matrix gives $|c|\leq\sqrt{ab}$, and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\boxed{V_t=\int_0^t|c|dC\leq\int_0^t\sqrt{ab}\,dC\leq\left(\int_0^ta\,dC\right)^{1/2}\left(\int_0^tb\,dC\right)^{1/2}=[M]_t^{1/2}[N]_t^{1/2}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The [martingale product identity](../../../stochastic-calculus.md#martingale-product-identity) says that $N_tK_t-[N,K]_t$ is a [martingale](../../../martingale.md). Passing to the terminal values of the square-integrable martingales and using $N_0=K_0=0$ gives

$$
\mathbb E[N_\infty K_\infty]=\mathbb E[N,K]_\infty.
$$

The [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) identity for a [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is

$$
[H\mathbin\cdot M,K]_t=\int_0^tH_s\,d[M,K]_s.
$$

Applying the same product identity to $H\mathbin\cdot M$ and $K$ therefore gives

$$
\boxed{\mathbb E[(H\mathbin\cdot M)_\infty K_\infty]=\mathbb E[H\mathbin\cdot M,K]_\infty.}
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Let $L=N-H\mathbin\cdot M$. It is a continuous square-integrable [martingale](../../../martingale.md), and the assumed bracket identity gives

$$
[L,K]_t=[N,K]_t-\int_0^tH_s\,d[M,K]_s=0
$$

for every continuous square-integrable martingale $K$. Choose $K=L$ and use part (i):

$$
\mathbb E[L_\infty^2]=\mathbb E[L]_\infty=0.
$$

**Thus $L_\infty=0$ almost surely, and the [conditional expectation](../../../measure-theory.md#conditional-expectation) property gives $L_t=\mathbb E[L_\infty\mid\mathcal F_t]=0$ for every $t$. Hence $N=H\mathbin\cdot M$ up to [indistinguishability of stochastic processes](../../../stochastic-process.md#indistinguishability-of-stochastic-processes).**

## 3

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Fix $0\leq r\leq t$. Since $M$ is a [martingale](../../../martingale.md),

$$
\operatorname{Cov}(M_{t+s}-M_t,M_r)=\mathbb E\!\left[M_r\,\mathbb E[M_{t+s}-M_t\mid\mathcal F_t]\right]=0.
$$

Every finite vector consisting of $M_{t+s}-M_t$ and past values $M_{r_1},\ldots,M_{r_n}$ has a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution). Therefore [uncorrelated jointly normal variables are independent](../../../probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent), so the increment is independent of every finite vector of past values. A [Monotone class theorem](../../../measure-theory.md#monotone-class-theorem) then extends this to independence from $\mathcal F_t=\sigma(M_r:0\leq r\leq t)$. This is the [independent increments of a Gaussian martingale](../../../stochastic-process.md#independent-increments-of-a-gaussian-martingale).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Define the deterministic function $f(t)=\mathbb E[M_t^2]$. The independent increments from part (i) show that $f$ is increasing and that $M_t^2-f(t)$ is a [martingale](../../../martingale.md). Mean-square continuity follows from path continuity and the Gaussian laws, so $f$ is continuous.

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) also says that $M_t^2-[M]_t$ is a [local martingale](../../../martingale.md#local-martingale). Their difference $[M]_t-f(t)$ is therefore a continuous [finite-variation process](../../../stochastic-calculus.md#finite-variation-process) that is also a local martingale. By the theorem that a [continuous finite-variation local martingale is constant](../../../martingale.md#continuous-finite-variation-local-martingale-is-constant), and because the difference starts at zero,

$$
[M]_t=f(t)
$$

for all $t\geq0$ almost surely.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

**False.** Let $Z\sim N(0,1)$ and define $X_t=tZ$. This is a centered continuous [Gaussian process](../../../stochastic-process.md#gaussian-process). Its [natural filtration](../../../stochastic-process.md#natural-filtration) satisfies $Z=X_s/s\in\mathcal F_s^X$ for every $s>0$, and hence, for $0<s<t$,

$$
\mathbb E[X_t\mid\mathcal F_s^X]=tZ=\frac tsX_s\ne X_s
$$

with positive probability. Thus $X$ is not a [martingale](../../../martingale.md) and does not belong to the stated martingale class.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

**True.** The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem), with an independent continuation of the Brownian motion if $f$ is bounded, represents

$$
M_t=W_{[M]_t}=W_{f(t)}.
$$

Because $f$ is deterministic, every finite vector $(M_{t_1},\ldots,M_{t_n})$ is a finite vector of a [Brownian motion](../../../brownian-motion.md) at deterministic times and therefore has a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution). Hence $M$ is a [Gaussian process](../../../stochastic-process.md#gaussian-process). This is the [deterministic quadratic variation characterizes a Gaussian continuous local martingale](../../../stochastic-process.md#deterministic-quadratic-variation-characterizes-a-gaussian-continuous-local-martingale) result.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

The function $z\mapsto\log|z|$ is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) on the [annulus](../../../topology.md#annulus-mathematics) $r_1<|z|<r_2$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) therefore makes $\log|B_{t\wedge\tau}|$ a bounded [martingale](../../../martingale.md). The [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
\log r=\mathbb E[\log|B_\tau|]=p\log r_1+(1-p)\log r_2,
$$

where $p=\mathbb P(|B_\tau|=r_1)$. Solving this [linear equation](../../../linear-algebra.md#linear-equation) yields the [planar Brownian annulus hitting probability](../../../brownian-motion.md#planar-brownian-annulus-hitting-probability)

$$
\boxed{p=\frac{\log r_2-\log r}{\log r_2-\log r_1}.}
$$

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

**No such function exists.** Continuity on the compact closed unit disk makes $u$ bounded near the origin. The [removable singularity for a bounded harmonic function](../../../partial-differential-equation.md#removable-singularity-for-a-bounded-harmonic-function) extends $u$ harmonically across the origin. The extended function is continuous on the closed disk and vanishes on its boundary, so the [maximum principle for harmonic functions](../../../partial-differential-equation.md#maximum-principle-for-harmonic-functions), applied to both $u$ and $-u$, forces $u=0$ throughout the disk. This contradicts $u(0,0)=1$.

## 4

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

On $[\tau,\sigma)$ the Brownian path does not meet zero, so the [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) $x\mapsto|x|^\delta$ is twice continuously differentiable along the path. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
dY_t=\delta|B_t|^{\delta-1}\operatorname{sign}(B_t)dB_t+\frac{\delta(\delta-1)}2|B_t|^{\delta-2}dt.
$$

Since $Y_t=|B_t|^\delta$, this becomes

$$
dY_t=\delta Y_t^{(\delta-1)/\delta}d\widehat B_t+\frac{\delta(\delta-1)}2Y_t^{(\delta-2)/\delta}dt,
$$

where $\widehat B_t=\int_0^t\operatorname{sign}(B_s)dB_s$ is a standard [Brownian motion](../../../brownian-motion.md) by the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion). Thus the displayed equation in the paper is valid after the customary renaming of $\widehat B$ as $B$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let

$$
A_t=\int_0^t\delta^2Y_u^{2(\delta-1)/\delta}du=\int_0^t\delta^2|B_u|^{2\delta-2}du.
$$

The clock $A$ is an [absolutely continuous function](../../../sobolev-space.md#absolutely-continuous-function) and is strictly increasing: its derivative is positive away from the [Brownian zero set](../../../brownian-motion.md#brownian-zero-set), which has zero [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). It also tends to infinity. This is immediate for $\delta=1$; for $\delta>1$, recurrence and the [Strong Markov property](../../../markov-process.md#strong-markov-property) imply that the [Brownian occupation time](../../../brownian-motion.md#brownian-occupation-time) of, for example, $\{x:1<|x|<2\}$ is unbounded, while the integrand is bounded below there by $\delta^2$.

**Thus $A$ is continuous, strictly increasing, and maps $[0,\infty)$ onto itself. Its [inverse function](../../../function.md#inverse-function) $\tau_s=A^{-1}(s)$ is finite, continuous, and strictly increasing.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Part (b) shows that $s\mapsto\tau_s$ is finite and continuous. Since both $t\mapsto B_t$ and the [power function](../../../statistical-modelling.md#power-function-of-a-statistical-test) $x\mapsto|x|^\delta$ are continuous, their composition

$$
X_s=Y_{\tau_s}=|B_{\tau_s}|^\delta
$$

is continuous. This is an instance of a [time change of a continuous process](../../../stochastic-process.md#time-change-of-a-continuous-process).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

As printed, the requested conclusion is false for $\delta\ne1$. On an interval on which $X$ stays positive, the [time change of a continuous process](../../../stochastic-process.md#time-change-of-a-continuous-process) satisfies $d\tau_s=ds/(\delta^2X_s^{2(\delta-1)/\delta})$. The time-changed martingale term has [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $s$, so the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) identifies it with a standard Brownian motion $\widetilde B$. Dividing the drift in part (a) by the derivative of the clock gives

$$
\frac{\frac{\delta(\delta-1)}2X_s^{(\delta-2)/\delta}}{\delta^2X_s^{2(\delta-1)/\delta}}=\frac{\delta-1}{2\delta X_s}.
$$

Consequently the construction actually satisfies

$$
dX_s=\frac{\delta-1}{2\delta X_s}ds+d\widetilde B_s,
$$

which is the [Bessel process](../../../brownian-motion.md#bessel-process) equation of dimension $2-1/\delta$. It equals the paper's claimed drift $(\delta-1)/(2X_s)$ only when $\delta=1$. The mismatch between the specified power, clock, and conclusion is therefore a typographical error in the question.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

For the equation actually produced by the preceding construction, namely the [Bessel process](../../../brownian-motion.md#bessel-process) equation of dimension $2-1/\delta$, the drift has [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity) on every compact subset of $(0,\infty)$. Starting at any positive time and position, [pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) therefore makes the time-changed process agree until its first hit of zero with the [maximal local solution of a stochastic differential equation](../../../stochastic-calculus.md#maximal-local-solution-of-a-stochastic-differential-equation). For $\delta>1$, its dimension lies in $(1,2)$, so it can hit zero; the time-change construction then supplies further excursions, whereas the maximal local solution on $(0,\infty)$ stops at that first hit.

For $\delta=1$, $X_s=|B_s|$ is [Reflected Brownian motion](../../../brownian-motion.md#reflected-brownian-motion); away from zero it agrees with the maximal local solution of $dX=d\widetilde B$. For the dimension-$\delta$ equation printed in the paper, the preceding construction does not agree with the maximal local solution unless $\delta=1$, for the coefficient mismatch established in part (d).

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Let $Z=\{t:B_t=0\}$. Since $A$ is the clock from part (b) and $\tau=A^{-1}$,

$$
\{s:X_s=0\}=A(Z).
$$

For $\delta>1$, the [absolutely continuous function](../../../sobolev-space.md#absolutely-continuous-function) $A$ has derivative $A'(t)=\delta^2|B_t|^{2\delta-2}=0$ on $Z$. The one-dimensional area bound for an absolutely continuous function therefore gives

$$
\lambda(A(Z))\leq\int_ZA'(t)dt=0.
$$

For $\delta=1$, $A_t=t$ and the conclusion follows directly because the [Brownian zero set](../../../brownian-motion.md#brownian-zero-set) has zero [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Hence the zero set of $X$ has zero Lebesgue measure almost surely.

## 5

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

The relation $P\ll\widetilde P$ is an instance of [absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures): it means that every $\widetilde P$-null [event](../../../probability-theory.md#event) is also $P$-null,

$$
\widetilde P(A)=0\implies P(A)=0.
$$

By the [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem), this is equivalent to the existence of a nonnegative [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) $dP/d\widetilde P$ whose $\widetilde P$-expectation is one.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

For a continuous local martingale $M$ with $M_0=0$, its [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) is

$$
\mathcal E(M)_t=\exp\!\left(M_t-\frac12[M]_t\right).
$$

It is the unique solution of the [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) $dZ_t=Z_t\,dM_t$, $Z_0=1$, and is a nonnegative [local martingale](../../../martingale.md#local-martingale).

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

One continuous form of the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) is as follows. Let $M$ be a continuous local martingale under $P$, and suppose $Z=\mathcal E(M)$ is a true martingale on $[0,T]$. Define $Q$ by $dQ=Z_TdP$. Then every continuous $P$-local martingale $N$ becomes the continuous $Q$-local martingale

$$
\widetilde N_t=N_t-[N,M]_t.
$$

In particular, if $M_t=\int_0^t\theta_s\,dW_s$, then $\widetilde W_t=W_t-\int_0^t\theta_sds$ is a $Q$-Brownian motion.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Work first under [Wiener measure](../../../brownian-motion.md#wiener-measure) $P$ with coordinate [Brownian motion](../../../brownian-motion.md) $X$. Boundedness of $b$ implies the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition), so

$$
Z_T=\exp\!\left(\int_0^Tb(X_s)dX_s-\frac12\int_0^Tb(X_s)^2ds\right)
$$

has expectation one. Define $Q$ by $dQ=Z_TdP$. The [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) makes

$$
W_t=X_t-\int_0^tb(X_s)ds
$$

a $Q$-Brownian motion, and hence $(X,W,Q)$ is a [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation).

For [uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law), start with any weak solution under $Q$ and apply the inverse [change of measure](../../../measure-theory.md#change-of-measure) with density $\mathcal E(-\int b(X_s)dW_s)_T$. Boundedness again gives the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition), and under the resulting measure $P$ the process $X$ is Brownian. Reversing the density expresses the law of $X$ under $Q$ as the same functional $Z_T$ of a Wiener path. It is therefore independent of the chosen weak solution. This proves the [Weak existence and uniqueness in law for an additive-noise SDE with bounded drift](../../../stochastic-calculus.md#weak-existence-and-uniqueness-in-law-for-an-additive-noise-sde-with-bounded-drift).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

**False.** For a common sequence, each term of which is a refining deterministic [partition of an interval](../../../real-analysis.md#partition-of-an-interval), standard Brownian paths have [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) $t$ almost surely, whereas the paths $t\mapsto B_{2t}$ have quadratic variation $2t$ almost surely. These two path properties define disjoint measurable subsets of $C([0,1])$, so the two laws are [mutually singular measures](../../../measure-theory.md#mutually-singular-measures). In particular, the law of $B_{2\cdot}$ is not absolutely continuous with respect to [Wiener measure](../../../brownian-motion.md#wiener-measure). This is the [Pathwise quadratic variation distinguishes Brownian speeds](../../../stochastic-calculus.md#pathwise-quadratic-variation-distinguishes-brownian-speeds) argument.

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

**True.** Since $f\in C^1[0,1]$, it lies in the [Cameron-Martin space of Wiener measure](../../../brownian-motion.md#cameron-martin-space-of-wiener-measure). The [Cameron-Martin theorem](../../../brownian-motion.md#cameron-martin-theorem) says that the translated law is equivalent, and in particular absolutely continuous, with respect to [Wiener measure](../../../brownian-motion.md#wiener-measure). Its [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) is

$$
\boxed{\exp\!\left(\int_0^1f'(s)dB_s-\frac12\int_0^1f'(s)^2ds\right).}
$$

<h4 id="5/c/iii">iii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/c/iii)

**False for a general continuous $f$.** For example, take $f(t)=t^{1/3}$. The [Brownian Hölder regularity](../../../brownian-motion.md#brownian-holder-regularity) gives $B_t/t^{1/3}\to0$ almost surely as $t\downarrow0$, while

$$
\frac{B_t+f(t)}{t^{1/3}}\longrightarrow1
$$

almost surely. The original and translated path laws therefore concentrate on disjoint measurable events and are [mutually singular measures](../../../measure-theory.md#mutually-singular-measures).

More generally, the [Cameron-Martin theorem](../../../brownian-motion.md#cameron-martin-theorem) gives the exact criterion: translation by $f$ is absolutely continuous precisely when $f$ is an [absolutely continuous function](../../../sobolev-space.md#absolutely-continuous-function), $f(0)=0$, and $f'\in L^2[0,1]$.

## 6

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Fix $t>0$ and define $w(s,y)=u(t-s,|y|)$ for $0\leq s\leq t$. The assumed smooth extension and the [Neumann boundary condition](../../../differential-equation.md#neumann-boundary-condition) at zero make $w$ a $C^{1,2}$ function. The [heat equation](../../../diffusion-equation.md#heat-equation) gives

$$
w_s+\frac12w_{yy}=0.
$$

The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) therefore makes $w(s,B_s)$ a local martingale. Stop first when $|B|$ leaves a large compact interval. The exponential growth bound and the finite exponential moments of the maximum of [Brownian motion](../../../brownian-motion.md) on $[0,t]$ give [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability), so localization and the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) yield

$$
u(t,x)=w(0,x)=\mathbb E_x[w(t,B_t)]=\mathbb E_x[f(|B_t|)].
$$

This is the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) for the Neumann heat problem.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Let $p_t(z)=(2\pi t)^{-1/2}e^{-z^2/(2t)}$ be the [heat kernel](../../../diffusion-equation.md#heat-kernel) for $u_t=\frac12u_{xx}$. The symmetry of the [Gaussian distribution](../../../probability-theory.md#normal-distribution) gives the method-of-images formula

$$
v(t,x)=\int_0^\infty f(y)\bigl(p_t(x-y)+p_t(x+y)\bigr)dy.
$$

This is the [Neumann heat kernel on a half-line](../../../diffusion-equation.md#neumann-heat-kernel-on-a-half-line). [Differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) shows that $v\in C^{1,2}$ for $t,x>0$ and that $v_t=\frac12v_{xx}$. At $x=0$, the two differentiated kernel terms cancel, so $v_x(t,0)=0$. The [Gaussian approximate identity](../../../diffusion-equation.md#gaussian-approximate-identity) gives $v(t,x)\to f(x)$ as $t\downarrow0$, while the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives continuity up to $x=0$. Finally $|v(t,x)|\leq\lVert f\rVert_\infty$, which is stronger than the required exponential bound. Thus $v$ satisfies every condition in the displayed boundary-value problem.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Let $\rho=t\wedge\tau_0\wedge\tau_1$ and apply the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $u(t-s,B_s)$ for $0\leq s\leq\rho$. The [heat equation](../../../diffusion-equation.md#heat-equation) cancels the drift, so the stopped process is a bounded [martingale](../../../martingale.md). The [optional sampling theorem for a supermartingale](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives $u(t,x)=\mathbb E_x[u(t-\rho,B_\rho)]$. On the three mutually exclusive terminal events, the initial and [Dirichlet boundary conditions](../../../differential-equation.md#dirichlet-boundary-condition) identify this value as

$$
u(t,x)=\mathbb E_x\!\left[g(B_t)\mathbf1_{\{t<\tau_0\wedge\tau_1\}}+f_1(t-\tau_0)\mathbf1_{\{\tau_0<t\wedge\tau_1\}}+f_2(t-\tau_1)\mathbf1_{\{\tau_1<t\wedge\tau_0\}}\right].
$$

This is the [probabilistic representation of the heat equation with time-dependent Dirichlet data](../../../diffusion-equation.md#probabilistic-representation-of-the-heat-equation-with-time-dependent-dirichlet-data).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
