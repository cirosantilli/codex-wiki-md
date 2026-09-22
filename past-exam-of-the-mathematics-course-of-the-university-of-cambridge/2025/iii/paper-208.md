# Paper 208

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_208.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_208.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Hoeffding lemma](../../../probability-inequality.md#hoeffding-lemma) states that if $a\leq X\leq b$ almost surely, then for every real $\lambda$,

$$
\log\mathbb E e^{\lambda(X-\mathbb EX)}
\leq\frac{\lambda^2(b-a)^2}{8}.
$$

Convexity of $e^{\lambda x}$ bounds it on $[a,b]$ by the secant joining its endpoint values. Taking expectations reduces the centered moment-generating function to that of a two-point variable on $\{a,b\}$ having the same mean. After rescaling to $[0,1]$, its logarithm is

$$
-\lambda q+\log(1-q+qe^\lambda),
$$

where $q$ is its mean. Twice differentiating in $\lambda$ shows that the second derivative is a Bernoulli variance and hence at most $1/4$. The value and first derivative vanish at zero, so Taylor's theorem gives at most $\lambda^2/8$. Rescaling proves the claim.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For $X\sim\operatorname{Bernoulli}(p)$,

$$
H(X)=p\log\frac1p+(1-p)\log\frac1{1-p}.
$$

The inequality $-\log(1-p)\leq p/(1-p)$ bounds the second term by $p$. Also $\log x\leq2\sqrt x$ for $x\geq1$, so $p\log(1/p)\leq2\sqrt p$. Hence

$$
\boxed{H(X)\leq2\sqrt p+p.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $q_i=\min(p_i,1-p_i)$. Applying part (b) after possibly replacing $X_i$ by $1-X_i$ gives $H(X_i)\leq2\sqrt{q_i}+q_i$. If $q_i<\delta_i$, then, because $0<\delta_i<1$, this is less than $3\sqrt{\delta_i}$, contradicting the assumption. Thus $p_i,1-p_i\geq\delta_i$.

The centered variables

$$
Y_i=\log P_i(X_i)+H(X_i)
$$

are independent and have mean zero. Their two possible values differ by

$$
\left|\log\frac{p_i}{1-p_i}\right|
\leq|\log\delta_i|.
$$

Applying [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) to $\sum_iY_i$ gives

$$
\boxed{\mathbb P\left(\log P(X_1,\ldots,X_n)+H(X_1,\ldots,X_n)\leq-t\right)
\leq\exp\left(-\frac{2t^2}{\sum_i(\log\delta_i)^2}\right).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Independence makes [varentropy](../../../information-theory.md#varentropy) additive. For a Bernoulli variable,

$$
V_H(X_i)=p_i(1-p_i)
\left(\log\frac{p_i}{1-p_i}\right)^2.
$$

Part (c) bounds the logarithm by $|\log\delta_i|$, while $p_i(1-p_i)\leq1/4$. Therefore

$$
\boxed{V_H(X_1,\ldots,X_n)=\sum_iV_H(X_i)
\leq\frac14\sum_{i=1}^n(\log\delta_i)^2.}
$$

## 2

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Apply the [Poincaré inequality in probability theory](../../../probability-inequality.md#poincare-inequality-in-probability-theory) to $g=e^{\lambda f/2}$. Since $\lVert\nabla f\rVert\leq1$,

$$
F(\lambda)-F(\lambda/2)^2
\leq C_P(X)\frac{\lambda^2}{4}F(\lambda).
$$

Hence

$$
F(\lambda)\leq
\left(1-\frac{\lambda^2C_P(X)}4\right)^{-1}
F(\lambda/2)^2.
$$

Iterating this estimate $m$ times yields

$$
F(\lambda)\leq
\prod_{k=0}^{m-1}
\left(1-\frac{\lambda^2C_P(X)}{4^{k+1}}\right)^{-2^k}
F(\lambda/2^m)^{2^m},
$$

valid under the stated bound on $\lambda$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Since $\mathbb Ef(X)=0$ and the moment-generating function is finite near zero, $\log F(u)=O(u^2)$. Consequently

$$
2^m\log F(\lambda/2^m)=O(2^{-m})\to0,
$$

which proves $F(\lambda/2^m)^{2^m}\to1$.

For $\lambda_*=C_P(X)^{-1/2}$, part (a) and the elementary bound $-\log(1-x)\leq4x/3$ for $0\leq x\leq1/4$ give

$$
\log F(\lambda_*)
\leq\sum_{k\geq0}2^k[-\log(1-4^{-(k+1)})]
\leq\frac23<\log3.
$$

**Thus $F(\lambda_*)\leq3$.**

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [Chernoff bound](../../../probability-inequality.md#chernoff-bound) and part (b) give

$$
\mathbb P(f(X)\geq t)
\leq e^{-\lambda_*t}F(\lambda_*)
\leq3e^{-t/\sqrt{C_P(X)}}.
$$

Apply the same argument to $-f$ and use the [union bound](../../../probability-inequality.md#boole-s-inequality) to obtain

$$
\mathbb P(|f(X)|\geq t)
\leq6e^{-t/\sqrt{C_P(X)}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Subtract a constant so that $f(0)=0$, and write $m=\mathbb Ef(Y)$, $V=\operatorname{Var}f(Y)$, and $A=\mathbb E f'(Y)^2$. The supplied identity applied to $f$ and $f^2$ gives

$$
m=\mathbb E[\operatorname{sgn}(Y)f'(Y)],
\qquad
\mathbb Ef(Y)^2=2\mathbb E[\operatorname{sgn}(Y)f(Y)f'(Y)].
$$

By [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), $m^2\leq A$ and

$$
V=\mathbb Ef^2-m^2
\leq2\sqrt{(V+m^2)A}-m^2.
$$

**Thus $V+m^2\leq2\sqrt{(V+m^2)A}$, so $V+m^2\leq4A$ and in particular $V\leq4A$. Therefore the standard Laplace distribution has $C_P(Y)\leq4$.**

## 3

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For standard Gaussian measure $\gamma$, the [Gaussian Poincaré inequality](../../../probability-inequality.md#gaussian-poincare-inequality) is

$$
\operatorname{Var}_\gamma h\leq\int(h')^2d\gamma.
$$

The [Gaussian logarithmic Sobolev inequality](../../../probability-inequality.md#gaussian-logarithmic-sobolev-inequality) is

$$
\operatorname{Ent}_\gamma(h^2)
\leq2\int(h')^2d\gamma,
$$

where $\operatorname{Ent}_\gamma(G)=\int G\log G\,d\gamma-(\int Gd\gamma)\log\int Gd\gamma$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Set $h=\sqrt{f/\phi}$. Then $\int h^2d\gamma=1$ and

$$
D(f\Vert\phi)=\operatorname{Ent}_\gamma(h^2).
$$

Moreover,

$$
h'=\frac h2\left(\frac{f'}f-\frac{\phi'}\phi\right),
\qquad
\int(h')^2d\gamma=\frac14J(f\Vert\phi).
$$

The [Gaussian logarithmic Sobolev inequality](../../../probability-inequality.md#gaussian-logarithmic-sobolev-inequality) therefore gives

$$
\boxed{D(f\Vert\phi)\leq\frac12J(f\Vert\phi).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

With the same $h$, the squared [Hellinger distance](../../../probability-and-statistics.md#hellinger-distance) is

$$
d_H(f,\phi)^2=\frac12\int(h-1)^2d\gamma
=1-\int h\,d\gamma.
$$

Since $0\leq\int h\,d\gamma\leq1$,

$$
1-\int h\,d\gamma
\leq1-\left(\int h\,d\gamma\right)^2
=\operatorname{Var}_\gamma h.
$$

The [Gaussian Poincaré inequality](../../../probability-inequality.md#gaussian-poincare-inequality) and the derivative calculation in part (b) yield

$$
\boxed{d_H(f,\phi)^2\leq\frac14J(f\Vert\phi).}
$$

## 4

↑ **Parent:** [Paper 208](paper-208.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $W=Z-\mathbb EZ$ and $\psi(\lambda)=\log\mathbb E_Pe^{\lambda W}$. For any $Q\ll P$ and real $\lambda$, define the exponential tilt

$$
\frac{dP_\lambda}{dP}=e^{\lambda W-\psi(\lambda)}.
$$

Positivity of relative entropy gives

$$
D(Q\Vert P)=D(Q\Vert P_\lambda)
+\lambda\mathbb E_QW-\psi(\lambda)
\geq\lambda\mathbb E_QW-\psi(\lambda).
$$

Thus every $Q$ with $\mathbb E_QW\geq t$ has $D(Q\Vert P)\geq\sup_{\lambda\geq0}\{\lambda t-\psi(\lambda)\}=\psi^*(t)$.

For $0<t<b$, continuity of $\psi'$ supplies $\lambda_t>0$ with $\psi'(\lambda_t)=t$. Under $P_{\lambda_t}$, $\mathbb EW=t$, and direct substitution gives

$$
D(P_{\lambda_t}\Vert P)
=\lambda_t t-\psi(\lambda_t)=\psi^*(t).
$$

This tilt attains the constrained infimum and proves the identity.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For any coupling $\pi$ of $X\sim P$ and $Y\sim Q$ and every $A\subseteq\Omega$,

$$
P(A)-Q(A)
=\mathbb P_\pi(X\in A,Y\notin A)
-\mathbb P_\pi(X\notin A,Y\in A).
$$

Its absolute value is at most $\mathbb P_\pi(X\ne Y)$. Taking the supremum over $A$ and then the infimum over couplings proves

$$
\boxed{d_{\mathrm{TV}}(P,Q)
\leq\inf_{\pi\in\Pi(P,Q)}\mathbb P_\pi(X\ne Y).}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For each $i$, the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) between $\operatorname{Bernoulli}(p_i)$ and $\operatorname{Poisson}(p_i)$ is

$$
p_i(1-e^{-p_i})\leq p_i^2.
$$

Indeed, compare their masses at zero, one, and the Poisson tail; the positive excess of Bernoulli mass at one is $p_i(1-e^{-p_i})$. A maximal coupling therefore gives a pair $(X_i,N_i)$ with mismatch probability at most $p_i^2$. Couple these pairs independently. Then

$$
\mathbb P\left(\sum_iX_i\ne\sum_iN_i\right)
\leq\sum_i p_i^2
$$

by the union bound. Since $\sum_iN_i\sim\operatorname{Poisson}(\sum_ip_i)=\operatorname{Poisson}(\nu)$, part (b) yields

$$
\boxed{d_{\mathrm{TV}}(P,Q)\leq\sum_{i=1}^np_i^2.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
