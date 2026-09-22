# Paper 205

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_205.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_205.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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

## 1

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A symmetric function $k:\mathcal X\times\mathcal X\to\mathbb R$ is a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) when, for every $m$, every $x_1,\ldots,x_m\in\mathcal X$, and every $c\in\mathbb R^m$,

$$
\sum_{i,j=1}^mc_ic_jk(x_i,x_j)\geq0.
$$

Equivalently, every associated [kernel matrix](../../../probability-and-statistics.md#kernel-matrix) is a [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix).

A [Reproducing kernel Hilbert space](../../../probability-and-statistics.md#reproducing-kernel-hilbert-space) $\mathcal H$ on $\mathcal X$ is a [Hilbert space](../../../hilbert-space.md) of real-valued functions such that every point-evaluation map $f\mapsto f(x)$ is continuous. The [Riesz representation theorem](../../../hilbert-space.md#riesz-representation-theorem) then gives a function $k(x,\cdot)\in\mathcal H$ satisfying the [reproducing property](../../../probability-and-statistics.md#reproducing-property)

$$
f(x)=\langle f,k(x,\cdot)\rangle_{\mathcal H}.
$$

Its reproducing kernel is $k(x,y)=\langle k(x,\cdot),k(y,\cdot)\rangle_{\mathcal H}$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Suppose a [feature map](../../../probability-and-statistics.md#feature-map) $\phi:\mathbb R^d\to\mathbb R^p$ represented the [Gaussian kernel](../../../probability-and-statistics.md#gaussian-kernel). Choose $n>p$, a unit vector $e$, and points $x_i=iae$ for $i=0,\ldots,n-1$. Their [kernel matrix](../../../probability-and-statistics.md#kernel-matrix) is

$$
K_{ij}=\exp\!\left(-\frac{a^2(i-j)^2}{2\sigma^2}\right)=r^{(i-j)^2},
\qquad r=e^{-a^2/(2\sigma^2)}.
$$

For sufficiently large $a$, hence sufficiently small $r$, every row satisfies

$$
\sum_{j\ne i}|K_{ij}|\leq2\sum_{m\geq1}r^{m^2}<1=K_{ii}.
$$

Thus $K$ is a symmetric [strictly diagonally dominant matrix](../../../vector-space.md#strictly-diagonally-dominant-matrix) with positive diagonal and is therefore a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), so $\operatorname{rank}K=n$.

On the other hand, if $\Phi$ is the $n\times p$ matrix whose $i$th row is $\phi(x_i)^T$, then $K=\Phi\Phi^T$ and $\operatorname{rank}K\leq p<n$, a contradiction. Hence every feature-space realization of the Gaussian kernel requires an [infinite-dimensional vector space](../../../vector-space.md#infinite-dimensional-vector-space).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $x,y>0$, the [Laplace transform](../../../analysis.md#laplace-transform) identity

$$
\frac1{x+y}=\int_0^\infty e^{-tx}e^{-ty}\,dt
$$

exhibits $k_1$ as an inner product of the [feature functions](../../../probability-and-statistics.md#feature-map) $t\mapsto e^{-tx}$ in $L^2(0,\infty)$. More explicitly, for any real $c_i$ and positive $x_i$,

$$
\sum_{i,j}c_ic_jk_1(x_i,x_j)
=\int_0^\infty\left(\sum_i c_i e^{-tx_i}\right)^2dt\geq0.
$$

**Therefore $k_1$ is a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel).**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put

$$
a(x,y)=\frac{x^Ty}{\lVert x\rVert^2+\lVert y\rVert^2}.
$$

The numerator is the [linear kernel](../../../probability-and-statistics.md#linear-kernel), while the reciprocal of the denominator is the kernel from part c applied to $\lVert x\rVert^2$ and $\lVert y\rVert^2$. The [product of positive-semidefinite kernels](../../../probability-and-statistics.md#product-of-positive-semidefinite-kernels) therefore shows that $a$ is a positive-semidefinite kernel. The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and the [arithmetic-geometric mean inequality](../../../mathematical-optimization.md#arithmetic-geometric-mean-inequality) give $|a(x,y)|\leq1/2$, so

$$
k_2(x,y)=\frac{a(x,y)}{1-a(x,y)}=\sum_{m=1}^\infty a(x,y)^m.
$$

Each power is positive semidefinite by the [Schur product theorem](../../../linear-algebra.md#schur-product-theorem), and the convergent sum is positive semidefinite.

Moreover $k_2(x,x)=1$. If $\Phi$ is its canonical [feature map](../../../probability-and-statistics.md#feature-map), then

$$
d(x,y)^2=2-2k_2(x,y)=\lVert\Phi(x)-\Phi(y)\rVert^2.
$$

The feature-space norm gives symmetry and the [triangle inequality](../../../topological-analysis.md#triangle-inequality). Finally, $d(x,y)=0$ implies $k_2(x,y)=1$, hence $a(x,y)=1/2$ and

$$
2x^Ty=\lVert x\rVert^2+\lVert y\rVert^2,
$$

which is equivalent to $\lVert x-y\rVert^2=0$. Thus $d$ is a [metric](../../../topological-analysis.md#metric) rather than merely a [pseudometric](../../../topological-analysis.md#pseudometric).

## 2

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The matrix $S$ is the [sample covariance matrix](../../../variance.md#sample-covariance-matrix)

$$
S=\frac1n\sum_{r=1}^n(x_r-\bar x)(x_r-\bar x)^T,
\qquad \bar x=\frac1n\sum_{r=1}^nx_r.
$$

Changing $n$ to $n-1$ is another convention, but the objective must use the same convention throughout.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The differential of the [log-determinant](../../../linear-algebra.md#log-determinant) is $d\log\det\Omega=\operatorname{Tr}(\Omega^{-1}d\Omega)$. The [subdifferential](../../../convex-optimization.md#subdifferential) of the entrywise $\ell^1$ norm consists of symmetric matrices $Z$ with

$$
Z_{ij}=\operatorname{sgn}(\Omega_{ij})\quad\hbox{if }\Omega_{ij}\ne0,
\qquad Z_{ij}\in[-1,1]\quad\hbox{if }\Omega_{ij}=0.
$$

The [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) for the [Graphical Lasso](../../../variance.md#graphical-lasso) are therefore

$$
-\widehat\Omega^{-1}+S+\lambda Z=0,
\qquad Z\in\partial\lVert\widehat\Omega\rVert_{1,\mathrm{entry}}.
$$

Because $-\log\det\Omega$ is [strictly convex](../../../real-analysis.md#strictly-convex-function) on the [positive-definite matrices](../../../linear-algebra.md#positive-definite-matrix), these conditions characterize the unique minimizer whenever it exists.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Multiply the [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) on the right by $\widehat\Omega$ and take the [matrix trace](../../../linear-algebra.md#matrix-trace):

$$
-p+\operatorname{Tr}(S\widehat\Omega)+\lambda\operatorname{Tr}(Z\widehat\Omega)=0.
$$

Symmetry and the defining property of the [subgradient of the absolute value](../../../real-analysis.md#subgradient-of-the-absolute-value) give

$$
\operatorname{Tr}(Z\widehat\Omega)
=\sum_{i,j}Z_{ij}\widehat\Omega_{ij}
=\sum_{i,j}|\widehat\Omega_{ij}|.
$$

Consequently the last two terms in the objective sum to $p$, and hence

$$
\boxed{Q(\widehat\Omega)=-\log\det\widehat\Omega+p.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $\widehat\Omega^{(k)}$ solve the $k$th diagonal-block problem and set

$$
\widetilde\Omega=
\begin{bmatrix}\widehat\Omega^{(1)}&0\\0&\widehat\Omega^{(2)}\end{bmatrix}.
$$

Its inverse is block diagonal. On each diagonal block, the [Graphical-Lasso Karush-Kuhn-Tucker conditions](../../../variance.md#graphical-lasso-karush-kuhn-tucker-conditions) hold by the definition of $\widehat\Omega^{(k)}$. On the off-diagonal blocks choose

$$
Z^{(12)}=-S^{(12)}/\lambda,
\qquad Z^{(21)}=-S^{(21)}/\lambda.
$$

The assumed inequalities $|S_{ij}|\leq\lambda$ ensure that every entry lies in $[-1,1]$, exactly the allowed [subgradient](../../../real-analysis.md#subgradient) at a zero entry of $\widetilde\Omega$.

**Thus $-\widetilde\Omega^{-1}+S+\lambda Z=0$ on every block. The KKT conditions and the fact that the objective is [strictly convex](../../../real-analysis.md#strictly-convex-function) prove that $\widetilde\Omega=\widehat\Omega$, giving the claimed block decomposition.**

## 3

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

With the normalization used here, the [Lasso](../../../probability-and-statistics.md#lasso) estimator minimizes

$$
\frac1{2n}\lVert Y-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_1.
$$

Optimality at $\widehat\beta$ relative to the feasible point $\beta^0$ gives

$$
\frac1{2n}\lVert Y-X\widehat\beta\rVert_2^2+\lambda\lVert\widehat\beta\rVert_1
\leq\frac1{2n}\lVert Y-X\beta^0\rVert_2^2+\lambda\lVert\beta^0\rVert_1.
$$

The columns of $X$ are centered, so $X^T\mathbf1=0$ and the centered noise produces the same [score function](../../../statistical-modelling.md#informant-function) as $\varepsilon$. Expanding the two squared norms and cancelling the noise norm yields the standard [Basic inequality for the Lasso](../../../probability-and-statistics.md#basic-inequality-for-the-lasso)

$$
\frac1{2n}\lVert X(\widehat\beta-\beta^0)\rVert_2^2
\leq\frac1n(\widehat\beta-\beta^0)^TX^T\varepsilon
+\lambda\lVert\beta^0\rVert_1-\lambda\lVert\widehat\beta\rVert_1.
$$

Thus the displayed inequality in the question has a factor-of-two typo: its left side should be $\lVert X(\widehat\beta-\beta^0)\rVert_2^2/(2n)$, or both terms on its right should be doubled. No scaling of the usual squared-error Lasso objective produces the three displayed coefficients simultaneously. Parts b and d explicitly ask us to use the stated inequality, so their requested constants follow from that stated version.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $\delta=\widehat\beta-\beta^0$. On $\Omega$, [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) gives

$$
\frac1n\delta^TX^T\varepsilon
\leq\lVert\delta\rVert_1\frac{\lVert X^T\varepsilon\rVert_\infty}{n}
\leq\frac\lambda2\lVert\delta\rVert_1.
$$

Since $\beta_N^0=0$, the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\lVert\beta^0\rVert_1-\lVert\widehat\beta\rVert_1
\leq\lVert\delta_S\rVert_1-\lVert\delta_N\rVert_1.
$$

Substitution in the [Basic inequality for the Lasso](../../../probability-and-statistics.md#basic-inequality-for-the-lasso), followed by discarding the nonnegative prediction-error term, yields

$$
\frac\lambda2\lVert\delta_N\rVert_1
\leq\frac{3\lambda}{2}\lVert\delta_S\rVert_1.
$$

**Therefore $\lVert\widehat\beta_N-\beta_N^0\rVert_1\leq3\lVert\widehat\beta_S-\beta_S^0\rVert_1$, the [Lasso cone condition](../../../probability-and-statistics.md#lasso-cone-condition).**

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For each column $X_j$, the normalized score is

$$
W_j=\frac1nX_j^T\varepsilon=\frac1n\sum_{i=1}^nX_{ij}\varepsilon_i.
$$

The errors are independent [Rademacher random variables](../../../probability-theory.md#rademacher-distribution), and $\lVert X_j\rVert_2^2=n$. The [Hoeffding lemma](../../../probability-inequality.md#hoeffding-lemma) therefore makes $W_j$ a [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution) with variance proxy $1/n$, so

$$
\mathbb P(|W_j|>t)\leq2e^{-nt^2/2}.
$$

The [union bound](../../../probability-inequality.md#boole-s-inequality) with $t=\lambda/2$ gives

$$
\mathbb P(\Omega)
\geq1-2p\exp\!\left(-\frac{n\lambda^2}{8}\right).
$$

For $\lambda=A\sqrt{\log p/n}$ this becomes

$$
\mathbb P(\Omega)\geq1-2p^{,1-A^2/8}.
$$

In particular, if $A>\sqrt8$, the lower bound tends to one as $p\to\infty$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Part b places $\delta=\widehat\beta-\beta^0$ in the [Lasso cone condition](../../../probability-and-statistics.md#lasso-cone-condition). Keeping the prediction-error term in the same argument gives

$$
\frac1n\lVert X\delta\rVert_2^2
\leq\frac{3\lambda}{2}\lVert\delta_S\rVert_1
\leq\frac{3\lambda\sqrt{|S|}}2\lVert\delta\rVert_2,
$$

where the second step is the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). The [restricted eigenvalue condition](../../../probability-and-statistics.md#restricted-eigenvalue-condition) gives

$$
\frac1n\lVert X\delta\rVert_2^2>\gamma\lVert\delta\rVert_2^2
$$

for nonzero $\delta$ in this cone. Division by $\lVert\delta\rVert_2$ proves

$$
\lVert\widehat\beta-\beta^0\rVert_2
\leq\frac{3\lambda\sqrt{|S|}}{2\gamma}.
$$

The result is immediate when $\delta=0$.

## 4

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [Square-root Lasso](../../../probability-and-statistics.md#square-root-lasso) estimator with regularization parameter $\gamma>0$ is

$$
\widehat\beta
=\underset{\beta\in\mathbb R^p}{\operatorname{argmin}}
\left\{\frac1{\sqrt n}\lVert Y-X\beta\rVert_2+\gamma\lVert\beta\rVert_1\right\}.
$$

Unlike the ordinary [Lasso](../../../probability-and-statistics.md#lasso), its tuning parameter does not require prior knowledge of the noise standard deviation $\sigma$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

One standard construction uses the [Debiased Lasso](../../../probability-and-statistics.md#debiased-lasso). Starting from the [Square-root Lasso](../../../probability-and-statistics.md#square-root-lasso) estimate $\widehat\beta$, estimate a vector $\widehat\Theta_j$ that approximately inverts the $j$th column of the empirical Gram matrix $\widehat\Sigma=X^TX/n$, for example by a [Nodewise Lasso](../../../probability-and-statistics.md#nodewise-lasso). Define

$$
\widetilde\beta_j
=\widehat\beta_j+\widehat\Theta_j^T\frac{X^T(Y-X\widehat\beta)}n,
\qquad
\widehat V_j=\widehat\Theta_j^T\widehat\Sigma\widehat\Theta_j,
$$

and estimate $\sigma$ by $\widehat\sigma=\lVert Y-X\widehat\beta\rVert_2/\sqrt n$. The approximate two-sided level-$\alpha$ test rejects $H_j^\beta$ when

$$
\left|\frac{\sqrt n\,\widetilde\beta_j}{\widehat\sigma\sqrt{\widehat V_j}}\right|>z_{1-\alpha/2},
$$

where $z_{1-\alpha/2}$ is a [standard normal quantile](../../../probability-theory.md#standard-normal-quantile).

Sufficient high-dimensional conditions include a [Compatibility condition for the Lasso](../../../probability-and-statistics.md#compatibility-condition-for-the-lasso) bounded away from zero, $\gamma\asymp\sqrt{\log p/n}$, $\log p=o(n)$, and

$$
\frac{s\log p}{\sqrt n}\longrightarrow0,
$$

together with the corresponding sparsity and consistency conditions for the nodewise inverse-Gram estimate. Under these assumptions the [Debiased-Lasso asymptotic normality](../../../probability-and-statistics.md#debiased-lasso-asymptotic-normality) makes the rejection probability under $H_j^\beta$ tend to $\alpha$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

If $B=\varnothing$, then for every $j$ at least one of $H_j^\beta$ and $H_j^\eta$ is true. Since

$$
\{q_j\leq t\}=\{q_j^\beta\leq t\}\cap\{q_j^\eta\leq t\},
$$

validity of the [p-value](../../../statistical-modelling.md#p-value) for whichever component null is true implies $\mathbb P(q_j\leq t)\leq t$. Therefore the [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P\!\left(\min_{1\leq j\leq p}q_j\leq\frac\alpha p\right)
\leq\sum_{j=1}^p\mathbb P\!\left(q_j\leq\frac\alpha p\right)
\leq\alpha.
$$

This is the [Bonferroni correction](../../../statistical-modelling.md#bonferroni-correction) for the composite intersection alternatives.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Let $I_0=B^c$ and $m_0=|I_0|$. Each $q_j$ with $j\in I_0$ is a valid [p-value](../../../statistical-modelling.md#p-value) by the argument in part c. If the [Holm step-down procedure](../../../statistical-modelling.md#holm-bonferroni-method) selects any index from $I_0$, let $r$ be the rank of the first such index. All $r-1$ earlier selections belong to $B$, so

$$
r\leq|B|+1=p-m_0+1,
\qquad p-r+1\geq m_0.
$$

Selection through rank $r$ implies

$$
q_{\tau(r)}\leq\frac\alpha{p-r+1}\leq\frac\alpha{m_0}.
$$

Consequently

$$
\mathbb P(\widehat B\not\subseteq B)
\leq\mathbb P\!\left(\min_{j\in I_0}q_j\leq\frac\alpha{m_0}\right)
\leq\sum_{j\in I_0}\mathbb P\!\left(q_j\leq\frac\alpha{m_0}\right)
\leq\alpha.
$$

**Thus the procedure controls the [familywise error rate](../../../statistical-modelling.md#familywise-error-rate) without requiring independence among the p-values.**

## 5

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [kernel ridge regression](../../../probability-and-statistics.md#kernel-ridge-regression) estimator is

$$
\widehat f_\lambda
=\underset{f\in\mathcal H}{\operatorname{argmin}}
\left\{\frac1n\sum_{i=1}^n(Y_i-f(x_i))^2+\lambda\lVert f\rVert_{\mathcal H}^2\right\}.
$$

By the [representer theorem](../../../probability-and-statistics.md#representer-theorem), $\widehat f_\lambda=\sum_{j=1}^n\alpha_jk(x_j,\cdot)$. If $K_{ij}=k(x_i,x_j)$, substitution and differentiation give

$$
(K+n\lambda I)\alpha=Y.
$$

Thus

$$
\alpha=(K+n\lambda I)^{-1}Y,
\qquad
\widehat Y=H_\lambda Y,
\qquad
H_\lambda=K(K+n\lambda I)^{-1}.
$$

The matrix $H_\lambda$ is the [kernel-ridge hat matrix](../../../probability-and-statistics.md#kernel-ridge-hat-matrix).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [leave-one-out residual identity for a linear smoother](../../../statistical-learning.md#leave-one-out-residual-identity-for-a-linear-smoother), obtained from the [block matrix inverse](../../../linear-algebra.md#block-matrix-inverse) or the [Sherman–Morrison formula](../../../linear-algebra.md#sherman-morrison-formula), is

$$
Y_i-\widehat f_{\lambda,-i}(x_i)
=\frac{Y_i-\widehat Y_i}{1-(H_\lambda)_{ii}}.
$$

Hence

$$
\widehat T_\lambda
=\frac1n\sum_{i=1}^n
\left(\frac{Y_i-(H_\lambda Y)_i}{1-(H_\lambda)_{ii}}\right)^2.
$$

Compute once the [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) $K=U\operatorname{diag}(d_1,\ldots,d_n)U^T$ in $O(n^3)$ operations and the vector $U^TY$ in $O(n^2)$. For each $\lambda_\ell$, set

$$
h_r(\lambda_\ell)=\frac{d_r}{d_r+n\lambda_\ell}.
$$

Then compute

$$
H_{\lambda_\ell}Y
=U\operatorname{diag}(h_r(\lambda_\ell))U^TY,
\qquad
(H_{\lambda_\ell})_{ii}=\sum_{r=1}^nU_{ir}^2h_r(\lambda_\ell).
$$

Both calculations take $O(n^2)$ operations per tuning parameter, after which the displayed leave-one-out formula costs $O(n)$. All $L$ scores therefore require $O(n^3+Ln^2)$ operations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
