# Paper 326

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_326.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_326.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)

## 1

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take a minimizing sequence for the [variational regularization](../../../inverse-problem.md#variational-regularization) functional

$$
F(u)=\frac12\|Au-f\|_Y^2+\alpha J(u).
$$

Its [coercivity](../../../real-analysis.md#coercive-function) makes the sequence bounded. Since $X$ is a [reflexive Banach space](../../../functional-analysis.md#reflexive-banach-space), a subsequence converges weakly to some $u\in X$. A convex norm-lower-semicontinuous functional has [weak lower semicontinuity](../../../functional-analysis.md#weak-lower-semicontinuity), so this applies to both $J$ and the convex continuous map $u\mapsto\|Au-f\|_Y^2$. Therefore

$$
F(u)\leq\liminf_nF(u_n)=\inf_XF,
$$

and $u$ is a minimizer. This is the [direct method in the calculus of variations](../../../calculus-of-variations.md#direct-method-in-the-calculus-of-variations).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

An element $u^\dagger$ is a $J$-minimizing solution when

$$
Au^\dagger=f,
\qquad
J(u^\dagger)=\inf\{J(u):Au=f\}.
$$

It satisfies the [source condition in variational regularization](../../../inverse-problem.md#source-condition-in-variational-regularization) when there is a $w^\dagger\in Y^*$ such that

$$
\boxed{p^\dagger=A^*w^\dagger\in\partial J(u^\dagger)},
$$

where $\partial J(u^\dagger)$ is the [subdifferential](../../../convex-optimization.md#subdifferential) of the [convex functional](../../../real-analysis.md#convex-function) $J$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $\widehat u_\alpha$ minimize the nonsquared-residual objective. Comparison with $u^\dagger$ gives

$$
\|A\widehat u_\alpha-f\|_Y
+\alpha[J(\widehat u_\alpha)-J(u^\dagger)]\leq0.
$$

The source subgradient inequality gives

$$
J(\widehat u_\alpha)-J(u^\dagger)
\geq\langle w^\dagger,A\widehat u_\alpha-f\rangle.
$$

Consequently,

$$
0\geq
\|A\widehat u_\alpha-f\|_Y
+\alpha\langle w^\dagger,A\widehat u_\alpha-f\rangle
\geq
(1-\alpha\|w^\dagger\|_{Y^*})
\|A\widehat u_\alpha-f\|_Y.
$$

Thus for

$$
\boxed{\alpha_0=
\begin{cases}
\|w^\dagger\|_{Y^*}^{-1},&w^\dagger\ne0,\\
+\infty,&w^\dagger=0,
\end{cases}}
$$

every $0<\alpha<\alpha_0$ forces $A\widehat u_\alpha=f$. The original comparison then gives $J(\widehat u_\alpha)\leq J(u^\dagger)$, so $\widehat u_\alpha$ is itself $J$-minimizing. If $J$ is [strictly convex](../../../real-analysis.md#strictly-convex-function), its restriction to the affine solution set has at most one minimizer, hence $\widehat u_\alpha=u^\dagger$. This is an [exact penalty method](../../../inverse-problem.md#exact-penalty-method).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $p\in\partial J(v)$, the [Bregman divergence](../../../inverse-problem.md#bregman-divergence) is

$$
D_J^p(u,v)=J(u)-J(v)-\langle p,u-v\rangle.
$$

Put $r=A\widehat u_{\alpha,\delta}-f^\delta$ and $e=f^\delta-f$, so $\|e\|_Y\leq\delta$. Comparison with $u^\dagger$ gives

$$
\|r\|_Y+\alpha J(\widehat u_{\alpha,\delta})
\leq\delta+\alpha J(u^\dagger).
$$

Using $p^\dagger=A^*w^\dagger$,

$$
\begin{aligned}
D_J^{p^\dagger}(\widehat u_{\alpha,\delta},u^\dagger)
&=J(\widehat u_{\alpha,\delta})-J(u^\dagger)
-\langle w^\dagger,r+e\rangle\\
&\leq
\left(\frac1\alpha+\|w^\dagger\|_{Y^*}\right)\delta
+\left(\|w^\dagger\|_{Y^*}-\frac1\alpha\right)\|r\|_Y.
\end{aligned}
$$

For $0<\alpha<\alpha_0$ the last coefficient is negative, so

$$
\boxed{
D_J^{p^\dagger}(\widehat u_{\alpha,\delta},u^\dagger)
\leq C_\alpha\delta,
\qquad
C_\alpha=\frac1\alpha+\|w^\dagger\|_{Y^*}}.
$$

The estimate holds for any fixed admissible $\alpha$; it does not require $\alpha\to0$ with the noise level.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The exact solution is feasible because

$$
\|Au^\dagger-f^\delta\|_Y=\|f-f^\delta\|_Y\leq\delta\leq c\delta.
$$

The feasible set $E_\delta$ is convex and weakly closed. A minimizing sequence has bounded residual and bounded $J$; the coercivity assumption from part (a), applied to a fixed positive weighted objective, makes it bounded in $X$. Reflexivity gives a weakly convergent subsequence, and weak lower semicontinuity of the residual and $J$ keeps its limit feasible and minimizing.

Since $\widehat u_\delta$ minimizes $J$ over $E_\delta$,

$$
J(\widehat u_\delta)\leq J(u^\dagger).
$$

The [source condition in variational regularization](../../../inverse-problem.md#source-condition-in-variational-regularization) and feasibility then yield

$$
\begin{aligned}
D_J^{p^\dagger}(\widehat u_\delta,u^\dagger)
&\leq-\langle w^\dagger,A\widehat u_\delta-f\rangle\\
&\leq\|w^\dagger\|_{Y^*}
\left(\|A\widehat u_\delta-f^\delta\|_Y
+\|f^\delta-f\|_Y\right)\\
&\leq(c+1)\|w^\dagger\|_{Y^*}\delta.
\end{aligned}
$$

Thus the claimed constant is $\boxed{C=(c+1)\|w^\dagger\|_{Y^*}}$.

## 2

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The kernel $k(x,y)=e^{-|x-y|}$ is real and symmetric. For $f,g\in L^2[0,1]$, [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) gives

$$
\langle Kf,g\rangle
=\int_0^1\int_0^1k(x,y)f(y)\overline{g(x)}\,dy\,dx
=\langle f,Kg\rangle,
$$

so $K$ is self-adjoint. It is linear, and because $k\in L^2([0,1]^2)$ it is a [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator), hence bounded, with

$$
\boxed{\|K\|\leq\|k\|_{L^2([0,1]^2)}<\infty.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Suppose $Kf=\lambda f$. Differentiating the integral expression on the two sides of $y=x$ gives

$$
(Kf)''=Kf-2f,
\qquad
(Kf)'(0)=Kf(0),
\qquad
(Kf)'(1)=-Kf(1).
$$

Therefore

$$
f''=\frac{\lambda-2}{\lambda}f=-\omega^2f,
\qquad
f'(0)=f(0),
\qquad
f'(1)=-f(1).
$$

The first boundary condition makes

$$
f(x)=A\left(\cos(\omega x)+\frac1\omega\sin(\omega x)\right).
$$

Substitution into the second gives

$$
2\cos\omega+\left(\frac1\omega-\omega\right)\sin\omega=0,
$$

or

$$
\boxed{\frac{2\omega}{\omega^2-1}=\tan\omega},
\qquad
\boxed{-\omega^2=\frac{\lambda-2}{\lambda}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Extend $f$ by zero outside $[0,1]$. Since the [Fourier transform](../../../analysis.md#fourier-transform) of $e^{-|x|}$ is $2/(1+\xi^2)>0$,

$$
\langle Kf,f\rangle
=\frac1{2\pi}\int_{\mathbb R}
\frac{2}{1+\xi^2}|\widehat f(\xi)|^2\,d\xi>0
$$

for $f\ne0$. Thus every eigenvalue is positive. From the relation in part (b),

$$
\boxed{\lambda=\frac2{1+\omega^2}>0}.
$$

The transcendental equation has its successive roots in intervals separated by the poles and zeros of $\tan\omega$, so $\omega_n$ grows linearly with $n$. Hence

$$
\boxed{\lambda_n=\frac2{1+\omega_n^2}=O(n^{-2})}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The compact self-adjoint operator $K$ has an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of eigenvectors $e_n$. Part (c) gives $\lambda_n>0$ and $\sum_n\lambda_n<\infty$, so $K$ is positive and trace class, exactly the required condition for a [covariance operator of a Gaussian measure](../../../stochastic-process.md#covariance-operator-of-a-gaussian-measure) on a Hilbert space.

For independent standard normal variables $\xi_n$, define the [Hilbert-space Gaussian series](../../../stochastic-process.md#hilbert-space-gaussian-series)

$$
\boxed{
U=m+\sum_{n=1}^\infty\sqrt{\lambda_n}\,\xi_ne_n}.
$$

Because $\mathbb E\|U-m\|^2=\sum_n\lambda_n<\infty$, the series converges in $L^2(\Omega;X)$ and almost surely. Its law is the [Gaussian measure](../../../stochastic-process.md#gaussian-measure) $N(m,K)$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For observed $v\in\mathbb R^N$, the Gaussian likelihood is

$$
\boxed{
\pi(v\mid u)
=(2\pi\sigma^2)^{-N/2}
\exp\left[-\frac1{2\sigma^2}\|v-G(u)\|_{\mathbb R^N}^2\right]}.
$$

Thus the [Bayesian inverse problem](../../../stochastic-process.md#bayesian-inverse-problem) is to determine the posterior distribution of $U$ given $V=v$. With

$$
\Phi(u;v)=\frac1{2\sigma^2}\|v-G(u)\|^2,
$$

Bayes' formula gives

$$
\boxed{
\frac{d\mu^v}{d\mu_0}(u)
=\frac1{Z(v)}e^{-\Phi(u;v)},
\qquad
Z(v)=\int_Xe^{-\Phi(u;v)}\,d\mu_0(u)}.
$$

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

The [total variation distance](../../../probability-and-statistics.md#total-variation-distance) is

$$
d_{\rm TV}(\mu,\nu)=\sup_{B\in\mathcal B(X)}|\mu(B)-\nu(B)|.
$$

The problem is a [well-posed Bayesian inverse problem in total variation](../../../stochastic-process.md#well-posed-bayesian-inverse-problem-in-total-variation) when every $v\in\mathbb R^N$ determines a unique posterior $\mu^v$ and

$$
v_n\to v\quad\Longrightarrow\quad
d_{\rm TV}(\mu^{v_n},\mu^v)\to0.
$$

The heat solution operator at positive time is bounded from $L^2[0,1]$ to $C[0,1]$, so the finite sensor map $G:X\to\mathbb R^N$ is bounded and continuous. Therefore $\Phi(u;v)$ is jointly continuous and $0<e^{-\Phi}\leq1$. The normalizer satisfies $0<Z(v)\leq1$. If $v_n\to v$, the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives both

$$
Z(v_n)\to Z(v)
$$

and convergence in $L^1(\mu_0)$ of the normalized posterior densities. Since total variation is one half of this $L^1$ distance for absolutely continuous measures, $d_{\rm TV}(\mu^{v_n},\mu^v)\to0$. Existence, uniqueness, and continuous dependence all follow.

## 3

↑ **Parent:** [Paper 326](paper-326.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Hadamard well-posedness](../../../inverse-problem.md#well-posed-problem) requires existence, uniqueness, and continuous dependence of $u$ on $f$. A compact operator with infinite-dimensional range cannot have closed range: otherwise its inverse on the orthogonal complement of its kernel would be bounded, making the identity on an infinite-dimensional space compact. Hence the inverse on $\operatorname{ran}A$ is unbounded. If $\ker A\ne\{0\}$ uniqueness also fails, and data outside the range have no exact solution. In every case at least stability fails, so the inverse problem is ill posed.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

If $\|K\|<1$, the partial [Neumann series](../../../banach-algebra.md#neumann-series) satisfies

$$
(I-K)\sum_{n=0}^NK^n=I-K^{N+1}.
$$

Since $\|K^{N+1}\|\leq\|K\|^{N+1}\to0$, the series converges in operator norm and

$$
\boxed{(I-K)^{-1}=\sum_{n=0}^\infty K^n}.
$$

If $\tau\ne0$ and $\|I-\tau K\|<1$, apply this identity to $I-\tau K$:

$$
\tau K=I-(I-\tau K),
\qquad
\boxed{K^{-1}=\tau\sum_{n=0}^\infty(I-\tau K)^n}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [normal equation for a linear inverse problem](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) is

$$
\boxed{A^*Au=A^*f}.
$$

It has a solution exactly when

$$
f\in\operatorname{ran}A\oplus(\operatorname{ran}A)^\perp
=\operatorname{dom}(A^\dagger).
$$

When solutions exist they form

$$
A^\dagger f+\ker A.
$$

They are unique exactly when $\ker A=\{0\}$, while $A^\dagger f$ is always the unique solution in $(\ker A)^\perp$ and the solution of minimum norm. Here $A^\dagger$ is the [Moore-Penrose inverse](../../../linear-algebra.md#moore-penrose-inverse).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The operator $A^*A$ is positive, self-adjoint, and compact. Because $\operatorname{ran}A$ is infinite dimensional, the [spectral theorem for compact Hermitian operators](../../../compact-operator.md#spectral-theorem-for-compact-hermitian-operators) gives positive spectral values tending to zero. Even if $\ker A=\{0\}$, zero remains in the spectrum as a limit point. Hence for every $\tau$,

$$
\|I-\tau A^*A\|
=\sup_{\lambda\in\sigma(A^*A)}|1-\tau\lambda|
\geq1.
$$

The strict inequality $\|I-\tau K\|<1$ needed for the operator-norm [Neumann series](../../../banach-algebra.md#neumann-series) is impossible, so formula (3) cannot be applied directly to invert $A^*A$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $(\sigma_j,u_j,v_j)$ be a singular system for $A$. The [Picard criterion](../../../inverse-problem.md#picard-criterion) for $f\in\operatorname{dom}(A^\dagger)$ is

$$
\sum_j\frac{|\langle f,v_j\rangle|^2}{\sigma_j^2}<\infty
$$

after discarding the component in $(\operatorname{ran}A)^\perp$. For $0<\tau<\|A\|^{-2}$, the partial series acts diagonally:

$$
Q_Nf
=\sum_j
\frac{1-(1-\tau\sigma_j^2)^{N+1}}{\sigma_j}
\langle f,v_j\rangle u_j.
$$

For each $j$ the multiplier in the numerator tends to one and lies in $[0,1]$. The Picard summability condition therefore supplies an $\ell^2$ dominating sequence, so the [dominated convergence theorem](../../../measure-theory.md#dominated-convergence-theorem) gives

$$
\boxed{Q_Nf\longrightarrow
\sum_j\frac{\langle f,v_j\rangle}{\sigma_j}u_j
=A^\dagger f}.
$$

This is the series form of [Landweber iteration](../../../inverse-problem.md#landweber-iteration).

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

For $\alpha>0$, put $N(\alpha)=\lfloor\alpha^{-1}\rfloor$ and define the bounded operator

$$
R_\alpha
=\tau\sum_{n=0}^{N(\alpha)}
(I-\tau A^*A)^nA^*.
$$

Part (e) shows $R_\alpha f\to A^\dagger f$ for every $f\in\operatorname{dom}(A^\dagger)$ as $\alpha\downarrow0$. Since $\|I-\tau A^*A\|\leq1$,

$$
\|R_\alpha\|
\leq\tau(N(\alpha)+1)\|A\|.
$$

Choose the a priori rule

$$
\boxed{\alpha(\delta)=\sqrt\delta}.
$$

Then $N(\alpha(\delta))\to\infty$ while

$$
\delta\|R_{\alpha(\delta)}\|
\leq\tau\|A\|\delta(N(\alpha(\delta))+1)
\longrightarrow0.
$$

For $\|f^\delta-f\|\leq\delta$,

$$
\|R_{\alpha(\delta)}f^\delta-A^\dagger f\|
\leq
\delta\|R_{\alpha(\delta)}\|
+\|R_{\alpha(\delta)}f-A^\dagger f\|
\longrightarrow0.
$$

**Thus $\{R_\alpha\}$ with this parameter rule is a [regularization of an inverse problem](../../../inverse-problem.md#regularization-of-an-inverse-problem).**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
