# Paper 205

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_205.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_205.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [1](#3/1)
    - [Solution](#3/1/solution)
  - [2](#3/2)
    - [Solution](#3/2/solution)
  - [3](#3/3)
    - [Solution](#3/3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A procedure controls the [familywise error rate](../../../statistical-modelling.md#familywise-error-rate) at level $\alpha$ when, for every configuration of true nulls $I$,

$$
\mathbb P(\text{at least one }H_i, i\in I,
\text{ is rejected})\leq\alpha.
$$

Let $i_*=\min I$. The step-down procedure can reject any true null only if it reaches and rejects $H_{i_*}$, which requires $p_{i_*}\leq\alpha$. Since a valid [p-value](../../../statistical-modelling.md#p-value) under its null satisfies $\mathbb P(p_{i_*}\leq\alpha)\leq\alpha$, the procedure controls FWER without any assumption on dependence among the p-values.

A distribution $P$ has the [global Markov property for a directed acyclic graph](../../../causal-inference.md#global-markov-property-for-a-directed-acyclic-graph) $G$ when every [D-separation](../../../combinatorics.md#d-separation) statement $A\mathrel{\perp_G}B\mid C$ implies the corresponding [conditional independence](../../../random-variable.md#conditional-independence) $Z_A\perp\!\!\!\perp Z_B\mid Z_C$ under $P$.

If $G\in\mathcal S$ has nonadjacent vertices $j,k$, choose a [topological ordering](../../../combinatorics.md#topological-ordering). Suppose $j$ precedes $k$. Then $j$ is a non-descendant and non-parent of $k$, so the directed local Markov property gives

$$
Z_j\perp\!\!\!\perp Z_k\mid Z_{\operatorname{pa}_G(k)}.
$$

The reversed ordering case is analogous. Hence

$$
H_0\subseteq\bigcup_{S\subseteq[p]\setminus\{j,k\}}H_S.
$$

Use the [intersection-union test](../../../statistical-modelling.md#intersection-union-test): reject $H_0$ exactly when $p_S\leq\alpha$ for every $S$. Under $H_0$, at least one $H_{S_*}$ is true, so

$$
\mathbb P(\text{false rejection of }H_0)
\leq\mathbb P(p_{S_*}\leq\alpha)\leq\alpha.
$$

This is nontrivial because it rejects whenever every tested conditional independence is rejected.

## 2

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The Gaussian maximum-likelihood covariance estimate is

$$
\boxed{\widehat\Sigma=\frac1n\sum_{i=1}^n
(x_i-\overline x)(x_i-\overline x)^T.}
$$

For each $i,k$,

$$
|(AB)_{ik}|
\leq\sum_j|A_{ij}||B_{jk}|
\leq\|A\|_\infty\sum_j|B_{jk}|
\leq\|A\|_\infty\|B\|_{L^1},
$$

so $\|AB\|_\infty\leq\|A\|_\infty\|B\|_{L^1}$. If $A$ is square and symmetric, its maximum row sum equals its maximum column sum, and the same calculation gives

$$
\|AB\|_\infty\leq\|A\|_{L^1}\|B\|_\infty.
$$

Both the objective $\|\Omega\|_1=\sum_j\|\Omega_j\|_1$ and the constraints separate by columns. Replacing one column of a global minimizer by a better feasible column would improve the global objective. Therefore each $\widehat\Omega_j$ minimizes

$$
\|\beta\|_1
\quad\text{subject to}\quad
\|\widehat\Sigma\beta-e_j\|_\infty\leq\lambda.
$$

Moreover,

$$
\|\widehat\Sigma\Omega^0_j-e_j\|_\infty
=\|(\widehat\Sigma-\Sigma^0)\Omega^0_j\|_\infty
\leq\|\widehat\Sigma-\Sigma^0\|_\infty
\|\Omega^0_j\|_1\leq\lambda.
$$

Thus $\Omega^0_j$ is feasible and

$$
\|\widehat\Omega_j\|_1\leq\|\Omega^0_j\|_1.
$$

For every column,

$$
\begin{aligned}
\|\Sigma^0(\widehat\Omega_j-\Omega^0_j)\|_\infty
&\leq\|(\Sigma^0-\widehat\Sigma)\widehat\Omega_j\|_\infty
 +\|\widehat\Sigma\widehat\Omega_j-e_j\|_\infty\\
&\leq\lambda+\lambda=2\lambda.
\end{aligned}
$$

Finally $\widehat\Omega-\Omega^0=\Omega^0\Sigma^0(\widehat\Omega-\Omega^0)$, and symmetry of $\Omega^0$ gives

$$
\boxed{\|\widehat\Omega-\Omega^0\|_\infty
\leq2\lambda\|\Omega^0\|_{L^1}.}
$$

This is the basic error bound for the [CLIME precision-matrix estimator](../../../variance.md#clime-precision-matrix-estimator).

## 3

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="3/1">1</h3>

↑ **Parent:** [3](#3)

<h4 id="3/1/solution">Solution</h4>

↑ **Parent:** [1](#3/1)

A [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) on $\mathcal X$ is a symmetric function $k:\mathcal X^2\to\mathbb R$ such that, for every $x_1,\ldots,x_n$ and $c_1,\ldots,c_n$,

$$
\sum_{i,j=1}^nc_ic_jk(x_i,x_j)\geq0.
$$

If $k(x,x')=\langle\phi(x),\phi(x')\rangle$ for a [feature map](../../../probability-and-statistics.md#feature-map) into an [inner product space](../../../linear-algebra.md#inner-product-space), then

$$
\sum_{i,j}c_ic_jk(x_i,x_j)
=\left\|\sum_ic_i\phi(x_i)\right\|^2\geq0.
$$

Thus every feature-map inner product is a kernel. If $\alpha_1,\alpha_2\geq0$, then each finite quadratic form for $\alpha_1k_1+\alpha_2k_2$ is the corresponding nonnegative linear combination, so **nonnegative linear combinations of kernels are kernels**.

<h3 id="3/2">2</h3>

↑ **Parent:** [3](#3)

<h4 id="3/2/solution">Solution</h4>

↑ **Parent:** [2](#3/2)

For fixed $x_1,\ldots,x_n$ and coefficients $c_i$, every $k_m$ satisfies

$$
\sum_{i,j}c_ic_jk_m(x_i,x_j)\geq0.
$$

The sum is finite, so pointwise convergence permits passage to the limit:

$$
\sum_{i,j}c_ic_jk(x_i,x_j)
=\lim_{m\to\infty}\sum_{i,j}c_ic_jk_m(x_i,x_j)
\geq0.
$$

Symmetry also passes to the limit. Hence **a pointwise limit of kernels is a kernel**.

<h3 id="3/3">3</h3>

↑ **Parent:** [3](#3)

<h4 id="3/3/solution">Solution</h4>

↑ **Parent:** [3](#3/3)

For a finite sample, the Gram matrix of $k_1k_2$ is the entrywise product of the two positive-semidefinite Gram matrices. The [Schur product theorem](../../../linear-algebra.md#schur-product-theorem) makes it positive semidefinite, proving the product closure.

The [Gaussian kernel](../../../probability-and-statistics.md#gaussian-kernel) with bandwidth $\sigma^2$ is

$$
\boxed{k_\sigma(x,x')=
\exp\left(-\frac{\|x-x'\|_2^2}{2\sigma^2}\right).}
$$

Factor it as

$$
e^{-\|x\|^2/(2\sigma^2)}e^{-\|x'\|^2/(2\sigma^2)}
\sum_{m=0}^\infty\frac{(x^Tx')^m}{m!\sigma^{2m}}.
$$

The linear kernel $x^Tx'$ is positive semidefinite; products and nonnegative scalar multiples preserve positivity, as does multiplication by $a(x)a(x')$. The partial sums are therefore kernels, and pointwise-limit closure proves that the Gaussian kernel is positive semidefinite.

## 4

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A vector $g$ is a [subgradient](../../../real-analysis.md#subgradient) of a [convex function](../../../real-analysis.md#convex-function) $f$ at $x$ when

$$
f(y)\geq f(x)+g^T(y-x)\qquad\text{for every }y.
$$

A point $x$ minimizes $f$ exactly when $0\in\partial f(x)$. For absolute value,

$$
\partial|x|=
\begin{cases}
\{-1\},&x<0,\\
[-1,1],&x=0,\\
\{1\},&x>0.
\end{cases}
$$

[Coordinate descent](../../../convex-optimization.md#coordinate-descent) repeatedly minimizes the objective over one coordinate while holding the others fixed, cycling through coordinates until convergence.

The [Lasso](../../../probability-and-statistics.md#lasso) solves

$$
\min_{\beta\in\mathbb R^p}
\frac1{2n}\|Y-X\beta\|_2^2+\lambda\|\beta\|_1.
$$

For the first update, define the partial residual and score

$$
r^{(0)}=Y-\sum_{j=2}^pX_j\widehat\beta_j^{(0)},
\qquad R=X_1^Tr^{(0)}.
$$

Since $\|X_1\|_2^2=n$, the coordinate objective differs by a constant from

$$
\frac12\beta_1^2-\frac Rn\beta_1+\lambda|\beta_1|.
$$

Its subgradient condition gives the [soft thresholding](../../../probability-and-statistics.md#soft-thresholding) update

$$
\boxed{\widehat\beta_1^{(1)}=S_\lambda(R/n).}
$$

For the stated [Berhu penalty](../../../probability-and-statistics.md#berhu-penalty), the derivative is $\operatorname{sgn}(t)$ when $0<|t|\leq\delta$ and $t/\delta$ when $|t|>\delta$. The coordinatewise [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) therefore give

$$
\boxed{
\widehat\beta_1^{(1)}=
\begin{cases}
S_\lambda(R/n),&|S_\lambda(R/n)|\leq\delta,\\[2mm]
\dfrac{R/n}{1+\lambda/\delta},&\text{otherwise}.
\end{cases}}
$$

## 5

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Put $\Delta=\Theta-\Sigma$ and let $\beta$ lie in the compatibility cone. Then

$$
|\beta^T\Delta\beta|
\leq\|\Delta\|_\infty\|\beta\|_1^2
\leq16\|\Delta\|_\infty\|\beta_S\|_1^2
\leq\frac{\phi_\Sigma^2(S)}{2|S|}\|\beta_S\|_1^2.
$$

Subtracting this from the defining lower bound for $\beta^T\Sigma\beta$ and taking the infimum gives the [stability of a compatibility constant under entrywise perturbation](../../../probability-and-statistics.md#stability-of-a-compatibility-constant-under-entrywise-perturbation):

$$
\boxed{\phi_\Theta^2(S)\geq\frac12\phi_\Sigma^2(S).}
$$

A centered random variable $W$ is a [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution) with parameter $\sigma$ when

$$
\mathbb E e^{tW}\leq e^{\sigma^2t^2/2}
\qquad(t\in\mathbb R).
$$

The [Chernoff bound](../../../probability-inequality.md#chernoff-bound) gives $\mathbb P(W>t)\leq e^{-t^2/(2\sigma^2)}$.

For fixed $j,k$, the variables

$$
W_i=X_{ij}X_{ik}-\Sigma_{jk}
$$

are independent, centered, and lie in $[-2,2]$, hence are sub-Gaussian with parameter $2$. Their mean is sub-Gaussian with parameter $2/\sqrt n$, so

$$
\mathbb P(|\widehat\Sigma_{jk}-\Sigma_{jk}|>t)
\leq2e^{-nt^2/8}.
$$

A [union bound](../../../probability-inequality.md#boole-s-inequality) over at most $p^2$ pairs with $t=4\sqrt{2\log(p)/n}$ yields

$$
\boxed{\mathbb P\left(
\|\widehat\Sigma-\Sigma\|_\infty>
4\sqrt{\frac{2\log p}{n}}
\right)\leq\frac2{p^2}.}
$$

The minimum-eigenvalue bound and [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) imply

$$
\beta^T\Sigma\beta\geq c_{\min}\|\beta\|_2^2
\geq\frac{c_{\min}}{|S|}\|\beta_S\|_1^2,
$$

so $\phi_\Sigma^2(S)\geq c_{\min}$. A sufficient uniform condition is

$$
\boxed{c_{\min}\geq128s\sqrt{\frac{2\log p}{n}}.}
$$

Indeed, on the concentration event the entrywise error is at most $c_{\min}/(32s)\leq\phi_\Sigma^2(S)/(32|S|)$ for every $0<|S|\leq s$. The perturbation result then gives $\phi_{\widehat\Sigma}^2(S)\geq c_{\min}/2$ simultaneously, with probability at least $1-2p^{-2}$.

## 6

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The term $\gamma\|\beta\|_2^2/2$ is strictly convex, while the remaining terms are convex, so the [elastic net](../../../probability-and-statistics.md#elastic-net-regularization) objective is strictly convex and its minimizer is unique. If two columns of $X$ are identical, swapping their coefficients leaves the objective unchanged. Uniqueness then forces those coefficients to be equal.

The [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) are

$$
\frac1nX^T(X\widehat\beta-Y)+\gamma\widehat\beta
+\lambda\widehat z=0,
$$

where

$$
\widehat z_j=
\begin{cases}
\operatorname{sgn}(\widehat\beta_j),&\widehat\beta_j\ne0,\\
[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

Assume $Y=X\beta^0$ and $\operatorname{sgn}(\widehat\beta)=\operatorname{sgn}(\beta^0)=s$. The active equations give

$$
(X_S^TX_S+n\gamma I)\widehat\beta_S
=X_S^TX_S\beta_S^0-n\lambda s_S.
$$

The inactive KKT inequalities become

$$
\boxed{\left\|X_N^TX_S(X_S^TX_S+n\gamma I)^{-1}
\left(\frac\gamma\lambda\beta_S^0+s_S\right)
\right\|_\infty\leq1.}
$$

Conversely, define $\widetilde\beta_N=0$ and

$$
\widetilde\beta_S=(X_S^TX_S+n\gamma I)^{-1}
(X_S^TX_S\beta_S^0-n\lambda s_S).
$$

If the displayed inequality holds and $\operatorname{sgn}(\widetilde\beta_S)=s_S$, the active equations and inactive inequalities together satisfy every KKT condition. Convexity and uniqueness imply $\widetilde\beta=\widehat\beta$, proving sign recovery.

The final sign condition printed in the question omits the factor $n$ before $\lambda$. For the objective as stated, the corrected expression above is required; without that correction, the claimed converse does not follow from the KKT equations.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
