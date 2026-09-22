# Paper 224

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_224.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_224.pdf)

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
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)

## 1

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For nonnegative $a_i,b_i$, with $a=\sum_i a_i$ and $b=\sum_i b_i$, the [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality) is

$$
\sum_i a_i\log\frac{a_i}{b_i}\geq a\log\frac ab,
$$

with the usual extended-value conventions. Equality holds when $a_i/b_i$ is constant wherever $a_i>0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $0\leq\lambda\leq1$ and put $P=\lambda P_1+(1-\lambda)P_2$ and $Q=\lambda Q_1+(1-\lambda)Q_2$. For each alphabet symbol $x$, apply the [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality) to $a_1=\lambda P_1(x)$, $a_2=(1-\lambda)P_2(x)$ and the corresponding $b$ values. Summing over $x$ gives

$$
D(P\Vert Q)
\leq\lambda D(P_1\Vert Q_1)
+(1-\lambda)D(P_2\Vert Q_2),
$$

which is joint [convexity](../../../real-analysis.md#convex-function) in $(P,Q)$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For $Z=\mathbb E_Qe^g$, define the exponentially tilted mass function $Q_g(x)=Q(x)e^{g(x)}/Z$. [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) gives

$$
0\leq D_e(P\Vert Q_g)
=D_e(P\Vert Q)-\mathbb E_Pg+\log Z.
$$

Rearranging proves

$$
D_e(P\Vert Q)\geq\mathbb E_Pg-log\mathbb E_Qe^g.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The preceding inequality supplies the upper bound on the supremum. If $P$ has full support relative to $Q$, choose $g(x)=\log(P(x)/Q(x))$; then $\mathbb E_Qe^g=1$ and the objective equals $D_e(P\Vert Q)$. If $P(x)=0$ at some symbols, use this choice on the support of $P$ and put $g(x)=-M$ elsewhere. Letting $M\to\infty$ gives the same value. Finiteness of $D(P\Vert Q)$ guarantees that $Q$ is positive on the support of $P$. This proves the [Gibbs variational principle for relative entropy](../../../probability-and-statistics.md#gibbs-variational-principle-for-relative-entropy).

## 2

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $X_1,X_2,\ldots$ be i.i.d. with mass function $Q$ on a finite alphabet, and let $\widehat P_n$ be their [empirical distribution](../../../information-theory.md#type-information-theory). [Sanov theorem](../../../information-theory.md#sanov-theorem) states that for every set $\Gamma$ of probability mass functions,

$$
-\inf_{R\in\Gamma^\circ}D_e(R\Vert Q)
\leq\liminf_{n\to\infty}\frac1n\log\mathbb P(\widehat P_n\in\Gamma)
$$

and

$$
\limsup_{n\to\infty}\frac1n\log\mathbb P(\widehat P_n\in\Gamma)
\leq-\inf_{R\in\overline\Gamma}D_e(R\Vert Q),
$$

where interior and closure use the probability-simplex topology. Thus the empirical distributions satisfy a [large deviation principle](../../../convergence-of-random-variables.md#large-deviation-principle) with rate function $D_e(\mathord\cdot\Vert Q)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The likelihood-ratio event depends only on the type $R=\widehat P_n$ and is

$$
\sum_xR(x)\log\frac{P(x)}{Q(x)}\geq0,
$$

equivalently $D(R\Vert Q)\geq D(R\Vert P)$. This constraint defines a closed subset of the finite probability simplex, so Sanov's upper bound gives the exponent

$$
C(P,Q)=\inf_{R:\,D(R\Vert Q)\geq D(R\Vert P)}D_e(R\Vert Q).
$$

It is strictly positive: the only distribution with zero divergence from $Q$ is $R=Q$, but $Q$ violates the constraint because $0=D(Q\Vert Q)<D(Q\Vert P)$. Compactness and continuity under full support keep the infimum away from zero. This exponent is the [Chernoff information](../../../information-theory.md#chernoff-information) between $P$ and $Q$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

An error implies that some $\theta\ne\theta^*$ has likelihood at least that of $\theta^*$. A finite [union bound](../../../probability-inequality.md#boole-s-inequality) and part (b) therefore give

$$
\limsup_{n\to\infty}\frac1n\log
\mathbb P(\widehat\theta_n\ne\theta^*)
\leq-C^*(\Theta),
$$

where

$$
C^*(\Theta)=
\min_{\theta\ne\theta^*}
\inf_{R:\,D(R\Vert P_{\theta^*})\geq D(R\Vert P_\theta)}
D_e(R\Vert P_{\theta^*}).
$$

Every inner infimum is strictly positive by the argument in part (b), and the minimum of finitely many positive numbers is positive.

## 3

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For feasible mass functions $Q_1,Q_2$ at distortion levels $d_1,d_2$, the mixture $Q=\lambda Q_1+(1-\lambda)Q_2$ has nonzero-symbol mass at most $\lambda d_1+(1-\lambda)d_2$. Concavity of [information entropy](../../../information-theory.md#information-entropy) gives

$$
H(Q)\geq\lambda H(Q_1)+(1-\lambda)H(Q_2).
$$

Taking maximizing sequences proves

$$
\phi(\lambda d_1+(1-\lambda)d_2)
\geq\lambda\phi(d_1)+(1-\lambda)\phi(d_2).
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Regard the alphabet as the cyclic group $\mathbb Z/m\mathbb Z$ and put $E=X-Y$. For each $y$, subtraction by $y$ is a bijection, so

$$
H(X\mid Y=y)=H(E\mid Y=y)\leq\phi(d_y),
\qquad
d_y=\mathbb P(X\ne Y\mid Y=y).
$$

By concavity of $\phi$, its monotonicity in the distortion allowance, and $\mathbb E d_Y=\mathbb P(X\ne Y)\leq d$,

$$
H(X\mid Y)
\leq\mathbb E\phi(d_Y)
\leq\phi(\mathbb E d_Y)
\leq\phi(d).
$$

Therefore

$$
\boxed{I(X;Y)=H(X)-H(X\mid Y)\geq H(X)-\phi(d).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The previous part gives $R(d)\geq\log m-\phi(d)$ for uniform $X$. To attain the bound, take $Y$ uniform on $\mathbb Z/m\mathbb Z$, choose an independent error $E$ whose mass function attains $\phi(d)$, and set $X=Y+E$. Then $X$ is uniform, $\mathbb P(X\ne Y)=\mathbb P(E\ne0)\leq d$, and

$$
H(X\mid Y)=H(E)=\phi(d).
$$

**Thus $I(X;Y)=\log m-\phi(d)$ and equality holds. This is the [rate-distortion function](../../../information-theory.md#rate-distortion-function) of a uniform source under [Hamming distortion](../../../information-theory.md#hamming-distortion).**

## 4

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The direct codes-distributions correspondence says that every mass function $Q$ on a finite alphabet admits a binary [prefix code](../../../coding-theory.md#prefix-code) with lengths $L(x)=\lceil-\log_2Q(x)\rceil$. Conversely, every binary prefix code has lengths satisfying the [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) $K=\sum_x2^{-L(x)}\leq1$, and hence defines the mass function $Q_C(x)=2^{-L(x)}/K$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For the distribution $Q_C$ from part (a),

$$
L(x)=-\log_2Q_C(x)-\log_2K.
$$

Therefore

$$
\mathbb E_P L(X)
=H(P)+D(P\Vert Q_C)-\log_2K
\geq H(P),
$$

by [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) and $K\leq1$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

For any fixed threshold $R$, minimizing the excess-length probability means assigning the available strings shorter than $R$ to the most probable symbols. Repeating this exchange argument simultaneously for every threshold orders symbols by decreasing probability and assigns binary strings from shortest to longest. There are $2^\ell$ words of length $\ell$, so the $k$th word in shortlex order has length

$$
L^*(x_k)=\lfloor\log_2k\rfloor.
$$

This is the [optimal one-to-one binary code](../../../information-theory.md#optimal-one-to-one-binary-code).

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

For decreasing probabilities, the first $x$ symbols each have probability at least $P(x)$, so $xP(x)\leq1$. Hence

$$
\boxed{L^*(x)=\lfloor\log_2x\rfloor
\leq\log_2x\leq-\log_2P(x).}
$$

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Relabeling an arbitrary alphabet in decreasing probability order makes part (ii) pointwise:

$$
L^*(x)\leq-\log_2P(x).
$$

It immediately implies

$$
\mathbb P(L^*(X)\geq R)
\leq\mathbb P(-\log_2P(X)\geq R)
$$

and, after taking expectations,

$$
\mathbb E L^*(X)\leq H(X).
$$

This reverses the prefix-code lower bound from part (b). A general one-to-one code need not decode concatenated codewords instantaneously or uniquely, so it is not constrained by Kraft's inequality.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
