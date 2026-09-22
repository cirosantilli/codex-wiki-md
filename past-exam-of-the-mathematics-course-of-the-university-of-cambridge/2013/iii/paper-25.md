# Paper 25

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_25.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_25.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [1](#1/a/1)
      - [Solution](#1/a/1/solution)
    - [2](#1/a/2)
      - [Solution](#1/a/2/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [1](#1/c/1)
      - [Solution](#1/c/1/solution)
    - [2](#1/c/2)
      - [Solution](#1/c/2/solution)
    - [3](#1/c/3)
      - [Solution](#1/c/3/solution)
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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
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

## 1

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/1">1</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/1/solution">Solution</h5>

↑ **Parent:** [1](#1/a/1)

Choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(e_j)$ of the [separable Hilbert space](../../../hilbert-space.md#separable-hilbert-space) and independent standard [normal random variables](../../../probability-theory.md#gaussian-random-variable) $(Z_j)$ on a common [probability space](../../../probability-theory.md#probability-space). In finite dimension the sums below are finite; in dimension zero take $X(0)=0$. In infinite dimension define

$$
S_N(h)=\sum_{j=1}^N\langle h,e_j\rangle Z_j.
$$

Independence, centring and unit variance give

$$
\mathbb E|S_N(h)-S_M(h)|^2=\sum_{j=M+1}^N\langle h,e_j\rangle^2\longrightarrow0.
$$

By the [Parseval identity for a Hilbertian basis](../../../hilbert-space.md#parseval-identity-for-a-hilbertian-basis), the coefficient sequence is square-summable. Completeness of $L^2(\Omega)$ therefore supplies a limit, and we define

$$
\boxed{X(h)=\lim_{N\to\infty}S_N(h)\quad\text{in }L^2(\Omega).}
$$

Every partial-sum map is linear, and passage to the $L^2$ limit preserves this identity. Thus for each fixed $a,b,g,h$, $X(ag+bh)=aX(g)+bX(h)$ as an $L^2$ identity, hence an [almost sure equality](../../../convergence-of-random-variables.md#almost-sure-equality). This constructs an [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process).

The usual meaning is almost-sure linearity for each fixed choice of arguments. A version linear simultaneously for every argument can also be chosen: select a [Hamel basis](../../../vector-space.md#basis) of $H$, choose a measurable representative of $X$ on each basis vector, and extend each sample algebraically by finite sums. For every fixed $h$, this extension equals the constructed $L^2$ variable almost surely, so all its required distributions are unchanged.

<h4 id="1/a/2">2</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/2/solution">Solution</h5>

↑ **Parent:** [2](#1/a/2)

For the construction above, independence of the [normal random variables](../../../probability-theory.md#gaussian-random-variable) makes $S_N(h)$ normal with mean zero and variance $v_N=\sum_{j\le N}\langle h,e_j\rangle^2$. Its [characteristic function](../../../probability-theory.md#characteristic-function) is $\exp(-\theta^2v_N/2)$. The $L^2$ convergence gives $L^1$ convergence, and

$$
\left|\mathbb E e^{i\theta S_N(h)}-\mathbb E e^{i\theta X(h)}\right|\le |\theta|\,\mathbb E|S_N(h)-X(h)|\longrightarrow0.
$$

Since $v_N\to\|h\|^2$ by the [Parseval identity for a Hilbertian basis](../../../hilbert-space.md#parseval-identity-for-a-hilbertian-basis), the limiting [characteristic function](../../../probability-theory.md#characteristic-function) identifies

$$
\boxed{X(h)\sim N(0,\|h\|^2).}
$$

This includes $h=0$, where the [normal distribution](../../../probability-theory.md#normal-distribution) is degenerate at zero.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For any $r_1,\ldots,r_n\in\mathbb R$, the linearity from part (a) gives

$$
\sum_{j=1}^n r_jX(h_j)=X\left(\sum_{j=1}^n r_jh_j\right)
$$

almost surely, and the right side has a [normal distribution](../../../probability-theory.md#normal-distribution). This is the defining linear-combination criterion for a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution); singular [covariance matrices](../../../variance.md#covariance-matrix) are allowed.

Passing to the limit in the inner products of the partial sums gives

$$
\boxed{\operatorname{Cov}(X(g),X(h))=\mathbb E[X(g)X(h)]=\sum_j\langle g,e_j\rangle\langle h,e_j\rangle=\langle g,h\rangle.}
$$

The passage to the limit is justified by [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and $L^2$ convergence. Equivalently, the vector's [characteristic function](../../../probability-theory.md#characteristic-function) is

$$
\mathbb E\exp\left(i\sum_jr_jX(h_j)\right)=\exp\left(-\frac12\sum_{j,k}r_jr_k\langle h_j,h_k\rangle\right).
$$

Thus both joint normality and the complete [covariance matrix](../../../variance.md#covariance-matrix) follow from the Hilbert-space inner product.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/1">1</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/1/solution">Solution</h5>

↑ **Parent:** [1](#1/c/1)

Apply the construction of part (a) to the real [Hilbert space](../../../hilbert-space.md) $H=L^2([0,\infty),du)$, and set

$$
\boxed{W_t=X(\mathbf1_{[0,t]})\quad(t\ge0).}
$$

Choose $X(0)=0$. The interval of length zero represents the zero vector of $H$, so **$W_0=0$**. All variables are defined on the single [probability space](../../../probability-theory.md#probability-space) already used for the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process).

<h4 id="1/c/2">2</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/2/solution">Solution</h5>

↑ **Parent:** [2](#1/c/2)

For $0\le s<t$, linearity of the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process) gives

$$
W_t-W_s=X(\mathbf1_{(s,t]})\quad\text{almost surely}.
$$

The squared $L^2$ norm of this indicator is $t-s$, so part (a) yields

$$
\boxed{W_t-W_s\sim N(0,t-s).}
$$

Also, the [covariance](../../../variance.md#covariance) formula gives $\operatorname{Cov}(W_s,W_t)=s\wedge t$, the [Brownian covariance kernel](../../../random-variable.md#brownian-covariance-kernel). The Gaussian statement concerns the signed increment.

<h4 id="1/c/3">3</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/3/solution">Solution</h5>

↑ **Parent:** [3](#1/c/3)

Let $\Delta_j=W_{t_j}-W_{t_{j-1}}$ for $1\le j\le n$. These increments are jointly normal, because each is obtained by evaluating the [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process) on an interval indicator. Indicators of distinct intervals are orthogonal in $L^2([0,\infty))$, so

$$
\operatorname{Cov}(\Delta_j,\Delta_k)=0\qquad(j\ne k).
$$

By [uncorrelated jointly Gaussian variables are independent](../../../probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent), **the increments on all these disjoint intervals are independent**. Reversing the sign of the first increment, as in the printed list, preserves this independence.

The three requested properties have now been obtained without an existence theorem for [Brownian motion](../../../brownian-motion.md). One can also obtain continuous paths: the [Gaussian fourth moment](../../../probability-theory.md#gaussian-fourth-moment) gives $\mathbb E|W_t-W_s|^4=3|t-s|^2$. The [Kolmogorov continuity theorem](../../../stochastic-process.md#kolmogorov-continuity-theorem) therefore supplies a continuous modification on every finite time interval, which can be chosen consistently on the half-line. Modification preserves every finite-dimensional distribution and hence the independent Gaussian increments. This yields [Brownian motion](../../../brownian-motion.md) itself.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The density $Z=\exp(X(k)-\|k\|^2/2)$ is strictly positive. The [Gaussian moment-generating function](../../../probability-theory.md#moment-generating-function-of-a-normal-distribution) gives $\mathbb E Z=1$, so it defines an [equivalent probability measure](../../../measure-theory.md#equivalent-probability-measure).

The joint [normal distribution](../../../probability-theory.md#normal-distribution) of $(X(h),X(k))$, with [covariance](../../../variance.md#covariance) $\langle h,k\rangle$, gives the mixed exponential formula

$$
\mathbb E_{\mathbb P}e^{X(k)+i\theta X(h)}=\exp\left(\frac12\|k\|^2+i\theta\langle h,k\rangle-\frac12\theta^2\|h\|^2\right).
$$

Multiplying by the normalizing and centring factors therefore yields

$$
\mathbb E_{\mathbb Q}e^{i\theta(X(h)-\langle h,k\rangle)}=\exp\left(-\frac12\theta^2\|h\|^2\right).
$$

The [characteristic function](../../../probability-theory.md#characteristic-function) identifies the answer:

$$
\boxed{X(h)-\langle h,k\rangle\sim N(0,\|h\|^2)\quad\text{under }\mathbb Q.}
$$

This is [exponential tilting of an isonormal Gaussian process](../../../stochastic-process.md#exponential-tilting-of-an-isonormal-gaussian-process): the mean shifts by the inner product while its [covariance](../../../variance.md#covariance) remains unchanged.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

If $T\le s$, then $\phi(W_T)K$ is $\mathcal F_s$-measurable. Independence and centring of the future [Brownian increment](../../../brownian-motion.md#brownian-increment) make the desired left side zero; the time multiplier on the right is zero as well.

Suppose $T>s$. Conditional on $\mathcal F_s$, write $W_T=W_s+U$ and $W_t-W_s=V$. The pair $(U,V)$ is jointly normal and independent of $\mathcal F_s$, with

$$
\mathbb E V=0,\qquad\operatorname{Cov}(U,V)=\min(T-s,t-s)=T\wedge t-T\wedge s.
$$

Apply the supplied [Gaussian integration by parts](../../../probability-theory.md#stein-s-lemma-probability) formula to $z\mapsto\phi(W_s+z)$, treating the known $W_s$ as its parameter. This gives

$$
\mathbb E[\phi(W_T)(W_t-W_s)\mid\mathcal F_s]=(T\wedge t-T\wedge s)\mathbb E[\phi'(W_T)\mid\mathcal F_s].
$$

Multiply by the bounded $\mathcal F_s$-measurable $K$ and use the defining property of [conditional expectation](../../../measure-theory.md#conditional-expectation). Thus **the required expectation identity holds for every $s<t$, including intervals crossing or lying after $T$**.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

First take a bounded elementary [predictable process](../../../martingale.md#predictable-process) $\alpha=\sum_jK_j\mathbf1_{(s_j,t_j]}$, with each $K_j$ bounded and $\mathcal F_{s_j}$-measurable and with finite time support. The [Itô integral](../../../stochastic-calculus.md#ito-integral) is the corresponding finite sum $\sum_jK_j(W_{t_j}-W_{s_j})$. Applying part (a) term by term gives

$$
\mathbb E\left[\phi(W_T)\int_0^\infty\alpha_u\,dW_u\right]=\mathbb E\int_0^T\phi'(W_T)\alpha_u\,du.
$$

Such elementary [predictable processes](../../../martingale.md#predictable-process) are dense among predictable processes in $L^2(d\mathbb P\,du)$. The [Itô isometry](../../../stochastic-calculus.md#ito-isometry) makes the left functional continuous, with bound

$$
\left|\mathbb E\left[\phi(W_T)\int\alpha\,dW\right]\right|\le\|\phi\|_\infty\left(\mathbb E\int_0^\infty\alpha_u^2\,du\right)^{1/2}.
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) makes the right functional continuous, with bound $\|\phi'\|_\infty\sqrt T\left(\mathbb E\int\alpha_u^2du\right)^{1/2}$. Approximation therefore proves **the same identity for every allowed predictable $\alpha$**. The integral over the infinite time interval is the $L^2$ limit of its finite-horizon [Itô integrals](../../../stochastic-calculus.md#ito-integral).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The terminal variable $F=\phi(W_T)$ is bounded and hence [square-integrable](../../../measure-theory.md#square-integrable-function). In the completed natural [Brownian filtration](../../../brownian-motion.md#brownian-filtration), the [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) says that any square-integrable $\mathcal F_T$-measurable variable admits a representation

$$
F=\mathbb E F+\int_0^T\beta_u\,dW_u
$$

with $\beta$ predictable and $\mathbb E\int_0^T\beta_u^2du<\infty$. Extend $\beta$ by zero after $T$. Thus the requested constant and integrability are

$$
\boxed{c=\mathbb E\phi(W_T),\qquad\mathbb E\int_0^\infty\beta_u^2du=\operatorname{Var}(\phi(W_T)).}
$$

Expectation determines $c$ uniquely. If two integrands give the same representation, the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives $\mathbb E\int_0^\infty(\beta_u-\widetilde\beta_u)^2du=0$. Consequently **$\beta$ is unique up to $d\mathbb P\,du$-almost everywhere equality**, rather than pointwise equality at every time. The corresponding integral martingales are indistinguishable.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Multiply the representation in part (c) by $\int_0^\infty\alpha_u\,dW_u$ and take expectations. This [Itô integral](../../../stochastic-calculus.md#ito-integral) has mean zero, and the bilinear form of the [Itô isometry](../../../stochastic-calculus.md#ito-isometry) gives

$$
\mathbb E\left[\phi(W_T)\int_0^\infty\alpha_u\,dW_u\right]=\mathbb E\int_0^\infty\beta_u\alpha_u\,du.
$$

Equating this with part (b), and writing both ordinary integrals with the same time variable, yields

$$
\boxed{\mathbb E\int_0^\infty\left(\beta_u-\phi'(W_T)\mathbf1_{\{u\le T\}}\right)\alpha_u\,du=0.}
$$

All terms are integrable by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), the assumed square integrability of $\alpha$, and boundedness of $\phi'$. This is an orthogonality statement against [predictable processes](../../../martingale.md#predictable-process); its second term need not itself be predictable.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Set $Z_t=\mathbb E[\phi'(W_T)\mid\mathcal F_t]$. The [Brownian martingale representation theorem](../../../brownian-motion.md#brownian-martingale-representation-theorem) applied to the bounded terminal variable $\phi'(W_T)$ supplies a continuous adapted version of $Z$, so it is [predictable](../../../martingale.md#predictable-process). Hence

$$
\gamma_t=Z_t\mathbf1_{\{t\le T\}}
$$

is predictable and satisfies $\mathbb E\int\gamma_t^2dt\le T\|\phi'\|_\infty^2$. For every square-integrable [predictable process](../../../martingale.md#predictable-process) $\alpha$, conditioning at each deterministic time and using [Fubini theorem](../../../measure-theory.md#fubini-s-theorem) gives

$$
\mathbb E\int_0^T\phi'(W_T)\alpha_t\,dt=\mathbb E\int_0^T Z_t\alpha_t\,dt.
$$

Thus part (d) says $\mathbb E\int(\beta_t-\gamma_t)\alpha_tdt=0$. Taking $\alpha=\beta-\gamma$, which is an allowed predictable square-integrable process, makes its squared norm zero. We conclude

$$
\boxed{\beta_t=\mathbb E[\phi'(W_T)\mid\mathcal F_t]\mathbf1_{\{t\le T\}}\quad d\mathbb P\,dt\text{-almost everywhere}.}
$$

This is the [Clark-Ocone formula for a smooth Brownian terminal payoff](../../../brownian-motion.md#clark-ocone-formula-for-a-smooth-brownian-terminal-payoff), with exactly the uniqueness established in part (c).

<h2 id="3">3</h2>

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $t_j=j2^{-n}$ and $\Delta_j=X_{t_{j+1}}-X_{t_j}$. Telescoping $X_{t_{j+1}}^2-X_{t_j}^2=2X_{t_j}\Delta_j+\Delta_j^2$ gives

$$
M_1^{(n)}=\sum_{j=0}^{2^n-1}X_{t_j}\Delta_j.
$$

The [martingale transform](../../../martingale.md#martingale-transform) summands are orthogonal in $L^2$: for an earlier summand, conditioning on the sigma-algebra at the start of the later increment makes the cross expectation zero. Hence

$$
\mathbb E(M_1^{(n)})^2=\sum_j\mathbb E[X_{t_j}^2\Delta_j^2]\le C^2\sum_j\mathbb E\Delta_j^2.
$$

The [martingale](../../../martingale.md) increments themselves are also orthogonal. Since $X_0=0$, their variance sum equals $\mathbb E X_1^2\le C^2$. Therefore

$$
\boxed{\mathbb E(M_1^{(n)})^2\le C^4.}
$$

Only discrete martingale orthogonality is used here; no pre-existing [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) calculation is needed.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The defining relation gives $A_1^{(n)}=X_1^2-2M_1^{(n)}$. Applying $(r-s)^2\le2r^2+2s^2$ and the bound from part (a),

$$
\mathbb E(A_1^{(n)})^2\le2\mathbb E X_1^4+8\mathbb E(M_1^{(n)})^2\le2C^4+8C^4.
$$

Thus

$$
\boxed{\mathbb E(A_1^{(n)})^2\le10C^4,}
$$

uniformly in the dyadic mesh. This controls the approximations to [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) without assuming that their limits already exist.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For $n>m$, define $r_j=\lfloor j2^{m-n}\rfloor2^{-m}$ and $h_j=X_{j2^{-n}}-X_{r_j}$. Each $h_j$ is measurable at time $j2^{-n}$, so the summands in the given difference formula are orthogonal [martingale transforms](../../../martingale.md#martingale-transform). Therefore

$$
\mathbb E|M_1^{(n)}-M_1^{(m)}|^2=\mathbb E\sum_{j=1}^{2^n-1}h_j^2\left(X_{(j+1)2^{-n}}-X_{j2^{-n}}\right)^2.
$$

Let

$$
\omega_m=\sup\{|X_t-X_s|:s,t\in[0,1],\ |t-s|\le2^{-m}\}.
$$

Path continuity on the compact interval gives $\omega_m\to0$ almost surely, and $\omega_m\le2C$. Since $0\le j2^{-n}-r_j<2^{-m}$, $|h_j|\le\omega_m$. Thus, by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and part (b),

$$
\mathbb E|M_1^{(n)}-M_1^{(m)}|^2\le\mathbb E[\omega_m^2A_1^{(n)}]\le\sqrt{10}\,C^2(\mathbb E\omega_m^4)^{1/2}\longrightarrow0.
$$

The last step is the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem). The bound is uniform in $n>m$, and the other ordering follows by symmetry. Hence **the terminal martingale transforms are Cauchy in $L^2$**.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For every $t$, subtraction of the definitions gives

$$
A_t^{(n)}-A_t^{(m)}=-2(M_t^{(n)}-M_t^{(m)}).
$$

The difference of the two supplied [continuous martingales](../../../martingale.md#continuous-martingale) is a square-integrable martingale on $[0,1]$; for each fixed mesh its finite sums are bounded. For this [dyadic quadratic variation of a bounded continuous martingale](../../../stochastic-calculus.md#dyadic-quadratic-variation-of-a-bounded-continuous-martingale), the [Doob L2 maximal inequality](../../../martingale.md#doob-l2-maximal-inequality) therefore gives

$$
\mathbb E\sup_{0\le t\le1}|A_t^{(n)}-A_t^{(m)}|^2\le16\mathbb E|M_1^{(n)}-M_1^{(m)}|^2\longrightarrow0.
$$

Thus **the dyadic approximations to quadratic variation are Cauchy for the expected squared uniform norm**, as required. No monotonicity in time of the partially completed squared-increment sums is needed.

## 4

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The drift $b(z)=\tanh z$ has derivative $b'(z)=1/\cosh^2z$, so $|b'(z)|\le1$. Hence it is globally Lipschitz. The diffusion coefficient $\sigma(z)=1$ is globally Lipschitz as well, and both coefficients satisfy a linear growth bound.

The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../stochastic-calculus.md#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients) states that globally Lipschitz coefficients with linear growth give, for each deterministic initial point, an adapted continuous [strong solution of a stochastic differential equation](../../../stochastic-calculus.md#strong-solution-of-a-stochastic-differential-equation) on every finite interval, with pathwise uniqueness and no finite-time explosion. Applying this theorem gives **a unique strong solution for every $X_0=x\in\mathbb R$**, satisfying

$$
X_t=x+\int_0^t\tanh X_s\,ds+W_t.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $f(z)=1/\cosh z$. Differentiating gives

$$
f'(z)=-f(z)\tanh z,\qquad f''(z)=f(z)(2\tanh^2z-1).
$$

Therefore the diffusion operator satisfies $\frac12f''+\tanh z\,f'=-\frac12f$. Applying the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) to $Y_t=e^{t/2}f(X_t)$ cancels its drift:

$$
dY_t=-Y_t\tanh X_t\,dW_t.
$$

So $Y$ is a positive [local martingale](../../../martingale.md#local-martingale). On every finite interval $[0,R]$, $0<Y_t\le e^{R/2}$. The [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion) makes it a true martingale on that interval. Since $R$ is arbitrary,

$$
\boxed{Y_t=\frac{e^{t/2}}{\cosh X_t}\text{ is a positive martingale},\qquad\mathbb EY_t=\frac1{\cosh x}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For $0\le t\le T$, set $Z_t=\cosh x\,Y_t$. Part (b) gives $Z_0=1$, $\mathbb EZ_T=1$, and $Z_t>0$. Its stochastic differential is

$$
dZ_t=Z_t\eta_t\,dW_t,\qquad\eta_t=-\tanh X_t.
$$

Thus $Z$ is the [stochastic exponential](../../../stochastic-calculus.md#doleans-dade-exponential) of $\int\eta\,dW$. The [Novikov condition](../../../stochastic-calculus.md#novikov-s-condition) also holds, since $\exp(\frac12\int_0^T\eta_t^2dt)\le e^{T/2}$.

The [Girsanov theorem](../../../stochastic-calculus.md#girsanov-theorem) says that under the measure with [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) $Z_T$, the process $W_t-\int_0^t\eta_sds$ is a [Brownian motion](../../../brownian-motion.md) up to $T$. Substituting the sign of $\eta$ and the original [stochastic differential equation](../../../stochastic-calculus.md#stochastic-differential-equation) gives

$$
\boxed{W_t^{\mathbb Q}=W_t+\int_0^t\tanh X_s\,ds=X_t-x.}
$$

The density is strictly positive, so $\mathbb Q$ and $\mathbb P$ are [equivalent probability measures](../../../measure-theory.md#equivalent-probability-measure).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Under $\mathbb Q$, $X_T=x+W_T^{\mathbb Q}$ has density $\varphi_T(z-x)=(2\pi T)^{-1/2}\exp(-(z-x)^2/(2T))$. The reciprocal [Radon-Nikodym derivative](../../../measure-theory.md#radon-nikodym-derivative) depends only on $X_T$:

$$
\frac{d\mathbb P}{d\mathbb Q}=\frac{\cosh X_T}{\cosh x}e^{-T/2}.
$$

Consequently the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) under the original measure is

$$
\boxed{p_T(x,z)=\frac{\cosh z}{\cosh x}\frac{e^{-T/2}}{\sqrt{2\pi T}}\exp\left(-\frac{(z-x)^2}{2T}\right),\qquad z\in\mathbb R.}
$$

It integrates to one because $\mathbb E_{\mathbb Q}\cosh X_T=e^{T/2}\cosh x$. Completing the square also gives the useful [mixture distribution](../../../probability-theory.md#mixture-distribution) form

$$
p_T(x,z)=\frac{e^x}{2\cosh x}\varphi_T(z-x-T)+\frac{e^{-x}}{2\cosh x}\varphi_T(z-x+T).
$$

Thus the terminal law is a mixture of $N(x+T,T)$ and $N(x-T,T)$ with the displayed positive weights. The [diffusion with hyperbolic tangent drift](../../../stochastic-calculus.md#diffusion-with-hyperbolic-tangent-drift) density also exhibits the [Doob h-transform](../../../markov-process.md#doob-h-transform) with $h(z)=\cosh z$.

## 5

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a deterministic $t\le T$, conditional symmetry makes the [conditional characteristic function](../../../probability-theory.md#conditional-characteristic-function) of $X_T-X_t$ invariant under $\theta\mapsto-\theta$. The bounded real and imaginary parts of the exponential are legitimate test functions. Hence

$$
e^{-2i\theta X_t}M_t=e^{-i\theta X_t}\mathbb E[e^{i\theta(X_T-X_t)}\mid\mathcal F_t]=e^{-i\theta X_t}\mathbb E[e^{-i\theta(X_T-X_t)}\mid\mathcal F_t]=\mathbb E[e^{-i\theta X_T}\mid\mathcal F_t].
$$

The right side is a bounded complex martingale. Both sides have continuous versions by the assumptions; equality on rational times and continuity make them indistinguishable. Thus **$e^{-2i\theta X_t}M_t$ is a martingale** on $[0,T]$. Complex martingale assertions mean the corresponding assertions for both real and imaginary parts.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $A=\langle X\rangle$ be the [quadratic variation](../../../stochastic-calculus.md#quadratic-variation). We use bilinear [quadratic covariation](../../../stochastic-calculus.md#quadratic-covariation) for the complex martingale: $\langle M,X\rangle=\langle\operatorname{Re}M,X\rangle+i\langle\operatorname{Im}M,X\rangle$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
d(e^{-2i\theta X_t})=-2i\theta e^{-2i\theta X_t}\,dX_t-2\theta^2e^{-2i\theta X_t}\,dA_t.
$$

By the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule), the finite-variation part of $d(e^{-2i\theta X}M)$ is

$$
e^{-2i\theta X_t}\left(-2\theta^2 M_t\,dA_t-2i\theta\,d\langle M,X\rangle_t\right).
$$

Part (a) says the product is a martingale, so uniqueness of the continuous semimartingale decomposition makes this finite-variation part zero. For $\theta\ne0$, division gives

$$
\boxed{d\langle M,X\rangle_t=i\theta M_t\,d\langle X\rangle_t.}
$$

For $\theta=0$, $M\equiv1$ and both sides are zero, so the identity holds without exception.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Put $F_t=\exp(-i\theta X_t-\frac12\theta^2A_t)$. The [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives

$$
dF_t=-i\theta F_t\,dX_t-\theta^2F_t\,dA_t.
$$

The explicit decreasing exponential contributes half the finite-variation term; the other half is the quadratic correction from $e^{-i\theta X_t}$. Now the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) and part (b) yield

$$
d(F_tM_t)=F_t\,dM_t-i\theta F_tM_t\,dX_t-\theta^2F_tM_t\,dA_t-i\theta F_t\,d\langle M,X\rangle_t=F_t\,dM_t-i\theta F_tM_t\,dX_t.
$$

The finite-variation terms cancel because $-i\theta(i\theta)=\theta^2$. This proves the product is a [local martingale](../../../martingale.md#local-martingale). Moreover $|F_t|=e^{-\theta^2A_t/2}\le1$ and $|M_t|\le1$. The [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion) therefore proves **the product is a true martingale**.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

At the terminal time, $M_T=e^{i\theta X_T}$, so the martingale from part (c) has terminal value $e^{-\theta^2\langle X\rangle_T/2}$. Its initial value is $M_0$, since $X_0=\langle X\rangle_0=0$. Taking expectations gives

$$
\boxed{\mathbb E e^{i\theta X_T}=\mathbb E e^{-\theta^2\langle X\rangle_T/2}.}
$$

Here $M_0$ may be a nonconstant $\mathcal F_0$-measurable variable; the [tower property of conditional expectation](../../../measure-theory.md#law-of-total-expectation) still gives $\mathbb EM_0=\mathbb E e^{i\theta X_T}$. This [characteristic function under conditionally symmetric martingale increments](../../../martingale.md#characteristic-function-under-conditionally-symmetric-martingale-increments) identity relates the [characteristic function](../../../probability-theory.md#characteristic-function) of the terminal martingale to the [Laplace transform of a nonnegative random variable](../../../probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) given by its [quadratic variation](../../../stochastic-calculus.md#quadratic-variation).

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Fix $T>0$. The given [normal distribution](../../../probability-theory.md#normal-distribution) and part (d) imply

$$
\mathbb E e^{-\lambda\langle X\rangle_T}=e^{-\lambda T}\qquad(\lambda\ge0).
$$

One can deduce determinism without any moment assumption on the bracket. Put $Z=e^{-\langle X\rangle_T}$. Taking $\lambda=1,2$ gives $\mathbb EZ=e^{-T}$ and $\mathbb EZ^2=e^{-2T}$, so $\operatorname{Var}(Z)=0$. Therefore $\langle X\rangle_T=T$ almost surely. Applying this at every rational time and using continuity of [quadratic variation](../../../stochastic-calculus.md#quadratic-variation) gives $\langle X\rangle_t=t$ simultaneously for all $t\ge0$ outside a single null set.

The [Lévy characterization of Brownian motion](../../../brownian-motion.md#levy-characterization-of-brownian-motion) states that a continuous local martingale starting at zero with this bracket is [Brownian motion](../../../brownian-motion.md) in its filtration. To see the independent-increment conclusion directly, the [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) shows that $e^{i\theta X_t+\theta^2t/2}$ is a martingale on any fixed bounded time interval: it is a local martingale with a deterministic bound on its modulus. Thus

$$
\mathbb E[e^{i\theta(X_t-X_s)}\mid\mathcal F_s]=e^{-\theta^2(t-s)/2}.
$$

The deterministic [conditional characteristic function](../../../probability-theory.md#conditional-characteristic-function) identifies an $N(0,t-s)$ increment independent of $\mathcal F_s$. Together with the given path continuity and $X_0=0$, this proves **$X$ is Brownian motion**.

## 6

↑ **Parent:** [Paper 25](paper-25.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let $a(x)=\sigma(x)\sigma(x)^{\mathsf T}$. The multidimensional [Itô formula](../../../stochastic-calculus.md#ito-s-lemma) gives the second-order [diffusion generator](../../../stochastic-process.md#diffusion-generator)

$$
\boxed{\mathcal L f(x)=\sum_{i=1}^d b_i(x)\partial_i f(x)+\frac12\sum_{i,j=1}^d a_{ij}(x)\partial_i\partial_jf(x).}
$$

Indeed,

$$
f(X_t)-\int_0^t(\mathcal Lf)(X_s)\,ds=f(X_0)+\int_0^t\nabla f(X_s)^{\mathsf T}\sigma(X_s)\,dW_s.
$$

The integrand is locally bounded along the continuous path after stopping on compact sets, because the coefficients and derivatives are continuous. Thus the final [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) is a [local martingale](../../../martingale.md#local-martingale). No global growth or uniqueness assumption on this already-given [weak solution of a stochastic differential equation](../../../stochastic-calculus.md#weak-solution-of-a-stochastic-differential-equation) is needed.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Apply the [Itô product rule](../../../stochastic-calculus.md#ito-product-rule) to the deterministic discount factor and $u(X_t)$:

$$
d(e^{-\lambda t}u(X_t))=e^{-\lambda t}(\mathcal Lu-\lambda u)(X_t)\,dt+e^{-\lambda t}\nabla u(X_t)^{\mathsf T}\sigma(X_t)\,dW_t.
$$

The prescribed differential equation makes the drift vanish. Therefore

$$
\boxed{M_t=e^{-\lambda t}u(X_t)\text{ is a local martingale}.}
$$

This is the discounted generator-eigenfunction martingale underlying the [Feynman-Kac formula](../../../stochastic-calculus.md#feynman-kac-formula).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Continuity and adaptedness make the first boundary hit a [stopping time](../../../martingale.md#stopping-time). A continuous path starting in the open domain cannot leave it before meeting its boundary. Thus $X_{t\wedge T}\in\mathcal D\cup\partial\mathcal D$, with the usual interpretation when $T=\infty$. If $|u|\le K$ on this set, then

$$
|M_{t\wedge T}|=e^{-\lambda(t\wedge T)}|u(X_{t\wedge T})|\le K.
$$

The stopped process is a bounded [local martingale](../../../martingale.md#local-martingale); the [bounded local martingale criterion](../../../martingale.md#bounded-local-martingale-criterion) makes it a martingale and, in fact, a [uniformly integrable martingale](../../../martingale.md#uniformly-integrable-martingale). The [martingale convergence theorem](../../../martingale.md#martingale-convergence-theorem) gives **almost sure and $L^1$ convergence** as $t\to\infty$.

Its limit can also be identified pathwise. On $\{T<\infty\}$ the stopped process is eventually constant at $e^{-\lambda T}u(X_T)$. On $\{T=\infty\}$ its absolute value is at most $Ke^{-\lambda t}$ and hence tends to zero. Thus the limit is $e^{-\lambda T}u(X_T)\mathbf1_{\{T<\infty\}}$.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

On the event $T<\infty$, continuity puts $X_T$ on the boundary, where $u=1$. The limit found in part (c) is therefore $e^{-\lambda T}$, defining this expression to be zero when $T=\infty$. Taking expectations and using the bounded convergence justified in part (c) gives

$$
\boxed{\mathbb E e^{-\lambda T}=\mathbb E M_\infty=\mathbb E M_0=u(X_0).}
$$

The conclusion does not require almost-sure finiteness of $T$. It is the [discounted boundary-hitting representation](../../../stochastic-calculus.md#discounted-boundary-hitting-representation) for a bounded solution of $\mathcal Lu=\lambda u$.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

For the drifted [Brownian motion](../../../brownian-motion.md) $Y_t=y+B_t+at$ on $(0,\infty)$, the [diffusion generator](../../../stochastic-process.md#diffusion-generator) is $\mathcal L=\frac12\frac{d^2}{dz^2}+a\frac{d}{dz}$. Seek a bounded solution of $\mathcal Lu=\lambda u$ with $u(0)=1$. The exponential ansatz $u(z)=e^{rz}$ gives

$$
\frac12r^2+ar=\lambda,\qquad r=-a\pm\sqrt{a^2+2\lambda}.
$$

Because $\lambda>0$, the plus root is positive and the minus root is negative. Boundedness on $[0,\infty)$ therefore selects

$$
u(z)=\exp\left(-z\left(a+\sqrt{a^2+2\lambda}\right)\right).
$$

It satisfies the boundary condition and all hypotheses of part (d). Hence

$$
\boxed{\mathbb E e^{-\lambda S}=\exp\left(-y\left(a+\sqrt{a^2+2\lambda}\right)\right).}
$$

This is the [first-passage Laplace transform for Brownian motion with drift](../../../markov-process.md#first-passage-laplace-transform-for-brownian-motion-with-drift), with $e^{-\lambda\infty}=0$. At $a=0$ it reduces to $e^{-y\sqrt{2\lambda}}$. As $\lambda\downarrow0$, it gives $\mathbb P(S<\infty)=e^{-2y\max(a,0)}$, agreeing with certainty of hitting when the drift points towards zero and a possible escape when it points away.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
