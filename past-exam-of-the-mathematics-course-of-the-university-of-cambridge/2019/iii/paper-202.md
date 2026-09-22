# Paper 202

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_202.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_202.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [Solution](#1/1/solution)
    - [2](#1/1/2)
      - [Solution](#1/1/2/solution)
    - [3](#1/1/3)
      - [Solution](#1/1/3/solution)
    - [4](#1/1/4)
      - [Solution](#1/1/4/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
    - [3](#2/2/3)
      - [Solution](#2/2/3/solution)
- [3](#3)
  - [1](#3/1)
    - [Solution](#3/1/solution)
  - [2](#3/2)
    - [Solution](#3/2/solution)
  - [3](#3/3)
    - [Solution](#3/3/solution)
    - [4](#3/3/4)
      - [Solution](#3/3/4/solution)
- [4](#4)
  - [1](#4/1)
    - [Solution](#4/1/solution)
  - [2](#4/2)
    - [Solution](#4/2/solution)
  - [3](#4/3)
    - [Solution](#4/3/solution)
- [5](#5)
  - [1](#5/1)
    - [Solution](#5/1/solution)
  - [2](#5/2)
    - [Solution](#5/2/solution)
  - [3](#5/3)
    - [Solution](#5/3/solution)
- [6](#6)
  - [1](#6/1)
    - [Solution](#6/1/solution)
  - [2](#6/2)
    - [Solution](#6/2/solution)
  - [3](#6/3)
    - [Solution](#6/3/solution)

## 1

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Let $(\tau_n)$ be a [localizing sequence](../../../martingale.md#localizing-sequence) for $M$. For $s\leq t$, the [optional sampling theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives

$$
\mathbb E[M_{t\wedge\tau_n}\mid\mathcal F_s]=M_{s\wedge\tau_n}.
$$

Both sides converge almost surely to $M_t$ and $M_s$, and $|M_{u\wedge\tau_n}|\leq Z$. Conditional dominated convergence therefore yields $\mathbb E[M_t\mid\mathcal F_s]=M_s$, so $M$ is a [martingale](../../../martingale.md). Moreover, the family $(M_t)_{t\geq0}$ is dominated by the integrable random variable $Z$, hence is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability). Thus **$M$ is a uniformly integrable martingale**.

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/solution">Solution</h5>

↑ **Parent:** [2](#1/1/2)

Put $A_t=\int_0^tH_s^2ds$. It is continuous and tends to infinity almost surely, so $A_{T_\sigma}=\sigma^2$. Define the right-continuous inverse $T(u)=\inf\{t:A_t>u\}$ and

$$
W_u=\int_0^{T(u)}H_s\,dB_s.
$$

The time-change theorem for local martingales shows that $W$ is a continuous local martingale in the time-changed filtration, and

$$
\langle W\rangle_u=A_{T(u)}=u.
$$

For completeness, this proves the required case of the [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem): for every $\theta\in\mathbb R$, [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) makes $\exp(i\theta W_u+\theta^2u/2)$ a local martingale; stopping and conditioning show that $W_v-W_u$ has conditional characteristic function $e^{-\theta^2(v-u)/2}$. Hence the increments are independent centered normal variables with the Brownian variances, and continuity makes $W$ a [Brownian motion](../../../brownian-motion.md). Consequently

$$
X_\sigma=W_{\sigma^2}\sim N(0,\sigma^2).
$$

Thus **$X_\sigma$ is centered Gaussian with variance $\sigma^2$**.

<h4 id="1/1/3">3</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/3/solution">Solution</h5>

↑ **Parent:** [3](#1/1/3)

For $\theta>0$, the [Exponential martingale for Brownian motion](../../../brownian-motion.md#exponential-martingale-for-brownian-motion) and the [Doob maximal inequality for a nonnegative submartingale](../../../martingale.md#doob-maximal-inequality-for-a-nonnegative-submartingale) give

$$
\mathbb P\left(\sup_{t\leq s}B_t\geq a\right)
\leq\exp\left(-\theta a+\frac12\theta^2s\right).
$$

Taking $\theta=a/s$ gives $e^{-a^2/(2s)}$. Apply the same argument to $-B$ and use the [union bound](../../../probability-inequality.md#boole-s-inequality):

$$
\boxed{\mathbb P\left(\sup_{t\leq s}|B_t|\geq a\right)
\leq2e^{-a^2/(2s)}.}
$$

<h4 id="1/1/4">4</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/4/solution">Solution</h5>

↑ **Parent:** [4](#1/1/4)

[Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
dM_t=M_t\nabla f(B_t)\cdot dB_t,
$$

so $M$ is a positive [local martingale](../../../martingale.md#local-martingale). On every finite interval $[0,T]$, the hypotheses imply

$$
\int_0^T|\nabla f(B_s)|^2ds
\leq C_T\left(1+\sup_{s\leq T}|B_s|^{2-\epsilon}\right).
$$

The [Gaussian tail bound](../../../probability-and-statistics.md#gaussian-tail-bound) of the Brownian maximum has finite exponential moments of every subquadratic power. Therefore [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds on $[0,T]$, and the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) $M$ is a true martingale there. Since $T$ was arbitrary, **$M$ is a true martingale**.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

Write $\Delta_iM=M_{t_i}-M_{t_{i-1}}$ and $Q=\sum_i(\Delta_iM)^2$. The identity

$$
Q=M_t^2-M_0^2-2\sum_iM_{t_{i-1}}\Delta_iM
$$

shows, using the [martingale-difference orthogonality](../../../martingale.md#martingale-difference-orthogonality), that

$$
\begin{aligned}
\mathbb E[Q^2]
&\leq2\mathbb E[(M_t^2-M_0^2)^2]
 +8\mathbb E\left[\left(\sum_iM_{t_{i-1}}\Delta_iM\right)^2\right]\\
&\leq2C^4+8C^2\mathbb E[Q].
\end{aligned}
$$

Also $\mathbb E[Q]=\mathbb E[M_t^2]-\mathbb E[M_0^2]\leq C^2$. Hence $\mathbb E[Q^2]\leq10C^4$, which in particular proves the requested bound

$$
\boxed{\mathbb E[Q^2]\leq48C^4.}
$$

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

Because $\|b'\|_\infty<\infty$, the function $b$ is [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity). the [Picard-Lindelöf theorem](../../../differential-equation.md#picard-lindelof-theorem), proved by iteration on

$$
x^{(0)}(t)=x_0+w(t),\qquad
x^{(n+1)}(t)=x_0+w(t)+\int_0^tb(x^{(n)}(s))ds
$$

converges uniformly on every compact interval. The usual factorial estimate proves convergence for arbitrary interval length, and the [Gronwall inequality](../../../probability-and-statistics.md#gronwall-inequality) proves uniqueness. Thus there is a unique global continuous solution.

For $w=W$, induction shows that $X_t^{(n)}$ is $\mathcal F_t$-measurable: its value uses only $(W_s)_{s\leq t}$ and earlier iterates up to time $t$. The pointwise limit $X_t$ is therefore $\mathcal F_t$-measurable. Hence **$X$ is adapted to $(\mathcal F_t)$**.

<h4 id="2/2/3">3</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/3/solution">Solution</h5>

↑ **Parent:** [3](#2/2/3)

Let $\tau_n$ be the first exit from a compact interval on which $H<n$, chosen so that $\tau_n\uparrow T$, and let $m=\inf H> -\infty$. By [Itô formula](../../../stochastic-calculus.md#ito-s-lemma),

$$
dH(X_t)=H'(X_t)dB_t+\left(\frac12H''(X_t)-H'(X_t)^2\right)dt.
$$

The assumption gives the drift bound $\frac12H''-(H')^2\leq C$. After stopping,

$$
\mathbb E[H(X_{t\wedge\tau_n})]\leq H(x)+Ct.
$$

If $h_n=\inf\{H(y):y\text{ lies outside the }n\text{th compact interval}\}$, then $h_n\to\infty$ because $H$ is [coercive](../../../linear-algebra.md#coercive-bilinear-form), and

$$
(h_n-m)\mathbb P(\tau_n\leq t)
\leq H(x)+Ct-m.
$$

Thus $\mathbb P(T\leq t)=0$ for every $t$, and **$T=\infty$ almost surely**.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/solution">Solution</h4>

↑ **Parent:** [1](#3/1)

For an SDE driven by Brownian motion, a [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) is adapted to the completed filtration generated by a prescribed Brownian motion and satisfies the equation on that space. A [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) consists of a probability space, filtration, Brownian motion, and adapted solution satisfying the equation. [Uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law) means that any two weak solutions with the same initial law have the same law as processes. [Pathwise uniqueness](../../../stochastic-calculus.md#pathwise-uniqueness) means that two solutions on the same filtered space, driven by the same Brownian motion and having the same initial value, are indistinguishable.

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/solution">Solution</h4>

↑ **Parent:** [2](#3/2)

Since $B_{T_a}=0$, applying [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $B_t^3$ after $T_a$ gives

$$
dX_t=3B_t\,dt+3B_t^2\,dB_t
=3\operatorname{sign}(X_t)|X_t|^{1/3}dt+3|X_t|^{2/3}dB_t.
$$

Before $T_a$, both sides vanish. Since $T_a$ is a stopping time determined by $B$, this is a [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation).

Taking $a=0$ gives $X_t=B_t^3$, whereas any $a>0$ gives a solution that remains zero until $T_a$; these differ with positive probability while using the same Brownian motion and initial value. Therefore **pathwise uniqueness fails**.

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/solution">Solution</h4>

↑ **Parent:** [3](#3/3)

One form of the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) is the following. For bounded sufficiently regular $f,V$ and

$$
u(t,x)=\mathbb E_x\left[
 e^{-\int_0^tV(B_s)ds}f(B_t)
\right],
$$

one has

$$
\partial_tu=\frac12\Delta u-Vu,
\qquad u(0,x)=f(x).
$$

Conversely, a bounded classical solution has this representation. To prove it, fix $t$ and apply [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to

$$
e^{-\int_0^sV(B_r)dr}u(t-s,B_s),\qquad0\leq s\leq t.
$$

The PDE cancels its drift. The remaining stochastic integral is a martingale, so taking expectations at $s=0,t$ gives the representation; the converse follows by the same calculation and uniqueness for the parabolic boundary-value problem.

<h4 id="3/3/4">4</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/4/solution">Solution</h5>

↑ **Parent:** [4](#3/3/4)

Apply the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula) with $V(x)=\sigma x$ and terminal function $1$. The ansatz $u(t,x)=e^{A(t)x+C(t)}$ gives

$$
A'=-\sigma,\qquad C'=\frac12A^2,qquad A(0)=C(0)=0.
$$

Thus $A(t)=-\sigma t$ and $C(t)=\sigma^2t^3/6$, so

$$
\boxed{\mathbb E_x\exp\left(-\sigma\int_0^tB_sds\right)
=\exp\left(-\sigma tx+\frac{\sigma^2t^3}{6}\right).}
$$

Equivalently, the [Integral of Brownian motion](../../../brownian-motion.md#integral-of-brownian-motion) is Gaussian with mean $xt$ and variance $t^3/3$.

<h2 id="4">4</h2>

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="4/1">1</h3>

↑ **Parent:** [4](#4)

<h4 id="4/1/solution">Solution</h4>

↑ **Parent:** [1](#4/1)

For every real $\lambda$, the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) of $\lambda(M-M_s)+(N-N_s)$ on $[s,t]$ is nonnegative:

$$
\lambda^2\Delta\langle M\rangle
+2\lambda\Delta\langle M,N\rangle
+\Delta\langle N\rangle\geq0.
$$

Its discriminant is therefore nonpositive. This gives the pathwise [Kunita-Watanabe inequality](../../../stochastic-calculus.md#kunita-watanabe-inequality)

$$
\boxed{|\langle M,N\rangle_t-\langle M,N\rangle_s|
\leq\sqrt{\langle M\rangle_t-\langle M\rangle_s}
\sqrt{\langle N\rangle_t-\langle N\rangle_s}.}
$$

<h3 id="4/2">2</h3>

↑ **Parent:** [4](#4)

<h4 id="4/2/solution">Solution</h4>

↑ **Parent:** [2](#4/2)

Let $W$ be a Brownian motion, set $X=W$, and define

$$
B_t=\int_0^t\operatorname{sign}(W_s)dW_s.
$$

This is a continuous local martingale with quadratic variation $t$, hence is Brownian by the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion). Since $\operatorname{sign}^2=1$,

$$
dX_t=dW_t=\operatorname{sign}(X_t)dB_t,
$$

which gives a weak solution.

Suppose a strong solution existed. It has quadratic variation $t$, so $X$ itself is Brownian. The supplied [Tanaka formula](../../../stochastic-calculus.md#tanaka-s-formula) gives $|X_t|=B_t+L_t$, and $L$ is adapted to the completed filtration of $|X|$. Hence $B$ and $|X|$ generate the same completed filtration. Strongness would make $X$, and therefore $\operatorname{sign}(X_t)$, measurable with respect to the history of $|X|$. But a Brownian excursion has an independent symmetric sign; in particular, conditionally on the reflected Brownian path, the sign at a fixed nonzero time is not measurable. This contradiction proves that **no strong solution exists**.

<h3 id="4/3">3</h3>

↑ **Parent:** [4](#4)

<h4 id="4/3/solution">Solution</h4>

↑ **Parent:** [3](#4/3)

The solution is the [geometric Brownian motion](../../../stochastic-calculus.md#geometric-brownian-motion)

$$
X_t=x\exp\left((\beta-\tfrac12\sigma^2)t+\sigma B_t\right)>0.
$$

Its [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) is

$$
Lf(x)=\beta xf'(x)+\frac12\sigma^2x^2f''(x).
$$

For $\gamma=1-2\beta/\sigma^2\ne0$, one has $L(x^\gamma)=0$. Optional stopping of $X_{t\wedge T_r\wedge T_R}^\gamma$ and the boundary values therefore give

$$
\boxed{\mathbb P_x(T_r<T_R)=
\frac{R^\gamma-x^\gamma}{R^\gamma-r^\gamma},
\qquad \gamma=1-\frac{2\beta}{\sigma^2}.}
$$

## 5

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="5/1">1</h3>

↑ **Parent:** [5](#5)

<h4 id="5/1/solution">Solution</h4>

↑ **Parent:** [1](#5/1)

A [simple predictable process](../../../martingale.md#simple-predictable-process) has the form

$$
H_s=\sum_{i=0}^{n-1}\xi_i\mathbf1_{(t_i,t_{i+1}]}(s),
$$

where each bounded $\xi_i$ is $\mathcal F_{t_i}$-measurable. Define

$$
(H\mathbin\cdot B)_t
=\sum_i\xi_i(B_{t\wedge t_{i+1}}-B_{t\wedge t_i}).
$$

Independent centered Brownian increments show directly by conditioning that this is a martingale. The same conditional expansion, using $\mathbb E[(B_v-B_u)^2\mid\mathcal F_u]=v-u$, shows that

$$
\boxed{(H\mathbin\cdot B)_t^2-\int_0^tH_s^2ds
\text{ is a martingale}.}
$$

<h3 id="5/2">2</h3>

↑ **Parent:** [5](#5)

<h4 id="5/2/solution">Solution</h4>

↑ **Parent:** [2](#5/2)

Since $B_t=\int_0^t1\,dB_s$, the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) and polarization give

$$
\boxed{\mathbb E\left[B_t\int_0^tf(s)dB_s\right]
=\int_0^t1\cdot f(s)ds
=\int_0^tf(s)ds.}
$$

<h3 id="5/3">3</h3>

↑ **Parent:** [5](#5)

<h4 id="5/3/solution">Solution</h4>

↑ **Parent:** [3](#5/3)

With $A_t=\int_0^t\mu(s)ds$, the product rule gives

$$
d(e^{-A_t}X_t)=e^{-A_t}X_t\sigma(t)dB_t,
$$

so $X_te^{-A_t}$ is a local martingale under $\mathbb P$.

Set $\theta(t)=\mu(t)/\sigma(t)$. This is bounded and compactly supported, so [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds and

$$
Z_\infty=\exp\left(-\int_0^\infty\theta(s)dB_s
-\frac12\int_0^\infty\theta(s)^2ds\right)
$$

defines a probability measure $d\mathbb Q=Z_\infty d\mathbb P$. By the [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem), $W_t=B_t+\int_0^t\theta(s)ds$ is Brownian under $\mathbb Q$, and

$$
dX_t=X_t\sigma(t)dW_t.
$$

Thus **$X$ is a local martingale under $\mathbb Q$**.

## 6

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="6/1">1</h3>

↑ **Parent:** [6](#6)

<h4 id="6/1/solution">Solution</h4>

↑ **Parent:** [1](#6/1)

A continuous finite-variation path has zero [quadratic variation](../../../stochastic-calculus.md#quadratic-variation). Hence a continuous finite-variation martingale $M$ satisfies $\langle M\rangle=0$. After localizing to make it square-integrable,

$$
\mathbb E[(M_t-M_0)^2]=\mathbb E[\langle M\rangle_t]=0.
$$

Letting the localization level tend to infinity shows that **$M_t=M_0$ for every $t$ almost surely**; continuity makes the equality simultaneous in $t$.

<h3 id="6/2">2</h3>

↑ **Parent:** [6](#6)

<h4 id="6/2/solution">Solution</h4>

↑ **Parent:** [2](#6/2)

Write $Z_t=\int_0^te^{-B_s}d\widetilde B_s$, so $X_t=e^{B_t}Z_t$. Independence gives $\langle B,\widetilde B\rangle=0$, and [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) yields

$$
dX_t=\frac12X_tdt+X_tdB_t+d\widetilde B_t.
$$

The martingale part has quadratic variation $(1+X_t^2)dt$, so on an enlarged description it equals $\sqrt{1+X_t^2}\,dW_t$. Thus $X$ is a weak solution of

$$
dU_t=\frac12U_tdt+\sqrt{1+U_t^2}\,dW_t,qquad U_0=0.
$$

On the other hand, another application of Itô's formula gives

$$
dY_t=\frac12Y_tdt+\cosh(B_t)dB_t
=\frac12Y_tdt+\sqrt{1+Y_t^2}\,dB_t.
$$

Both coefficients are [Lipschitz continuous](../../../real-analysis.md#lipschitz-continuity), so [uniqueness in law](../../../stochastic-calculus.md#uniqueness-in-law) gives **$X$ and $Y$ the same law**.

<h3 id="6/3">3</h3>

↑ **Parent:** [6](#6)

<h4 id="6/3/solution">Solution</h4>

↑ **Parent:** [3](#6/3)

The [variation-of-constants formula](../../../functional-analysis.md#variation-of-constants-formula) gives, when $a\ne0$,

$$
X_t=e^{-at}x+\frac ba(1-e^{-at})
+\sigma\int_0^te^{-a(t-u)}dB_u.
$$

Therefore, with $m=\min(s,t)$,

$$
\begin{aligned}
\operatorname{cov}(X_t,X_s)
&=\sigma^2\int_0^me^{-a(t-u)}e^{-a(s-u)}du\\
&=\boxed{\frac{\sigma^2}{2a}
\left(e^{-a|t-s|}-e^{-a(t+s)}\right)}.
\end{aligned}
$$

If $a=0$, then $X_t=x+bt+\sigma B_t$ and

$$
\boxed{\operatorname{cov}(X_t,X_s)=\sigma^2\min(t,s).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
