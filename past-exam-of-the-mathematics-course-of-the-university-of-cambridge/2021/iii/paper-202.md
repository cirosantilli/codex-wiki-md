# Paper 202

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_202.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_202.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
    - [iv](#5/a/iv)
      - [Solution](#5/a/iv/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $V(t)$ be the total variation of $f$ on $[0,t]$. The [Jordan decomposition of a function of bounded variation](../../../real-analysis.md#jordan-decomposition-of-a-function-of-bounded-variation) is

$$
g(t)=\frac{V(t)+f(t)}2,
\qquad
h(t)=\frac{V(t)-f(t)}2.
$$

For $s<t$, the inequality $V(t)-V(s)\geq|f(t)-f(s)|$ shows that both increments are nonnegative, so $g,h$ are nondecreasing and $f=g-h$. Right-continuity of the [finite variation](../../../real-analysis.md#total-variation-of-a-function) function $f$ implies right-continuity of $V$, and hence of $g,h$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

It suffices by part a to treat a nondecreasing right-continuous integrator, whose increments define a finite Lebesgue–Stieltjes measure $\mu_f$ on $[0,1]$. Let $\alpha_n$ be the left-endpoint step approximation on the dyadic intervals. The displayed sum is exactly

$$
\int_{(0,1]}\alpha_n\,d\mu_f.
$$

The [continuous function](../../../calculus.md#continuous-function) $\alpha$ is uniformly continuous on the compact interval, so $\|\alpha_n-\alpha\|_\infty\to0$. Therefore

$$
\left|\int(\alpha_n-\alpha)\,df\right|
\leq\|\alpha_n-\alpha\|_\infty V(1)\longrightarrow0.
$$

Apply this separately to $g$ and $h$ to obtain the asserted [Lebesgue-Stieltjes integral](../../../measure-theory.md#lebesgue-stieltjes-integration) limit.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For any partition of $[0,t]$,

$$
f(t)^2-f(0)^2
=2\sum_k f(t_{k-1})(f(t_k)-f(t_{k-1}))
+\sum_k(f(t_k)-f(t_{k-1}))^2.
$$

The final sum is at most the largest increment of $f$ times its total variation. It tends to zero because $f$ is uniformly continuous. Part b then gives the integration-by-parts identity

$$
2\int_0^tf(s)\,df(s)=f(t)^2-f(0)^2.
$$

**Thus the formula stated in the question holds when $f(0)=0$; for a general initial value the necessary endpoint correction is $-f(0)^2$.**

## 2

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The elementary discrete integration-by-parts identity is

$$
[X]^{(n)}_t=X_t^2-2M_t^{(n)}.
$$

By the supplied fact, $M^{(n)}\to M$ in $L^2$ of the uniform norm. Define

$$
[X]_t=X_t^2-2M_t.
$$

Then

$$
\mathbb E\sup_{t\geq0}|[X]^{(n)}_t-[X]_t|^2
=4\mathbb E\sup_{t\geq0}|M_t^{(n)}-M_t|^2\longrightarrow0,
$$

which proves i, while

$$
X^2-[X]=2M
$$

is an $L^2$-bounded martingale, proving ii.

Choose a subsequence converging uniformly almost surely. For $s<t$, all complete dyadic increments between $s$ and $t$ contribute nonnegative squares; only the two boundary increments can affect monotonicity, and they vanish uniformly by continuity of $X$. Passing to the limit gives $[X]_s\leq[X]_t$. Thus $[X]$ is nondecreasing and is the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) of $X$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Choose stopping times $T_m\uparrow\infty$ such that $X^{T_m}$ is a bounded martingale. Part a constructs $[X^{T_m}]$. Uniqueness in the identity

$$
(X^{T_m})^2-[X^{T_m}]\text{ is a local martingale}
$$

shows consistency on overlapping stopped intervals, so define $[X]_{t\wedge T_m}=[X^{T_m}]_t$. The stopped dyadic sums converge uniformly on every compact interval in probability, and

$$
X^2-[X]
$$

is a local martingale. This localization constructs the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) of every continuous [local martingale](../../../martingale.md#local-martingale).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Letting $t\to\infty$ in the [Burkholder-Davis-Gundy inequalities](../../../martingale.md#burkholder-davis-gundy-inequalities) with exponent two gives absolute constants $c,C>0$ such that

$$
c\,\mathbb E[X]_\infty
\leq\mathbb E\sup_{t\geq0}|X_t|^2
\leq C\,\mathbb E[X]_\infty.
$$

Since $[X]$ is nondecreasing, $\mathbb E[X]_\infty=\sup_t\mathbb E[X]_t$. Thus one of the two quantities in the question is finite exactly when the other is.

## 3

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Apply [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $\phi(x)=x\log x$. Since $\phi''(x)=1/x$,

$$
M_1\log M_1-M_0\log M_0
=\int_0^1(1+\log M_t)\,dM_t
+\frac12\int_0^1\frac{d[M]_t}{M_t}.
$$

Boundedness of $\log M$ makes the stochastic integral a true martingale of mean zero. Taking expectations proves

$$
\boxed{\mathbb E(M_1\log M_1)=\mathbb E(M_0\log M_0)+\frac12\mathbb E\int_0^1\frac{d[M]_t}{M_t}}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The heat-semigroup form is $U(t,x)=P_{1-t}(f^2)(x)$. For $s<t$, independence and additivity of Brownian increments give

$$
\begin{aligned}
\mathbb E[U(t,W_t)\mid\mathcal F_s^W]
&=\mathbb E[f(W_t+B_{1-t})^2\mid\mathcal F_s^W]\\
&=\mathbb E[f(W_s+\widetilde B_{1-s})^2\mid\mathcal F_s^W]\\
&=U(s,W_s),
\end{aligned}
$$

where $\widetilde B_{1-s}$ is an independent $N(0,1-s)$ increment. Thus $M_t=U(t,W_t)$ is a [martingale](../../../martingale.md).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The backward heat equation and [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) give

$$
dM_t=U_x(t,W_t)\,dW_t,
\qquad
d[M]_t=U_x(t,W_t)^2dt.
$$

Moreover $M_1=f(W_1)^2$ and $M_0=\mathbb E f(W_1)^2$. Substitution into part a yields

$$
\boxed{
\mathbb E[f(W_1)^2\log f(W_1)^2]
=\mathbb E[f(W_1)^2]\log\mathbb E[f(W_1)^2]
+\frac12\mathbb E\int_0^1\frac{U_x(t,W_t)^2}{U(t,W_t)}\,dt.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The supplied derivative identity and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
U_x(t,x)^2
\leq4U(t,x)\,\mathbb E[f'(x+B_{1-t})^2].
$$

Therefore

$$
\frac12\mathbb E\int_0^1\frac{U_x(t,W_t)^2}{U(t,W_t)}dt
\leq2\int_0^1\mathbb E[f'(W_t+B_{1-t})^2]dt.
$$

The sum $W_t+B_{1-t}$ is standard normal for every $t$, so the right side is $2\mathbb E f'(W_1)^2$. Part c proves the [Gaussian logarithmic Sobolev inequality](../../../probability-inequality.md#gaussian-logarithmic-sobolev-inequality)

$$
\boxed{
\mathbb E[f(W_1)^2\log f(W_1)^2]
\leq\mathbb E[f(W_1)^2]\log\mathbb E[f(W_1)^2]
+2\mathbb E[f'(W_1)^2].}
$$

## 4

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Continuity gives $X_{\tau_a}=a$ on $\{\tau_a<\infty\}$. The stopped process $X^{\tau_a}$ is bounded by $a$ and is therefore a true martingale. Hence

$$
1=\mathbb E X_{t\wedge\tau_a}
=a\mathbb P(\tau_a\leq t)+\mathbb E[X_t\mathbf1_{\{\tau_a>t\}}].
$$

The second term tends to zero by bounded convergence because $X_t\to0$ and it is bounded by $a$. Thus

$$
\boxed{\mathbb P(\tau_a<\infty)=\mathbb P(\sup_{t\geq0}X_t>a)=\frac1a}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Dambis-Dubins-Schwarz theorem](../../../martingale.md#dambis-dubins-schwarz-theorem) says that there is Brownian motion $W$ such that

$$
M_t=W_{[M]_t}.
$$

When $[M]$ is strictly increasing, define its inverse

$$
T_s=\inf\{t:[M]_t>s\}
$$

and set $W_s=M_{T_s}$. Optional sampling shows that $W$ is a continuous local martingale, while time change gives $[W]_s=s$. The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) makes $W$ Brownian, and inverse time change gives the displayed representation.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Set $s=[M]_t$. By hypothesis $s\to\infty$, and part b gives

$$
M_t-\frac12[M]_t=W_s-\frac s2
=s\left(\frac{W_s}s-\frac12\right).
$$

Since $W_s/s\to0$ almost surely, the expression tends to $-\infty$ almost surely.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [Doléans-Dade exponential](../../../stochastic-calculus.md#doleans-dade-exponential)

$$
X_t=\exp\left(M_t-\frac12[M]_t\right)
$$

is a positive continuous local martingale with $X_0=1$, and part c shows $X_t\to0$. Apply part a with $a=e^y$:

$$
\boxed{
\mathbb P\left(\sup_{t\geq0}\left\{M_t-\frac12[M]_t\right\}>y\right)
=\mathbb P(\sup_tX_t>e^y)=e^{-y}.}
$$

## 5

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

A weak solution consists of a filtered probability space carrying a Brownian motion $W$ and an adapted continuous process $X$ satisfying

$$
X_t=X_0+\int_0^tb(X_s)ds+\int_0^t\sigma(X_s)dW_s.
$$

The probability space and Brownian motion are part of the unknown solution.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

A strong solution is adapted to the augmented filtration generated by a prescribed Brownian motion and initial condition; equivalently, it is constructed measurably from that given noise.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Uniqueness in law means that any two weak solutions with the same initial distribution have the same probability distribution on path space.

<h4 id="5/a/iv">iv</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/a/iv)

Pathwise uniqueness means that two solutions on the same filtered space, driven by the same Brownian motion and with the same initial value, are indistinguishable.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Define the [scale function of a one-dimensional diffusion](../../../stochastic-calculus.md#scale-function-stochastic-processes)

$$
g(x)=\int_0^x\exp\left(-2\int_0^yb(z)dz\right)dy.
$$

Then $g'>0$, so $g$ is strictly increasing, and

$$
\frac12g''+bg'=0.
$$

By [Itô formula](../../../stochastic-calculus.md#ito-s-lemma),

$$
dY_t=d(g(X_t))=g'(X_t)dW_t,
$$

so $Y=g(X)$ is a [local martingale](../../../martingale.md#local-martingale).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Let

$$
h(y)=g'(g^{-1}(y)).
$$

Differentiating and using the scale equation gives

$$
h'(y)=\frac{g''(x)}{g'(x)}=-2b(x),
\qquad x=g^{-1}(y).
$$

Since $b$ is bounded, $h$ has global [Lipschitz continuity](../../../real-analysis.md#lipschitz-continuity). Thus

$$
dY_t=h(Y_t)dW_t
$$

has a pathwise unique strong solution by the standard Lipschitz existence-and-uniqueness theorem for a [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation). Applying the deterministic inverse $g^{-1}$ gives a strong solution $X$, and uniqueness of $Y$ gives pathwise uniqueness of $X$.

## 6

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

An $x$-admissible strategy is a predictable vector of holdings $\phi=(\phi^0,\ldots,\phi^d)$ that is integrable against the asset prices, is [self-financing](../../../mathematical-finance.md#self-financing-portfolio), has initial wealth

$$
V_0=\sum_i\phi_0^iS_0^i=x,
$$

and whose wealth process $V_t=\sum_i\phi_t^iS_t^i$ remains nonnegative.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

An [arbitrage](../../../mathematical-finance.md#arbitrage) is a zero-initial-wealth admissible self-financing strategy with $V_T\geq0$ almost surely and $\mathbb P(V_T>0)>0$ for some finite horizon $T$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Write $\mu_t=(\mu_t^{(1)},\ldots,\mu_t^{(d)})^T$ and define the market price of risk

$$
\theta_t=\sigma_t^{-1}(\mu_t-r_t\mathbf1).
$$

It is bounded by hypothesis. The stochastic exponential

$$
Z_t=\exp\left(-\int_0^t\theta_s^T dW_s-\frac12\int_0^t|\theta_s|^2ds\right)
$$

is a true martingale by the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition). Define the equivalent measure $Q$ by $dQ=Z_TdP$. The [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) makes

$$
W_t^Q=W_t+\int_0^t\theta_sds
$$

a Brownian motion under $Q$. After discounting by the bank account, every risky price has zero drift and is a $Q$-local martingale.

The discounted wealth of an admissible self-financing strategy is a nonnegative local martingale and hence a [supermartingale](../../../martingale.md#supermartingale). If an arbitrage existed, its zero initial value would imply nonpositive expected terminal discounted wealth under $Q$, while that wealth is nonnegative and positive with positive $Q$-probability. This contradiction proves that the market has no arbitrage; it is the needed direction of the [equivalent local martingale measure](../../../mathematical-finance.md#equivalent-local-martingale-measure) criterion.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Let $X$ be a positive strict local martingale solving

$$
dX_t=X_t^2dW_t,
$$

and fix $T>0$. Use the bank account $S^0=1$ and two risky assets

$$
S_t^1=X_t,
\qquad
S_t^2=\mathbb E[X_T\mid\mathcal F_t],
\qquad0\leq t\leq T.
$$

Both discounted prices are nonnegative local martingales under the physical measure itself, so the same supermartingale argument as in part c rules out arbitrage. At maturity,

$$
S_T^1=X_T=S_T^2.
$$

But strictness means $\mathbb E[X_T\mid\mathcal F_t]<X_t$ for some earlier $t$ on a set of positive probability, so the two prices are not indistinguishable before $T$. This no-arbitrage market violates the Law of One Price.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
