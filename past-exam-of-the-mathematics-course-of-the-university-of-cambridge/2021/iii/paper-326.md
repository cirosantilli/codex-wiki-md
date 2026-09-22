# Paper 326

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_326.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_326.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [Solution](#1/1/solution)
    - [2](#1/1/2)
      - [Solution](#1/1/2/solution)
    - [3](#1/1/3)
      - [a](#1/1/3/a)
        - [Solution](#1/1/3/a/solution)
      - [b](#1/1/3/b)
        - [Solution](#1/1/3/b/solution)
      - [c](#1/1/3/c)
        - [Solution](#1/1/3/c/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
    - [3](#2/2/3)
      - [a](#2/2/3/a)
        - [Solution](#2/2/3/a/solution)
      - [b](#2/2/3/b)
        - [Solution](#2/2/3/b/solution)
- [3](#3)
  - [1](#3/1)
    - [a](#3/1/a)
      - [Solution](#3/1/a/solution)
    - [b](#3/1/b)
      - [Solution](#3/1/b/solution)
    - [c](#3/1/c)
      - [Solution](#3/1/c/solution)
    - [d](#3/1/d)
      - [Solution](#3/1/d/solution)
  - [2](#3/2)
    - [a](#3/2/a)
      - [Solution](#3/2/a/solution)
    - [b](#3/2/b)
      - [Solution](#3/2/b/solution)
  - [3](#3/3)
    - [a](#3/3/a)
      - [Solution](#3/3/a/solution)
    - [b](#3/3/b)
      - [Solution](#3/3/b/solution)
    - [c](#3/3/c)
      - [Solution](#3/3/c/solution)
    - [d](#3/3/d)
      - [Solution](#3/3/d/solution)
- [4](#4)
  - [1](#4/1)
    - [Solution](#4/1/solution)
  - [2](#4/2)
    - [a](#4/2/a)
      - [Solution](#4/2/a/solution)
    - [b](#4/2/b)
      - [Solution](#4/2/b/solution)
    - [c](#4/2/c)
      - [Solution](#4/2/c/solution)
  - [3](#4/3)
    - [Solution](#4/3/solution)

## 1

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

A problem is [well posed in the sense of Hadamard](../../../inverse-problem.md#well-posed-problem) when a solution exists for every admissible datum, is unique, and depends [continuously](../../../calculus.md#continuous-function) on the datum. It is ill posed if any one of these three properties fails.

For the [inverse problem](../../../inverse-problem.md) $Au=f$, a [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem) is a family of bounded maps $R_\alpha:Y\to X$ that approximate the generally unbounded [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) $A^\dagger$. It is a [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem) if there is a parameter rule $\alpha=\alpha(\delta,f^\delta)$ such that

$$
\alpha(\delta,f^\delta)\longrightarrow0,
\qquad
\sup_{\|f^\delta-f\|\leq\delta}
\|R_{\alpha(\delta,f^\delta)}f^\delta-A^\dagger f\|
\longrightarrow0
$$

as $\delta\downarrow0$ for every $f\in\mathcal D(A^\dagger)$.

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/solution">Solution</h5>

↑ **Parent:** [2](#1/1/2)

Let $(\sigma_i,x_i,y_i)$ be the [singular system of a compact operator](../../../inverse-problem.md#singular-system-of-a-compact-operator). Since $P_nx_i=x_i$ for $i\leq n$ and $P_nx_i=0$ for $i>n$, the truncated operator $T_n=AP_n$ has the finite [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition)

$$
T_nx_i=\sigma_i y_i\quad(i\leq n),
\qquad
T_nx_i=0\quad(i>n).
$$

Consequently

$$
T_n^\dagger y
=\sum_{i=1}^n\frac{\langle y,y_i\rangle}{\sigma_i}x_i
=A^\dagger Q_ny,
$$

so $\boxed{T_n^\dagger=A^\dagger Q_n}$.

For completeness, $T_n^\dagger T_n=P_n$ on $(\ker A)^\perp$ and $T_nT_n^\dagger=Q_n$. These are self-adjoint [orthogonal projectors](../../../hilbert-space.md#orthogonal-projection), and hence

$$
T_nT_n^\dagger T_n=T_n,
\qquad
T_n^\dagger T_nT_n^\dagger=T_n^\dagger.
$$

**Thus all four [Penrose equations](../../../linear-algebra.md#penrose-equations) hold, which verifies the formula independently of the singular expansion.**

<h4 id="1/1/3">3</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/3/a">a</h5>

↑ **Parent:** [3](#1/1/3)

<h6 id="1/1/3/a/solution">Solution</h6>

↑ **Parent:** [A](#1/1/3/a)

Repeated substitution in [Landweber iteration](../../../inverse-problem.md#landweber-iteration) from $u_0=0$ gives

$$
u_k
=\tau\sum_{j=0}^{k-1}(I-\tau A^*A)^jA^*f.
$$

On the $i$th singular vector, $A^*A$ has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\sigma_i^2$ and $A^*y_i=\sigma_ix_i$. The finite [geometric series](../../../real-analysis.md#geometric-series) therefore gives

$$
\boxed{
u_k=\sum_i
\frac{1-(1-\tau\sigma_i^2)^k}{\sigma_i}
\langle f,y_i\rangle x_i}.
$$

This is a [spectral regularization method](../../../inverse-problem.md#spectral-regularization-method) with filter

$$
\boxed{g_k(\lambda)=\frac{1-(1-\tau\lambda)^k}{\lambda},
\qquad
u_k=g_k(A^*A)A^*f.}
$$

<h5 id="1/1/3/b">b</h5>

↑ **Parent:** [3](#1/1/3)

<h6 id="1/1/3/b/solution">Solution</h6>

↑ **Parent:** [B](#1/1/3/b)

The regularization parameter is the [stopping index](../../../statistical-learning.md#early-stopping) $k$: increasing $k$ reduces the approximation bias but amplifies noise. Equivalently one may use the parameter $\alpha=1/k$, which tends to zero as $k\to\infty$.

<h5 id="1/1/3/c">c</h5>

↑ **Parent:** [3](#1/1/3)

<h6 id="1/1/3/c/solution">Solution</h6>

↑ **Parent:** [C](#1/1/3/c)

It is sufficient that

$$
\boxed{0<\tau<\frac{2}{\|A\|^2}},
$$

and that the stopping rule obey

$$
k(\delta)\longrightarrow\infty,
\qquad
\delta\sqrt{k(\delta)}\longrightarrow0.
$$

For example, $k(\delta)=\lfloor\delta^{-1}\rfloor$ works.

For exact data $f\in\mathcal D(A^\dagger)$, each factor $(1-\tau\sigma_i^2)^k$ tends to zero. The [Picard criterion](../../../inverse-problem.md#picard-criterion) makes $\langle f,y_i\rangle/\sigma_i$ square summable, while $|1-(1-\tau\sigma_i^2)^k|$ is uniformly bounded. The [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) on the resulting series yields $u_k(f)\to A^\dagger f$.

For noisy data with $\|f^\delta-f\|\leq\delta$, the filter representation gives

$$
\|u_k(f^\delta)-u_k(f)\|
\leq
\delta\sup_{0<\sigma\leq\|A\|}
\frac{|1-(1-\tau\sigma^2)^k|}{\sigma}
\leq C_\tau\delta\sqrt{k}.
$$

Indeed, when $\tau\sigma^2\leq1$, [Bernoulli's inequality](../../../algebra.md#bernoulli-s-inequality) gives $1-(1-\tau\sigma^2)^k\leq\min(k\tau\sigma^2,1)$; when $\tau\sigma^2>1$, the quotient is uniformly bounded because $\tau\|A\|^2<2$. Hence the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\|u_{k(\delta)}(f^\delta)-A^\dagger f\|
\leq C_\tau\delta\sqrt{k(\delta)}
+\|u_{k(\delta)}(f)-A^\dagger f\|
\longrightarrow0,
$$

which proves that early-stopped Landweber iteration is a [convergent regularization of an inverse problem](../../../inverse-problem.md#convergent-regularization-of-an-inverse-problem).

<h2 id="2">2</h2>

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

For $u\in L^1(\Omega)$, its [total variation seminorm on a domain](../../../inverse-problem.md#total-variation-seminorm-on-a-domain) is

$$
\operatorname{TV}(u)
=\sup\left\{
\int_\Omega u\,\operatorname{div}\varphi\,dx:
\varphi\in C_c^1(\Omega;\mathbb R^n),\ 
\|\varphi\|_\infty\leq1
\right\}.
$$

The corresponding [bounded-variation space](../../../inverse-problem.md#function-of-bounded-variation-on-a-domain) and its zero-mean subspace are

$$
BV(\Omega)=\{u\in L^1(\Omega):\operatorname{TV}(u)<\infty\},
\qquad
BV_0(\Omega)=\left\{u\in BV(\Omega):\int_\Omega u\,dx=0\right\}.
$$

If $u_\Omega=|\Omega|^{-1}\int_\Omega u\,dx$, the [Poincaré inequality for total variation](../../../inverse-problem.md#poincare-inequality-for-total-variation) is

$$
\boxed{\|u-u_\Omega\|_{L^1(\Omega)}\leq C_\Omega\operatorname{TV}(u)}.
$$

In particular, $\|u\|_{L^1}\leq C_\Omega\operatorname{TV}(u)$ for $u\in BV_0(\Omega)$.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

A $J$-minimizing solution is an exact solution $u_J^\dagger$ satisfying

$$
Au_J^\dagger=f,
\qquad
J(u_J^\dagger)=\inf\{J(u):Au=f\}.
$$

The [source condition in variational regularization](../../../inverse-problem.md#source-condition-in-variational-regularization) says that some $p^\dagger\in Y$ satisfies

$$
\boxed{A^*p^\dagger\in\partial J(u_J^\dagger)},
$$

where $\partial J$ is the [subdifferential](../../../convex-optimization.md#subdifferential).

Fix $\alpha>0$. The [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition) for

$$
F_g(u)=\frac12\|Au-g\|_Y^2+\alpha J(u)
$$

at $u_J^\dagger$ is

$$
0\in A^*(Au_J^\dagger-g)+\alpha\partial J(u_J^\dagger).
$$

If the source condition holds, choose $g=f+\alpha p^\dagger$. Since $Au_J^\dagger=f$, the displayed inclusion holds. Because the objective is a [convex function](../../../real-analysis.md#convex-function), this condition is necessary and sufficient for global minimality.

Conversely, if the stated range condition holds for some $g$, optimality supplies $\xi\in\partial J(u_J^\dagger)$ with

$$
A^*(f-g)+\alpha\xi=0.
$$

**Thus $\xi=A^*((g-f)/\alpha)$, which is precisely the source condition. This proves the equivalence.**

<h4 id="2/2/3">3</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/3/a">a</h5>

↑ **Parent:** [3](#2/2/3)

<h6 id="2/2/3/a/solution">Solution</h6>

↑ **Parent:** [A](#2/2/3/a)

For an [absolutely one-homogeneous functional](../../../convex-optimization.md#absolutely-one-homogeneous-functional) $J$, the subdifferential has the characterization

$$
p\in\partial J(u)
\quad\Longleftrightarrow\quad
\langle p,u\rangle=J(u)
\ 
\text{and}
\ 
\langle p,v\rangle\leq J(v)\quad\text{for every }v.
$$

If $c>0$, then $J(cu)=cJ(u)$, so

$$
\langle p,cu\rangle=c\langle p,u\rangle=cJ(u)=J(cu).
$$

The second condition does not involve the base point. Therefore

$$
\boxed{\partial J(cu)=\partial J(u)}.
$$

<h5 id="2/2/3/b">b</h5>

↑ **Parent:** [3](#2/2/3)

<h6 id="2/2/3/b/solution">Solution</h6>

↑ **Parent:** [B](#2/2/3/b)

Because $\lambda f\in\partial J(f)$ and $1-\lambda\alpha>0$ when $\alpha<1/\lambda$, part a gives

$$
\lambda f\in\partial J((1-\lambda\alpha)f).
$$

Set $u=(1-\lambda\alpha)f$. Then

$$
0=u-f+\alpha\lambda f
\in u-f+\alpha\partial J(u).
$$

This is the [subgradient optimality condition](../../../real-analysis.md#subgradient-optimality-condition) for

$$
\frac12\|u-f\|^2+\alpha J(u).
$$

The squared norm is [strictly convex](../../../real-analysis.md#strictly-convex-function), so the objective has at most one minimizer. Hence

$$
\boxed{u=(1-\lambda\alpha)f}
$$

is its unique minimizer.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/a">a</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/a/solution">Solution</h5>

↑ **Parent:** [A](#3/1/a)

A [Bayesian inverse problem](../../../stochastic-process.md#bayesian-inverse-problem) consists of a [prior distribution](../../../statistical-inference.md#prior-probability) $\mu_0$ on the unknown $u\in X$, a reference measure on the data space $Y$, and a jointly [measurable](../../../measure-theory.md#measurable-function) likelihood $L(u;y)$ such that $L(u;\mathord\cdot)$ is a [probability density function](../../../continuous-probability-distribution.md#probability-density-function) for $\mu_0$-almost every $u$. For observed data $y$, [Bayes' theorem](../../../probability-theory.md#bayes-theorem) defines the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) by

$$
\boxed{
\frac{d\mu^y}{d\mu_0}(u)
=\frac{L(u;y)}{Z(y)},
\qquad
Z(y)=\int_XL(u;y)\,d\mu_0(u)},
$$

provided $0<Z(y)<\infty$.

<h4 id="3/1/b">b</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/b/solution">Solution</h5>

↑ **Parent:** [B](#3/1/b)

The [total variation distance](../../../probability-and-statistics.md#total-variation-distance) is

$$
\boxed{d_{\mathrm{TV}}(\mu,\nu)
=\sup_{B\in\mathcal B_X}|\mu(B)-\nu(B)|}.
$$

If both measures have densities $p,q$ with respect to a common [dominating measure](../../../measure-theory.md#dominating-measure), then $d_{\mathrm{TV}}(\mu,\nu)=\frac12\int|p-q|$.

<h4 id="3/1/c">c</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/c/solution">Solution</h5>

↑ **Parent:** [C](#3/1/c)

The problem is a [well-posed Bayesian inverse problem in total variation](../../../stochastic-process.md#well-posed-bayesian-inverse-problem-in-total-variation) when a unique posterior $\mu^y$ exists for every $y\in Y$ and the posterior map is continuous:

$$
y_n\longrightarrow y
\quad\Longrightarrow\quad
d_{\mathrm{TV}}(\mu^{y_n},\mu^y)\longrightarrow0.
$$

**Thus the metric supplies the precise meaning of continuous dependence on the observed data in the Bayesian version of [Hadamard well-posedness](../../../inverse-problem.md#well-posed-problem).**

<h4 id="3/1/d">d</h4>

↑ **Parent:** [1](#3/1)

<h5 id="3/1/d/solution">Solution</h5>

↑ **Parent:** [D](#3/1/d)

The following four assumptions are sufficient, with statements understood for $\mu_0$-almost every $u$ and every $y$:

- $L(u;\mathord\cdot)$ is a strictly positive [probability density function](../../../continuous-probability-distribution.md#probability-density-function) on the data space.
- $L(\mathord\cdot;y)\in L^1(X,\mu_0)$.
- There is one $h\in L^1(X,\mu_0)$ such that $L(u;y)\leq h(u)$ for all $y$.
- For each relevant $u$, the map $y\mapsto L(u;y)$ is [continuous](../../../calculus.md#continuous-function).

The first two assumptions give $0<Z(y)<\infty$. The last two allow the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) to prove $L^1(\mu_0)$ continuity of the normalized posterior density, which is equivalent to continuity in [total variation distance](../../../probability-and-statistics.md#total-variation-distance).

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/a">a</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/a/solution">Solution</h5>

↑ **Parent:** [A](#3/2/a)

The noise has the product [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution) density

$$
g(y)=\prod_{j=1}^ke^{-2|y_j|}=e^{-2\|y\|_1},
$$

which is normalized because $\int_{\mathbb R}e^{-2|t|}\,dt=1$. By translation invariance of [Lebesgue measure](../../../measure-theory.md#lebesgue-measure), the conditional law of $A(u)+N$ has density

$$
p(y\mid u)=g(y-A(u))
=\exp[-2\|y-A(u)\|_1].
$$

Hence an associated [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
\boxed{L(u;y)=\exp[-2\|y-A(u)\|_1]}.
$$

The map $(u,y)\mapsto y-A(u)$ is measurable because $A$ is measurable and vector subtraction is [continuous](../../../calculus.md#continuous-function). Composition with the continuous norm and exponential functions proves that $L$ is jointly measurable.

<h4 id="3/2/b">b</h4>

↑ **Parent:** [2](#3/2)

<h5 id="3/2/b/solution">Solution</h5>

↑ **Parent:** [B](#3/2/b)

We may take the everywhere-defined representative

$$
\boxed{L_0(u;y)=\exp[-2\|y-A(u)\|_1]}.
$$

It agrees with the likelihood from part a, hence certainly agrees $\mu_0\otimes\lambda_k$-almost everywhere. For every $u$, it is a strictly positive density in $y$ and is continuous in $y$. Moreover

$$
0<L_0(u;y)\leq1,
$$

so the constant function $h(u)=1$ is an integrable dominator for every [probability measure](../../../probability-theory.md#probability-measure) $\mu_0$. All four sufficient assumptions from part 1d therefore hold, and the Bayesian inverse problem is well posed in [total variation distance](../../../probability-and-statistics.md#total-variation-distance).

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/a">a</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/a/solution">Solution</h5>

↑ **Parent:** [A](#3/3/a)

Take

$$
\boxed{\nu=\mu+\mu_0}.
$$

This is a [finite measure](../../../measure-theory.md#finite-measure), hence a [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure). If $\nu(B)=0$, nonnegativity gives $\mu(B)=\mu_0(B)=0$, so both $\mu$ and $\mu_0$ are [absolutely continuous](../../../measure-theory.md#absolute-continuity-of-measures) with respect to $\nu$.

<h4 id="3/3/b">b</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/b/solution">Solution</h5>

↑ **Parent:** [B](#3/3/b)

Write $p=d\mu/d\rho$ and $q=d\mu_0/d\rho$, whose existence follows from the [Radon-Nikodym theorem](../../../measure-theory.md#radon-nikodym-theorem). Since

$$
(\sqrt p-\sqrt q)^2\leq p+q,
$$

we have

$$
\int_X(\sqrt p-\sqrt q)^2\,d\rho
\leq\int_X(p+q)\,d\rho=2.
$$

**Thus the defining integral is finite and the [Hellinger distance](../../../probability-and-statistics.md#hellinger-distance) is well defined.**

<h4 id="3/3/c">c</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/c/solution">Solution</h5>

↑ **Parent:** [C](#3/3/c)

For nonnegative $p,q$,

$$
(\sqrt p-\sqrt q)^2
=\frac{(p-q)^2}{(\sqrt p+\sqrt q)^2}
\leq|p-q|.
$$

Integrating and using the density formula for [total variation distance](../../../probability-and-statistics.md#total-variation-distance) gives

$$
\boxed{
d_{\mathrm{Hel}}(\mu,\mu_0)^2
\leq\int_X|p-q|\,d\rho
=2d_{\mathrm{TV}}(\mu,\mu_0)}.
$$

<h4 id="3/3/d">d</h4>

↑ **Parent:** [3](#3/3)

<h5 id="3/3/d/solution">Solution</h5>

↑ **Parent:** [D](#3/3/d)

Every posterior given by [Bayes' theorem](../../../probability-theory.md#bayes-theorem) is absolutely continuous with respect to its prior $\mu_0$, so it belongs to $\operatorname{Prob}(X,\mathcal B_X,\mu_0)$. If $y_n\to y$, total-variation well-posedness gives

$$
d_{\mathrm{TV}}(\mu^{y_n},\mu^y)\longrightarrow0.
$$

Part c, now using the common dominating measure $\mu_0$, yields

$$
d_{\mathrm{Hel}}(\mu^{y_n},\mu^y)^2
\leq2d_{\mathrm{TV}}(\mu^{y_n},\mu^y)
\longrightarrow0.
$$

Existence and uniqueness are unchanged. The problem is therefore a [well-posed Bayesian inverse problem in Hellinger distance](../../../stochastic-process.md#well-posed-bayesian-inverse-problem-in-hellinger-distance).

## 4

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="4/1">1</h3>

↑ **Parent:** [4](#4)

<h4 id="4/1/solution">Solution</h4>

↑ **Parent:** [1](#4/1)

A [Gaussian measure](../../../stochastic-process.md#gaussian-measure) $\mu$ on a real separable [Banach space](../../../banach-space.md) $X$ is a [Borel probability measure](../../../measure-theory.md#borel-measure) such that $\ell_*\mu$ is a one-dimensional [normal distribution](../../../probability-theory.md#normal-distribution) for every [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) $\ell\in X^*$. Its mean $m\in X$ and [covariance operator of a Gaussian measure](../../../stochastic-process.md#covariance-operator-of-a-gaussian-measure) $C:X^*\to X$ are characterized by

$$
\ell(m)=\int_X\ell(u)\,d\mu(u),
$$

and

$$
\ell_2(C\ell_1)
=\int_X\ell_1(u-m)\ell_2(u-m)\,d\mu(u)
$$

for all $\ell_1,\ell_2\in X^*$.

<h3 id="4/2">2</h3>

↑ **Parent:** [4](#4)

<h4 id="4/2/a">a</h4>

↑ **Parent:** [2](#4/2)

<h5 id="4/2/a/solution">Solution</h5>

↑ **Parent:** [A](#4/2/a)

The [indicator functions](../../../measure-theory.md#indicator-function) satisfy

$$
\|\varphi_1\|_{L^2}^2=\lambda_1(A)<\infty,
\qquad
\|\varphi_2\|_{L^2}^2=1-\lambda_1(A)<\infty.
$$

**Therefore $\varphi_1,\varphi_2\in L^2[0,1]$.**

<h4 id="4/2/b">b</h4>

↑ **Parent:** [2](#4/2)

<h5 id="4/2/b/solution">Solution</h5>

↑ **Parent:** [B](#4/2/b)

For every $h\in L^2[0,1]$, the [continuous linear functional](../../../topological-vector-space.md#continuous-linear-functional) induced by the [inner product](../../../linear-algebra.md#inner-product) gives

$$
\langle U,h\rangle
=\xi_1\langle\varphi_1,h\rangle
+\xi_2\langle\varphi_2,h\rangle.
$$

This is a [normal random variable](../../../probability-theory.md#normal-distribution) because it is a [linear combination of independent normal random variables](../../../probability-theory.md#linear-combination-of-independent-normal-random-variables). Hence the law of $U$ is a [Gaussian measure](../../../stochastic-process.md#gaussian-measure). Its mean is zero, and independence together with $\operatorname{Var}(\xi_i)=1/2$ gives

$$
\mathbb E[\langle U,h\rangle\langle U,g\rangle]
=\frac12\langle\varphi_1,h\rangle\langle\varphi_1,g\rangle
+\frac12\langle\varphi_2,h\rangle\langle\varphi_2,g\rangle.
$$

Thus its [covariance operator of a Gaussian measure](../../../stochastic-process.md#covariance-operator-of-a-gaussian-measure) is

$$
\boxed{
Ch=\frac12\langle\varphi_1,h\rangle\varphi_1
+\frac12\langle\varphi_2,h\rangle\varphi_2}.
$$

<h4 id="4/2/c">c</h4>

↑ **Parent:** [2](#4/2)

<h5 id="4/2/c/solution">Solution</h5>

↑ **Parent:** [C](#4/2/c)

The supports of $\varphi_1$ and $\varphi_2$ are disjoint, so they are [orthogonal vectors](../../../linear-algebra.md#orthogonal-vectors). Substitution in the covariance formula gives

$$
C\varphi_1
=\frac12\|\varphi_1\|^2\varphi_1
=\frac{\lambda_1(A)}2\varphi_1,
$$

and

$$
C\varphi_2
=\frac12\|\varphi_2\|^2\varphi_2
=\frac{1-\lambda_1(A)}2\varphi_2.
$$

Therefore the associated [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
\boxed{\gamma_1=\frac{\lambda_1(A)}2,
\qquad
\gamma_2=\frac{1-\lambda_1(A)}2}.
$$

<h3 id="4/3">3</h3>

↑ **Parent:** [4](#4)

<h4 id="4/3/solution">Solution</h4>

↑ **Parent:** [3](#4/3)

Put $c_i=\int_D\varphi_i(x)\,d\lambda_n(x)$. The stated scalar random variable is

$$
Z=\int_DU(x)\,d\lambda_n(x)
=\sum_{i=1}^k\sqrt{\nu_i}\,c_i\xi_i.
$$

As a finite [linear combination of independent normal random variables](../../../probability-theory.md#linear-combination-of-independent-normal-random-variables), it is normally distributed. Its mean is zero and its variance is

$$
\boxed{\operatorname{Var}(Z)
=\frac12\sum_{i=1}^k\nu_i
\left(\int_D\varphi_i\,d\lambda_n\right)^2}.
$$

Finally, [orthonormality](../../../linear-algebra.md#orthonormal-set) of the $\varphi_i$ gives

$$
\|U\|_X^2=\sum_{i=1}^k\nu_i\xi_i^2.
$$

Since $\mathbb E\xi_i^2=1/2$,

$$
\boxed{\int_\Omega\|U\|_X^2\,d\mathbb P
=\frac12\sum_{i=1}^k\nu_i}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
