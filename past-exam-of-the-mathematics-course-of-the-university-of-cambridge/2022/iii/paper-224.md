# Paper 224

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_224.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_224.pdf)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Stein's lemma](../../../information-theory.md#stein-s-lemma-information-theory) states that for distinct probability mass functions $P,Q$ on a finite alphabet, the best exponential decay rate of the [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) $\beta_n=Q^{\otimes n}(B_n)$ among tests whose [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) $\alpha_n=P^{\otimes n}(B_n^c)$ is eventually at most any fixed $\epsilon\in(0,1)$ is

$$
\lim_{n\to\infty}-\frac1n\log_2\beta_n=D(P\Vert Q).
$$

For the direct part, define the information-density typical region

$$
B_n=\left\{x_1^n:
\frac1n\log_2\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\geq D(P\Vert Q)-\delta
\right\}.
$$

The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) under $P$ gives $\alpha_n\to0$, while

$$
\begin{aligned}
\beta_n
&=\sum_{x_1^n\in B_n}Q^{\otimes n}(x_1^n)\\
&\leq2^{-n\{D(P\Vert Q)-\delta\}}
\sum_{x_1^n\in B_n}P^{\otimes n}(x_1^n)\\
&\leq2^{-n\{D(P\Vert Q)-\delta\}}.
\end{aligned}
$$

For the converse, let

$$
C_n=\left\{x_1^n:
\frac1n\log_2\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\leq D(P\Vert Q)+\delta
\right\}.
$$

Again $P^{\otimes n}(C_n)\to1$. Any test with $P^{\otimes n}(B_n)\geq1-\epsilon$ satisfies

$$
P^{\otimes n}(B_n\cap C_n)\geq1-\epsilon-o(1).
$$

On $C_n$, $Q^{\otimes n}\geq2^{-n(D+\delta)}P^{\otimes n}$, hence

$$
\beta_n\geq2^{-n(D+\delta)}\{1-\epsilon-o(1)\}.
$$

**Thus $\limsup_n-n^{-1}\log_2\beta_n\leq D+\delta$. Letting $\delta\downarrow0$ proves optimality.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Using the paper's full-$\ell^1$ convention, the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) is

$$
\lVert P-Q\rVert_{\rm TV}
=\sum_{a\in A}|P(a)-Q(a)|.
$$

Let $A_+=\{a:P(a)\geq Q(a)\}$. Since the signed differences sum to zero,

$$
\lVert P-Q\rVert_{\rm TV}
=2\sum_{a\in A_+}\{P(a)-Q(a)\}
=2\{P(A_+)-Q(A_+)\}.
$$

For every $B\subseteq A$, its positive difference is at most the sum over $A_+$, and its negative difference has the same bound by taking the complement. Therefore

$$
\boxed{\lVert P-Q\rVert_{\rm TV}
=2\sup_{B\subseteq A}|P(B)-Q(B)|.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $B_n$ be the region on which the test chooses $P_n$. Then

$$
e_1^{(n)}(B_n)+e_2^{(n)}(B_n)
=P_n(B_n^c)+Q_n(B_n)
=1-\{P_n(B_n)-Q_n(B_n)\}.
$$

Minimizing over decision regions is therefore equivalent to maximizing the signed difference. Part b gives

$$
\min_{B_n\subseteq A^n}P_e^{(n)}(B_n)
=1-\sup_{B_n}\{P_n(B_n)-Q_n(B_n)\}
=1-\frac12\lVert P_n-Q_n\rVert_{\rm TV}.
$$

The minimizing region is $\{x:P_n(x)\geq Q_n(x)\}$, the equal-prior [Neyman-Pearson decision region](../../../information-theory.md#neyman-pearson-decision-region).

## 2

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For an independent identically distributed source with mass function $P$ on a finite alphabet and a fixed compression rate $R>H(P)$, the optimal probability of decoding error has exponent

$$
E(R)=\min_{Q:H(Q)\geq R}D(Q\Vert P),
$$

meaning that the best fixed-rate codes satisfy

$$
\lim_{n\to\infty}-\frac1n\log_2P_e^{(n)}=E(R)
$$

at continuity points of the exponent.

For the direct part, let $m=|A|$ and

$$
\eta_n=\frac{m\log_2(n+1)}n.
$$

Encode every sequence whose [type](../../../information-theory.md#type-information-theory) $Q$ satisfies $H(Q)\leq R-\eta_n$. The [method of types](../../../information-theory.md#method-of-types) bounds the number of such sequences by

$$
(n+1)^m2^{n(R-\eta_n)}=2^{nR},
$$

so they fit into a rate-$R$ codebook. The error probability obeys

$$
\begin{aligned}
P_e^{(n)}
&\leq\sum_{Q:H(Q)>R-\eta_n}P^{\otimes n}(T(Q))\\
&\leq(n+1)^m
2^{-n\min_{Q:H(Q)>R-\eta_n}D(Q\Vert P)}.
\end{aligned}
$$

Compactness of the probability simplex and continuity of entropy and relative entropy on the support of $P$ give

$$
\liminf_{n\to\infty}-\frac1n\log_2P_e^{(n)}
\geq\min_{Q:H(Q)\geq R}D(Q\Vert P)=E(R),
$$

which is the direct bound.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The test accepts $P$ when $D(\widehat P_n\Vert P)\leq\delta$. Under $P$, the [method of types](../../../information-theory.md#method-of-types) gives

$$
e_1^{(n)}
\leq(n+1)^{|A|}2^{-n\delta},
$$

so

$$
D_1(\delta)=\delta.
$$

Under $Q$, accepting $P$ requires a type in the closed set $\{R:D(R\Vert P)\leq\delta\}$. Therefore

$$
e_2^{(n)}
\leq(n+1)^{|A|}2^{-nD_2(\delta)},
$$

where

$$
D_2(\delta)
=\min_{R:D(R\Vert P)\leq\delta}D(R\Vert Q).
$$

Consequently $\limsup_n n^{-1}\log_2e_i^{(n)}\leq-D_i(\delta)$ for $i=1,2$. The first exponent is positive when $\delta>0$. Because relative entropy vanishes only when its arguments agree, the second is positive exactly while $Q$ lies outside the constraint set. Thus both are strictly positive for

$$
\boxed{0<\delta<D(Q\Vert P).}
$$

## 3

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [type](../../../information-theory.md#type-information-theory) of $x_1^n\in A^n$ is its empirical mass function

$$
\widehat P_{x_1^n}(a)
=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i=a\}},
\qquad a\in A.
$$

For a product source $Q^{\otimes n}$,

$$
\begin{aligned}
Q^{\otimes n}(x_1^n)
&=\prod_{i=1}^nQ(x_i)
=\prod_{a\in A}Q(a)^{n\widehat P_{x_1^n}(a)}\\
&=2^{-n\{H(\widehat P_{x_1^n})+D(\widehat P_{x_1^n}\Vert Q)\}},
\end{aligned}
$$

with the usual convention that the probability is zero if the string uses a symbol outside the support of $Q$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [type class](../../../information-theory.md#type-class) is

$$
T(P)=\{x_1^n:\widehat P_{x_1^n}=P\}.
$$

We first prove a multinomial-mode lemma. If $K=(K_a)_{a\in A}$ has the multinomial law with parameters $n$ and an $n$-type $P$, then $K=nP$ is a mode. Indeed, if $k_a<nP(a)$ and $k_b>nP(b)$, moving one count from $b$ to $a$ changes the probability by the factor

$$
\frac{P(a)}{P(b)}\frac{k_b}{k_a+1}\geq1.
$$

Repeated transfers reach $nP$ without decreasing probability. There are at most $(n+1)^m$ count vectors, so the modal vector has probability at least $(n+1)^{-m}$.

Every string in $T(P)$ has $P^{\otimes n}$-probability

$$
\prod_aP(a)^{nP(a)}=2^{-nH(P)}.
$$

The lemma therefore gives

$$
(n+1)^{-m}
\leq P^{\otimes n}(T(P))
=|T(P)|2^{-nH(P)},
$$

and hence

$$
\boxed{|T(P)|\geq(n+1)^{-m}2^{nH(P)}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Draw $X_1^n$ uniformly from $B$ and let $J$ be uniform on $\{1,\ldots,n\}$ independently. Then

$$
\mathbb P(X_J=a)
=\frac1{|B|}\sum_{x_1^n\in B}\widehat P_{x_1^n}(a)
=P_B(a).
$$

If $P_i$ denotes the marginal law of $X_i$, this also says $P_B=n^{-1}\sum_iP_i$. Since $X_1^n$ is uniform on $B$,

$$
\log_2|B|=H(X_1^n).
$$

[Subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy) followed by [concavity of information entropy](../../../information-theory.md#concavity-of-information-entropy) gives

$$
H(X_1^n)
\leq\sum_{i=1}^nH(P_i)
\leq nH\!\left(\frac1n\sum_{i=1}^nP_i\right)
=nH(P_B).
$$

Exponentiating proves $|B|\leq2^{nH(P_B)}$.

## 4

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The binary [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) says that codeword lengths $l_1,l_2,\ldots$ of a [prefix code](../../../coding-theory.md#prefix-code) satisfy

$$
\sum_i2^{-l_i}\leq1.
$$

Conversely, suppose positive integer lengths obey this inequality and arrange them in nondecreasing order. Construct codewords greedily in the infinite binary tree. Before assigning length $l_i$, each earlier codeword of length $l_j\leq l_i$ excludes exactly $2^{l_i-l_j}$ nodes at depth $l_i$. Thus the number excluded is

$$
\sum_{j<i}2^{l_i-l_j}
=2^{l_i}\sum_{j<i}2^{-l_j}
<2^{l_i},
$$

where strictness follows because the remaining term $2^{-l_i}$ occurs in the full Kraft sum. A free depth-$l_i$ node therefore exists. Assign it as the next codeword; choosing a node not below an earlier codeword preserves prefix-freeness. Induction constructs the required prefix code.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $p_k=\mathbb P(X=k)$. Monotonicity gives

$$
1\geq\sum_{j=1}^kp_j\geq kp_k,
$$

so $p_k\leq1/k$ and therefore $\log_2k\leq\log_2(1/p_k)$ whenever $p_k>0$. Hence

$$
\boxed{\mathbb E[\log_2X]
=\sum_{k\geq1}p_k\log_2k
\leq\sum_{k\geq1}p_k\log_2\frac1{p_k}
=H(X)<\infty.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A distribution on $\{1,2,\ldots\}$ must have $\mu\geq1$. For $\mu>1$, put $p=1/\mu$ and let

$$
G(k)=p(1-p)^{k-1}.
$$

For any mass function $P$ with mean $\mu$, [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) gives

$$
\begin{aligned}
D(P\Vert G)
&=-H(P)-\log_2p-(\mu-1)\log_2(1-p)\\
&=H(G)-H(P)\geq0.
\end{aligned}
$$

**Thus the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) uniquely maximizes entropy. For $\mu=1$, the only admissible law is the point mass at one, which is the limiting geometric case $p=1$.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For $\lambda\in\mathbb R$, define the finite-alphabet [exponential family](../../../exponential-family.md)

$$
P_\lambda(x)=\frac{2^{\lambda f(x)}}{Z(\lambda)},
\qquad
Z(\lambda)=\sum_{y\in A}2^{\lambda f(y)}.
$$

The mean $\mathbb E_{P_\lambda}f$ is continuous and nondecreasing in $\lambda$, with limits $\min f$ and $\max f$ as $\lambda\to-\infty$ and $+\infty$. The strict interior assumption on $v$ therefore supplies a $\lambda$ with $\mathbb E_{P_\lambda}f=v$.

For any other $P$ satisfying the same constraint,

$$
D(P\Vert P_\lambda)
=-H(P)-\lambda v+\log_2Z(\lambda),
$$

so

$$
H(P)=\log_2Z(\lambda)-\lambda v-D(P\Vert P_\lambda)
\leq H(P_\lambda).
$$

Equality in [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) holds only for $P=P_\lambda$. Hence this Gibbs-form mass function is the unique entropy maximizer.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
