# Paper 205

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_205.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_205.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write

$$
L(\beta)=\frac1n\sum_{i=1}^n\left[-y_ix_i^T\beta+\log(1+e^{y_ix_i^T\beta})\right].
$$

Its score is

$$
\nabla_jL(\beta)=-\frac1n\sum_{i=1}^n\frac{y_ix_{ij}}{1+e^{y_ix_i^T\beta}}.
$$

The [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) for [L1-penalized logistic regression](../../../statistical-modelling.md#l1-penalized-logistic-regression) are therefore

$$
-\frac1n\sum_{i=1}^n\frac{y_ix_{ij}}{1+e^{y_ix_i^T\widehat\beta}}+\lambda z_j=0,
\qquad
z_j\in\begin{cases}
\{\operatorname{sgn}(\widehat\beta_j)\},&\widehat\beta_j\ne0,\\
[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The scalar [logistic loss](../../../statistical-modelling.md#logistic-loss) $u\mapsto-u+\log(1+e^u)$ is strictly convex because its second derivative is $e^u/(1+e^u)^2>0$. If $\widehat\beta$ and $\widetilde\beta$ are minimizers but $X\widehat\beta\ne X\widetilde\beta$, strict convexity of the loss as a function of the fitted vector and convexity of the [L1 norm](../../../functional-analysis.md#l1-norm) make the objective at their midpoint strictly smaller than the common minimum. This contradiction proves that

$$
\boxed{X\widehat\beta=X\widetilde\beta}
$$

for every pair of solutions.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Part b shows that all solutions have the same fitted vector, hence the same score and the same set $E$. The KKT conditions show that every nonzero coordinate of any solution belongs to $E$, since a nonzero coefficient forces the corresponding score to have absolute value $\lambda$. Thus every solution is supported on $E$ and satisfies

$$
X_E\beta_E=X\widehat\beta.
$$

If $\operatorname{rank}(X_E)=|E|$, the linear map $u\mapsto X_Eu$ is injective. Consequently $\beta_E$ and hence $\beta$ are unique.

## 2

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For $s=|S|>0$, the [compatibility constant](../../../probability-and-statistics.md#compatibility-constant) in the convention used here is

$$
\boxed{\phi_{\widehat\Sigma}^2(S)
=s\inf\left\{\delta^T\widehat\Sigma\delta:
\lVert\delta_S\rVert_1=1,
\ \lVert\delta_{S^c}\rVert_1\leq3\right\}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $D$ be the block-diagonal part of $\widehat\Sigma=n^{-1}X^TX$. The within-block eigenvalue assumption gives $\delta^TD\delta\geq\eta\lVert\delta\rVert_2^2$. On the compatibility cone with $\lVert\delta_S\rVert_1=1$,

$$
\lVert\delta\rVert_1\leq4,
\qquad
\lVert\delta\rVert_2^2\geq\frac1s.
$$

The off-block assumption therefore gives

$$
\left|\delta^T(\widehat\Sigma-D)\delta\right|
\leq\frac{\eta}{32p}\lVert\delta\rVert_1^2
\leq\frac{\eta}{2p}
\leq\frac{\eta}{2s}.
$$

It follows that $\delta^T\widehat\Sigma\delta\geq\eta/(2s)$, and hence

$$
\boxed{\phi_{\widehat\Sigma}^2(S)\geq\eta/2}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Because $\lVert X_j\rVert_2=\sqrt n$, each coordinate of $X^T\varepsilon/n$ is $N(0,\sigma^2/n)$. The [Gaussian tail bound](../../../probability-and-statistics.md#gaussian-tail-bound) and a [union bound](../../../probability-inequality.md#boole-s-inequality) give

$$
\mathbb P\left(\left\lVert\frac{X^T\varepsilon}{n}\right\rVert_\infty>\frac\lambda2\right)
\leq2p\exp\left(-\frac{n\lambda^2}{8\sigma^2}\right)
=2p^{-(A^2/8-1)}.
$$

On the complementary score event, the standard [Basic inequality for the Lasso](../../../probability-and-statistics.md#basic-inequality-for-the-lasso), cone argument, and compatibility oracle inequality give, for $S=\operatorname{supp}(\beta^0)$,

$$
\frac1n\lVert X(\widehat\beta-\beta^0)\rVert_2^2
+\lambda\lVert\widehat\beta-\beta^0\rVert_1
\leq\frac{16\lambda^2s}{\phi_{\widehat\Sigma}^2(S)}.
$$

Using part b and $\lambda^2=A^2\sigma^2\log p/n$ proves

$$
\boxed{
\frac1n\lVert X(\widehat\beta-\beta^0)\rVert_2^2
+\lambda\lVert\widehat\beta-\beta^0\rVert_1
\leq\frac{32A^2\sigma^2\log p}{\eta}\frac{s}{n}}
$$

with the required probability.

## 3

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $u=0$ the assertion is immediate under the natural zero-vector convention. For $u\ne0$, the rows $a_r$ of $A$ are independent and $a_r^Tu/\lVert u\rVert_2$ is a centered unit-variance [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution). Its centered square is [sub-exponential](../../../probability-and-statistics.md#subexponential-distribution-light-tailed). The corresponding Bernstein estimate, in the explicit [Rademacher Johnson–Lindenstrauss transform](../../../functional-analysis.md#rademacher-johnson-lindenstrauss-transform) form, is

$$
\mathbb P\left(\left|\frac1d\sum_{r=1}^d
\frac{(a_r^Tu)^2}{\lVert u\rVert_2^2}-1\right|\geq t\right)
\leq2e^{-dt^2/136},
\qquad0<t<1.
$$

Since the sum in the event is $\lVert Au\rVert_2^2/\lVert u\rVert_2^2$, this is the claimed inequality.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Apply part a to each of the at most $n(n-1)/2$ nonzero differences $u_i-u_j$. For $w_i=Au_i/\sqrt d$, the [union bound](../../../probability-inequality.md#boole-s-inequality) makes the probability of any failure at most

$$
\frac{n(n-1)}2\,2e^{-dt^2/136}
<n^2e^{-dt^2/136}.
$$

The assumed inequality $d>272\log(n/\sqrt\varepsilon)/t^2$ makes this smaller than $\varepsilon$. Hence, simultaneously for every distinct pair,

$$
1-t\leq\frac{\lVert w_i-w_j\rVert_2^2}{\lVert u_i-u_j\rVert_2^2}\leq1+t
$$

with probability at least $1-\varepsilon$, which is the finite-set [Johnson–Lindenstrauss lemma](../../../functional-analysis.md#johnson-lindenstrauss-lemma).

## 4

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Regard each centered random variable $g(x)$ as a vector $h_x$ in the Hilbert space $L^2(\mathbb P)$. Then

$$
\operatorname{Var}(g(x)-g(x'))=\lVert h_x-h_{x'}\rVert_2^2,
$$

so $k$ is the [Gaussian kernel](../../../probability-and-statistics.md#gaussian-kernel) on the finite subset $\{h_x:x\in\mathcal X\}$ of that Hilbert space. More explicitly,

$$
k(x,x')=e^{-\lVert h_x\rVert^2/(2\eta^2)}e^{-\lVert h_{x'}\rVert^2/(2\eta^2)}
\sum_{m=0}^\infty\frac{\langle h_x,h_{x'}\rangle^m}{m!\eta^{2m}}.
$$

Every power of the inner-product kernel is [positive semidefinite](../../../probability-and-statistics.md#positive-semidefinite-kernel), and the [closure property of positive-semidefinite kernels](../../../probability-and-statistics.md#closure-property-of-positive-semidefinite-kernels) under nonnegative sums, pointwise limits, and multiplication by one-variable factors proves that $k$ is positive definite.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [kernel ridge regression](../../../probability-and-statistics.md#kernel-ridge-regression) estimator minimizes

$$
\sum_{i=1}^n\{y_i-f(x_i)\}^2+\lambda\lVert f\rVert_{\mathcal H}^2.
$$

By the [representer theorem](../../../probability-and-statistics.md#representer-theorem), its fitted-value vector is

$$
\widehat f=K(K+\lambda I)^{-1}y.
$$

Writing $f$ for the true value vector, the variance contribution to $\mathbb E\lVert f-\widehat f\rVert_2^2$ is

$$
\sigma^2\operatorname{tr}\{K^2(K+\lambda I)^{-2}\}
=\sigma^2\sum_{i=1}^n\frac{d_i^2}{(d_i+\lambda)^2}.
$$

The squared bias is $\lVert\lambda(K+\lambda I)^{-1}f\rVert_2^2$. In an orthonormal eigenbasis of $K$, the scalar inequality

$$
\frac{\lambda^2}{(d+\lambda)^2}\leq\frac{\lambda}{4d},
$$

which is equivalent to $4d\lambda\leq(d+\lambda)^2$, yields

$$
\boxed{
\mathbb E\sum_{i=1}^n\{f^0(x_i)-\widehat f_\lambda(x_i)\}^2
\leq\sigma^2\sum_{i=1}^n\frac{d_i^2}{(d_i+\lambda)^2}
+\frac\lambda4f^TK^{-1}f}.
$$

For $\lVert f\rVert_2=1$, only the last term varies. The [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) of $K^{-1}$ is maximized by a unit eigenvector associated with its largest eigenvalue $1/d_n$, equivalently an eigenvector of $K$ associated with $d_n$.

## 5

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the uncentered [sample covariance matrix](../../../variance.md#sample-covariance-matrix)

$$
\widehat\Sigma=\frac1n\sum_{i=1}^nx_ix_i^T,
\qquad
\widehat v_\ell=a_\ell^T\widehat\Sigma a_\ell.
$$

Then $v_\ell=a_\ell^T\Sigma a_\ell$ and, simultaneously for every unit vector $a_\ell$,

$$
|\widehat v_\ell-v_\ell|
\leq\lVert\widehat\Sigma-\Sigma\rVert_{\mathrm{op}}.
$$

Here $\lVert\Sigma\rVert_{\mathrm{op}}=1$ and the [effective rank of a covariance matrix](../../../variance.md#effective-rank-of-a-covariance-matrix) satisfies

$$
r(\Sigma)=\operatorname{tr}\Sigma=\sum_{j=1}^d\frac1j\leq1+\log d.
$$

The [Gaussian sample-covariance operator-norm bound](../../../variance.md#gaussian-sample-covariance-operator-norm-bound) therefore gives, with probability at least $1-e^{-\delta}$,

$$
\lVert\widehat\Sigma-\Sigma\rVert_{\mathrm{op}}
\leq C_0\left\{
\sqrt{\frac{\log d+1+\delta}{n}}
+\frac{\log d+1+\delta}{n}\right\}.
$$

Under the assumed upper bound on $\log d+1+\delta$, the second term is at most the first. Thus the stronger simultaneous estimate

$$
|\widehat v_\ell-v_\ell|
\leq C_1\sqrt{\frac{\log d+1+\delta}{n}}
$$

holds for every $\ell$. Squaring and using that the displayed ratio is at most one gives the inequality requested in the question after enlarging the universal constant $C$.

## 6

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Taking $\Theta=0$ gives $\lVert\Sigma\Theta-I\rVert_{\max}=1$, so every matrix is $1$-invertible. The smallest admissible value is

$$
\inf_\Theta\lVert\Sigma\Theta-I\rVert_{\max}.
$$

The map inside the norm is affine in $\Theta$, and a norm composed with an affine map is a [convex function](../../../real-analysis.md#convex-function). The space of matrices is a convex feasible set, so this is a [convex optimization](../../../convex-optimization.md) problem.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Put $\widehat\Sigma=X^TX/n$. Direct substitution of $Y=X\beta^0+\varepsilon$ into the [Debiased Lasso](../../../probability-and-statistics.md#debiased-lasso) gives

$$
\sqrt n(\widehat b-\beta^0)
=\underbrace{\frac1{\sqrt n}\widehat\Theta^TX^T\varepsilon}_{W}
+\underbrace{\sqrt n(I-\widehat\Theta^T\widehat\Sigma)(\widehat\beta-\beta^0)}_{\Delta}.
$$

Conditionally on the deterministic design,

$$
\boxed{W\sim N_p(0,\widehat\Theta^T\widehat\Sigma\widehat\Theta)}.
$$

The assumed [approximate inverse of a Gram matrix](../../../probability-and-statistics.md#approximate-inverse-of-a-gram-matrix) property and [Holder inequality](../../../functional-analysis.md#holder-inequality) imply

$$
\lVert\Delta\rVert_\infty
\leq\sqrt n\lVert I-\widehat\Theta^T\widehat\Sigma\rVert_{\max}
\lVert\widehat\beta-\beta^0\rVert_1
\leq\sqrt{\log p}\,\lVert\widehat\beta-\beta^0\rVert_1.
$$

**Thus $\rho(n,p)=\sqrt{\log p}$.**

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

A sufficient set of assumptions is: the columns of the deterministic designs have Euclidean norm at most $\sqrt n$; the true support has size $s$; the [compatibility constant](../../../probability-and-statistics.md#compatibility-constant) on that support is bounded below uniformly; $\log p=o(n)$; and $s\log p/\sqrt n\to0$. Choose $A$ large enough that the Gaussian score event

$$
\left\lVert X^T\varepsilon/n\right\rVert_\infty\leq\lambda/2
$$

has probability tending to one. The standard compatibility oracle inequality then gives

$$
\lVert\widehat\beta-\beta^0\rVert_1
=O_p\left(s\sqrt{\frac{\log p}{n}}\right).
$$

Part b consequently yields

$$
\lVert\Delta\rVert_\infty
=O_p\left(\frac{s\log p}{\sqrt n}\right).
$$

Equivalently, for a sufficiently large constant $c$,

$$
\mathbb P\left(\lVert\Delta\rVert_\infty>\frac{cs\log p}{\sqrt n}\right)\longrightarrow0.
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
