# Paper 202

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20202.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20202.pdf)

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
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Apply [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $Z_t^{(A)}=\exp(A X_t-A^2t/2)$. Its [semimartingale decomposition](../../../stochastic-calculus.md#semimartingale-decomposition) is

$$
dZ_t^{(A)}=A Z_t^{(A)}\,dX_t
+\frac{A^2}{2}Z_t^{(A)}\bigl(d[X]_t-dt\bigr).
$$

The second term is a continuous [finite-variation process](../../../stochastic-calculus.md#finite-variation-process). Since $Z^{(A)}$ is assumed to be a [local martingale](../../../martingale.md#local-martingale), uniqueness of the semimartingale decomposition makes this term identically zero. Both $A$ and $Z^{(A)}$ are nonzero, so the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) of $X$ is $[X]_t=t$.

The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) now says that $X_t-X_0$ is a [Brownian motion](../../../brownian-motion.md). Consequently

$$
Z_t^{(a)}=e^{aX_0}
\exp\!\left(a(X_t-X_0)-\frac{a^2t}{2}\right)
$$

is a constant multiple of an [exponential Brownian martingale](../../../brownian-motion.md#exponential-brownian-martingale). It is therefore a true martingale for every $a\in\mathbb R$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Set $K_t=\sqrt{H_t}$ and define the [stochastic integral](../../../stochastic-calculus.md#stochastic-integral)

$$
W_t=\int_0^t\frac1{\sqrt{H_s}}\,dX_s.
$$

Strict positivity and predictability of $H$ make the integrand locally admissible. The process $W$ is a continuous local martingale starting from zero, and the [quadratic variation of a stochastic integral](../../../stochastic-calculus.md#quadratic-variation-of-a-stochastic-integral) gives

$$
[W]_t=\int_0^t\frac1{H_s}\,d[X]_s
=\int_0^t\frac1{H_s}H_s\,ds=t.
$$

By the [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion), $W$ is a Brownian motion. The [associativity of stochastic integration](../../../stochastic-calculus.md#associativity-of-stochastic-integration) then yields

$$
\int_0^tK_s\,dW_s
=\int_0^t\sqrt{H_s}\frac1{\sqrt{H_s}}\,dX_s
=X_t-X_0,
$$

which is the required representation.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use first the test function $f(x)=x$. The assumed [martingale problem](../../../stochastic-calculus.md#martingale-problem) says that

$$
Y_t=X_t-X_0-\int_0^t b(X_s)\,ds
$$

is a continuous local martingale. Next use $f(x)=x^2$ to see that

$$
X_t^2-X_0^2-\int_0^t\bigl(2X_sb(X_s)+\sigma(X_s)^2\bigr)\,ds
$$

is a local martingale. On the other hand, [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) applied to $X=X_0+\int b(X_s)ds+Y$ shows that

$$
X_t^2-X_0^2-\int_0^t2X_sb(X_s)\,ds-[Y]_t
$$

is a local martingale. Their difference is both a continuous local martingale and a finite-variation process, so

$$
[Y]_t=\int_0^t\sigma(X_s)^2\,ds.
$$

Part (b), with $H_s=\sigma(X_s)^2>0$, supplies a Brownian motion $W$ such that

$$
Y_t=\int_0^t\sigma(X_s)\,dW_s.
$$

Therefore

$$
X_t=X_0+\int_0^t b(X_s)\,ds+\int_0^t\sigma(X_s)\,dW_s,
$$

so $X$ is a [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) to the stated equation.

## 2

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $(X_n)$ be [Cauchy](../../../real-analysis.md#cauchy-sequence) in the norm

$$
\lVert X\rVert=\mathbb E\sup_{t\geq0}|X_t|.
$$

Choose a subsequence $(X_{n_k})$ for which

$$
\sum_{k=1}^{\infty}\lVert X_{n_{k+1}}-X_{n_k}\rVert<\infty.
$$

[Tonelli theorem](../../../measure-theory.md#tonelli-theorem) implies

$$
\sum_k\sup_{t\geq0}|X_{n_{k+1}}(t)-X_{n_k}(t)|<\infty
$$

almost surely. The subsequence therefore converges uniformly on $[0,\infty)$, outside one null event, to a continuous process $X$. For each $t$, $X_t$ is the almost-sure limit of $\mathcal F_t$-measurable variables; completeness of the filtration makes the chosen version adapted. The same summable bound and [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) show that $\mathbb E\sup_t|X_t|<\infty$ and that $X_{n_k}\to X$ in norm.

Since the original sequence is Cauchy, the usual triangle argument upgrades convergence of the subsequence to $X_n\to X$ in norm. Thus the space of indistinguishability classes is a [Banach space](../../../banach-space.md).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix a deterministic horizon $T$ and $\varepsilon>0$. For every localization index $N$,

$$
\mathbb P\!\left(\sup_{t\leq T}|X_n(t)-X(t)|>\varepsilon\right)
\leq \mathbb P(T_N\leq T)
+\frac1\varepsilon\lVert X_n^{T_N}-X^{T_N}\rVert
$$

by [Markov inequality](../../../probability-inequality.md#markov-inequality). Because $T_N\uparrow\infty$ almost surely, the first term tends to zero as $N\to\infty$. For fixed $N$, the second tends to zero as $n\to\infty$. Taking first the limit superior in $n$ and then $N\to\infty$ proves

$$
\sup_{t\leq T}|X_n(t)-X(t)|\longrightarrow0
$$

in probability. This is precisely [uniform convergence on compacts in probability](../../../stochastic-process.md#uniform-convergence-on-compacts-in-probability).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the [continuous semimartingale decomposition](../../../stochastic-calculus.md#continuous-semimartingale-decomposition) $X=X_0+M+A$, where $M$ is a continuous local martingale and $A$ is a continuous adapted [finite-variation process](../../../stochastic-calculus.md#finite-variation-process). Pointwise limits preserve predictability, so $H$ is predictable; it is bounded by the common bound for the $H_n$.

Localize so that $[M]_\infty$ and the total variation $V(A)_\infty$ are bounded. The [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) and the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) give

$$
\mathbb E\sup_t\left|\int_0^t(H_n-H)\,dM\right|^2
\leq4\mathbb E\int_0^\infty(H_n-H)^2\,d[M]
\longrightarrow0
$$

by the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). For the finite-variation part,

$$
\sup_t\left|\int_0^t(H_n-H)\,dA\right|
\leq\int_0^\infty|H_n-H|\,dV(A)
\longrightarrow0
$$

almost surely, again by dominated convergence, now for each sample path. Hence the two integrals converge uniformly in probability after every localization. Part (b) removes the localization and proves

$$
\int H_n\,dX\longrightarrow\int H\,dX
$$

u.c.p.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Put

$$
f_n(x)=\frac1n\log\cosh(nx).
$$

Then $f_n\to|\mathord\cdot|$ uniformly, $f_n'(x)=\tanh(nx)$, and $f_n''(x)=n\operatorname{sech}^2(nx)$. [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
f_n(X_t)=f_n(X_0)+\int_0^t\tanh(nX_s)\,dX_s
+\frac12\int_0^t n\operatorname{sech}^2(nX_s)\,d[X]_s.
$$

The bounded predictable integrands $\tanh(nX)$ converge pointwise to $\operatorname{sgn}(X)$, with $\operatorname{sgn}(0)=0$. Part (c) therefore makes the stochastic integrals converge u.c.p. The left-hand side converges u.c.p. to $|X|$, so the increasing continuous processes

$$
A_t^{(n)}=\frac12\int_0^t n\operatorname{sech}^2(nX_s)\,d[X]_s
$$

also converge u.c.p. Their limit $A$ has a continuous increasing version: extract almost-sure locally uniform convergence from each compact interval and use a diagonal argument. We obtain

$$
|X_t|=|X_0|+\int_0^t\operatorname{sgn}(X_s)\,dX_s+A_t,
$$

the [Tanaka formula](../../../stochastic-calculus.md#tanaka-s-formula) with $A=L_t^0(X)$. It expresses $|X|$ as a continuous local martingale plus a continuous finite-variation process, so $|X|$ is a continuous semimartingale.

## 3

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For the level-$N$ dyadic partition, write

$$
V_N(t)=\sum_{k=1}^{2^N}
|f(k2^{-N}\wedge t)-f((k-1)2^{-N}\wedge t)|.
$$

The dyadic partitions are nested, so the [triangle inequality](../../../topological-analysis.md#triangle-inequality) makes $V_N(t)$ nondecreasing in $N$, and $\lVert f_t\rVert=\lim_NV_N(t)$.

Fix $t_1<t_2$. As the mesh tends to zero, the last dyadic point before $t_1$ approaches $t_1$. Refining from there to $t_2$, the triangle inequality says that the added variation is at least $|f(t_2)-f(t_1)|$ minus the two endpoint errors, which tend to zero by [continuity](../../../calculus.md#continuous-function). Therefore

$$
\lim_N\bigl(V_N(t_2)-V_N(t_1)\bigr)
\geq|f(t_2)-f(t_1)|.
$$

Since $\lVert f\rVert<\infty$, both limits are finite and may be subtracted, giving

$$
\boxed{\lVert f_{t_2}\rVert-\lVert f_{t_1}\rVert
\geq|f(t_2)-f(t_1)|.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Every dyadic partition is among the finite partitions on the right-hand side, so the displayed supremum is at least $\lVert f\rVert$. For the converse, the claim is immediate if $\lVert f\rVert=\infty$. If it is finite, apply part (a) to every interval of an arbitrary partition $0\leq t_0<\cdots<t_n=1$:

$$
|f(t_k)-f(t_{k-1})|
\leq\lVert f_{t_k}\rVert-\lVert f_{t_{k-1}}\rVert.
$$

Summing telescopes and gives

$$
\sum_{k=1}^n|f(t_k)-f(t_{k-1})|
\leq\lVert f_1\rVert-\lVert f_{t_0}\rVert
\leq\lVert f\rVert.
$$

Taking the supremum proves that the dyadic definition equals the usual [total variation of a function](../../../real-analysis.md#total-variation-of-a-function).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

If $f$ is [continuously differentiable](../../../calculus.md#continuously-differentiable-function), then for every finite partition the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) give

$$
\sum_{k=1}^n|f(t_k)-f(t_{k-1})|
\leq\sum_{k=1}^n\int_{t_{k-1}}^{t_k}|f'(s)|\,ds
\leq\int_0^1|f'(s)|\,ds<\infty.
$$

Part (b) therefore implies $\lVert f\rVert<\infty$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $k\geq1$, set

$$
t_k=\frac1{(k+\tfrac12)\pi}.
$$

Then $t_k\downarrow0$ and $f(t_k)=(-1)^k t_k$. Consecutive values have opposite signs, so

$$
|f(t_{k+1})-f(t_k)|=t_{k+1}+t_k.
$$

Finite partitions containing $t_N,t_{N-1},\ldots,t_1$ therefore have variation at least

$$
\sum_{k=1}^{N-1}(t_{k+1}+t_k),
$$

which diverges with $N$ by comparison with the [harmonic series](../../../real-analysis.md#harmonic-series). Part (b) now gives $\lVert f\rVert=\infty$.

## 4

↑ **Parent:** [Paper 202](paper-202.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Factor the square root of the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) as

$$
\sqrt{S_T}
=\sqrt{S_0}\,
\mathcal E\!\left(\frac12(M-M_0)\right)_T
\exp\!\left(-\frac18[M]_T\right).
$$

The stochastic exponential in this expression is a positive local martingale and hence a [supermartingale](../../../martingale.md#supermartingale), so its expectation is at most one. If $[M]_T\geq a$ almost surely, then

$$
\boxed{\mathbb E\sqrt{S_T}
\leq\sqrt{S_0}e^{-a/8}
\mathbb E\mathcal E\!\left(\frac12(M-M_0)\right)_T
\leq\sqrt{S_0}e^{-a/8}.}
$$

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

If $[M]_T\leq b$, the [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) holds for $(M-M_0)/2$ because

$$
\mathbb E\exp\!\left(\frac18[M]_T\right)\leq e^{b/8}<\infty.
$$

Its stochastic exponential is therefore a true martingale with expectation one. Using the factorization from part (i),

$$
\boxed{\mathbb E\sqrt{S_T}
\geq\sqrt{S_0}e^{-b/8}
\mathbb E\mathcal E\!\left(\frac12(M-M_0)\right)_T
=\sqrt{S_0}e^{-b/8}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

With zero interest rate, the bank account is constant. The risky asset $S$ is a continuous local martingale by assumption, while the [European contingent claim](../../../mathematical-finance.md#european-contingent-claim) price

$$
C_t=\mathbb E(\sqrt{S_T}\mid\mathcal F_t)
$$

is a true martingale by the defining property of [conditional expectation](../../../measure-theory.md#conditional-expectation). Thus the original probability measure is an [equivalent local martingale measure](../../../mathematical-finance.md#equivalent-local-martingale-measure) for all traded discounted prices. The [fundamental theorem of asset pricing](../../../mathematical-finance.md#fundamental-theorem-of-asset-pricing) then excludes arbitrage for admissible self-financing strategies.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

In the [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model),

$$
S_t=S_0\exp\!\left(\sigma W_t-\frac12\sigma^2t\right).
$$

Conditioning on $\mathcal F_t$ and using the [moment-generating function](../../../probability-theory.md#moment-generating-function) of the independent Gaussian increment $W_T-W_t$ gives

$$
C_t=\sqrt{S_t}\exp\!\left(-\frac18\sigma^2(T-t)\right)
=c(t,S_t).
$$

The function $c$ satisfies the zero-rate [Black-Scholes equation](../../../mathematical-finance.md#black-scholes-equation), so [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) leaves only its stochastic term:

$$
dC_t=\partial_sc(t,S_t)\,dS_t.
$$

Consequently the required [delta hedge](../../../mathematical-finance.md#delta-hedge) is

$$
\boxed{\Delta(t,s)=\partial_sc(t,s)
=\frac1{2\sqrt s}\exp\!\left(-\frac18\sigma^2(T-t)\right).}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For this square-root payoff, the time-zero [Black-Scholes model](../../../mathematical-finance.md#black-scholes-model) price at volatility $\widehat\sigma$ is

$$
C_0=\sqrt{S_0}\exp\!\left(-\frac18T\widehat\sigma^2\right).
$$

Parts (a)(i) and (a)(ii), together with $a\leq[M]_T\leq b$, give

$$
\sqrt{S_0}e^{-b/8}
\leq C_0
\leq\sqrt{S_0}e^{-a/8}.
$$

The exponential is strictly decreasing, so comparison with the defining Black-Scholes price gives

$$
a\leq T\widehat\sigma^2\leq b.
$$

**Thus the [Black-Scholes implied volatility](../../../mathematical-finance.md#black-scholes-implied-volatility) lies between the lower and upper realized-variance bounds.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
