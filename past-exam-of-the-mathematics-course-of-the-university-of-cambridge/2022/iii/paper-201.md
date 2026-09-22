# Paper 201

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_201.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_201.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)
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
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The partial sums $S_n$ are a [martingale](../../../martingale.md), as are $S_n^2-n$. Since the increment has mean zero and nonzero variance, there are $\delta_+,\delta_->0$ with $\mathbb P(X_1\geq\delta_+)>0$ and $\mathbb P(X_1\leq-\delta_-)>0$. From any point in $(-a,b)$, a sufficiently long run of either kind exits the interval. Independence in consecutive blocks therefore bounds $\mathbb P(T>km)$ by a geometric sequence. In particular, $T<\infty$ almost surely and $\mathbb ET<\infty$.

Apply the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) first to $T\wedge n$. Since the increments are bounded and $\mathbb ET<\infty$, the stopped variables are uniformly integrable and passage to the limit gives

$$
\mathbb E S_T=0.
$$

Applying the same argument to $S_n^2-n$, using $|S_T|\leq\max\{a,b\}+c$, gives

$$
\boxed{\mathbb E(S_T^2-T)=0,
\qquad
\mathbb E S_T^2=\mathbb ET.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

On upper exit, $b\leq S_T\leq b+c$; on lower exit, $-a-c\leq S_T\leq-a$. With $p=\mathbb P(S_T\geq b)$ and $\mathbb ES_T=0$,

$$
pb-(1-p)(a+c)\leq0
\leq p(b+c)-(1-p)a.
$$

Solving gives

$$
\frac a{a+b+c}\leq p\leq\frac{a+c}{a+b+c}.
$$

Moreover $(S_T+a)(S_T-b)\geq0$, so $\mathbb ES_T^2\geq ab$, which is stronger than the requested lower bound. Also $S_T\in[-a-c,b+c]$, and hence

$$
(S_T+a+c)(b+c-S_T)\geq0.
$$

Taking expectations and using $\mathbb ES_T=0$ gives $\mathbb ES_T^2\leq(a+c)(b+c)$, stronger than the requested upper bound. Since

$$
ab\geq\frac{ab(a+b)}{a+b+c},
\qquad
(a+c)(b+c)\leq
\frac{(a+c)(b+c)(a+b+2c)}{a+b+c},
$$

the two stated estimates follow from part a.

## 2

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) states that for independent identically distributed integrable random variables,

$$
\frac{S_n}{n}\longrightarrow\mu
\quad\text{almost surely}.
$$

To prove it, set $Y_n=X_n\mathbf1_{\{|X_n|\leq n\}}$. The tail-sum formula gives $\sum_n\mathbb P(X_n\ne Y_n)<\infty$, so the [Borel-Cantelli lemmas](../../../probability-theory.md#borel-cantelli-lemmas) make the two sequences eventually equal. Also

$$
\sum_{n=1}^\infty\frac{\operatorname{Var}(Y_n)}{n^2}
\leq\mathbb E\left[
X_1^2\sum_{n\geq|X_1|}\frac1{n^2}\right]
\leq C\mathbb E|X_1|<\infty.
$$

The [Kolmogorov convergence theorem](../../../convergence-of-random-variables.md#kolmogorov-convergence-theorem) implies that $\sum_n(Y_n-\mathbb EY_n)/n$ converges almost surely, and [Kronecker lemma](../../../real-analysis.md#kronecker-lemma) yields

$$
\frac1n\sum_{j=1}^n(Y_j-\mathbb EY_j)\to0.
$$

Finally $\mathbb EY_n\to\mu$, so the [Cesaro mean](../../../real-analysis.md#cesaro-mean) of these expectations tends to $\mu$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

After replacing $X_j$ by $X_j-\mu$, the maximal inequality for independent averages gives

$$
\left\|\sup_{m\geq1}\frac{|S_m|}{m}\right\|_{L^p}
\leq C_p\|X_1\|_{L^p},
\qquad p>1.
$$

This follows from the [Doob Lp maximal inequality](../../../martingale.md#doob-lp-maximal-inequality) by dyadically grouping the partial sums. The strong law makes

$$
\sup_{m\geq n}\frac{|S_m|}{m}\longrightarrow0
$$

almost surely. The displayed maximal function is in $L^p$, so [dominated convergence](../../../measure-theory.md#dominated-convergence-theorem) applied to its $p$th power proves convergence in $L^p$.

## 3

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Prokhorov's theorem](../../../convergence-of-random-variables.md#prokhorov-s-theorem) says that a sequence of Borel probability measures on $\mathbb R$ is relatively compact for [weak convergence of probability measures](../../../convergence-of-random-variables.md#weak-convergence-of-probability-measures) exactly when it is tight: for every $\epsilon>0$, some compact $K$ satisfies $\sup_n\mu_n(\mathbb R\setminus K)<\epsilon$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $z=y/\lambda$. Direct integration gives

$$
\lambda\int_0^{1/\lambda}(1-\cos uy)\,du
=1-\frac{\sin z}{z}.
$$

For $|z|\geq1$, the right side has a positive infimum $c_0$ because $\sin z/z<1$ there and it tends to one at infinity. Thus the claimed inequality holds with $C=c_0^{-1}$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The masses $\mu_n(\mathbb R)=\psi_n(0)$ converge and are therefore bounded. Part b and [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) give

$$
\mu_n(\{|y|\geq\lambda\})
\leq C\lambda\int_0^{1/\lambda}
\bigl(\psi_n(0)-\operatorname{Re}\psi_n(u)\bigr)\,du.
$$

The integrands are uniformly bounded. By pointwise convergence and the continuity of $\psi$ at zero, the right side can be made uniformly small for all sufficiently large $n$ by taking $\lambda$ large; finitely many remaining measures are individually tight. Thus $(\mu_n)$ is tight. Applying [Prokhorov's theorem](../../../convergence-of-random-variables.md#prokhorov-s-theorem) after normalizing the masses, or adjoining missing mass at one fixed point, gives a weakly convergent subsequence.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

**Yes.** If a subsequence converges weakly to $\nu$, bounded continuity of $e^{iuy}$ gives

$$
\widehat\nu(u)=\lim_k\psi_{n(k)}(u)=\psi(u).
$$

The [uniqueness theorem for characteristic functions](../../../probability-theory.md#uniqueness-theorem-for-characteristic-functions) makes $\nu$ unique. Tightness implies that every subsequence has a further weakly convergent subsequence, and every such limit is $\nu$. This subsequence criterion proves that the entire sequence converges weakly to $\nu$.

## 4

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

If $t\leq s$, then $\mathbb E(X_t\mid\mathcal F_s)=X_t$. If $s<t\leq1$, [Gaussian conditional expectation](../../../statistical-modelling.md#gaussian-conditional-expectation) for the [Brownian bridge](../../../brownian-motion.md#brownian-bridge) between $(s,X_s)$ and $(1,X_1)$ gives

$$
\boxed{\mathbb E(X_t\mid\mathcal F_s)
=X_s+\frac{t-s}{1-s}(X_1-X_s).}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Since $X_1-X_s$ is centered Gaussian with variance $1-s$,

$$
\mathbb E\int_0^1\frac{|X_1-X_s|}{1-s}\,ds
=C\int_0^1(1-s)^{-1/2}\,ds<\infty.
$$

[Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) therefore shows that the defining integral for $A_1$ is absolutely finite almost surely.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $s<r<1$, part a gives

$$
\mathbb E\left(\left.\frac{X_1-X_r}{1-r}\right|\mathcal F_s\right)
=\frac{X_1-X_s}{1-s}.
$$

Conditional Fubini then yields

$$
\mathbb E(A_t-A_s\mid\mathcal F_s)
=\frac{t-s}{1-s}(X_1-X_s)
=\mathbb E(X_t-X_s\mid\mathcal F_s).
$$

**Hence $\mathbb E(M_t\mid\mathcal F_s)=M_s$, so $M$ is a martingale.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The process $M$ is continuous and Gaussian. Since $A$ has finite variation,

$$
[M]_t=[X]_t=t.
$$

The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) makes $M$ a Brownian motion in the enlarged filtration.

Moreover,

$$
\operatorname{Cov}(M_t,X_1)
=t-\int_0^t\frac{\operatorname{Cov}(X_1-X_s,X_1)}{1-s}\,ds
=t-\int_0^t1\,ds=0.
$$

Every finite vector from $M$ is jointly Gaussian with $X_1$, so zero covariance implies independence. Thus the whole process $M$ is independent of $X_1$.

## 5

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The function $u(x)=\epsilon/|x|$ is [harmonic](../../../partial-differential-equation.md#harmonic-function) on $\{|x|>\epsilon\}$, equals one on the target sphere, and tends to zero at infinity. Optional stopping at the first hit of radius $\epsilon$ and the first exit from a ball of radius $R$ gives

$$
\mathbb P_x(\tau_\epsilon<\tau_R)
=\frac{|x|^{-1}-R^{-1}}{\epsilon^{-1}-R^{-1}}.
$$

Letting $R\to\infty$ and taking $|x|=1$ yields $\mathbb P_x(\tau_\epsilon<\infty)=\epsilon$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Project Brownian motion modulo $\mathbb Z^3$ to the compact three-dimensional [torus](../../../topology.md#torus). The projected process has normalized volume as invariant probability measure and is irreducible, so it visits every nonempty open set infinitely often almost surely. The image of $S_3$ contains the radius-$\epsilon$ ball about the origin. Hence the original Brownian motion hits $S_3$ at an unbounded set of times.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

**Yes.** Quotient only the first coordinate modulo $\mathbb Z$. The resulting process lives on $\mathbb T\times\mathbb R^2$ and the image of $S_1$ is the radius-$\epsilon$ ball about $(0,0,0)$. The two noncompact coordinates form [planar Brownian motion](../../../brownian-motion.md#planar-brownian-motion), which is recurrent; during its infinitely many returns to a smaller disc, the independent circle coordinate has a fixed positive chance of lying in the required interval. The [Strong Markov property](../../../markov-process.md#strong-markov-property) then shows that the target ball is visited infinitely often. Lifting back proves that $S_1$ is hit at unbounded times.

## 6

↑ **Parent:** [Paper 201](paper-201.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [Poisson random measure](../../../probability-theory.md#poisson-point-process) $N$ of intensity $\mu$ assigns to disjoint measurable sets independent random variables, and

$$
N(A)\sim\operatorname{Poisson}(\mu(A))
$$

whenever $\mu(A)<\infty$, with the usual countable-additivity requirement.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

A [Lévy process](../../../stochastic-process.md#levy-process) starts at zero almost surely, has stationary independent increments, and is stochastically continuous; one normally takes its càdlàg modification.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Independent [Poisson processes](../../../probability-theory.md#poisson-process) have stationary independent increments, so their weighted sum does too and is stochastically continuous. Moreover,

$$
\mathbb E e^{iuX_t}
=\prod_{k=1}^n
\exp\{t\lambda_k(e^{iua_k}-1)\}
=e^{t\psi(u)},
$$

where

$$
\psi(u)=\sum_{k=1}^n\lambda_k(e^{iua_k}-1).
$$

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Let $N(ds,dy)$ be a Poisson random measure on $(0,\infty)^2$ with intensity $ds\,K(dy)$ and define

$$
X_t=\int_{(0,t]\times(0,\infty)}y\,N(ds,dy).
$$

The assumption $\int yK(dy)<\infty$ makes this integral finite on compact time intervals. The exponential formula for a Poisson random measure gives

$$
\mathbb Ee^{iuX_t}
=\exp\left\{t\int_{(0,\infty)}(e^{iuy}-1)K(dy)\right\},
$$

so $X$ is a Lévy process with exponent $\psi$.

Choose finite-valued measurable functions $q_n\geq0$ which vanish off $[1/n,n]$ and satisfy

$$
\int|q_n(y)-y|K(dy)\longrightarrow0.
$$

This is possible by truncation followed by approximation by simple functions. Put

$$
X_t^n=\int_{(0,t]\times(0,\infty)}q_n(y)\,N(ds,dy).
$$

The measure of the support of $q_n$ is finite, and $q_n$ takes finitely many values, so $X^n$ is a simple pure-jump Lévy process. Under this common coupling,

$$
\boxed{\mathbb E\sup_{s\leq t}|X_s^n-X_s|
\leq\mathbb E\int_{(0,t]\times(0,\infty)}
|q_n(y)-y|\,N(ds,dy)
=t\int|q_n-y|\,dK\longrightarrow0.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
