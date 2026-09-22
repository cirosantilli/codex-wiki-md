# Paper 205

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_205.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_205.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
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
- [2](#2)
  - [Solution](#2/solution)
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
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [Solution](#6/solution)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)

## 1

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) on a nonempty set $\mathcal X$ is a symmetric function $k:\mathcal X\times\mathcal X\to\mathbb R$ such that, for every $n\geq1$, every $x_1,\ldots,x_n\in\mathcal X$, and every $c_1,\ldots,c_n\in\mathbb R$,

$$
\sum_{r,s=1}^n c_rc_s k(x_r,x_s)\geq0.
$$

Equivalently, every finite [kernel matrix](../../../probability-and-statistics.md#kernel-matrix) $(k(x_r,x_s))_{r,s}$ is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix).

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [Gaussian kernel](../../../probability-and-statistics.md#gaussian-kernel) with bandwidth $\sigma^2>0$ is

$$
\boxed{k_\sigma(x,y)=\exp\!\left(-\frac{\|x-y\|_2^2}{2\sigma^2}\right).}
$$

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Every $2\times2$ principal [submatrix](../../../vector-space.md#submatrix) of a [kernel matrix](../../../probability-and-statistics.md#kernel-matrix) is positive semidefinite, so

$$
|k_\tau(x,y)|^2\leq k_\tau(x,x)k_\tau(y,y).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) for integrals therefore gives

$$
\int_{-\infty}^{\infty}|k_\tau(x,y)|\,d\tau
\leq
\left(\int_{-\infty}^{\infty}k_\tau(x,x)\,d\tau\right)^{1/2}
\left(\int_{-\infty}^{\infty}k_\tau(y,y)\,d\tau\right)^{1/2}<\infty.
$$

Thus every entry of $k(x,y)=\int k_\tau(x,y)d\tau$ is well defined. For any finite coefficients $c_r$ and points $x_r$, linearity of the integral gives

$$
\sum_{r,s}c_rc_s k(x_r,x_s)
=\int_{-\infty}^{\infty}\sum_{r,s}c_rc_s k_\tau(x_r,x_s)\,d\tau\geq0,
$$

because the integrand is nonnegative. Hence $k$ is a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel). This proves the [integral closure of positive-semidefinite kernels](../../../probability-and-statistics.md#integral-closure-of-positive-semidefinite-kernels).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The [Gamma integral](../../../complex-analysis.md#gamma-integral) $u^{-1/2}=\pi^{-1/2}\int_0^\infty t^{-1/2}e^{-ut}dt$ gives

$$
\frac1{\sqrt{\alpha+\|x-y\|_2^2}}
=\frac1{\sqrt\pi}\int_0^\infty
 t^{-1/2}e^{-\alpha t}e^{-t\|x-y\|_2^2}\,dt.
$$

For each $t>0$, the last factor is a [Gaussian kernel](../../../probability-and-statistics.md#gaussian-kernel), and the remaining weight is nonnegative. The diagonal integral equals $\alpha^{-1/2}<\infty$, so part ii shows that the displayed function is a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For points $x_1,\ldots,x_n$ and coefficients $c_1,\ldots,c_n$,

$$
\sum_{r,s=1}^n c_rc_s k(x_r,x_s)
=\mathbb E\!\left[\left(\sum_{r=1}^n c_r\widehat\phi(x_r)\right)^2\right]\geq0.
$$

The bound $|\widehat\phi|\leq M$ ensures that this [expected value](../../../probability-theory.md#expected-value) is finite. Symmetry is immediate, so an expected outer product of a [random feature map](../../../probability-and-statistics.md#random-feature-map) always defines a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Let $V_1,\ldots,V_d$ be independent standard [Cauchy random variables](../../../probability-theory.md#cauchy-random-variable). Their [characteristic functions](../../../probability-theory.md#characteristic-function) and independence give

$$
\mathbb E e^{i\lambda V^T(x-y)}
=\prod_{j=1}^d e^{-\lambda|x_j-y_j|}
=e^{-\lambda\|x-y\|_1}.
$$

Taking real parts yields

$$
e^{-\lambda\|x-y\|_1}
=\mathbb E\!\left[
\cos(\lambda V^Tx)\cos(\lambda V^Ty)
+\sin(\lambda V^Tx)\sin(\lambda V^Ty)
\right].
$$

For each realization of $V$, both products are rank-one [positive-semidefinite kernels](../../../probability-and-statistics.md#positive-semidefinite-kernel). Their sum and then their expectation remain positive semidefinite by the [closure property of positive-semidefinite kernels](../../../probability-and-statistics.md#closure-property-of-positive-semidefinite-kernels). This is a [Random Fourier feature](../../../probability-and-statistics.md#random-fourier-features) representation of the [Laplace kernel](../../../probability-and-statistics.md#laplace-kernel).

## 2

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [familywise error rate](../../../statistical-modelling.md#familywise-error-rate) is

$$
\operatorname{FWER}=\mathbb P(\text{at least one true null hypothesis is rejected}).
$$

The [Bonferroni correction](../../../statistical-modelling.md#bonferroni-correction) rejects $H_i$ when $p_i\leq\alpha/m$. Since a valid [p-value](../../../statistical-modelling.md#p-value) is [super-uniform](../../../statistical-modelling.md#super-uniform-random-variable) under its null, the [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\operatorname{FWER}
\leq\sum_{i\in I_0}\mathbb P(p_i\leq\alpha/m)
\leq |I_0|\frac\alpha m\leq\alpha.
$$

**No independence assumption is needed.**

For the [closed testing procedure](../../../statistical-modelling.md#closed-testing-procedure), form the intersection hypothesis $H_I=\bigcap_{i\in I}H_i$ for every nonempty $I\subseteq\{1,\ldots,m\}$ and choose a level-$\alpha$ local test for each $H_I$. Reject $H_i$ exactly when every $H_I$ with $i\in I$ is rejected by its local test. If any true $H_i$ is rejected, then the intersection $H_{I_0}$ of all true nulls is rejected. Since its local test has [significance level](../../../statistical-modelling.md#significance-level) $\alpha$,

$$
\operatorname{FWER}\leq\mathbb P(H_{I_0}\text{ is rejected})\leq\alpha.
$$

This is the [closed-testing control of the familywise error rate](../../../statistical-modelling.md#closed-testing-control-of-the-familywise-error-rate).

Write $W=\sum_{j=1}^m w_j$. Procedure (A) is the [Weighted Bonferroni correction](../../../statistical-modelling.md#weighted-bonferroni-correction): it rejects $H_i$ when $p_i\leq\alpha w_i/W$. Therefore

$$
\operatorname{FWER}
\leq\sum_{i\in I_0}\frac{\alpha w_i}{W}
\leq\alpha.
$$

Procedure (B) is the [Weighted Holm step-down procedure](../../../statistical-modelling.md#weighted-holm-step-down-procedure). Let $k$ be the first rank in the ordering $q_{(1)}<\cdots<q_{(m)}$ whose hypothesis is a true null, and put $W_0=\sum_{i\in I_0}w_i$. If any true null is rejected, the procedure reaches step $k$ and

$$
q_{(k)}\leq\frac\alpha{\sum_{j=k}^m w_{(j)}}\leq\frac\alpha{W_0},
$$

because every true null remains among ranks $k,\ldots,m$. Hence

$$
\{\text{a true null is rejected}\}
\subseteq
\bigcup_{i\in I_0}\left\{p_i\leq\frac{\alpha w_i}{W_0}\right\},
$$

and another [union bound](../../../probability-inequality.md#boole-s-inequality) gives FWER at most $\alpha$.

At step $k$, procedure (B) divides by the total weight still under consideration, which is no larger than $W$. Its critical values therefore increase as hypotheses are rejected. Moreover, if procedure (A) would reject a hypothesis, every earlier ordered $q$ also passes the initial threshold, so procedure (B) reaches and rejects it. Thus (B) contains every rejection of (A) and can make strictly more rejections while retaining the same strong FWER control.

## 3

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Under the null, $\varepsilon_1$ and $\xi_1$ have [conditional independence](../../../random-variable.md#conditional-independence) given $z_1$. The [law of total expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\boxed{\mathbb E(\varepsilon_1^2\xi_1^2)
=\mathbb E\!\left[
\mathbb E(\varepsilon_1^2\mid z_1)
\mathbb E(\xi_1^2\mid z_1)
\right]
\leq C^2.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Conditional on the covariates and all responses used to construct $\widehat g$, the residual $\varepsilon_i$ has conditional second moment at most $C$; [conditional independence](../../../random-variable.md#conditional-independence) under the null is what permits this conditioning. Consequently

$$
\mathbb E\!\left[\frac1n\sum_{i=1}^n\varepsilon_i^2G_i^2\right]
\leq C\,\mathbb E\!\left[\frac1n\sum_{i=1}^nG_i^2\right]\longrightarrow0.
$$

The [Markov inequality](../../../probability-inequality.md#markov-inequality) proves

$$
\frac1n\sum_i\varepsilon_i^2G_i^2\xrightarrow{p}0.
$$

Next, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
\left|\frac1n\sum_i\xi_i\varepsilon_i^2G_i\right|
\leq
\left(\frac1n\sum_i\varepsilon_i^2G_i^2\right)^{1/2}
\left(\frac1n\sum_i\varepsilon_i^2\xi_i^2\right)^{1/2}.
$$

The first factor converges to zero in probability. The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) and part a make the second $O_p(1)$, so the product converges to zero in probability.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Two applications of the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
\left|\frac1n\sum_iF_iG_i\varepsilon_i\xi_i\right|
\leq
\left(\frac1n\sum_iF_i^2G_i^2\right)^{1/2}
\left(\frac1n\sum_i\varepsilon_i^2\xi_i^2\right)^{1/2}
\xrightarrow{p}0
$$

and

$$
\frac1n\sum_i|\varepsilon_iF_i|G_i^2
\leq
\left(\frac1n\sum_iF_i^2G_i^2\right)^{1/2}
\left(\frac1n\sum_i\varepsilon_i^2G_i^2\right)^{1/2}
\xrightarrow{p}0.
$$

Here the empirical residual second moment is again $O_p(1)$ by the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers), while the assumed product error and the conclusion of part b are $o_p(1)$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write

$$
R_i=(x_i-\widehat f(z_i))(y_i-\widehat g(z_i))
=(\varepsilon_i+F_i)(\xi_i+G_i).
$$

Expanding $R_i^2$ gives the leading term $\varepsilon_i^2\xi_i^2$ and terms of the forms treated in parts b and c, together with their versions obtained by interchanging $(\varepsilon,F)$ and $(\xi,G)$. For example, the pure error terms are $\varepsilon_i^2G_i^2$, $\xi_i^2F_i^2$, and $F_i^2G_i^2$, and each cross term is controlled by [Cauchy-Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality) from these. Hence

$$
\tau_D^2=\frac1n\sum_iR_i^2
=\frac1n\sum_i\varepsilon_i^2\xi_i^2+o_p(1)
\xrightarrow{p}\mathbb E(\varepsilon_1^2\xi_1^2).
$$

Assuming this limit is positive, the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) yields $\tau_D\xrightarrow{p}\{\mathbb E(\varepsilon_1^2\xi_1^2)\}^{1/2}$. Combining this with the assumed [convergence in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) of $\sqrt n\tau_N$ and applying the [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) gives

$$
T=\frac{\sqrt n\tau_N}{\tau_D}\xrightarrow{d}N(0,1).
$$

This is the [studentization of the generalized covariance measure statistic](../../../random-variable.md#studentization-of-the-generalized-covariance-measure-statistic).

## 4

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A centered [random variable](../../../random-variable.md) $X$ is [sub-Gaussian](../../../probability-and-statistics.md#sub-gaussian-distribution) with parameter $a>0$ when

$$
\mathbb E e^{tX}\leq e^{a^2t^2/2}
$$

for every $t\in\mathbb R$.

The [Bernstein concentration inequality for products of sub-Gaussian variables](../../../probability-and-statistics.md#bernstein-concentration-inequality-for-products-of-sub-gaussian-variables) quoted in the course says that if each coordinate of the identically distributed pairs $(U_i,V_i)$ is sub-Gaussian with parameter $\sigma/4$, then

$$
\mathbb P\!\left(\left|\frac1n\sum_{i=1}^n
\{U_iV_i-\mathbb E(U_iV_i)\}\right|\geq t\right)
\leq2\exp\!\left(-\frac{2nt^2}{\sigma^2(\sigma^2+t)}\right).
$$

Since $U^TV=\sum_iU_iV_i$, this is the required bound. It follows by observing that a product of sub-Gaussian variables is [sub-exponential](../../../probability-and-statistics.md#subexponential-distribution-light-tailed) and applying [Bernstein's inequality](../../../probability-inequality.md#bernstein-inequalities-probability-theory) to the independent centered products.

For any vector $\delta$ admissible in the definition of $\phi_\Sigma^2$, one has $\|\delta\|_1\leq4$. The [entrywise maximum norm](../../../vector-space.md#entrywise-maximum-norm) bound therefore implies

$$
|\delta^T(\Theta-\Sigma)\delta|
\leq\max_{j,k}|\Theta_{jk}-\Sigma_{jk}|\,\|\delta\|_1^2
\leq\frac{\phi_\Sigma^2}{2s}.
$$

By the definition of the [compatibility constant](../../../probability-and-statistics.md#compatibility-constant), $\delta^T\Sigma\delta\geq\phi_\Sigma^2/s$, and hence

$$
\delta^T\Theta\delta\geq\frac{\phi_\Sigma^2}{2s}.
$$

Taking the infimum proves $\phi_\Theta^2\geq\phi_\Sigma^2/2$. This is the [stability of a compatibility constant under entrywise perturbation](../../../probability-and-statistics.md#stability-of-a-compatibility-constant-under-entrywise-perturbation).

Put $C=X^TX/n$. Applying the product concentration bound with the stated $t$ and using $t\leq\sigma^2/3$ gives, for every $j,k$,

$$
\mathbb P(|C_{jk}-\Sigma_{jk}|>t)
\leq2e^{-3\log(p+1)}=\frac2{(p+1)^3}.
$$

There are $p(p+1)/2$ distinct entries in the symmetric matrix, so the [union bound](../../../probability-inequality.md#boole-s-inequality) shows that the event

$$
\mathcal E=\left\{\max_{j,k}|C_{jk}-\Sigma_{jk}|\leq t\right\}
$$

has probability at least $1-p/(p+1)^2\geq p/(p+1)$.

On $\mathcal E$, $|C_{jj}-1|\leq t$. Since $|\Sigma_{jk}|\leq1$ by [Cauchy-Schwarz](../../../probability-and-statistics.md#cauchy-schwarz-inequality), normalization of the sample columns gives

$$
|\widehat\Sigma_{jk}-\Sigma_{jk}|
=\left|\frac{C_{jk}}{\sqrt{C_{jj}C_{kk}}}-\Sigma_{jk}\right|
\leq\frac{2t}{1-t}.
$$

Choosing one coordinate of $S$ in the infimum shows $\phi_\Sigma^2\leq s$, so the assumed bound on $t$ is below one and, more precisely,

$$
t\leq\frac{\phi_\Sigma^2}{64s+\phi_\Sigma^2}
\quad\Longrightarrow\quad
\frac{2t}{1-t}\leq\frac{\phi_\Sigma^2}{32s}.
$$

The perturbation result now gives $\phi_{\widehat\Sigma}^2\geq\phi_\Sigma^2/2$ throughout $\mathcal E$, and therefore

$$
\boxed{\mathbb P(\phi_{\widehat\Sigma}^2\geq\phi_\Sigma^2/2)\geq\frac p{p+1}.}
$$

## 5

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

With the normalization used in the question, [ridge regression](../../../linear-regression.md#ridge-regression) solves

$$
\min_{\mu\in\mathbb R,\,\beta\in\mathbb R^p}
\bigl\|Y-\mu\mathbf1-X\beta\bigr\|_2^2+\lambda\|\beta\|_2^2.
$$

Differentiating with respect to $\mu$ and using the centered columns $X^T\mathbf1=0$ gives $\widehat\mu=\overline Y$. The [normal equation](../../../statistical-modelling.md#normal-equation) for $\beta$ is

$$
(X^TX+\lambda I)\widehat\beta=X^TY,
$$

so

$$
\widehat\beta=(X^TX+\lambda I)^{-1}X^TY.
$$

The [push-through identity](../../../linear-algebra.md#push-through-identity) then gives the equivalent dual form

$$
\boxed{\widehat\beta=X^T(XX^T+\lambda I)^{-1}Y.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Fix $j\in A$ and write

$$
R=\lambda I+X_{A\setminus\{j\}}X_{A\setminus\{j\}}^T,
\qquad a=X_j^TR^{-1}X_j\geq0.
$$

The matrix $R$ is [positive definite](../../../linear-algebra.md#positive-definite-matrix). Applying the [Sherman–Morrison formula](../../../linear-algebra.md#sherman-morrison-formula) to $R+X_jX_j^T$ yields

$$
\boxed{X_j^T(X_AX_A^T+\lambda I)^{-1}X_j
=a-\frac{a^2}{1+a}=\frac a{1+a}<1.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For the active set $A_k$, maintain

$$
M_k^{-1}=(X_{A_k}X_{A_k}^T+\lambda I)^{-1}.
$$

The initial $n\times n$ [matrix inverse](../../../linear-algebra.md#matrix-inverse) costs $O(n^3)$. At step $k$, compute $v_k=M_k^{-1}Y$ in $O(n^2)$ operations and all active ridge coefficients $X_{A_k}^Tv_k$ in $O(|A_k|n)$ operations; their smallest absolute value determines $j_k$.

After deleting $j_k$,

$$
M_{k+1}=M_k-X_{j_k}X_{j_k}^T.
$$

Part b ensures that the denominator in the [Sherman–Morrison formula](../../../linear-algebra.md#sherman-morrison-formula) is positive, and the rank-one downdate

$$
M_{k+1}^{-1}
=M_k^{-1}+
\frac{M_k^{-1}X_{j_k}X_{j_k}^TM_k^{-1}}
{1-X_{j_k}^TM_k^{-1}X_{j_k}}
$$

costs $O(n^2)$. Summing over the $p$ steps gives

$$
O(n^3)+O(pn^2)+O\!\left(n\sum_{k=1}^p|A_k|\right)
=O(n^3+pn^2+p^2n).
$$

Since $p\geq n$, both earlier terms are bounded by $O(p^2n)$, proving the claimed computational complexity within [computational complexity theory](../../../computer-science.md#computational-complexity-theory).

## 6

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

With the convention matching the constants below, the [Lasso](../../../probability-and-statistics.md#lasso) estimator is any minimizer

$$
\widehat\beta\in\underset{\beta\in\mathbb R^p}{\operatorname{argmin}}
\left\{\frac1n\|Y-X\beta\|_2^2+2\lambda\|\beta\|_1\right\}.
$$

Because $X^T\mathbf1=0$, the centered noise has the same score as $\varepsilon$: $X^T(\varepsilon-\overline\varepsilon\mathbf1)=X^T\varepsilon$. Each $X_j^T\varepsilon/n$ is sub-Gaussian with scale $1/\sqrt n$, so

$$
\mathbb P\!\left(\frac{2|X_j^T\varepsilon|}{n}>\lambda\right)
\leq2e^{-n\lambda^2/8}.
$$

For $\lambda=A\sqrt{\log p/n}$, a [union bound](../../../probability-inequality.md#boole-s-inequality) over the $p$ columns yields

$$
\mathbb P\!\left(\frac{2\|X^T\varepsilon\|_\infty}{n}\leq\lambda\right)
\geq1-2p^{-(A^2/8-1)}.
$$

Call this event $\mathcal T$.

The [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) for the Lasso say that there is $\widehat z\in\mathbb R^p$ such that

$$
\frac1nX^T(Y-X\widehat\beta)=\lambda\widehat z,
\qquad
\widehat z_j=
\begin{cases}
\operatorname{sgn}(\widehat\beta_j),&\widehat\beta_j\ne0,\\
[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

Equivalently, $\widehat z$ belongs to the [subdifferential](../../../convex-optimization.md#subdifferential) of the $\ell^1$ norm at $\widehat\beta$.

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let $\delta=\widehat\beta-\beta^0$. Comparing the Lasso objective at $\widehat\beta$ and $\beta^0$ gives the [Basic inequality for the Lasso](../../../probability-and-statistics.md#basic-inequality-for-the-lasso). On $\mathcal T$ it implies

$$
\frac1n\|X\delta\|_2^2
+2\lambda(\|\beta^0+\delta\|_1-\|\beta^0\|_1)
\leq\lambda\|\delta\|_1.
$$

Since

$$
\|\beta^0+\delta\|_1-\|\beta^0\|_1
\geq\|\delta_N\|_1-\|\delta_S\|_1,
$$

we obtain the [Lasso cone condition](../../../probability-and-statistics.md#lasso-cone-condition)

$$
\|\delta_N\|_1\leq3\|\delta_S\|_1.
$$

The [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) also give

$$
\widehat\Sigma\delta
=\frac1nX^T\varepsilon-\lambda\widehat z,
$$

so on $\mathcal T$,

$$
\|\widehat\Sigma\delta\|_\infty
\leq\frac\lambda2+\lambda=\frac{3\lambda}{2}.
$$

The assumed cone invertibility condition therefore yields

$$
\|\delta_S\|_\infty\leq\frac{3\lambda}{2\psi}.
$$

If $\min_{j\in S}|\beta_j^0|>3\lambda/(2\psi)$, then every active coefficient remains nonzero and retains its sign. Substituting $\lambda=A\sqrt{\log p/n}$ proves

$$
\operatorname{sgn}(\widehat\beta_S)=\operatorname{sgn}(\beta_S^0)
$$

on an event of the required probability. This is [Lasso sign recovery from cone invertibility](../../../probability-and-statistics.md#lasso-sign-recovery-from-cone-invertibility).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

On the same event, the [Lasso cone condition](../../../probability-and-statistics.md#lasso-cone-condition) and the coordinatewise bound from part a give

$$
\|\widehat\beta-\beta^0\|_1
=\|\delta_S\|_1+\|\delta_N\|_1
\leq4\|\delta_S\|_1
\leq4s\|\delta_S\|_\infty
\leq\frac{6s\lambda}{\psi}.
$$

With $\lambda=A\sqrt{\log p/n}$ this is exactly

$$
\boxed{\|\widehat\beta-\beta^0\|_1
\leq\frac{6sA}{\psi}\sqrt{\frac{\log p}{n}}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
