# Paper 225

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_225.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_225.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The kernel is the [Brownian bridge covariance kernel](../../../random-variable.md#brownian-bridge-covariance-kernel). If $C_X\phi=\lambda\phi$, differentiating the integral equation twice gives

$$
\lambda\phi''(t)=-\phi(t),\qquad \phi(0)=\phi(1)=0.
$$

The normalized solutions and eigenvalues are therefore

$$
\boxed{\phi_k(t)=\sqrt2\sin(k\pi t),\qquad
\lambda_k=\frac1{k^2\pi^2}},\qquad k\geq1.
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $V=(X_1(t_1),X_1(t_2))^T$. The [Karhunen–Loève expansion](../../../statistical-modelling.md#karhunen-loeve-expansion) and Gaussianity give

$$
\operatorname{Cov}(a_{1k},V)
=\lambda_k(\phi_k(t_1),\phi_k(t_2))
$$

and

$$
\operatorname{Cov}(V)=
\Sigma=
\begin{pmatrix}
c_X(t_1,t_1)&c_X(t_1,t_2)\\
c_X(t_2,t_1)&c_X(t_2,t_2)
\end{pmatrix}.
$$

The [conditional multivariate normal distribution](../../../probability-and-statistics.md#conditional-multivariate-normal-distribution) formula yields

$$
\boxed{
\mathbb E[a_{1k}\mid X_1(t_1),X_1(t_2)]
=\lambda_k(\phi_k(t_1),\phi_k(t_2))
\Sigma^{-1}
\begin{pmatrix}X_1(t_1)\\X_1(t_2)\end{pmatrix}}.
$$

If $\Sigma$ is singular, the same formula uses its Moore-Penrose pseudoinverse.

## 2

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let

$$
\overline C=\frac12(C_X+C_{X^*}),
\qquad
\overline C\phi_k=\lambda_k\phi_k,
$$

and estimate it by the average of the two within-sample [empirical covariance operators](../../../random-variable.md#empirical-covariance-operator). Let $(\widehat\lambda_k,\widehat\phi_k)$ be its leading empirical eigenpairs and let $\overline X_n,\overline X_n^*$ be the sample means. Use the [Two-sample FPCA mean statistic](../../../statistical-modelling.md#two-sample-fpca-mean-statistic)

$$
\boxed{
T_{n,K}=\frac n2\sum_{k=1}^K
\frac{\langle\overline X_n-\overline X_n^*,\widehat\phi_k\rangle^2}
{\widehat\lambda_k}}.
$$

Under $H_0$, the [Hilbert-space central limit theorem](../../../convergence-of-random-variables.md#hilbert-space-central-limit-theorem) gives

$$
\sqrt{\frac n2}(\overline X_n-\overline X_n^*)
\xrightarrow dG,
$$

where $G$ is a centered [Gaussian random element](../../../random-variable.md#gaussian-random-element) with covariance $\overline C$. Distinct eigenvalues give consistent empirical eigenpairs, up to signs, and the standardized leading scores are independent standard normal variables. Hence

$$
T_{n,K}\xrightarrow d\chi_K^2.
$$

Rejecting above the $(1-\alpha)$ quantile gives an asymptotic level-$\alpha$ test.

Under a fixed alternative $\delta=\mu-\mu^*$,

$$
\frac{T_{n,K}}n\xrightarrow p
\frac12\sum_{k=1}^K\frac{\langle\delta,\phi_k\rangle^2}{\lambda_k}.
$$

The test is consistent whenever one retained projection is nonzero. Alternatives orthogonal to the first $K$ eigenfunctions are invisible at fixed $K$. Under local alternatives $\delta=h/\sqrt n$, the limit is noncentral chi-squared with noncentrality $\frac12\sum_{k\leq K}\langle h,\phi_k\rangle^2/\lambda_k$.

## 3

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [square-root distance between covariance operators](../../../statistical-modelling.md#square-root-distance-between-covariance-operators) is

$$
d_R(C_1,C_2)=\lVert C_1^{1/2}-C_2^{1/2}\rVert_{\rm HS}.
$$

Writing $A_i=C_i^{1/2}$, minimizing $\sum_i\lVert A_i-A\rVert_{\rm HS}^2$ gives $A=n^{-1}\sum_iA_i$. Since this average is positive,

$$
\boxed{\widehat C_R=
\left(\frac1n\sum_{i=1}^nC_i^{1/2}\right)^2},
$$

the [square-root barycenter of covariance operators](../../../statistical-modelling.md#square-root-barycenter-of-covariance-operators).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Because $C_i=L_iL_i^*$ is a covariance operator,

$$
\lVert L_i\rVert_{\rm HS}^2
=\operatorname{tr}(L_iL_i^*)=\operatorname{tr}C_i<\infty.
$$

Thus both factors are [Hilbert-Schmidt](../../../compact-operator.md#hilbert-schmidt-operator). The product of two Hilbert-Schmidt operators is a [trace-class operator](../../../compact-operator.md#trace-class-operator), with

$$
\boxed{\lVert L_2^*L_1\rVert_1
\leq\lVert L_2\rVert_{\rm HS}\lVert L_1\rVert_{\rm HS}<\infty.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [Procrustes distance between covariance operators](../../../statistical-modelling.md#procrustes-distance-between-covariance-operators) is

$$
d_P(C_1,C_2)=\inf_{R\ {\rm unitary}}
\lVert L_1-L_2R\rVert_{\rm HS}.
$$

For unitary $R$,

$$
\lVert L_1-L_2R\rVert_{\rm HS}^2
=\lVert L_1\rVert_{\rm HS}^2+\lVert L_2\rVert_{\rm HS}^2
-2\operatorname{Re}\operatorname{tr}(R^*L_2^*L_1).
$$

The [polar decomposition of a bounded operator](../../../banach-algebra.md#polar-decomposition-of-a-bounded-operator) implies

$$
\sup_R\operatorname{Re}\operatorname{tr}(R^*L_2^*L_1)
=\lVert L_2^*L_1\rVert_1=\sum_{k=1}^\infty\sigma_k.
$$

Therefore

$$
\boxed{d_P(C_1,C_2)^2
=\lVert L_1\rVert_{\rm HS}^2+\lVert L_2\rVert_{\rm HS}^2
-2\sum_{k=1}^\infty\sigma_k}.
$$

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The common eigenbasis gives

$$
C_1^{1/2}\phi_k=\sqrt{\lambda_k}\phi_k,\qquad
C_2^{1/2}\phi_k=\sqrt{\lambda_k^*}\phi_k.
$$

Consequently

$$
\boxed{d_R(C_1,C_2)^2
=\sum_{k=1}^\infty(\sqrt{\lambda_k}-\sqrt{\lambda_k^*})^2}.
$$

For the positive square-root factors, the singular values of $C_2^{1/2}C_1^{1/2}$ are $\sqrt{\lambda_k\lambda_k^*}$, so

$$
d_P(C_1,C_2)^2
=\sum_k\lambda_k+\sum_k\lambda_k^*
-2\sum_k\sqrt{\lambda_k\lambda_k^*}
=d_R(C_1,C_2)^2.
$$

**Thus the distances coincide when the covariance operators commute and share an eigenbasis.**

## 4

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $B$ be the integral operator with kernel $\beta$. Since $Y=BX+\varepsilon$ and the centered error is independent of $X$,

$$
\mathbb E[a_kb_l]
=\mathbb E\!\left[a_k\langle BX,u_l\rangle\right].
$$

Writing $\beta_{lk}=\langle B\phi_k,u_l\rangle$ and using $\mathbb E[a_ka_j]=\lambda_k\mathbf1_{\{j=k\}}$ gives

$$
\mathbb E[a_kb_l]=\lambda_k\beta_{lk}.
$$

Expanding the [function-on-function linear model](../../../statistical-modelling.md#function-on-function-linear-model) kernel in the product basis therefore yields

$$
\boxed{\beta(t,s)=
\sum_{k=1}^\infty\sum_{l=1}^\infty
\frac{\mathbb E[a_kb_l]}{\lambda_k}\phi_k(s)u_l(t)}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Replacing $\phi_k$ by $-\phi_k$ also replaces $a_k$ by $-a_k$, so both $\mathbb E[a_kb_l]$ and $\phi_k(s)$ change sign and their product is unchanged. Replacing $u_l$ by $-u_l$ similarly replaces $b_l$ by $-b_l$. Every summand, and hence $\beta$, is independent of all eigenfunction sign choices.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Applying the regression operator from part i gives

$$
\mathbb E[Y(t)\mid X]
=\sum_{k=1}^\infty a_k
\left\{\sum_{l=1}^\infty
\frac{\mathbb E[a_kb_l]}{\lambda_k}u_l(t)\right\}.
$$

The uncorrelated scores satisfy $\operatorname{Var}(a_k)=\lambda_k$, while $\operatorname{Var}(Y(t))=\sum_l\gamma_lu_l(t)^2$. Hence

$$
\boxed{
R(t)=
\frac{\displaystyle
\sum_{k=1}^\infty\frac1{\lambda_k}
\left(\sum_{l=1}^\infty\mathbb E[a_kb_l]u_l(t)\right)^2}
{\displaystyle\sum_{l=1}^\infty\gamma_lu_l(t)^2}}.
$$

The sign cancellations from part ii leave every squared numerator term unchanged; changing the sign of $u_l$ also leaves each denominator term unchanged. Thus $R(t)$ is sign invariant.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
