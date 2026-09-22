# Paper 210

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20210.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20210.pdf)

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
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a centered [random variable](../../../random-variable.md) $X$, being [sub-Poisson in the right tail](../../../probability-inequality.md#sub-poisson-random-variable-in-the-right-tail) with variance parameter $\sigma^2$ means

$$
\log\mathbb E e^{\lambda X}
\leq\sigma^2(e^\lambda-\lambda-1)
\qquad(\lambda\geq0).
$$

It is [sub-Gamma in the right tail](../../../probability-inequality.md#sub-gamma-random-variable-in-the-right-tail) with variance parameter $v$ and scale parameter $c$ when

$$
\boxed{\log\mathbb E e^{\lambda X}
\leq\frac{v\lambda^2}{2(1-c\lambda)}
\qquad(0\leq\lambda<c^{-1}).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $q\geq2$, $q!\geq2\,3^{q-2}$. Hence, for $0\leq\lambda<3$,

$$
e^\lambda-1-\lambda
=\sum_{q=2}^\infty\frac{\lambda^q}{q!}
\leq\frac{\lambda^2}{2}\sum_{r=0}^\infty\left(\frac\lambda3\right)^r
=\frac{\lambda^2}{2(1-\lambda/3)}.
$$

Substitution into the defining [moment-generating function](../../../probability-theory.md#moment-generating-function) bound shows that $X$ is [sub-Gamma in the right tail](../../../probability-inequality.md#sub-gamma-random-variable-in-the-right-tail) with variance parameter $\sigma^2$ and scale parameter $1/3$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix $0\leq\lambda<c^{-1}$. Since $X$ is centered, the elementary inequality $\log u\leq u-1$ gives

$$
\log\mathbb E e^{\lambda X}
\leq\mathbb E(e^{\lambda X}-1-\lambda X).
$$

On ${X\leq0}$, use $e^u-1-u\leq u^2/2$ for $u\leq0$; on ${X>0}$, expand the [exponential function](../../../calculus.md#exponential-function) into its [power series](../../../real-analysis.md#power-series). The hypotheses therefore give

$$
\begin{aligned}
\mathbb E(e^{\lambda X}-1-\lambda X)
&\leq\frac{\lambda^2}{2}\mathbb E X^2
 +\sum_{q=3}^\infty\frac{\lambda^q}{q!}\mathbb E X_+^q\\
&\leq\frac{\sigma^2\lambda^2}{2}
 +\frac{\sigma^2}{2}\sum_{q=3}^\infty\lambda^qc^{q-2}
=\frac{\sigma^2\lambda^2}{2(1-c\lambda)}.
\end{aligned}
$$

This is precisely the [Sub-Gamma random variable in the right tail](../../../probability-inequality.md#sub-gamma-random-variable-in-the-right-tail) bound with variance parameter $\sigma^2$ and scale parameter $c$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

A centered [random variable](../../../random-variable.md) $Y$ is [sub-Gaussian](../../../probability-and-statistics.md#sub-gaussian-distribution) with variance parameter $\sigma^2$ when

$$
\log\mathbb E e^{\lambda Y}\leq\frac{\sigma^2\lambda^2}{2}
\qquad(\lambda\in\mathbb R).
$$

The [Chernoff bound](../../../probability-inequality.md#chernoff-bound), applied to $Y$ and $-Y$, yields

$$
\mathbb P(|Y|\geq t)\leq2e^{-t^2/(2\sigma^2)}.
$$

The [tail integral formula for moments](../../../probability-theory.md#tail-integral-formula-for-moments) and the substitution $u=t^2/(2\sigma^2)$ now give

$$
\begin{aligned}
\mathbb E|Y|^q
&=q\int_0^\infty t^{q-1}\mathbb P(|Y|\geq t)\,dt\\
&\leq2q\int_0^\infty t^{q-1}e^{-t^2/(2\sigma^2)}\,dt
=2\Gamma\left(\frac q2+1\right)(2\sigma^2)^{q/2}.
\end{aligned}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Write $s=\sigma_Y\sigma_Z$ and $W=YZ-\mathbb E(YZ)$. The variables $Y$ and $Z$ need not be [independent random variables](../../../random-variable.md#independent-random-variables). Part (d) and the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) imply, for every integer $q\geq2$,

$$
\mathbb E|YZ|^q
\leq\bigl(\mathbb E|Y|^{2q}\mathbb E|Z|^{2q}\bigr)^{1/2}
\leq2^{q+1}q!s^q.
$$

Also $|\mathbb E(YZ)|\leq s$ by Cauchy-Schwarz, because $\mathbb EY^2\leq\sigma_Y^2$ and $\mathbb EZ^2\leq\sigma_Z^2$. Thus $\mathbb EW^2=\operatorname{Var}(YZ)\leq16s^2$, and, for $q\geq3$,

$$
\mathbb EW_+^q
\leq2^{q-1}\left(\mathbb E|YZ|^q+|\mathbb E(YZ)|^q\right)
\leq2^{2q+1}q!s^q
=\frac{q!}{2}(64s^2)(4s)^{q-2}.
$$

Part (c) shows that $W$ is [sub-Gamma in the right tail](../../../probability-inequality.md#sub-gamma-random-variable-in-the-right-tail) with variance parameter $64s^2$ and scale parameter $4s$.

If $\mathbb E(YZ)\geq0$, then $W_+\leq(YZ)_+\leq|YZ|$. Consequently

$$
\mathbb EW_+^q\leq2^{q+1}q!s^q
=\frac{q!}{2}(16s^2)(2s)^{q-2},
$$

while $\mathbb EW^2\leq16s^2$. Another application of part (c) gives the improved variance parameter $16\sigma_Y^2\sigma_Z^2$ and scale parameter $2\sigma_Y\sigma_Z$.

## 2

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [kernel for density estimation](../../../nonparametric-statistics.md#kernel-for-density-estimation) is a bounded nonnegative integrable function $K$ with $\int_{\mathbb R}K=1$. Its bandwidth-$h$ rescaling is $K_h(u)=h^{-1}K(u/h)$, and the [kernel density estimator](../../../nonparametric-statistics.md#kernel-density-estimation) is

$$
\widehat f_n(x)=\frac1n\sum_{i=1}^nK_h(x-X_i).
$$

Fix $x$ and put $V_i=K_h(x-X_i)$. Since $K$ vanishes outside $[-1,1]$,

$$
\mathbb EV_1^2
\leq\frac{\lVert K\rVert_\infty^2}{h^2}
\int_{x-h}^{x+h}f(y)\,dy
=\frac{2\lVert K\rVert_\infty^2}{h}f_h(x).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) and [variance additivity for independent random variables](../../../variance.md#variance-additivity-for-independent-random-variables) give

$$
\mathbb E|\widehat f_n(x)-\mathbb E\widehat f_n(x)|
\leq\lVert K\rVert_\infty
\frac{2^{1/2}f_h(x)^{1/2}}{(nh)^{1/2}}.
$$

Nonnegativity also gives $\mathbb E|V_1-\mathbb EV_1|\leq2\mathbb EV_1\leq4\lVert K\rVert_\infty f_h(x)$. Taking the better estimate at each $x$ and applying [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) proves

$$
\mathbb E\int_{-\infty}^{\infty}|\widehat f_n-\mathbb E\widehat f_n|
\leq\lVert K\rVert_\infty\int_{-\infty}^{\infty}
\min\left\{
\frac{2^{1/2}f_h^{1/2}}{(nh)^{1/2}},4f_h
\right\}.
$$

For nonnegative $a,b$ and $0\leq\theta\leq1$, $\min{a,b}\leq a^\theta b^{1-\theta}$. Taking $\theta=2\rho$ yields

$$
\mathbb E\int|\widehat f_n-\mathbb E\widehat f_n|
\leq\frac{2^{2-3\rho}\lVert K\rVert_\infty}{(nh)^\rho}
\int f_h^{1-\rho}.
$$

For $\rho>0$, the [Holder inequality](../../../functional-analysis.md#holder-inequality) with conjugate exponents $(1-\rho)^{-1}$ and $\rho^{-1}$ gives

$$
\int f_h^{1-\rho}
\leq C_{\rho,\delta}^{\rho}
\left(\int(1+|x|)^\delta f_h(x)\,dx\right)^{1-\rho}.
$$

If $U$ is uniform on $[-1,1]$ and independent of $X_1$, then $X_1+hU$ has [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $f_h$. Since

$$
1+|X_1+hU|\leq(1+h)(1+|X_1|),
$$

the last integral is at most $(1+h)^\delta\int(1+|x|)^\delta f(x)\,dx$. Substitution proves the second displayed bound. The case $\rho=0$ is the first bound integrated using $\int f_h=1$ and follows directly.

## 3

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [linear estimator in nonparametric regression](../../../nonparametric-statistics.md#linear-estimator-in-nonparametric-regression) at $x_0$ has the form $\widehat m_n(x_0)=\sum_iW_i(x_0)Y_i$, where the weights may depend on the design, $x_0$, $p$, $h$, and $K$, but not on the responses. Put

$$
K_i=\prod_{j=1}^dK\left(\frac{x_{ij}-x_{0j}}h\right),
\qquad Q_i=Q_h(x_i-x_0),
$$

and define the [local polynomial Gram matrix](../../../nonparametric-statistics.md#local-polynomial-gram-matrix)

$$
B_n(x_0)=\frac1{nh^d}\sum_iK_iQ_iQ_i^\top,
\qquad \lambda_0=\lambda_{\min}(B_n(x_0)).
$$

When $\lambda_0>0$, the [weighted least squares](../../../statistical-modelling.md#weighted-least-squares) normal equations have the unique solution

$$
\widehat\beta=B_n(x_0)^{-1}\frac1{nh^d}\sum_iK_iQ_iY_i.
$$

Therefore $\widehat m_n(x_0)=\sum_iW_iY_i$, where the [effective kernel weight](../../../nonparametric-statistics.md#effective-kernel-weight) is

$$
W_i=\frac1{nh^d}e_1^\top B_n(x_0)^{-1}Q_iK_i.
$$

The identity

$$
\sum_iW_iQ_i^\top=e_1^\top
$$

shows that these weights exactly reproduce at $x_0$ every [multivariate polynomial](../../../polynomial.md#multivariate-polynomial) of total degree at most $p$. This is the required [polynomial reproduction property of local polynomial regression](../../../nonparametric-statistics.md#polynomial-reproduction-property-of-local-polynomial-regression).

Only grid points with $\lVert x_i-x_0\rVert_\infty\leq h$ have nonzero weight. There are at most $(2n_1h+1)^d\leq(4n_1h)^d=4^dnh^d$ such points because $n_1h\geq1/2$. On this support,

$$
\lVert Q_i\rVert_2^2
\leq\sum_{\alpha\in\mathbb N_0^d}\frac1{\alpha!}
=e^d,
$$

so the [operator norm](../../../continuous-dual-space.md#operator-norm) bound $\lVert B_n^{-1}\rVert_{\mathrm{op}}=\lambda_0^{-1}$ gives

$$
|W_i|\leq\frac{e^{d/2}\lVert K\rVert_\infty^d}{\lambda_0nh^d}.
$$

Because the errors are [independent random variables](../../../random-variable.md#independent-random-variables) with the stated variance bounds,

$$
\operatorname{Var}(\widehat m_n(x_0))
\leq\sigma^2\sum_iW_i^2
\leq\frac{(4e)^d\lVert K\rVert_\infty^{2d}\sigma^2}
{\lambda_0^2nh^d}.
$$

Thus $\gamma_1=d$.

Let $T_{x_0}$ be the [Multivariate Taylor polynomial](../../../calculus.md#multivariate-taylor-polynomial) of $m$ at $x_0$ through total degree $\beta_0$. The assumed [Hölder continuity](../../../sobolev-space.md#holder-condition) of the derivatives and

$$
\sum_{|\alpha|=\beta_0}\frac1{\alpha!}=\frac{d^{\beta_0}}{\beta_0!}
$$

give the [Taylor remainder](../../../calculus.md#taylor-remainder) bound

$$
|m(x)-T_{x_0}(x)|
\leq\frac{d^{\beta_0}L}{\beta_0!}\lVert x-x_0\rVert_\infty^\beta.
$$

Polynomial reproduction cancels $T_{x_0}$ in the bias. The same support count and weight bound give

$$
\sum_i|W_i|
\leq\frac{(4e^{1/2})^d\lVert K\rVert_\infty^d}{\lambda_0}.
$$

Consequently

$$
|\operatorname{Bias}(\widehat m_n(x_0))|
\leq
\frac{(4e^{1/2})^dd^{\beta_0}L\lVert K\rVert_\infty^d}
{\lambda_0\beta_0!}h^\beta,
$$

so $\gamma_2=\beta$.

## 4

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [pushforward measure](../../../measure-theory.md#pushforward-measure) of $\mu$ under $g$ is $g_*\mu$, defined for $B\in\mathcal B$ by

$$
(g_*\mu)(B)=\mu(g^{-1}(B)).
$$

The [Lebesgue decomposition theorem](../../../measure-theory.md#lebesgue-decomposition-theorem) says that if $\nu$ and $\mu$ are sigma-finite measures on the same measurable space, then uniquely

$$
\nu=\nu_{\mathrm{ac}}+\nu_{\mathrm{s}},
\qquad \nu_{\mathrm{ac}}\ll\mu,
\qquad \nu_{\mathrm{s}}\perp\mu.
$$

Let $f:[0,\infty)\to\mathbb R\cup{+\infty}$ be [convex](../../../real-analysis.md#convex-function) with $f(1)=0$. If $\lambda$ dominates the [probability distributions](../../../probability-theory.md#probability-distribution) $P,Q$, with densities $p,q$, their [f-divergence](../../../probability-and-statistics.md#f-divergence) is

$$
D_f(P\Vert Q)=\int q,f(p/q)\,d\lambda,
$$

using the lower-semicontinuous perspective convention where $q=0$. This definition is independent of the dominating measure.

The [data processing inequality for f-divergences](../../../probability-and-statistics.md#data-processing-inequality-for-f-divergences) states

$$
D_f(g_*P\Vert g_*Q)\leq D_f(P\Vert Q).
$$

To prove it, take $\lambda=P+Q$ and let $\mathcal G=g^{-1}(\mathcal B)$. If $p=dP/d\lambda$ and $q=dQ/d\lambda$, then the pullbacks of the densities of $g_*P$ and $g_*Q$ with respect to $g_*\lambda$ are respectively $\mathbb E_\lambda[p\mid\mathcal G]$ and $\mathbb E_\lambda[q\mid\mathcal G]$. The perspective $F(a,b)=bf(a/b)$ of a convex function is jointly convex. Conditional [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) therefore gives

$$
F(\mathbb E[p\mid\mathcal G],\mathbb E[q\mid\mathcal G])
\leq\mathbb E[F(p,q)\mid\mathcal G].
$$

Integration proves the claim.

The [Squared Hellinger distance](../../../probability-and-statistics.md#squared-hellinger-distance) is

$$
H^2(P,Q)=\int\left(\sqrt{dP/d\lambda}-\sqrt{dQ/d\lambda}\right)^2d\lambda.
$$

If $P,Q$ have densities $p,q$ with respect to a sigma-finite measure $\mu$, this becomes

$$
H^2(P,Q)=\int(\sqrt p-\sqrt q)^2d\mu
=2-2\int\sqrt{pq}\,d\mu.
$$

Fix any probability distribution $Q$ and set $p_j=P_j(A_j)$, $q_j=Q(A_j)$, and $t_j=H^2(P_j,Q)$. Applying the data processing inequality to the [indicator function](../../../measure-theory.md#indicator-function) of $A_j$ gives the Bernoulli Hellinger bound

$$
t_j\geq2-2\left(\sqrt{p_jq_j}+\sqrt{(1-p_j)(1-q_j)}\right).
$$

The hinted inequality implies

$$
(p_j-q_j)^2\leq t_j\left(1-\frac{t_j}{4}\right).
$$

The function $t\mapsto\sqrt{t(1-t/4)}$ is concave on $[0,2]$. Since the $A_j$ form a [set partition](../../../combinatorics.md#set-partition), $\sum_jq_j=1$, and [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives

$$
\begin{aligned}
\frac1M\sum_{j=1}^MP_j(A_j)
&\leq\frac1M+\frac1M\sum_{j=1}^M
\sqrt{t_j(1-t_j/4)}\\
&\leq\frac1M+
\sqrt{\frac1M\sum_{j=1}^Mt_j}
\sqrt{1-\frac1{4M}\sum_{j=1}^Mt_j}.
\end{aligned}
$$

Taking the infimum over $Q$ proves the stated inequality.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
