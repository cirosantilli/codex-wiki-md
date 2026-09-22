# Paper 32

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper32.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper32.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)

## 1

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Put $C=\sup_p\mathbb E|X_p|<\infty$. Since $x\mapsto x^+$ is an increasing [convex function](../../../real-analysis.md#convex-function), the [conditional Jensen inequality](../../../measure-theory.md#conditional-jensen-inequality) and the [submartingale](../../../martingale.md#submartingale) property give

$$
\mathbb E[X_{p+1}^+\mid\mathcal F_p]\geq\bigl(\mathbb E[X_{p+1}\mid\mathcal F_p]\bigr)^+\geq X_p^+.
$$

For fixed $n$ and $p\geq n$, the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) therefore implies

$$
\mathbb E[X_{p+1}^+\mid\mathcal F_n]\geq\mathbb E[X_p^+\mid\mathcal F_n].
$$

Choose versions for this countable family so that all these inequalities hold outside one null set. Its nonnegative increasing limit $M_n$ is $\mathcal F_n$-measurable. The [monotone convergence theorem](../../../measure-theory.md#monotone-convergence-theorem) shows that

$$
\mathbb EM_n=\lim_{p\to\infty}\mathbb EX_p^+\leq C.
$$

In particular the limit is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Thus **the increasing conditional means converge to an integrable nonnegative $M_n$**, rather than merely to a possibly infinite extended value. This is the construction of the [positive martingale majorant of an L1-bounded submartingale](../../../martingale.md#positive-martingale-majorant-of-an-l1-bounded-submartingale).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Use conditional [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) and the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) in the preceding construction:

$$
\begin{aligned}
\mathbb E[M_{n+1}\mid\mathcal F_n]
&=\lim_{p\to\infty}\mathbb E\bigl[\mathbb E[X_p^+\mid\mathcal F_{n+1}]\mid\mathcal F_n\bigr]\\
&=\lim_{p\to\infty}\mathbb E[X_p^+\mid\mathcal F_n]=M_n.
\end{aligned}
$$

This proves the [martingale](../../../martingale.md) property. The construction gives $M_n\geq0$ and $\sup_n\mathbb EM_n\leq C$, so $M$ is bounded in $L^1$. Taking $p=n$ in the increasing family also gives $M_n\geq X_n^+\geq X_n$. Define $Y_n=M_n-X_n$. Then $Y$ is nonnegative and adapted, and

$$
\mathbb E[Y_{n+1}\mid\mathcal F_n]
=M_n-\mathbb E[X_{n+1}\mid\mathcal F_n]\leq M_n-X_n=Y_n.
$$

Thus $Y$ is a [supermartingale](../../../martingale.md#supermartingale), with $\mathbb E|Y_n|\leq\mathbb EM_n+\mathbb E|X_n|\leq2C$. The requested conclusion is

$$
\boxed{X_n=M_n-Y_n,\qquad M\text{ a nonnegative }L^1\text{-bounded martingale},\quad Y\text{ a nonnegative }L^1\text{-bounded supermartingale}.}
$$

This [positive martingale majorant of an L1-bounded submartingale](../../../martingale.md#positive-martingale-majorant-of-an-l1-bounded-submartingale) is not asserted to have [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability); boundedness in $L^1$ alone does not imply that stronger property.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [almost sure supermartingale convergence theorem](../../../martingale.md#almost-sure-supermartingale-convergence-theorem) applies to the $L^1$-bounded [supermartingale](../../../martingale.md#supermartingale) $X$. Hence $X_n\to X_\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), and the [Fatou lemma](../../../measure-theory.md#fatou-s-lemma) gives $\mathbb E|X_\infty|\leq\sup_n\mathbb E|X_n|<\infty$. Take the version of $X_\infty$ obtained from the sequence, so it is measurable for $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$. Set

$$
M_n=\mathbb E[X_\infty\mid\mathcal F_n],\qquad Y_n=X_n-M_n.
$$

The [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) makes $M$ a [martingale](../../../martingale.md), and the [uniform integrability of conditional expectations](../../../convergence-of-random-variables.md#uniform-integrability-of-conditional-expectations) makes it [uniformly integrable](../../../convergence-of-random-variables.md#uniform-integrability). Explicitly, with $Z=X_\infty$, $C=\mathbb E|Z|$, and $R,K>0$, we have $|M_n|\leq R+\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}\mid\mathcal F_n]$, so

$$
\mathbb E[|M_n|\mathbf1_{\{|M_n|>K\}}]\leq\frac{RC}{K}+\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}].
$$

First choose $R$ large, then $K$ large. This proves [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability) uniformly in $n$.

The [uniformly integrable martingale convergence theorem](../../../martingale.md#uniformly-integrable-martingale-convergence-theorem) gives a limit $M_\infty$ both [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence) and in $L^1$. For $A\in\mathcal F_j$ and $n\geq j$, $\mathbb E[M_n\mathbf1_A]=\mathbb E[X_\infty\mathbf1_A]$. Passing to the $L^1$ limit and then extending from the algebra $\bigcup_j\mathcal F_j$ to $\mathcal F_\infty$ identifies $M_\infty=X_\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Finally,

$$
\mathbb E[Y_{n+1}\mid\mathcal F_n]=\mathbb E[X_{n+1}\mid\mathcal F_n]-M_n\leq Y_n,
\qquad Y_n=X_n-M_n\longrightarrow0\quad\text{a.s.}
$$

Thus **$X=M+Y$ with $M$ uniformly integrable and $Y$ a supermartingale tending almost surely to zero**. The [terminal decomposition of an L1-bounded supermartingale](../../../martingale.md#terminal-decomposition-of-an-l1-bounded-supermartingale) does not require $Y\geq0$ or $Y_n\to0$ in $L^1$. Indeed, for $X$ equal to the negative of the [fair-coin doubling martingale](../../../martingale.md#fair-coin-doubling-martingale), $X_\infty=0$, $M=0$, and $Y=X$ is negative and has constant absolute mean one.

## 2

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [moment-generating function](../../../probability-theory.md#moment-generating-function) satisfies $0<\phi(\lambda)<\infty$. The proposed process is nonnegative and adapted to the [natural filtration](../../../stochastic-process.md#natural-filtration) of the [random walk](../../../markov-process.md#random-walk), and [independence](../../../random-variable.md#independent-random-variables) of the increments gives

$$
\mathbb EM_n^\lambda=\frac{\prod_{j=1}^n\mathbb Ee^{\lambda X_j}}{\phi(\lambda)^n}=1.
$$

Moreover $X_{n+1}$ is independent of $\mathcal F_n$, so

$$
\mathbb E[M_{n+1}^\lambda\mid\mathcal F_n]
=\frac{e^{\lambda S_n}}{\phi(\lambda)^{n+1}}\mathbb Ee^{\lambda X_{n+1}}
=M_n^\lambda.
$$

Therefore **$M^\lambda$ is a mean-one nonnegative martingale**, the [exponential martingale of a random walk](../../../markov-process.md#exponential-martingale-of-a-random-walk). For $\lambda=0$ it is the constant process one.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For Borel sets $A_1,\ldots,A_n$, multiply the finite-time [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) into the product law of the increments:

$$
\begin{aligned}
\mathbb P_n^\lambda(X_1\in A_1,\ldots,X_n\in A_n)
&=\mathbb E\left[\prod_{j=1}^n\frac{e^{\lambda X_j}}{\phi(\lambda)}\mathbf1_{\{X_j\in A_j\}}\right]\\
&=\prod_{j=1}^n\int_{A_j}\frac{e^{\lambda x}}{\phi(\lambda)}\,\mu(dx).
\end{aligned}
$$

The factorization, extended from rectangles to the product [sigma-algebra](../../../measure-theory.md#sigma-algebra), proves [independence](../../../random-variable.md#independent-random-variables) and identical distributions. Their common law is the [exponential tilting](../../../probability-theory.md#exponential-tilting)

$$
\boxed{\mu^\lambda(dx)=\frac{e^{\lambda x}}{\phi(\lambda)}\mu(dx).}
$$

For $\lambda>0$, $|x|e^{\lambda x}$ is bounded on $x\leq0$, while $xe^{\lambda x}\leq C_\varepsilon e^{(\lambda+\varepsilon)x}$ on $x\geq0$. Choosing a small two-sided neighborhood of $\lambda$ still contained in $(0,\infty)$ gives an integrable dominating function for the derivative. [Differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) then yields

$$
\phi'(\lambda)=\int xe^{\lambda x}\,\mu(dx),\qquad
\boxed{\mathbb E^\lambda X_1=\frac{\phi'(\lambda)}{\phi(\lambda)}\quad(\lambda>0).}
$$

The [mean under one-sided exponential tilting](../../../probability-theory.md#mean-under-one-sided-exponential-tilting) needs an endpoint qualification. At $\lambda=0$, finiteness of positive [exponential moments](../../../probability-theory.md#exponential-moment) makes $X_1^+$ integrable, but gives no integrability of $X_1^-$. The formula holds with the right derivative and the extended mean $\phi'_+(0)=\mathbb EX_1\in[-\infty,\infty)$. To see this, apply [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) to $(1-e^{-hX_1^-})/h$ and [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) to $(e^{hX_1^+}-1)/h$ as $h\downarrow0$. A finite mean at zero is not guaranteed by the printed hypotheses: $\mu(\{-j\})=6/(\pi^2j^2)$, $j\geq1$, has finite $\phi(\lambda)$ for every $\lambda\geq0$ but $\mathbb EX_1=-\infty$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

First take $k$ to be a nonnegative integer. The [exponential tilting](../../../probability-theory.md#exponential-tilting) constructed from the independent increments restricts to $\mathbb P_n^\lambda$ on each $\mathcal F_n$. Since its [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) is strictly positive, finite-time change of measure gives

$$
\mathbb P(\tau_k\leq n)=\mathbb E^\lambda[(M_n^\lambda)^{-1}\mathbf1_{\{\tau_k\leq n\}}].
$$

Under the tilted law, $L_n=(M_n^\lambda)^{-1}$ is a [martingale](../../../martingale.md), because

$$
\mathbb E^\lambda[\phi(\lambda)e^{-\lambda X_{n+1}}]=\int\phi(\lambda)e^{-\lambda x}\frac{e^{\lambda x}}{\phi(\lambda)}\,\mu(dx)=1.
$$

Use the [stopped likelihood ratio under exponential tilting](../../../markov-process.md#stopped-likelihood-ratio-under-exponential-tilting) at this finite horizon. In detail, $\{\tau_k=j\}\in\mathcal F_j$, so

$$
\begin{aligned}
\mathbb E^\lambda[L_n\mathbf1_{\{\tau_k\leq n\}}]
&=\sum_{j=0}^n\mathbb E^\lambda[\mathbb E^\lambda(L_n\mid\mathcal F_j)\mathbf1_{\{\tau_k=j\}}]\\
&=\sum_{j=0}^n\mathbb E^\lambda[L_j\mathbf1_{\{\tau_k=j\}}]
=\mathbb E^\lambda[L_{\tau_k}\mathbf1_{\{\tau_k\leq n\}}].
\end{aligned}
$$

Here the last expression is defined only on the displayed event, so no value of $M_\infty^\lambda$ is being assumed. The [upward skip-free random walk](../../../markov-process.md#upward-skip-free-random-walk) has integer increments bounded above by one, which imply $S_{\tau_k}=k$ on a finite hit: the preceding value is at most $k-1$, and there is no upward overshoot. Consequently

$$
\boxed{\mathbb P(\tau_k\leq n)=e^{-\lambda k}\mathbb E^\lambda[\phi(\lambda)^{\tau_k}\mathbf1_{\{\tau_k\leq n\}}].}
$$

At $\lambda=\lambda_0$, the [mean under one-sided exponential tilting](../../../probability-theory.md#mean-under-one-sided-exponential-tilting) is finite and positive. The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives $S_n/n\to\phi'(\lambda_0)>0$ under $\mathbb P^{\lambda_0}$, so every integer level is hit [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Since $\phi(\lambda_0)=1$, passing to $n\to\infty$ gives

$$
\boxed{\mathbb P(\tau_k<\infty)=e^{-\lambda_0k},\qquad k\in\mathbb Z_{\geq0}.}
$$

Let $H=\sup_{n\geq0}S_n$. The event $\{H\geq k\}$ is exactly the finite-hit event: an integer sequence with all its values below $k$ has supremum at most $k-1$. Also $\mathbb P(H=\infty)=\lim_k e^{-\lambda_0k}=0$. Subtraction of consecutive tail probabilities gives the [geometric maximum of an upward skip-free random walk](../../../markov-process.md#geometric-maximum-of-an-upward-skip-free-random-walk):

$$
\boxed{\mathbb P(H=j)=(1-e^{-\lambda_0})e^{-\lambda_0j},\qquad j=0,1,2,\ldots.}
$$

This is the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) counting failures before the first success, with success parameter $1-e^{-\lambda_0}$.

The PDF writes only $k\geq0$, without explicitly declaring integer levels. If it is read as allowing real $k$, then $\tau_k=\tau_{\lceil k\rceil}$ and the displayed factor must be $e^{-\lambda\lceil k\rceil}$; the hitting probability is likewise $e^{-\lambda_0\lceil k\rceil}$. For example, increments $+1$ and $-1$ with probabilities $1/3$ and $2/3$ have $\lambda_0=\log2$: hitting level $1/2$ has probability $1/2$, not $2^{-1/2}$. The integer interpretation supplies the intended formula.

## 3

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix $x>0$ and let $A=\{M_0<x\}\in\mathcal F_0$. On $A$, [continuity](../../../calculus.md#continuous-function) of the paths implies $0\leq M_{t\wedge T_x}\leq x$, and $M_{T_x}=x$ on $\{T_x<\infty\}$. Bounded-time [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) gives, for every $t$,

$$
\mathbb E[\mathbf1_A M_{t\wedge T_x}\mid\mathcal F_0]=\mathbf1_A M_0.
$$

On $A\cap\{T_x=\infty\}$, the stopped process is $M_t\to0$; on $A\cap\{T_x<\infty\}$ it eventually equals $x$. The bound by $x$ permits conditional [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem), yielding

$$
x\mathbf1_A\mathbb P(T_x<\infty\mid\mathcal F_0)=\mathbf1_A M_0.
$$

On $A^c$, $T_x=0$, so the conditional hitting probability is one. Finally, a continuous nonnegative path tending to zero attains any positive supremum: after a sufficiently late time it is below half that supremum, and its maximum on the earlier compact interval is attained. Thus $\{M^*\geq x\}=\{T_x<\infty\}$, including equality at the level. We have proved the conditional form of the [maximal identity for a continuous nonnegative local martingale tending to zero](../../../martingale.md#maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero):

$$
\boxed{\mathbb P(M^*\geq x\mid\mathcal F_0)=1\wedge\frac{M_0}{x}.}
$$

The restriction to $A$ before taking the limit is important: $M_0$ need not be bounded, and the unstopped [martingale](../../../martingale.md) need not have [uniform integrability](../../../convergence-of-random-variables.md#uniform-integrability).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

On a product extension of the [probability space](../../../probability-theory.md#probability-space), take a [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) variable $U$ on $(0,1)$ independent of the original [sigma-algebra](../../../measure-theory.md#sigma-algebra). For $x>0$,

$$
\mathbb P(M_0/U\geq x\mid\mathcal F_0)
=\mathbb P(U\leq M_0/x\mid\mathcal F_0)
=1\wedge\frac{M_0}{x}.
$$

These are the same conditional tails as in the [maximal identity for a continuous nonnegative local martingale tending to zero](../../../martingale.md#maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero). Taking [expectations](../../../probability-theory.md#expected-value) identifies the unconditional [probability distributions](../../../probability-theory.md#probability-distribution):

$$
\boxed{M^*\ \stackrel{d}{=}\ M_0/U.}
$$

If $M_0=0$, define $M_0/U=0$; the endpoint $U=0$ is a null event if one uses $[0,1]$ instead. The possible atom at zero has mass $\mathbb P(M_0=0)$, since the conditional probability of a positive maximum is zero exactly on that event. For fixed $M_0=m>0$, the conditional law is the [Pareto distribution](../../../continuous-probability-distribution.md#pareto-distribution) of shape one and minimum $m$, with density $m/x^2$ on $x>m$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process), applied to the negative increments of the [Brownian motion](../../../brownian-motion.md) started at $a$, gives

$$
\mathbb P(T_0>t)=2\Phi(a/\sqrt t)-1\longrightarrow0,
$$

where $\Phi$ is the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function). Hence $T_0<\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The stopped [Brownian motion](../../../brownian-motion.md) $M_t=B_{t\wedge T_0}$ is a continuous nonnegative [martingale](../../../martingale.md), starts at $a$, and eventually vanishes. The [maximal identity for a continuous nonnegative local martingale tending to zero](../../../martingale.md#maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero) therefore gives, for $H=\sup_{0\leq t\leq T_0}B_t$,

$$
\mathbb P(H\geq x)=\begin{cases}1,&0<x\leq a,\\a/x,&x>a.\end{cases}
$$

Equivalently,

$$
\boxed{H\stackrel d=\frac aU,\qquad F_H(x)=\begin{cases}0,&x<a,\\1-a/x,&x\geq a,\end{cases}\qquad f_H(x)=\frac a{x^2}\mathbf1_{\{x>a\}}.}
$$

There is no atom at $a$. This is the [Pareto distribution](../../../continuous-probability-distribution.md#pareto-distribution) of shape one, or the translated version of the [maximum before a lower Brownian barrier](../../../brownian-motion.md#maximum-before-a-lower-brownian-barrier).

## 4

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For standard [Brownian motion](../../../brownian-motion.md) $B$ and $h>0$, let $T_h$ be its first hitting time of $h$. Define the reflected path by

$$
\widehat B_t=\begin{cases}B_t,&t\leq T_h,\\2h-B_t,&t>T_h,\end{cases}
$$

leaving a path unchanged if $T_h=\infty$. The **[Brownian reflection principle](../../../brownian-motion.md#reflection-principle-wiener-process)** says that $\widehat B$ has the same path [probability distribution](../../../probability-theory.md#probability-distribution) as $B$. In its endpoint form, for $t>0$ and every Borel set $A\subset(-\infty,h)$,

$$
\mathbb P(T_h\leq t,\ B_t\in A)=\mathbb P(B_t\in2h-A),
\qquad 2h-A=\{2h-y:y\in A\}.
$$

Here is a direct proof of preservation of the path law. For a fixed integer horizon $L$, let $T^{(m)}=2^{-m}\lceil2^mT_h\rceil\wedge L$, with an infinite first term interpreted as infinity. This is a [stopping time](../../../martingale.md#stopping-time) taking finitely many deterministic grid values. On $\{T^{(m)}=j2^{-m}\}$, the history determining that event is measurable at $j2^{-m}$, and subsequent [Brownian motion](../../../brownian-motion.md) increments are independent of that history. Those increments and their negatives have the same joint law, by symmetry of centered [normal distributions](../../../probability-theory.md#normal-distribution) and [independent increments](../../../stochastic-process.md#independent-increments). Thus reflecting after $T^{(m)}$ around $B_{T^{(m)}}$ preserves the full path law. For any fixed horizon $t<L$, the reflected paths converge uniformly on $[0,t]$ to the displayed reflected path, by [continuity](../../../calculus.md#continuous-function) as $T^{(m)}$ decreases to $T_h\wedge L$. This includes $T_h=\infty$, since reflection after $L$ has no effect before $t$. Passing to all finite-dimensional [probability distributions](../../../probability-theory.md#probability-distribution) proves the assertion; no prior recurrence claim is needed. Equivalently, the [Strong Markov property](../../../markov-process.md#strong-markov-property) gives the same proof by symmetry of the fresh increments after the hit. Reflection is an involution preserving the hitting event and mapping the indicated endpoint $y$ to $2h-y$. An endpoint above $h$ forces a hit by [continuity](../../../calculus.md#continuous-function); this proves the endpoint identity, rather than assuming it.

For $S_t=\sup_{0\leq s\leq t}B_s$, split $\{T_h\leq t\}$ according to whether $B_t$ is above or below $h$. Since $B_t$ has no atom at $h$, reflection gives

$$
\mathbb P(S_t\geq h)=\mathbb P(B_t\geq h)+\mathbb P(T_h\leq t,\ B_t<h)
=2\mathbb P(B_t\geq h)=\mathbb P(|B_t|\geq h).
$$

Both variables are nonnegative, so their positive tails identify the law:

$$
\boxed{S_t\stackrel d=|B_t|.}
$$

For $t>0$ this is the [half-normal distribution](../../../probability-theory.md#half-normal-distribution) of scale $\sqrt t$; at $t=0$ both variables vanish.

For the two separated intervals, put

$$
A_0=\sup_{a\leq t\leq b}B_t-B_b,\qquad Z=B_c-B_b,\qquad H=\sup_{0\leq u\leq d-c}(B_{c+u}-B_c).
$$

Here $A_0$ is measurable for $\mathcal F_b$, $Z$ has the [normal distribution](../../../probability-theory.md#normal-distribution) $N(0,c-b)$, and $H$ is a function of increments after $c$. The [independent increments](../../../stochastic-process.md#independent-increments) make these three objects mutually independent. The later absolute maximum is $B_b+Z+H$, so equality of the two maxima means $Z=A_0-H$. Conditional on $(A_0,H)$, this specifies a single value of the nondegenerate [normal distribution](../../../probability-theory.md#normal-distribution) $Z$, and hence has probability zero. Therefore

$$
\boxed{\mathbb P\left(\sup_{a\leq t\leq b}B_t=\sup_{c\leq t\leq d}B_t\right)=0.}
$$

This proves the [atomless maxima on separated Brownian intervals](../../../brownian-motion.md#atomless-maxima-on-separated-brownian-intervals) without incorrectly treating the two absolute maxima as independent.

## 5

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The exit time $T$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Indeed, if the [Brownian motion](../../../brownian-motion.md) is still in $(-b,a)$ at an integer time, its next unit increment exceeds $a+b$ with a fixed probability $p>0$ independent of the past; on this event it must exit before the next integer time. Consequently $\mathbb P(T>n)\leq(1-p)^n\to0$. Path [continuity](../../../calculus.md#continuous-function) gives $B_T\in\{a,-b\}$, and the two exit events partition the [probability space](../../../probability-theory.md#probability-space) up to null sets.

For each real $\lambda$, the [exponential Brownian martingale](../../../brownian-motion.md#exponential-brownian-martingale) $Z_t^\lambda=\exp(\lambda B_t-\lambda^2t/2)$ has expectation one. This follows directly from the [moment-generating function of a normal distribution](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) and [independent increments](../../../stochastic-process.md#independent-increments). At $t\wedge T$ its value is bounded by $e^{|\lambda|\max(a,b)}$. Bounded-time [optional stopping](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) and then [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) therefore give

$$
1=\mathbb E e^{\lambda B_T-\lambda^2T/2}.
$$

Write $p_\lambda=\mathbb E[e^{-\lambda^2T/2}\mathbf1_{\{T=T_a\}}]$ and $q_\lambda=\mathbb E[e^{-\lambda^2T/2}\mathbf1_{\{T=T_{-b}\}}]$. Applying the identity to $\lambda$ and $-\lambda$ yields

$$
e^{\lambda a}p_\lambda+e^{-\lambda b}q_\lambda=1,\qquad
e^{-\lambda a}p_\lambda+e^{\lambda b}q_\lambda=1.
$$

For $\lambda\ne0$, multiply the first equation by $e^{\lambda b}$, the second by $e^{-\lambda b}$, and subtract. Solving the resulting system gives

$$
\boxed{p_\lambda=\frac{\sinh(\lambda b)}{\sinh(\lambda(a+b))},\qquad q_\lambda=\frac{\sinh(\lambda a)}{\sinh(\lambda(a+b))}.}
$$

Adding and using the sum formula for the [hyperbolic sine](../../../calculus.md#hyperbolic-sine) gives the [asymmetric Brownian interval-exit transform](../../../brownian-motion.md#asymmetric-brownian-interval-exit-transform):

$$
\boxed{\mathbb E e^{-\lambda^2T/2}
=\frac{\sinh(\lambda a)+\sinh(\lambda b)}{\sinh(\lambda(a+b))}
=\frac{\cosh(\lambda(a-b)/2)}{\cosh(\lambda(a+b)/2)}.}
$$

At $\lambda=0$, the printed sine ratio is $0/0$ and needs its removable extension. [Dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) as $\lambda\to0$ gives

$$
\boxed{\mathbb P(T=T_a)=\frac b{a+b},\qquad\mathbb P(T=T_{-b})=\frac a{a+b},\qquad\mathbb E e^0=1.}
$$

Thus the formulas hold for every real parameter with this endpoint convention. The expectation on the left of the first formula is legible in the original PDF; the converted TeX's nested exponential is an OCR error.

## 6

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [Poisson random measure](../../../probability-theory.md#poisson-random-measure) with intensity the [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) $\mu$ is a random nonnegative integer-valued measure $M$ such that, for each outcome outside a single null set, $A\mapsto M(A)$ is countably additive, and for each measurable $A$, $M(A)$ is a measurable [random variable](../../../random-variable.md). For every measurable $A$ with $\mu(A)<\infty$,

$$
\mathbb P(M(A)=j)=e^{-\mu(A)}\frac{\mu(A)^j}{j!},\qquad j=0,1,2,\ldots;
$$

and for every finite collection of pairwise disjoint finite-intensity measurable sets, their counts are [independent random variables](../../../random-variable.md#independent-random-variables). These are integer-valued counts, with possible value infinity on infinite-intensity sets. In particular $\mu(A)=0$ implies $M(A)=0$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). The intensity identity is $\mathbb EM(A)=\mu(A)$, also in the extended sense.

For completeness, choose an increasing finite-intensity exhaustion $E_m\uparrow E$. Each $M(E_m)$ is finite [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence), simultaneously for all $m$, so $M$ is a [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). If $\mu(A)=\infty$, then $\mu(A\cap E_m)\to\infty$, and for any fixed integer $K$,

$$
\mathbb P(M(A)\leq K)\leq\mathbb P(M(A\cap E_m)\leq K)
=e^{-\mu(A\cap E_m)}\sum_{j=0}^K\frac{\mu(A\cap E_m)^j}{j!}\longrightarrow0.
$$

Hence $M(A)=\infty$ [almost surely](../../../convergence-of-random-variables.md#almost-sure-convergence). Independence for counts on arbitrary disjoint measurable sets follows by this exhaustion; an infinite count is a constant extended value. This convention completes the definition on a general [measurable space](../../../measure-theory.md#measurable-space), not just on bounded subsets of Euclidean space.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

For $r\geq0$, [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) of the ball is $v_dr^d$, so the [Poisson random measure](../../../probability-theory.md#poisson-random-measure) gives $N_r\sim\operatorname{Poisson}(v_dr^d)$ and

$$
\mathbb P(N_r=0)=e^{-v_dr^d}.
$$

By monotonicity of the balls, the set of radii with no points is an interval starting at zero. Thus $\{R\geq r\}=\{N_r=0\}$: if all smaller balls are empty then their union, the open ball of radius $r$, is empty; if that ball is empty then its radius belongs to the defining set. We obtain

$$
\mathbb P(R\geq r)=e^{-v_dr^d}.
$$

The continuous tail gives $\mathbb P(R=0)=0$ and $\mathbb P(R=\infty)=0$. Differentiating the [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) gives the [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
\boxed{f_R(r)=d v_d r^{d-1}e^{-v_dr^d}\mathbf1_{\{r>0\}}.}
$$

The substitution $u=v_dr^d$ proves that this density integrates to one; equivalently $v_dR^d$ has the unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution). This is the first-neighbour case of the [Kth-nearest-neighbour distance in a homogeneous Poisson point process](../../../probability-theory.md#kth-nearest-neighbour-distance-in-a-homogeneous-poisson-point-process).

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

First derive the [Laplace functional of a Poisson random measure](../../../probability-theory.md#laplace-functional-of-a-poisson-random-measure). For a simple nonnegative $g=\sum_jt_j\mathbf1_{A_j}$ on disjoint finite-intensity sets, independent [Poisson random variables](../../../discrete-probability-distribution.md#poisson-distribution) give

$$
\mathbb E e^{-M(g)}=\prod_j\exp\bigl(\mu(A_j)(e^{-t_j}-1)\bigr)
=\exp\left(-\int(1-e^{-g})\,d\mu\right).
$$

Increasing simple approximations, [monotone convergence](../../../measure-theory.md#monotone-convergence-theorem) for the integrals, and [bounded convergence theorem](../../../measure-theory.md#bounded-convergence-theorem) for the random exponentials prove the same identity for every nonnegative measurable $g$.

Here the intensity is [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Put $A=B(0,r)$ and

$$
L=\exp\left(-\int_{\mathbb R^d}(1-e^{-f(x)})\,dx\right)=\mathbb E e^{-M(f)}.
$$

The integral is finite because $f$ has compact support. Apply the [Laplace functional of a Poisson random measure](../../../probability-theory.md#laplace-functional-of-a-poisson-random-measure) to $f+t\mathbf1_A$, $t\geq0$:

$$
\mathbb E e^{-M(f)-tN_r}
=L\exp\left(-(1-e^{-t})\int_Ae^{-f(x)}\,dx\right).
$$

Differentiate from the right at $t=0$. The difference quotient on the random side is dominated by $N_r$, which is integrable with mean $v_dr^d$; the intensity integral is over a finite-volume ball. We obtain the [count-weighted Laplace functional of a Poisson random measure](../../../probability-theory.md#count-weighted-laplace-functional-of-a-poisson-random-measure):

$$
\boxed{\mathbb E[N_re^{-M(f)}]
=\exp\left(-\int_{\mathbb R^d}(1-e^{-f(x)})\,dx\right)\int_{B(0,r)}e^{-f(x)}\,dx.}
$$

At $r=0$, the ball is empty and both sides are zero.

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

For $r>0$, write $m_r=v_dr^d$, $a_r=\int_{B(0,r)}e^{-f(x)}\,dx$, and $L=\mathbb Ee^{-M(f)}$. The [count-weighted Laplace functional of a Poisson random measure](../../../probability-theory.md#count-weighted-laplace-functional-of-a-poisson-random-measure) and the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) give

$$
\frac{\mathbb E[N_re^{-M(f)}]}{\mathbb P(N_r\geq1)}=L\frac{a_r}{1-e^{-m_r}}.
$$

To compute the other numerator, on $\{N_r=0\}$ the inside contribution to $M(f)$ vanishes. The restrictions of the [Poisson random measure](../../../probability-theory.md#poisson-random-measure) to the ball and its complement are independent; this follows first for their simple-function integrals from independent counts, then by approximation. Hence

$$
\begin{aligned}
\mathbb E[e^{-M(f)}\mathbf1_{\{N_r=0\}}]
&=e^{-m_r}\exp\left(-\int_{B(0,r)^c}(1-e^{-f(x)})\,dx\right)\\
&=L e^{-a_r}.
\end{aligned}
$$

Subtract from $L$ and divide by $\mathbb P(N_r\geq1)$ to find

$$
\mathbb E[e^{-M(f)}\mid N_r\geq1]=L\frac{1-e^{-a_r}}{1-e^{-m_r}}.
$$

Continuity of $f$ at zero gives

$$
\left|\frac{a_r}{m_r}-e^{-f(0)}\right|\leq\sup_{|x|<r}|e^{-f(x)}-e^{-f(0)}|\longrightarrow0.
$$

Also $(1-e^{-z})/z\to1$ as $z\downarrow0$. Applying these facts to the two exact expressions proves the [small-ball conditioning for a Poisson random measure](../../../probability-theory.md#small-ball-conditioning-for-a-poisson-random-measure):

$$
\boxed{\lim_{r\downarrow0}\mathbb E[e^{-M(f)}\mid N_r\geq1]
=\lim_{r\downarrow0}\frac{\mathbb E[N_re^{-M(f)}]}{\mathbb P(N_r\geq1)}
=\exp\left(-f(0)-\int_{\mathbb R^d}(1-e^{-f(x)})\,dx\right).}
$$

One can also see equality of the limits without the exact first formula: since $0\leq e^{-M(f)}\leq1$, the difference of the two quantities lies between zero and $[m_r-(1-e^{-m_r})]/(1-e^{-m_r})\to0$. The conditioning is used only at positive $r$, where its event has positive probability; it is not conditioning directly on a point at the origin.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
