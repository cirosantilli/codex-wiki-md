# Paper 205

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_205.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_205.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
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

## 1

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [convex function](../../../real-analysis.md#convex-function) $f:\mathbb R^d\to\mathbb R$, its [subdifferential](../../../convex-optimization.md#subdifferential) at $x$ is

$$
\partial f(x)=\{g\in\mathbb R^d:f(y)\geq f(x)+g^T(y-x)\text{ for every }y\in\mathbb R^d\}.
$$

Its elements are the subgradients of $f$ at $x$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Only the $k$th block can have nonzero subgradient coordinates. If $\beta^{(k)}\ne0$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) shows that the unique supporting vector is $\beta^{(k)}/\lVert\beta^{(k)}\rVert_2$. At zero, the defining inequality is $\lVert h\rVert_2\geq u^Th$ for every block vector $h$, which is equivalent to $\lVert u\rVert_2\leq1$. Thus

$$
\partial f_k(\beta)=
\begin{cases}
\{u:u^{(j)}=0\ (j\ne k),\ u^{(k)}=\beta^{(k)}/\lVert\beta^{(k)}\rVert_2\},&\beta^{(k)}\ne0,\\
\{u:u^{(j)}=0\ (j\ne k),\ \lVert u^{(k)}\rVert_2\leq1\},&\beta^{(k)}=0.
\end{cases}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The differentiable loss has gradient $X^T(X\beta-Y)/n$. The [subdifferential sum rule](../../../convex-optimization.md#subdifferential-sum-rule) and part (b) give

$$
\partial Q(\beta)=\frac1nX^T(X\beta-Y)+\lambda\sqrt m\,u,
$$

where blockwise

$$
\boxed{u^{(k)}=\frac{\beta^{(k)}}{\lVert\beta^{(k)}\rVert_2}
\quad\text{if }\beta^{(k)}\ne0,
\qquad
\lVert u^{(k)}\rVert_2\leq1
\quad\text{if }\beta^{(k)}=0.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Suppose $\widehat\beta_1$ and $\widehat\beta_2$ minimize $Q$. Their midpoint is also a minimizer because $Q$ is a [convex function](../../../real-analysis.md#convex-function). The group penalty is convex, while the squared Euclidean norm is strictly convex in the fitted value. If $X\widehat\beta_1\ne X\widehat\beta_2$, strict convexity would make the midpoint objective strictly smaller than the minimum. Hence $X\widehat\beta_1=X\widehat\beta_2$, so the fitted values are unique.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Part (d) makes the residual and therefore $\widehat\nu=X^T(Y-X\widehat\beta)$ unique, so $E$ is unique. The [Karush-Kuhn-Tucker conditions](../../../mathematical-optimization.md#karush-kuhn-tucker-conditions) from part (c) imply that every nonzero block satisfies $\lVert\widehat\nu^{(k)}\rVert_2=n\lambda\sqrt m$. Hence $\widehat\beta^{(k)}=0$ for $k\notin E$.

Any two minimizers have the same fitted value and vanish outside $E$. Their difference $h$ is therefore supported on $E$ and satisfies $\widetilde Xh_E=0$. If $\widetilde X$ has full column rank, then $h_E=0$, proving uniqueness of $\widehat\beta$.

## 2

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Optimality gives $Q(\widehat\beta)\leq Q(\beta^0)$. Substitute $Y=X\beta^0+\varepsilon$, expand both squared norms, and cancel $\lVert\varepsilon\rVert_2^2/(2n)$. Rearranging gives

$$
\frac1{2n}\lVert X(\beta^0-\widehat\beta)\rVert_2^2
\leq\frac1n\varepsilon^TX(\widehat\beta-\beta^0)
+\lambda(\lVert\beta^0\rVert_1-\lVert\widehat\beta\rVert_1).
$$

This exposes a factor-of-two typo in the paper: its requested display has $1/n$ rather than $1/(2n)$ on the left while leaving the right side unchanged. For the objective printed in the paper, the displayed inequality above is the correct basic inequality. Part (b) explicitly asks us to use the stronger stated version, so the subsequent argument proceeds from that requested premise.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $\delta=\widehat\beta-\beta^0$. Standard [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution) and Gaussian-product concentration gives, for $n>\log p$,

$$
\mathbb P\left(\left\lVert\frac1nX^T\varepsilon\right\rVert_\infty
>A\sigma v\sqrt{\frac{\log p}{n}}\right)
\leq2p\exp(-A^2\log p/8).
$$

Thus $A=4$ makes this probability at most $2/p$. On the complementary event, the basic inequality and [Holder inequality](../../../functional-analysis.md#holder-inequality) give

$$
\frac1n\lVert X\delta\rVert_2^2
\leq\lambda\bigl(\lVert\delta\rVert_1+
\lVert\beta^0\rVert_1-\lVert\widehat\beta\rVert_1\bigr).
$$

The parenthesis is at most $2\lVert\delta\rVert_1$ by the triangle inequality and at most $2\lVert\beta^0\rVert_1$ by $\lVert\delta\rVert_1\leq\lVert\widehat\beta\rVert_1+\lVert\beta^0\rVert_1$. Substituting $\lambda=A\sigma v\sqrt{\log p/n}$ proves $\Omega_1$, whose probability tends to one.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put $s=\lVert\widehat\beta\rVert_0+\lVert\beta^0\rVert_0$. Since $\delta$ has at most $s$ nonzero coordinates, $\lVert\delta\rVert_1^2\leq s\lVert\delta\rVert_2^2$. On $\Omega_2$,

$$
\delta^T\widehat\Sigma\delta
\geq\delta^T\Sigma^0\delta-
\lVert\widehat\Sigma-\Sigma^0\rVert_\infty\lVert\delta\rVert_1^2
\geq\frac\mu2\lVert\delta\rVert_2^2,
$$

where $\widehat\Sigma=X^TX/n$. Write $R=\delta^T\widehat\Sigma\delta$. On $\Omega_1$,

$$
R\leq2A\sigma v\sqrt{\frac{\log p}{n}}\lVert\delta\rVert_1
\leq2A\sigma v\sqrt{\frac{2s\log p}{\mu n}}\sqrt R.
$$

Squaring after division by $\sqrt R$ proves

$$
\boxed{\frac1n\lVert X(\beta^0-\widehat\beta)\rVert_2^2
\leq8A^2\sigma^2v^2\frac{s\log p}{\mu n}.}
$$

## 3

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A symmetric function $k:\mathcal X^2\to\mathbb R$ is a [positive-definite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) when $\sum_{i,j}a_ia_jk(x_i,x_j)\geq0$ for every finite set of points and real coefficients. A [Reproducing kernel Hilbert space](../../../probability-and-statistics.md#reproducing-kernel-hilbert-space) $\mathcal H$ is a Hilbert space of functions whose evaluation maps are continuous. Its reproducing kernel satisfies $k(x,\cdot)\in\mathcal H$ and $f(x)=\langle f,k(x,\cdot)\rangle_{\mathcal H}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $U$ be uniform on $[0,2\pi]$, and independently let $W$ have density

$$
p(w)=\frac1{2\cosh(\pi w/2)}.
$$

The supplied [Fourier transform](../../../analysis.md#fourier-transform) identity, after the change of Fourier convention, gives

$$
\mathbb E\cos(Wz)=\frac1{\cosh z}.
$$

Also $\mathbb E_U[\cos(a+U)\cos(b+U)]=\tfrac12\cos(a-b)$. Therefore

$$
\mathbb E[\cos(Wx+U)\cos(Wy+U)]
=\frac1{2\cosh(x-y)}=k(x,y),
$$

so one may take $c=1$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For any $x_1,\ldots,x_N$ and $a_1,\ldots,a_N$, part (b) and linearity of expectation give

$$
\sum_{i,j}a_ia_jk(x_i,x_j)
=\mathbb E\left[\left(\sum_i a_i\cos(Wx_i+U)\right)^2\right]\geq0.
$$

Symmetry is immediate, so $k$ is a positive-definite kernel.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

On a grid $G\subset[-L,L]$ with mesh proportional to $\varepsilon$, [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) and a union bound give

$$
\mathbb P\left(\max_{x,y\in G}|k(x,y)-\phi(x)^T\phi(y)|>\varepsilon/2\right)
\leq C\frac{L^2}{\varepsilon^2}e^{-c\ell\varepsilon^2}.
$$

The density of $W$ has exponential tails. A [Chernoff bound](../../../probability-inequality.md#chernoff-bound) therefore shows that $\ell^{-1}\sum_i|W_i|$ is bounded by an absolute constant except on an event of probability $e^{-c'\ell}$. On that event, both the empirical kernel and $k$ are uniformly Lipschitz, so every pair $(x,y)$ is approximated by its nearest grid pair with total error at most $\varepsilon/2$. Enlarging constants and using $0<\varepsilon\leq1$ yields

$$
\boxed{\mathbb P\left(\sup_{x,y\in[-L,L]}|k(x,y)-\phi(x)^T\phi(y)|\geq\varepsilon\right)
\leq\frac{C_1L^2}{\varepsilon^2}e^{-C_2\ell\varepsilon^2}.}
$$

## 4

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A [p-value](../../../statistical-modelling.md#p-value) $p_i$ for $H_i$ is super-uniform under that null: $\mathbb P_{H_i}(p_i\leq u)\leq u$ for every $u\in[0,1]$. For the [Benjamini-Hochberg procedure](../../../statistical-modelling.md#benjamini-hochberg-procedure), order $p_{(1)}\leq\cdots\leq p_{(m)}$, set

$$
\widehat k=\max\{k:p_{(k)}\leq\alpha k/m\},
$$

with $\widehat k=0$ if the set is empty, and reject the hypotheses whose p-values are at most $p_{(\widehat k)}$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $R$ be the number of rejections and $I_0$ the true-null indices. For $i\in I_0$, remove $p_i$ and let $R_i$ be the number determined by the corresponding leave-one-out step-up rule. On $\{i\text{ rejected},R=r\}$ one has $p_i\leq\alpha r/m$ and $R_i=r$, while $R_i$ is independent of $p_i$. Hence super-uniformity gives

$$
\mathbb E\frac{\mathbf1_{\{i\text{ rejected}\}}}{R\vee1}
\leq\frac\alpha m.
$$

Summing over $i\in I_0$ proves that the [false discovery rate](../../../statistical-modelling.md#false-discovery-rate) is at most $|I_0|\alpha/m\leq\alpha$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Under the intersection null, every rejection is false, so the false-discovery proportion is $\mathbf1_{\{R>0\}}$ and its expectation is the [familywise error rate](../../../statistical-modelling.md#familywise-error-rate). Because the p-values are independent and exactly uniform, every super-uniform inequality in part (b) is an equality. Here $|I_0|=m$, and therefore

$$
\mathbb P(R>0)=\operatorname{FDR}=\alpha.
$$

Equivalently, the order-statistic identity in the hint gives the same equality by induction on $m$.

## 5

↑ **Parent:** [Paper 205](paper-205.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [ridge regression](../../../linear-regression.md#ridge-regression) estimator minimizes

$$
\lVert Y-X\beta\rVert_2^2+\lambda\lVert\beta\rVert_2^2.
$$

Its gradient vanishes exactly when $(X^TX+\lambda I)\beta=X^TY$. Since $\lambda>0$ makes this matrix positive definite,

$$
\boxed{\widehat\beta_\lambda=(X^TX+\lambda I)^{-1}X^TY.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use a [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) $X=UDV^T$. Then

$$
(X^TX+\lambda I)^{-1}X^T
=V(D^TD+\lambda I)^{-1}D^TU^T.
$$

Each nonzero singular value $d$ contributes $d/(d^2+\lambda)\to d^{-1}$, while each zero one contributes zero. Thus

$$
\lim_{\lambda\downarrow0}\widehat\beta_\lambda
=VD^+U^TY=(X^TX)^+X^TY,
$$

using the [Moore-Penrose inverse](../../../linear-algebra.md#moore-penrose-inverse).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Put $Z=[X,W]$. Its ridgeless minimum-norm fit is $Z^T(ZZ^T)^+Y$, so its first $p$ coordinates are

$$
\widetilde\beta_{1:p}=X^T(XX^T+WW^T)^+Y.
$$

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) applied entrywise gives $WW^T\to\lambda I_n$ almost surely as $d\to\infty$. Continuity of inversion then yields

$$
\widetilde\beta_{1:p}\longrightarrow
X^T(XX^T+\lambda I_n)^{-1}Y
=(X^TX+\lambda I_p)^{-1}X^TY=\widehat\beta_\lambda
$$

almost surely, where the middle equality is the [push-through identity](../../../linear-algebra.md#push-through-identity).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Because $x_*\sim N_p(0,I)$ is independent, conditional prediction risk equals $\mathbb E(\lVert\widehat\beta_\lambda-\beta^0\rVert_2^2\mid X)$. With $\widehat\Sigma=X^TX/n$ and $\lambda=n\ell$,

$$
\widehat\beta_\lambda-\beta^0
=-\ell(\widehat\Sigma+\ell I)^{-1}\beta^0
+\frac1n(\widehat\Sigma+\ell I)^{-1}X^T\varepsilon.
$$

The noise term has conditional mean zero and covariance $\frac{\sigma^2}{n}\,(\widehat\Sigma+\ell I)^{-1}\widehat\Sigma(\widehat\Sigma+\ell I)^{-1}$. Taking squared norms proves

$$
\boxed{R_X(\widehat\beta_\lambda)=
\ell^2(\beta^0)^T(\widehat\Sigma+\ell I)^{-2}\beta^0
+\frac{\sigma^2}{n}\operatorname{tr}\bigl(\widehat\Sigma(\widehat\Sigma+\ell I)^{-2}\bigr).}
$$

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Apply the stated deterministic equivalent for the squared resolvent with $\Theta_p=\beta^0(\beta^0)^T/r^2$. The bias term tends to $-\ell^2r^2m'(\ell)$. For the variance use

$$
\widehat\Sigma(\widehat\Sigma+\ell I)^{-2}
=(\widehat\Sigma+\ell I)^{-1}-\ell(\widehat\Sigma+\ell I)^{-2}.
$$

Normalized traces and $p/n\to\gamma$ therefore give

$$
R_X(\widehat\beta_\lambda)
\xrightarrow{\mathrm{a.s.}}
-\ell^2r^2m'(\ell)+\sigma^2\gamma\bigl(m(\ell)+\ell m'(\ell)\bigr).
$$

Thus the conclusion printed in the paper also has both signs involving $m'$ reversed. The hypotheses as printed imply the formula above; they cannot imply the requested one because $(\widehat\Sigma+\ell I)^{-2}$ is positive definite while $m'(\ell)\leq0$ for a resolvent limit.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
