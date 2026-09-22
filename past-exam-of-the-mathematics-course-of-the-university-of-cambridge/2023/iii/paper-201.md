# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_201.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $M_n=\mathbb E[Z\mid\mathcal F_n]$. Each $M_n$ is $\mathcal F_n$-measurable and integrable, with $|M_n|\leq\mathbb E[|Z|\mid\mathcal F_n]\leq1$. Since a [filtration](../../../stochastic-process.md#filtration-probability-theory) is increasing, the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E[M_{n+1}\mid\mathcal F_n]
=\mathbb E[\mathbb E[Z\mid\mathcal F_{n+1}]\mid\mathcal F_n]
=\mathbb E[Z\mid\mathcal F_n]=M_n.
$$

**Thus $(M_n)$ is the [conditional-expectation martingale](../../../martingale.md#conditional-expectation-martingale) associated with $Z$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives an almost-sure limit $M_\infty$, because $|M_n|\leq1$. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) also gives $M_n\to M_\infty$ in $L^1$.

To identify the limit, take $A\in\bigcup_n\mathcal F_n$. For some $N$, $A\in\mathcal F_N$, and for every $n\geq N$,

$$
\mathbb E[M_n\mathbf1_A]=\mathbb E[Z\mathbf1_A].
$$

Passing to the $L^1$ limit preserves this equality. The sets for which $\mathbb E[M_\infty\mathbf1_A]=\mathbb E[Z\mathbf1_A]$ form a monotone class containing the algebra $\bigcup_n\mathcal F_n$, so the equality holds throughout $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$. Since $M_\infty$ is $\mathcal F_\infty$-measurable, it is $\mathbb E[Z\mid\mathcal F_\infty]$. This proves the [conditional-expectation convergence along a filtration](../../../martingale.md#conditional-expectation-convergence-along-a-filtration) both almost surely and in $L^1$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Define $Z_n=\sup_{m\geq n}|X_m-X|$. Then $0\leq Z_n\leq2$ and $Z_n\downarrow0$ almost surely. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives $\mathbb E Z_n\to0$.

Set $W_n=\mathbb E[Z_n\mid\mathcal F_n]$. Since $Z_{n+1}\leq Z_n$, the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\mathbb E[W_{n+1}\mid\mathcal F_n]
=\mathbb E[Z_{n+1}\mid\mathcal F_n]
\leq W_n,
$$

so $(W_n)$ is a nonnegative [supermartingale](../../../martingale.md#supermartingale). The [almost sure supermartingale convergence theorem](../../../martingale.md#almost-sure-supermartingale-convergence-theorem) gives $W_n\to W_\infty$ almost surely, and [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) yields $\mathbb EW_\infty\leq\liminf_n\mathbb EW_n=0$. Hence $W_n\to0$ almost surely; because $\mathbb EW_n=\mathbb EZ_n\to0$, convergence also holds in $L^1$.

Finally,

$$
\left|\mathbb E[X_n\mid\mathcal F_n]-\mathbb E[X\mid\mathcal F_\infty]\right|
\leq W_n
+\left|\mathbb E[X\mid\mathcal F_n]-\mathbb E[X\mid\mathcal F_\infty]\right|.
$$

The second term tends to zero almost surely and in $L^1$ by part b. The first does so by the preceding argument, proving the [moving-variable conditional-expectation convergence](../../../martingale.md#moving-variable-conditional-expectation-convergence).

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [almost sure supermartingale convergence theorem](../../../martingale.md#almost-sure-supermartingale-convergence-theorem) says that a supermartingale whose negative parts have uniformly bounded expectations converges almost surely to a finite integrable limit. In particular, every nonnegative supermartingale converges almost surely.

Here the process is uniformly bounded, say $0\leq X_n\leq C$. Let $X_\infty=\lim_nX_n$, whose existence follows from the theorem. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) then gives

$$
\mathbb E[X_\infty]=\lim_{n\to\infty}\mathbb E[X_n].
$$

The limit on the right also exists directly because the expectations of a [supermartingale](../../../martingale.md#supermartingale) form a decreasing sequence.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $x\ne0$, the [Strong Markov property](../../../markov-process.md#strong-markov-property) at the first step gives the discrete mean-value identity

$$
v(x)=\frac16\sum_{|e|=1}v(x+e).
$$

At $x=0$, $v(0)=1$ while the same average is at most one. Thus $v$ is a bounded superharmonic function on $\mathbb Z^3$. Conditioning on the [natural filtration](../../../stochastic-process.md#natural-filtration) and using the one-step [Markov property](../../../markov-process.md#markov-property) gives

$$
\mathbb E[v(X_{n+1})\mid\mathcal F_n]
=\frac16\sum_{|e|=1}v(X_n+e)
\leq v(X_n).
$$

**Therefore $(v(X_n))$ is a nonnegative [supermartingale](../../../martingale.md#supermartingale).**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $A_n=\{X_m=0\text{ for some }m\geq n\}$. By the [Markov property](../../../markov-process.md#markov-property),

$$
v(X_n)=\mathbb P(A_n\mid\mathcal F_n).
$$

The events $A_n$ decrease to the event that the walk visits zero infinitely often, which has probability zero by the stated transience assumption. Hence

$$
\mathbb E[v(X_n)]=\mathbb P(A_n)\longrightarrow0.
$$

Part a and the [almost sure supermartingale convergence theorem](../../../martingale.md#almost-sure-supermartingale-convergence-theorem) give an almost-sure limit $V\geq0$. By [Fatou lemma](../../../measure-theory.md#fatou-s-lemma), $\mathbb EV\leq\liminf_n\mathbb E[v(X_n)]=0$, so $V=0$ almost surely.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The probability generating function of each $X_i$ is $\exp(z-1)$. Independence makes the generating function of $S_n$ equal to $\exp(n(z-1))$, so the [addition of independent Poisson random variables](../../../discrete-probability-distribution.md#addition-of-independent-poisson-random-variables) gives $S_n\sim\operatorname{Pois}(n)$.

The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has mean and variance $n$, hence $\mathbb E Y_n=0$ and $\mathbb E[Y_n^2]=1$. Since $Y_n^-\leq|Y_n|$, [Chebyshev inequality](../../../probability-inequality.md#chebyshev-inequality) gives

$$
\boxed{\mathbb P(Y_n^-\geq a)
\leq\mathbb P(|Y_n|\geq a)
\leq\frac1{a^2}.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Poisson central limit theorem](../../../discrete-probability-distribution.md#poisson-central-limit-theorem), or the ordinary [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) applied to the $X_i$, gives $Y_n\xrightarrow dY$ for a standard normal random variable $Y$. The negative-part map $x\mapsto x^-:=\max(-x,0)$ is continuous, so the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) gives

$$
\boxed{Y_n^-\xrightarrow dY^-.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $K>0$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and part a give

$$
\mathbb E\left[Y_n^-\mathbf1_{\{Y_n^->K\}}\right]
\leq\sqrt{\mathbb E[(Y_n^-)^2]}
\sqrt{\mathbb P(Y_n^->K)}
\leq\frac1K.
$$

Thus $(Y_n^-)$ is [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability). Combining this with the [weak convergence of random variables](../../../convergence-of-random-variables.md#convergence-in-distribution) from part b yields convergence of the first moments:

$$
\mathbb E[Y_n^-]\longrightarrow\mathbb E[Y^-].
$$

By symmetry of the standard normal density,

$$
\mathbb E[Y^-]
=\int_0^\infty x\frac{e^{-x^2/2}}{\sqrt{2\pi}}\,dx
=\frac1{\sqrt{2\pi}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $S_n\sim\operatorname{Pois}(n)$,

$$
\begin{aligned}
\mathbb E[(n-S_n)^+]
&=\sum_{k=0}^{n-1}(n-k)e^{-n}\frac{n^k}{k!}\\
&=n\mathbb P(S_n=n-1)
=e^{-n}\frac{n^{n+1}}{n!}.
\end{aligned}
$$

Consequently

$$
\mathbb E[Y_n^-]
=\frac1{\sqrt n}\mathbb E[(n-S_n)^+]
=\frac{e^{-n}n^{n+1/2}}{n!}.
$$

Part c says that this tends to $1/\sqrt{2\pi}$. Rearranging gives the [Stirling formula](../../../real-analysis.md#stirling-formula)

$$
\boxed{n!\sim\sqrt{2\pi n}\left(\frac ne\right)^n.}
$$

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $0\leq s\leq t$, write $B_t=B_s+(B_t-B_s)$. The increment is independent of $\mathcal F_s$ and is normally distributed with variance $t-s$. Its moment generating function gives

$$
\begin{aligned}
\mathbb E[M_\lambda(t)\mid\mathcal F_s]
&=e^{\lambda B_s-\lambda^2s/2}
\mathbb E\left[e^{\lambda(B_t-B_s)-\lambda^2(t-s)/2}\right]\\
&=M_\lambda(s).
\end{aligned}
$$

The process is integrable for every real $\lambda$, so it is the [exponential Brownian martingale](../../../brownian-motion.md#exponential-brownian-martingale).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Differentiate the conditional identity from part a. To justify doing so, fix a compact parameter interval $|\lambda|\leq L$. Every $n$th derivative of $M_\lambda(t)$ is a polynomial in $B_t,t,$ and $\lambda$ times $M_\lambda(t)$, and its absolute value is bounded by

$$
C_{n,L,t}(1+|B_t|^n)e^{(L+1)|B_t|}.
$$

This bound is integrable because a Gaussian random variable has every polynomially weighted exponential moment. Dominated differentiation of conditional expectation therefore gives

$$
\mathbb E\left[\frac{\partial^nM_\lambda(t)}{\partial\lambda^n}\,\middle|\,\mathcal F_s\right]
=\frac{\partial^nM_\lambda(s)}{\partial\lambda^n}.
$$

**Thus every [parameter derivative of the exponential Brownian martingale](../../../brownian-motion.md#parameter-derivative-of-the-exponential-brownian-martingale) is itself a martingale.**

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $T=\tau_b\wedge\tau_{-a}$ and $A=\{\tau_b<\tau_{-a}\}$. The [Brownian exit time](../../../brownian-motion.md#brownian-exit-time) $T$ is finite almost surely. Optional stopping of the bounded martingale $B_{t\wedge T}$ gives

$$
\mathbb P(A)=\frac{a}{a+b}.
$$

For $T_n=T\wedge n$, optional stopping of $B_t^2-t$ gives $\mathbb ET_n=\mathbb E[B_{T_n}^2]\leq\max(a^2,b^2)$. Letting $n\to\infty$ by monotone and bounded convergence proves $\mathbb ET=\mathbb E[B_T^2]=ab$.

The third derivative in part b at $\lambda=0$ is the cubic martingale $B_t^3-3tB_t$. Optional stopping at $T_n$ is valid because $T_n$ is bounded. Since $B_{T_n}$ is bounded and $T_n\to T$ in $L^1$, its stopped identity passes to the limit and gives

$$
\mathbb E[B_T^3]=3\mathbb E[TB_T].
$$

Put $x=\mathbb E[T\mathbf1_A]$ and $y=\mathbb E[T\mathbf1_{A^c}]$. Then $x+y=ab$, while

$$
b x-a y
=\frac13\left(b^3\frac a{a+b}-a^3\frac b{a+b}\right)
=\frac{ab(b-a)}3.
$$

Solving gives $x=ab(2a+b)/(3(a+b))$. Dividing by $\mathbb P(A)=a/(a+b)$ proves the [conditional Brownian interval-exit time](../../../brownian-motion.md#conditional-brownian-interval-exit-time) formula

$$
\boxed{\mathbb E[\tau_b\mid\tau_b<\tau_{-a}]
=\frac{b^2+2ab}{3}.}
$$

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) reflects a path after its first hit of $x>0$ and gives

$$
\mathbb P(M_t\geq x)=2\mathbb P(B_t\geq x).
$$

Symmetry of the centered [normal distribution](../../../probability-theory.md#normal-distribution) gives $2\mathbb P(B_t\geq x)=\mathbb P(|B_t|\geq x)$. Both random variables are nonnegative, so their tail distributions agree for every $x$, proving the [Brownian running maximum](../../../brownian-motion.md#brownian-running-maximum) identity $M_t\stackrel d=|B_t|$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Continuity on the compact interval ensures that a maximum time exists. Fix a rational $r\in(0,1)$ and define

$$
U_r=\max_{0\leq t\leq r}B_t-B_r,
\qquad
V_r=\max_{r\leq t\leq1}(B_t-B_r).
$$

By Brownian time reversal and the [Brownian running maximum](../../../brownian-motion.md#brownian-running-maximum) law, $U_r\stackrel d=|N(0,r)|$. Independent increments give $V_r\stackrel d=|N(0,1-r)|$ independently of $U_r$. Their continuous distributions imply $\mathbb P(U_r=V_r)=0$.

If the maximum were attained at two distinct times, a rational $r$ strictly between them would make the maxima on $[0,r]$ and $[r,1]$ equal, hence $U_r=V_r$. A countable union over rational $r$ still has probability zero. Therefore the [time of the Brownian maximum](../../../brownian-motion.md#time-of-the-brownian-maximum) is almost surely unique.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For fixed $s\in(0,1)$, uniqueness gives

$$
\{M^*\leq s\}
=\left\{\max_{t\leq s}B_t-B_s
\geq\max_{s\leq t\leq1}(B_t-B_s)\right\}.
$$

The two sides of the comparison are independent and distributed as $\sqrt s|Z_1|$ and $\sqrt{1-s}|Z_2|$ for independent standard normal random variables. Rotational invariance of $(Z_1,Z_2)$ makes its angle uniform, so

$$
\begin{aligned}
\mathbb P(M^*\leq s)
&=\mathbb P\left(\frac{|Z_2|}{|Z_1|}\leq\sqrt{\frac{s}{1-s}}\right)\\
&=\frac2\pi\arctan\sqrt{\frac{s}{1-s}}
=\frac2\pi\arcsin\sqrt s.
\end{aligned}
$$

The endpoint values follow by continuity. Thus the [time of the Brownian maximum](../../../brownian-motion.md#time-of-the-brownian-maximum) has the arcsine distribution.

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For $m>0$, the [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process) gives

$$
\mathbb P\left(\sup_{0\leq s\leq t}B_s\geq m\right)
=2\mathbb P(B_t\geq m)\longrightarrow1
$$

as $t\to\infty$. Hence Brownian motion hits every positive integer almost surely. Applying the same argument to $-B$ shows that it hits every negative integer almost surely. Taking the countable intersection of these probability-one events proves

$$
\limsup_{t\to\infty}B_t=+\infty,
\qquad
\liminf_{t\to\infty}B_t=-\infty.
$$

Arbitrarily late positive and negative values occur, and path continuity forces a zero between successive values of opposite sign. Thus [recurrence of one-dimensional Brownian motion](../../../brownian-motion.md#recurrence-of-one-dimensional-brownian-motion) gives infinitely many visits to zero.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The pair $(B,\widetilde B)$ is a Brownian motion in $\mathbb R^{2d}$. Assume inductively that $T_{i-1}<\infty$. By the [Strong Markov property](../../../markov-process.md#strong-markov-property) at $T_{i-1}$, the difference

$$
D_t=B^i_{T_{i-1}+t}-\widetilde B^i_{T_{i-1}+t}
$$

is a one-dimensional Brownian motion with variance rate two, started from its current value. By [recurrence of one-dimensional Brownian motion](../../../brownian-motion.md#recurrence-of-one-dimensional-brownian-motion), it hits zero in finite time almost surely. Hence $T_i<\infty$. Induction through $i=1,\ldots,d$ proves $T_d<\infty$ almost surely.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Start Brownian motions at arbitrary $x,y\in\mathbb R^d$. Use the successive meeting times from part b, but after coordinate $i$ meets, drive that coordinate of the second process with the first process's increments forever. The [Strong Markov property](../../../markov-process.md#strong-markov-property) shows that each marginal remains a $d$-dimensional Brownian motion. By part b every coordinate is eventually locked, so the resulting [coordinatewise coalescing coupling of Brownian motions](../../../brownian-motion.md#coordinatewise-coalescing-coupling-of-brownian-motions) has an almost surely finite coalescence time $T$.

Because $f$ is bounded and harmonic, [Dynkin formula for Brownian motion](../../../brownian-motion.md#dynkin-formula-for-brownian-motion) shows that $f(B_t^x)$ and $f(B_t^y)$ are bounded [martingales](../../../martingale.md). Therefore

$$
\begin{aligned}
|f(x)-f(y)|
&=\left|\mathbb E[f(B_t^x)-f(B_t^y)]\right|\\
&\leq2\|f\|_\infty\mathbb P(T>t).
\end{aligned}
$$

Since $T<\infty$ almost surely, the right side tends to zero. Thus $f(x)=f(y)$ for all $x,y$, proving the [Brownian coupling proof of the harmonic Liouville theorem](../../../partial-differential-equation.md#brownian-coupling-proof-of-the-harmonic-liouville-theorem).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
