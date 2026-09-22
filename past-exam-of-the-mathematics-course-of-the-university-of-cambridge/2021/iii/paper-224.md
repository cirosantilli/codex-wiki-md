# Paper 224

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_224.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_224.pdf)

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
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Stein's lemma](../../../information-theory.md#stein-s-lemma-information-theory) states that for testing $P^{\otimes n}$ against $Q^{\otimes n}$, the smallest [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) $\beta_n$ among tests with [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) at most any fixed $0<\varepsilon<1$ satisfies

$$
\boxed{\lim_{n\to\infty}-\frac1n\log\beta_n=D(P\Vert Q).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Neyman-Pearson lemma](../../../statistical-modelling.md#neyman-pearson-lemma) gives an optimal acceptance region for $P$ of the form

$$
B_n(\tau)=\left\{x_1^n:\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}\geq\tau\right\},
$$

with possible boundary randomization. If $\widehat P_n$ is the empirical mass function, then

$$
\frac1n\log\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
=D(\widehat P_n\Vert Q)-D(\widehat P_n\Vert P),
$$

so equivalently

$$
B_n(\tau)=\left\{D(\widehat P_n\Vert Q)-D(\widehat P_n\Vert P)\geq n^{-1}\log\tau\right\}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Fix $\delta>0$ and choose

$$
\tau_n=\exp\{n(D(P\Vert Q)-\delta)\}.
$$

Under $P$, the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) makes the normalized log likelihood ratio converge in probability to $D(P\Vert Q)$, so $P^{\otimes n}(B_n(\tau_n))\to1$. On this [Neyman-Pearson decision region](../../../information-theory.md#neyman-pearson-decision-region),

$$
Q^{\otimes n}\leq\tau_n^{-1}P^{\otimes n},
$$

and hence

$$
\beta_n\leq e^{-n(D(P\Vert Q)-\delta)}.
$$

Letting $\delta\downarrow0$ proves the direct bound.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For any region $B_n$ with $P^{\otimes n}(B_n)\geq1-\varepsilon$, let

$$
C_n=\left\{x_1^n:n^{-1}\log\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\leq D(P\Vert Q)+\delta\right\}.
$$

The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) gives $P^{\otimes n}(C_n)\to1$, so $P^{\otimes n}(B_n\cap C_n)\geq1-\varepsilon-o(1)$. Therefore

$$
\beta_n\geq Q^{\otimes n}(B_n\cap C_n)
\geq e^{-n(D(P\Vert Q)+\delta)}\{1-\varepsilon-o(1)\}.
$$

**Thus $\limsup-n^{-1}\log\beta_n\leq D(P\Vert Q)+\delta$; let $\delta\downarrow0$.**

## 2

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For finite $m$, independence and conditional [subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy) give

$$
\begin{aligned}
\sum_{i=1}^mI(X_i;Z)
&=H(X_1^m)-\sum_iH(X_i\mid Z)\\
&\leq H(X_1^m)-H(X_1^m\mid Z)
=I(X_1^m;Z)\leq H(Z).
\end{aligned}
$$

The partial sums increase because [mutual information](../../../information-theory.md#mutual-information) is nonnegative. Taking $m\to\infty$ proves $H(Z)\geq\sum_{i\geq1}I(X_i;Z)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $S_i=[n]\setminus\{i\}$, the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) gives

$$
H(X_{S_i})=\sum_{j\in S_i}H(X_j\mid X_{S_i\cap[j-1]}).
$$

Each summand is at least $H(X_j\mid X_1^{j-1})$ because [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy). Summing over $i$, each $j$ occurs $n-1$ times:

$$
\sum_{i=1}^nH(X_{S_i})
\geq(n-1)\sum_{j=1}^nH(X_j\mid X_1^{j-1})
=(n-1)H(X_1^n).
$$

This is the required special case of [Shearer's inequality](../../../information-theory.md#shearer-s-inequality).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Writing $Q_j$ for the $j$th marginal and using $P=\prod_jP_j$,

$$
D(Q\Vert P)=-H(Q)+\sum_j\mathbb E_{Q_j}[-\log P_j(Y_j)].
$$

The analogous formula for $D(Q^{(i)}\Vert P^{(i)})$ omits coordinate $i$. Consequently

$$
\begin{aligned}
\sum_i\{D(Q\Vert P)-D(Q^{(i)}\Vert P^{(i)})\}
&=-nH(Q)+\sum_iH(Q^{(i)})\\
&\quad+\sum_j\mathbb E_{Q_j}[-\log P_j(Y_j)].
\end{aligned}
$$

Part b makes $\sum_iH(Q^{(i)})\geq(n-1)H(Q)$, so the last display is at least $D(Q\Vert P)$.

## 3

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [three-point identity for relative entropy](../../../probability-and-statistics.md#three-point-identity-for-relative-entropy) is

$$
\boxed{D(P\Vert Q)=D(P\Vert R)+D(R\Vert Q)
+\sum_a\{P(a)-R(a)\}\log\frac{R(a)}{Q(a)}}.
$$

It follows by expanding and collecting logarithms. When the final sum vanishes, it is the [Pythagorean identity for relative entropy](../../../probability-and-statistics.md#pythagorean-identity-for-relative-entropy).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

For $Q_t=(1-t)Q^*+tQ^0$, convexity gives $Q_t\in E$. Minimality at $t=0$ implies

$$
0\leq\left.\frac d{dt}D(P\Vert Q_t)\right|_{0+}
=\sum_aP(a)\left(1-\frac{Q^0(a)}{Q^*(a)}\right).
$$

Since $P$ has full support and the minimum is finite, $Q^*$ has full support.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

For $A'=\{a:P'(a)>0\}$,

$$
\begin{aligned}
\sum_{a\in A'}P'(a)\left(1-\frac{P(a)Q^0(a)}{P'(a)Q^*(a)}\right)
&=1-\sum_{a\in A'}\frac{P(a)Q^0(a)}{Q^*(a)}\\
&\geq1-\sum_{a\in A}\frac{P(a)Q^0(a)}{Q^*(a)}\geq0,
\end{aligned}
$$

using nonnegativity and part i.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Expanding the three divergences gives

$$
D(P'\Vert Q^0)+D(P'\Vert P)-D(P'\Vert Q^*)
=\sum_{a\in A'}P'(a)\log\frac{P'(a)Q^*(a)}{P(a)Q^0(a)}.
$$

The inequality $\log u\geq1-u^{-1}$ bounds this below by the nonnegative expression in part ii. Hence

$$
\boxed{D(P'\Vert Q^0)+D(P'\Vert P)\geq D(P'\Vert Q^*)}.
$$

## 4

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The binary [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) states that codeword lengths $l(a)$ of a [prefix code](../../../coding-theory.md#prefix-code), or more generally a uniquely decodable code, satisfy

$$
\sum_a2^{-l(a)}\leq1.
$$

Conversely, positive integer lengths obeying this inequality can be realized by a binary prefix code.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The Shannon lengths are $l_S(a)=\lceil\log_2(1/P(a))\rceil$. Their [Competitive optimality of the Shannon code](../../../coding-theory.md#competitive-optimality-of-the-shannon-code) says that for every binary uniquely decodable code of lengths $l_C$ and every positive integer $k$,

$$
\mathbb P\{l_S(X)\geq l_C(X)+k\}\leq2^{-k+1}.
$$

On this event, $P(X)<2^{-l_C(X)-k+1}$. Summing and applying the [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) proves

$$
\boxed{\mathbb P\{l_S(X)\geq l_C(X)+k\}
\leq2^{-k+1}\sum_a2^{-l_C(a)}\leq2^{-k+1}.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Relabel the symbols so $p_1\geq\cdots\geq p_m$ and assign all finite binary strings in nondecreasing length order, beginning with the empty string. The $i$th string has length

$$
L(i)=\lfloor\log_2i\rfloor.
$$

Since $1\geq\sum_{j=1}^ip_j\geq ip_i$,

$$
L(i)\leq\log_2i\leq\log_2(1/p_i).
$$

Thus the [optimal one-to-one binary code](../../../information-theory.md#optimal-one-to-one-binary-code) satisfies

$$
\boxed{\mathbb E[L(X)]\leq\sum_ip_i\log_2(1/p_i)=H(X)}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For the uniform distribution, the code in part c has

$$
\mathbb E[L(X)]=\frac1m\sum_{i=1}^m\lfloor\log_2i\rfloor<\log_2m=H(X),
$$

because every summand is at most $\log_2m$ and at least one is strictly smaller. For $m=3$, the explicit code $C(1)=\lambda$, $C(2)=0$, $C(3)=1$ has mean length $2/3<\log_2 3$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
