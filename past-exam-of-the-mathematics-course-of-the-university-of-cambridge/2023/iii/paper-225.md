# Paper 225

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_225.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_225.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Karhunen–Loève expansion](../../../statistical-modelling.md#karhunen-loeve-expansion) has the following Hilbert-space form. Let $X$ be a square-integrable [Random element of a Hilbert space](../../../random-variable.md#hilbert-space-valued-random-variable) $H$, with mean $\mu$ and [covariance operator](../../../random-variable.md#covariance-operator) $C$. There are nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_1\geq\lambda_2\geq\cdots$ and orthonormal [eigenvectors](../../../linear-operator-theory.md#eigenvector) $\phi_k$ spanning the closure of the range of $C$ such that

$$
C\phi_k=\lambda_k\phi_k,
\qquad
X=\mu+\sum_{k\geq1}\xi_k\phi_k
$$

in $L^2(\Omega;H)$. The [functional principal component scores](../../../statistical-modelling.md#functional-principal-component-score)

$$
\xi_k=\langle X-\mu,\phi_k\rangle
$$

satisfy

$$
\mathbb E\xi_k=0,
\qquad
\mathbb E[\xi_j\xi_k]=\lambda_k\mathbf1_{\{j=k\}}.
$$

If $X$ is a [Gaussian random element](../../../random-variable.md#gaussian-random-element), the scores are independent normal random variables.

For the proof, $C$ is positive, self-adjoint, and [trace-class](../../../compact-operator.md#trace-class-operator), with

$$
\operatorname{tr}C=\mathbb E\lVert X-\mu\rVert^2<\infty.
$$

It is therefore [compact](../../../compact-operator.md), so the [spectral theorem for compact Hermitian operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) supplies the eigenpairs. Their score covariance is

$$
\mathbb E[\xi_j\xi_k]
=\langle C\phi_j,\phi_k\rangle
=\lambda_j\langle\phi_j,\phi_k\rangle.
$$

For the residual $R_m=X-\mu-\sum_{k=1}^m\xi_k\phi_k$, [Parseval identity](../../../fourier-analysis.md#parseval-identity) and the trace formula give

$$
\mathbb E\lVert R_m\rVert^2
=\operatorname{tr}C-\sum_{k=1}^m\lambda_k
=\sum_{k>m}\lambda_k\longrightarrow0.
$$

The centered variable's projection onto $\ker C$ has zero second moment and is therefore zero almost surely, which completes the mean-square expansion. When $C$ has a continuous covariance kernel, [Mercer's theorem](../../../functional-analysis.md#mercer-s-theorem) additionally expands that kernel as $c(s,t)=\sum_k\lambda_k\phi_k(s)\phi_k(t)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The stated kernel is the [Brownian bridge covariance kernel](../../../random-variable.md#brownian-bridge-covariance-kernel). Its eigenvalue equation is

$$
\lambda\phi(s)=\int_0^1\{\min(s,t)-st\}\phi(t)\,dt.
$$

The right-hand side vanishes at $s=0$ and $s=1$, and differentiating it twice gives

$$
\lambda\phi''(s)=-\phi(s),
\qquad
\phi(0)=\phi(1)=0.
$$

Thus the normalized eigenfunctions and eigenvalues are

$$
\phi_k(t)=\sqrt2\sin(k\pi t),
\qquad
\lambda_k=\frac1{k^2\pi^2},
\qquad k\geq1.
$$

The [Karhunen–Loève expansion](../../../statistical-modelling.md#karhunen-loeve-expansion) is consequently

$$
X(t)=\mu(t)+\sum_{k=1}^{\infty}\xi_k\sqrt2\sin(k\pi t)
=\mu(t)+\sum_{k=1}^{\infty}\frac{Z_k}{k\pi}\sqrt2\sin(k\pi t),
$$

with convergence in $L^2(\Omega;L^2[0,1])$, where $\mathbb EZ_k=0$ and $\mathbb E[Z_jZ_k]=\mathbf1_{\{j=k\}}$. Covariance alone does not imply that the $Z_k$ are independent or normal; they are independent standard normal variables when $X$ is Gaussian.

## 2

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $(\lambda_j,\phi_j)$ be the ordered eigenpairs of the common [covariance operator](../../../random-variable.md#covariance-operator) $C_X$, and write $\delta=\mu-\mu^*$. Estimate $C_X$ by the [pooled covariance operator](../../../random-variable.md#pooled-covariance-operator)

$$
\widehat C
=\frac1{2n}\sum_{i=1}^n\left[
(X_i-\overline X)\otimes(X_i-\overline X)
+(X_i^*-\overline X^*)\otimes(X_i^*-\overline X^*)
\right]
$$

and denote its first $K$ eigenpairs by $(\widehat\lambda_j,\widehat\phi_j)$. The sign ambiguity of each eigenfunction disappears after squaring. Consider the [Two-sample FPCA mean statistic](../../../statistical-modelling.md#two-sample-fpca-mean-statistic)

$$
T_{n,K}=\frac n2\sum_{j=1}^K
\frac{\langle\overline X-\overline X^*,\widehat\phi_j\rangle^2}
{\widehat\lambda_j}.
$$

Under $H_0$, the [Hilbert-space central limit theorem](../../../convergence-of-random-variables.md#hilbert-space-central-limit-theorem) gives

$$
\sqrt{\frac n2}(\overline X-\overline X^*)
\xrightarrow{d}G,
$$

where $G$ is a centered [Gaussian random element](../../../random-variable.md#gaussian-random-element) with covariance $C_X$. The assumed eigenvalue gaps give consistency of the estimated eigenvalues and eigenfunctions, so [Slutsky's theorem](../../../statistical-inference.md#slutsky-theorem) yields

$$
T_{n,K}\xrightarrow{d}\sum_{j=1}^K
\frac{\langle G,\phi_j\rangle^2}{\lambda_j}
\sim\chi_K^2.
$$

An asymptotic level-$\alpha$ test therefore rejects when $T_{n,K}$ exceeds the $(1-\alpha)$-quantile of the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $K$ degrees of freedom.

Under a fixed alternative,

$$
\frac{T_{n,K}}n\xrightarrow{p}
\frac12\sum_{j=1}^K\frac{\langle\delta,\phi_j\rangle^2}{\lambda_j}.
$$

The test is consequently consistent whenever the mean difference has a nonzero projection onto one of the retained principal components. A difference orthogonal to their span is invisible to this fixed-$K$ test, so $\mu\ne\mu^*$ alone does not guarantee consistency. Increasing $K$ with $n$ can recover such alternatives, but requires additional eigenvalue and approximation control.

## 3

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Because a strictly monotone map fixing both endpoints is increasing, the [change of variables formula](../../../calculus.md#change-of-variables-formula) $t=h(s)$ gives

$$
\lVert Y\rVert^2
=\int_0^1X(h^{-1}(t))^2\,dt
=\int_0^1X(s)^2h'(s)\,ds.
$$

Assuming $\mathbb E\lVert X\rVert^2>0$, define

$$
A=\frac{\mathbb E\int_0^1X(s)^2h'(s)\,ds}
{\mathbb E\int_0^1X(s)^2\,ds}.
$$

The Hilbert-space variance identity then gives

$$
\begin{aligned}
\mathbb E\lVert Y-\mu\rVert^2
&=\mathbb E\lVert Y\rVert^2-\lVert\mu\rVert^2\\
&=A\mathbb E\lVert X\rVert^2-\lVert\mu\rVert^2\\
&=A\mathbb E\lVert X-\nu\rVert^2+A\lVert\nu\rVert^2-\lVert\mu\rVert^2.
\end{aligned}
$$

Under the regularity needed to interchange expectation and differentiation, $\mathbb Eh'(s)=1$ because $\mathbb Eh(s)=s$. Hence

$$
A=1+
\frac{\int_0^1\operatorname{Cov}(X(s)^2,h'(s))\,ds}
{\mathbb E\lVert X\rVert^2}.
$$

**Thus $A=1$ exactly when the integrated covariance in the numerator vanishes. In particular, this holds when the amplitude $X$ and the time warp $h$ are [independent random variables](../../../random-variable.md#independent-random-variables).**

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

For these increasing warps, the [square-root velocity function](../../../statistical-modelling.md#square-root-velocity-function) is $Q(h)(t)=\sqrt{h'(t)}$. The [chain rule](../../../calculus.md#chain-rule) gives

$$
Q(h_i\circ\gamma)(t)
=Q(h_i)(\gamma(t))\sqrt{\gamma'(t)}.
$$

Therefore

$$
\begin{aligned}
\lVert Q(h_i\circ\gamma)-Q(h_j\circ\gamma)\rVert_2^2
&=\int_0^1
|Q(h_i)(\gamma(t))-Q(h_j)(\gamma(t))|^2\gamma'(t)\,dt\\
&=\int_0^1|Q(h_i)(u)-Q(h_j)(u)|^2\,du,
\end{aligned}
$$

where the last equality again uses the [change of variables formula](../../../calculus.md#change-of-variables-formula). Taking square roots proves invariance under common right composition by $\gamma$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

For positive trace-class covariance operators $C_i=L_iL_i^*$, their [Procrustes distance between covariance operators](../../../statistical-modelling.md#procrustes-distance-between-covariance-operators) is

$$
d_P(C_1,C_2)
=\inf_{R\in\mathcal O(H)}\lVert L_1-L_2R\rVert_{\mathrm{HS}},
$$

where $\mathcal O(H)$ is the group of [unitary operators](../../../vector-space.md#unitary-operator) on the real Hilbert space $H=L^2[0,1]$. Expanding the square gives the equivalent formula

$$
\boxed{d_P(C_1,C_2)^2
=\lVert L_1\rVert_{\mathrm{HS}}^2+\lVert L_2\rVert_{\mathrm{HS}}^2
-2\sup_{R\in\mathcal O(H)}\operatorname{tr}(R^*L_2^*L_1).}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Convergence in the [Hilbert-Schmidt norm](../../../compact-operator.md#hilbert-schmidt-norm) implies

$$
\lVert L_i^p\rVert_{\mathrm{HS}}^2
\longrightarrow\lVert L_i\rVert_{\mathrm{HS}}^2.
$$

Products of two Hilbert-Schmidt operators are [trace-class operators](../../../compact-operator.md#trace-class-operator), and the [Schatten norm Hölder inequality](../../../compact-operator.md#schatten-norm-holder-inequality) gives

$$
\begin{aligned}
\lVert(L_2^p)^*L_1^p-L_2^*L_1\rVert_1
&\leq
\lVert L_2^p-L_2\rVert_{\mathrm{HS}}\lVert L_1^p\rVert_{\mathrm{HS}}\\
&\quad+\lVert L_2\rVert_{\mathrm{HS}}\lVert L_1^p-L_1\rVert_{\mathrm{HS}}
\longrightarrow0.
\end{aligned}
$$

By [trace duality](../../../compact-operator.md#trace-duality), every unitary $R$ satisfies

$$
\left|\operatorname{tr}\!\left(R^*\{(L_2^p)^*L_1^p-L_2^*L_1\}\right)\right|
\leq\lVert(L_2^p)^*L_1^p-L_2^*L_1\rVert_1.
$$

Taking the supremum over $R$ shows that the supremum terms in the two Procrustes formulas converge. Combining this with convergence of the squared norms proves

$$
\boxed{d_P(C_1^p,C_2^p)^2\longrightarrow d_P(C_1,C_2)^2.}
$$

## 4

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Put

$$
\xi_{ik}=\langle X_i,B_k\rangle,
\qquad
\beta_K=\sum_{k=1}^Kc_kB_k,
\qquad
r_i=\langle X_i,\beta-\beta_K\rangle.
$$

With the $n$ by $K$ [design matrix](../../../linear-regression.md#design-matrix) $\Xi=(\xi_{ik})$, the [scalar-on-function linear model](../../../statistical-modelling.md#scalar-on-function-linear-model) becomes

$$
Y=\Xi c+r+\varepsilon.
$$

The [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimator based on the truncated model is

$$
\widehat c=(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}Y
=c+(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}r
+(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}\varepsilon.
$$

Thus the omitted tail produces the conditional bias $(\Xi^{\mathsf T}\Xi)^{-1}\Xi^{\mathsf T}r$.

Let

$$
\Sigma_{jk}=\mathbb E[\xi_{1j}\xi_{1k}]
=\langle C_XB_j,B_k\rangle,
\qquad
g_j=\mathbb E[\xi_{1j}r_1]
=\langle C_XB_j,\beta-\beta_K\rangle.
$$

The supplied [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) and noise limit give

$$
\widehat c\xrightarrow{p}c+\Sigma^{-1}g.
$$

For a general fixed basis, $g$ need not vanish, so the retained coefficients are asymptotically biased and the estimator is inconsistent even for $c$. Moreover, with fixed $K$ it cannot recover the full slope $\beta$ when $\beta-\beta_K\ne0$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

If the $B_k$ form the [eigenbasis](../../../linear-operator-theory.md#eigenbasis) of $C_X$, then

$$
\langle C_XB_j,B_\ell\rangle
=\lambda_j\mathbf1_{\{j=\ell\}}.
$$

The retained [functional principal component scores](../../../statistical-modelling.md#functional-principal-component-score) are therefore uncorrelated with every omitted score, so $g=0$. The least-squares estimates of $c_1,\ldots,c_K$ are consistent despite truncation. Fixed $K$ still estimates only the projection $\beta_K$; consistency for the complete function requires the truncation level to increase and the tail error to vanish.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $\Xi_{ik}=\langle X_i,B_k\rangle$ and define the [roughness penalty matrix](../../../statistical-modelling.md#roughness-penalty-matrix)

$$
\Omega_{jk}=\langle B_j'',B_k''\rangle
=\int_0^1B_j''(t)B_k''(t)\,dt.
$$

For $c=(c_1,\ldots,c_K)^{\mathsf T}$, the loss is the quadratic function

$$
L(c)=\lVert Y-\Xi c\rVert_2^2+\rho c^{\mathsf T}\Omega c.
$$

Its [normal equations](../../../statistical-modelling.md#normal-equation) are

$$
(\Xi^{\mathsf T}\Xi+\rho\Omega)c=\Xi^{\mathsf T}Y.
$$

Whenever $\Xi^{\mathsf T}\Xi+\rho\Omega$ is positive definite, the unique minimizer is

$$
\widehat c
=(\Xi^{\mathsf T}\Xi+\rho\Omega)^{-1}\Xi^{\mathsf T}Y,
\qquad
\widehat\beta(t)=\sum_{k=1}^K\widehat c_kB_k(t).
$$

For the usual choice $\rho\geq0$, the penalty matrix is positive semidefinite, so full column rank of $\Xi$ suffices. Since the question permits arbitrary real $\rho$, a sufficiently negative value can make the quadratic form indefinite; then the loss is unbounded below and no minimizer exists. In the singular positive-semidefinite case, the [Moore-Penrose inverse](../../../linear-algebra.md#moore-penrose-inverse) describes the minimum-norm solution whenever the normal equations are consistent.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
