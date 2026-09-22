# Paper 225

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_225.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_225.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
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
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

This is the [Brownian covariance kernel](../../../random-variable.md#brownian-covariance-kernel), so its integral operator is a [covariance operator](../../../random-variable.md#covariance-operator). To obtain its [eigendecomposition](../../../linear-operator-theory.md#spectral-decomposition), suppose $Uf=\lambda f$ with $\lambda\ne0$. Splitting the integral at $s$ gives

$$
\lambda f(s)=\int_0^s t f(t)dt+s\int_s^1f(t)dt.
$$

Differentiation yields $\lambda f'(s)=\int_s^1f(t)dt$ and $\lambda f''(s)=-f(s)$, with boundary conditions $f(0)=0$ and $f'(1)=0$. Hence the normalized eigenpairs are

$$
\phi_k(t)=\sqrt2\sin\!\left((k-\tfrac12)\pi t\right),
\qquad
\lambda_k=\frac1{(k-\tfrac12)^2\pi^2},
\qquad k\geq1.
$$

The eigenvalues are positive and summable, consistently with positivity and the [trace-class operator](../../../compact-operator.md#trace-class-operator) property of a covariance operator.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [identity operator](../../../vector-space.md#identity-operator) is positive and self-adjoint, but on the infinite-dimensional [Hilbert space](../../../hilbert-space.md) $L^2[0,1]$ it has eigenvalue one with infinite multiplicity. Consequently

$$
\operatorname{tr}I=\sum_{k=1}^{\infty}1=\infty.
$$

A square-integrable Hilbert-space random variable has a trace-class [covariance operator](../../../random-variable.md#covariance-operator) with trace $\mathbb E\lVert X\rVert^2<\infty$. The identity therefore cannot be such a covariance operator.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

This symmetric finite-rank [integral operator](../../../functional-analysis.md#integral-operator) is not positive. For $f(t)=1-\tfrac32t$, set $A_j=\int_0^1t^jf(t)dt$. Directly,

$$
A_0=\frac14,
\qquad
A_1=0,
\qquad
A_2=-\frac1{24}.
$$

The associated [quadratic form](../../../linear-algebra.md#quadratic-form) is

$$
\langle Uf,f\rangle
=\int_0^1\!\int_0^1(s+t)^2f(s)f(t)dsdt
=2A_0A_2+2A_1^2
=-\frac1{48}<0.
$$

Every [covariance operator](../../../random-variable.md#covariance-operator) is a [positive operator](../../../hilbert-space.md#positive-operator), so this operator is not a covariance operator.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $x\otimes y$ for the [rank-one operator](../../../compact-operator.md#rank-one-operator) $h\mapsto\langle h,y\rangle x$. The estimator is the kernel representation of the [empirical covariance operator](../../../random-variable.md#empirical-covariance-operator)

$$
\widehat C_{\mu_0}=\frac1n\sum_{i=1}^n(X_i-\mu_0)\otimes(X_i-\mu_0).
$$

Since $\mathbb EX=0$,

$$
\mathbb E\widehat C_{\mu_0}=C_X+\mu_0\otimes\mu_0.
$$

Thus the estimator has the fixed [bias of an estimator](../../../statistical-modelling.md#bias-of-an-estimator) $\mu_0\otimes\mu_0$ for $C_X$.

The fourth-moment assumption makes $(X_i-\mu_0)\otimes(X_i-\mu_0)$ square-integrable in the Hilbert space of [Hilbert-Schmidt operators](../../../compact-operator.md#hilbert-schmidt-operator). The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) therefore gives

$$
\widehat C_{\mu_0}\xrightarrow{p}C_X+\mu_0\otimes\mu_0.
$$

Consequently [consistency](../../../statistical-inference.md#consistency-statistics) for $C_X$ holds exactly when $\mu_0=0$. More precisely, if $Y=(X-\mu_0)\otimes(X-\mu_0)$, then

$$
\mathbb E\lVert\widehat C_{\mu_0}-C_X\rVert_{\mathrm{HS}}^2
=\lVert\mu_0\otimes\mu_0\rVert_{\mathrm{HS}}^2
+\frac1n\mathbb E\lVert Y-\mathbb EY\rVert_{\mathrm{HS}}^2
=\lVert\mu_0\rVert^4+O(n^{-1}).
$$

The [Hilbert-space central limit theorem](../../../convergence-of-random-variables.md#hilbert-space-central-limit-theorem) also yields

$$
\sqrt n\{\widehat C_{\mu_0}-(C_X+\mu_0\otimes\mu_0)\}
\xrightarrow dG,
$$

where $G$ is a centered [Gaussian random element](../../../random-variable.md#gaussian-random-element) in the Hilbert-Schmidt operator space with covariance determined by $Y$. Relative to $C_X$, the same fluctuation is displaced by $\sqrt n(\mu_0\otimes\mu_0)$ and hence does not have a finite centered limit when $\mu_0\ne0$.

## 2

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the [test statistic](../../../statistical-modelling.md#test-statistic)

$$
T_n=n\lVert\overline X_n\rVert^2,
\qquad
\overline X_n=\frac1n\sum_{i=1}^nX_i.
$$

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), the [Hilbert-space central limit theorem](../../../convergence-of-random-variables.md#hilbert-space-central-limit-theorem) gives $\sqrt n\,\overline X_n\xrightarrow dG$, where $G$ is centered Gaussian with covariance $C_X$. If $C_X\phi_j=\lambda_j\phi_j$, its [Karhunen–Loève expansion](../../../statistical-modelling.md#karhunen-loeve-expansion) and the [continuous mapping theorem](../../../convergence-of-random-variables.md#continuous-mapping-theorem) give

$$
T_n\xrightarrow d\lVert G\rVert^2
=\sum_{j\geq1}\lambda_jZ_j^2,
$$

for independent $Z_j\sim N(0,1)$. Reject for $T_n$ above the $(1-\alpha)$ quantile of this weighted chi-squared law; replacing the $\lambda_j$ by empirical covariance eigenvalues gives a [plug-in estimator](../../../statistical-inference.md#plug-in-estimator) of the critical value.

Under every [fixed alternative](../../../statistical-modelling.md#fixed-alternative) $\mu\ne0$, the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) gives $\overline X_n\xrightarrow p\mu$, so $T_n/n\xrightarrow p\lVert\mu\rVert^2$ and the test is consistent. Under a [local alternative](../../../statistical-modelling.md#local-alternative) $\mu_n=n^{-1/2}\delta$, the limit is $\lVert G+\delta\rVert^2$, which describes its local power.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $(\widehat\lambda_k,\widehat\phi_k)$ be the leading eigenpairs of the sample [covariance operator](../../../random-variable.md#covariance-operator). For fixed $K$ with $\lambda_1>\cdots>\lambda_K>\lambda_{K+1}$ and $\lambda_K>0$, the [FPCA mean test](../../../statistical-modelling.md#fpca-mean-test) uses

$$
T_{K,n}
=n\sum_{k=1}^K
\frac{\langle\overline X_n,\widehat\phi_k\rangle^2}
{\widehat\lambda_k}.
$$

Under the null, consistency of the empirical eigenpairs and the multivariate central limit theorem imply

$$
T_{K,n}\xrightarrow d\chi_K^2.
$$

The level-$\alpha$ test therefore rejects above the $(1-\alpha)$ quantile of the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $K$ degrees of freedom.

For a fixed mean $\mu$, if at least one leading coordinate $\langle\mu,\phi_k\rangle$, $k\leq K$, is nonzero, then $T_{K,n}\to\infty$ in probability and the test is consistent. It has only null-level asymptotic power against means orthogonal to the first $K$ principal component functions. Under $\mu_n=n^{-1/2}\delta$, the limit is noncentral chi-squared with noncentrality

$$
\boxed{\sum_{k=1}^K\frac{\langle\delta,\phi_k\rangle^2}{\lambda_k}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Assume the null distribution is a [centrally symmetric probability distribution](../../../probability-theory.md#centrally-symmetric-probability-distribution), so $X_i$ and $-X_i$ have the same law. A [sign-flip randomization test](../../../statistical-modelling.md#sign-flip-randomization-test) draws signs $s_i\in\{-1,1\}$ independently and recomputes, for example,

$$
T(s)=n\left\lVert\frac1n\sum_{i=1}^ns_iX_i\right\rVert^2.
$$

The exact p-value averages over all $2^n$ sign vectors:

$$
p=2^{-n}\#\{s:T(s)\geq T(1,\ldots,1)\}.
$$

With $B$ random sign vectors, including the observed configuration, the standard Monte Carlo version is $(1+\#\{b:T_b\geq T_0\})/(B+1)$, where $T_0$ is the observed statistic. Joint sign invariance under the null makes this finite-sample valid.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The squared-norm test is omnibus: every fixed nonzero mean eventually changes $\lVert\overline X_n\rVert$. Its null law, however, is an infinite weighted chi-squared distribution and requires accurate estimation of enough covariance eigenvalues; noisy low-variance directions can also make calibration inefficient.

The [FPCA mean test](../../../statistical-modelling.md#fpca-mean-test) has the simple $\chi_K^2$ limit and standardizes retained directions by their variances. It is effective when the signal lies in the leading principal component subspace, but choosing $K$ introduces a tuning decision and truncation makes the test blind to alternatives orthogonal to that subspace. Close or repeated eigenvalues also make individual empirical eigenfunctions unstable.

The [sign-flip randomization test](../../../statistical-modelling.md#sign-flip-randomization-test) can provide finite-sample calibration and avoids estimating a limiting covariance spectrum. Its exactness requires central symmetry, which is stronger than merely having zero mean, and exhaustive enumeration costs $2^n$ evaluations; Monte Carlo sign flips introduce simulation error. Its power still depends on the statistic used inside the randomization scheme.

## 3

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The minimizer is the arithmetic mean

$$
\overline C=\frac1n\sum_{k=1}^nC_k.
$$

It remains a positive self-adjoint trace-class operator and hence a [covariance operator](../../../random-variable.md#covariance-operator). The [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product) gives, for every Hilbert-Schmidt operator $C$,

$$
\sum_{k=1}^n\lVert C_k-C\rVert_{\mathrm{HS}}^2
=\sum_{k=1}^n\lVert C_k-\overline C\rVert_{\mathrm{HS}}^2
+n\lVert C-\overline C\rVert_{\mathrm{HS}}^2,
$$

because $\sum_k(C_k-\overline C)=0$. Thus $\overline C$ is the unique minimizer, including when the minimization is restricted to covariance operators.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For factorizations $C_i=L_iL_i^*$ and $C_j=L_jL_j^*$, the [Procrustes distance between covariance operators](../../../statistical-modelling.md#procrustes-distance-between-covariance-operators) is the following infimum over unitary operators $R$:

$$
d_P(C_i,C_j)=\inf_R\lVert L_i-L_jR\rVert_{\mathrm{HS}}.
$$

Unitary invariance of the Hilbert-Schmidt norm gives

$$
\lVert L_i-L_jR\rVert_{\mathrm{HS}}^2
=\lVert L_i\rVert_{\mathrm{HS}}^2+\lVert L_j\rVert_{\mathrm{HS}}^2
-2\operatorname{Re}\operatorname{tr}(L_i^*L_jR).
$$

The [polar decomposition of a bounded operator](../../../banach-algebra.md#polar-decomposition-of-a-bounded-operator) and trace duality imply

$$
\sup_R\operatorname{Re}\operatorname{tr}(L_i^*L_jR)
=\lVert L_j^*L_i\rVert_1
=\sum_{k=1}^{\infty}\sigma_k,
$$

where the last equality expresses the [trace norm](../../../functional-analysis.md#trace-norm) as the sum of the [singular values](../../../linear-algebra.md#singular-value). Taking the infimum proves

$$
\boxed{d_P(C_i,C_j)^2
=\lVert L_i\rVert_{\mathrm{HS}}^2+\lVert L_j\rVert_{\mathrm{HS}}^2-2\sum_{k=1}^{\infty}\sigma_k.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The two rank-one operators have orthogonal ranges. Their Hilbert-Schmidt inner product is zero, while $\lVert C_i\rVert_{\mathrm{HS}}=\lambda_i$, so the [Hilbert-Schmidt distance between covariance operators](../../../statistical-modelling.md#hilbert-schmidt-distance-between-covariance-operators) is

$$
d_L(C_1,C_2)=\sqrt{\lambda_1^2+\lambda_2^2}.
$$

For each $C_i$, the [positive square root of an operator](../../../hilbert-space.md#positive-square-root-of-an-operator) is $C_i^{1/2}=\sqrt{\lambda_i}\,e_i\otimes e_i$. Orthogonality therefore gives the [square-root distance between covariance operators](../../../statistical-modelling.md#square-root-distance-between-covariance-operators)

$$
d_R(C_1,C_2)=\sqrt{\lambda_1+\lambda_2}.
$$

Finally $C_2^{1/2}C_1^{1/2}=0$, so every singular value in the Procrustes cross-term vanishes. Hence

$$
\boxed{d_P(C_1,C_2)=\sqrt{\lambda_1+\lambda_2}.}
$$

## 4

↑ **Parent:** [Paper 225](paper-225.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $B$ be the [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator) with kernel $\beta$, so the [function-on-function linear model](../../../statistical-modelling.md#function-on-function-linear-model) is $Y=BX+\varepsilon$. Independence and centering give $\mathbb E[Y\mid X]=BX$. Let

$$
C_X\phi_j=\lambda_j\phi_j,
\qquad
C_Y\psi_k=\gamma_k\psi_k,
$$

and define the [functional principal component scores](../../../statistical-modelling.md#functional-principal-component-score)

$$
\xi_j=\langle X,\phi_j\rangle,
\qquad
\eta_k=\langle Y,\psi_k\rangle.
$$

The [cross-covariance operator](../../../statistical-modelling.md#cross-covariance-operator) identity $C_{YX}=BC_X$ gives, for every $\lambda_j>0$,

$$
\mathbb E[\eta_k\xi_j]
=\langle C_{YX}\phi_j,\psi_k\rangle
=\lambda_j\langle B\phi_j,\psi_k\rangle.
$$

Since $BX$ is centered, the requested integrated variance is $\mathbb E\lVert BX\rVert^2$. Applying the [Karhunen–Loève expansion](../../../statistical-modelling.md#karhunen-loeve-expansion) to $X$ and the [Parseval identity](../../../fourier-analysis.md#parseval-identity) in the $\psi_k$ basis yields

$$
\begin{aligned}
\int_0^1\operatorname{Var}(\mathbb E[Y(t)\mid X])dt
&=\mathbb E\lVert BX\rVert^2\\
&=\sum_{j:\lambda_j>0}\lambda_j\lVert B\phi_j\rVert^2\\
&=\sum_{j:\lambda_j>0}\sum_{k\geq1}
\frac{\{\mathbb E(\xi_j\eta_k)\}^2}{\lambda_j}.
\end{aligned}
$$

Equivalently, if $\rho_{jk}=\operatorname{Corr}(\xi_j,\eta_k)$, the expression is $\sum_k\gamma_k\sum_{j:\lambda_j>0}\rho_{jk}^2$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
