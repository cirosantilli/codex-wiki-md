# Paper 224

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_224.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_224.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Because $X$ and $Y$ are [independent random variables](../../../random-variable.md#independent-random-variables), conditioning on $Y$ merely translates $X$. The [conditional entropy under a deterministic change of variables](../../../information-theory.md#conditional-entropy-under-a-deterministic-change-of-variables) and the fact that [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy) therefore give

$$
H(X+Y)\geq H(X+Y\mid Y)=H(X\mid Y)=H(X).
$$

Interchanging $X$ and $Y$ similarly gives $H(X+Y)\geq H(Y)$, and hence

$$
H(X+Y)\geq\max\{H(X),H(Y)\}.
$$

The proof applies to countable alphabets whenever the displayed [information entropies](../../../information-theory.md#information-entropy) are finite.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $p=(1+\mu)^{-1}$. Since $X$ and the [geometric random variable](../../../discrete-probability-distribution.md#geometric-distribution) $Z$ have the same [expected value](../../../probability-theory.md#expected-value) $\mu$,

$$
\begin{aligned}
D(P_X\Vert P_Z)
&=\sum_{k\geq0}P_X(k)\log_2\frac{P_X(k)}{p(1-p)^k}\\
&=-H(X)-\log_2p-\mu\log_2(1-p)\\
&=H(Z)-H(X).
\end{aligned}
$$

This is also the entropy deficit relative to the [maximum entropy distribution on the nonnegative integers](../../../information-theory.md#maximum-entropy-distribution-on-the-nonnegative-integers).

The random variables $X$ and $-Z$ are independent, so part a gives $H(X-Z)\geq H(-Z)=H(Z)$. Consequently

$$
\begin{aligned}
2d_R(X,Z)-D(P_X\Vert P_Z)
&=2H(X-Z)-H(X)-H(Z)-\{H(Z)-H(X)\}\\
&=2\{H(X-Z)-H(Z)\}\geq0,
\end{aligned}
$$

which is the required bound in terms of the [Entropic Ruzsa distance](../../../information-theory.md#entropic-ruzsa-distance).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $p_k=P_X(k)$. The assumption $p_0=0$ ensures that $X-1$ still takes values in $\{0,1,\ldots\}$, and its [probability mass function](../../../probability-theory.md#probability-mass-function) at $k$ is $p_{k+1}$. Using the paper's unhalved $\ell^1$ convention for the [total variation distance](../../../probability-and-statistics.md#total-variation-distance),

$$
\begin{aligned}
\lVert P_X-P_{X-1}\rVert_{\mathrm{TV}}
&=\sum_{k\geq0}|p_k-p_{k+1}|\\
&=\sum_{k\geq0}\{p_k+p_{k+1}-2\min(p_k,p_{k+1})\}\\
&=1+(1-p_0)-2q=2(1-q).
\end{aligned}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $M=\max_kp_k$ and choose an index $m$ with $p_m=M$. Splitting the overlap sum at $m$ gives

$$
q\leq\sum_{k<m}p_k+\sum_{k\geq m}p_{k+1}=1-p_m=1-M,
$$

so $1-q\geq M$. Moreover, [information entropy dominates min-entropy](../../../information-theory.md#information-entropy-dominates-min-entropy) gives $H(X)\geq-\log_2M$, and hence $2^{-H(X)}\leq M\leq1-q$.

Apply [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality) in natural logarithms. Because the paper writes total variation as the full $\ell^1$ distance, part c yields

$$
(\log_e2)D(P_X\Vert P_{X-1})
=D_e(P_X\Vert P_{X-1})
\geq\frac12\lVert P_X-P_{X-1}\rVert_1^2
=2(1-q)^2.
$$

Combining the two estimates proves

$$
(\log_e2)D(P_X\Vert P_{X-1})
\geq2(1-q)^2
\geq2M^2
\geq2^{-2H(X)+1}.
$$

## 2

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [type](../../../information-theory.md#type-information-theory) of $x_1^n\in A^n$ is its [empirical distribution](../../../information-theory.md#type-information-theory)

$$
\widehat P_{x_1^n}(a)=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i=a\}},
\qquad a\in A.
$$

Its [type class](../../../information-theory.md#type-class) is

$$
T(P)=\{y_1^n\in A^n:\widehat P_{y_1^n}=P\}.
$$

Every string in $T(P)$ has $Q^n$-probability

$$
\prod_{a\in A}Q(a)^{nP(a)}
=2^{-n\{H(P)+D(P\Vert Q)\}},
$$

while the [method of types](../../../information-theory.md#method-of-types) gives $|T(P)|\leq2^{nH(P)}$. Therefore

$$
\boxed{Q^n(T(P))\leq2^{-nD(P\Vert Q)}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The conditional [probability mass function](../../../probability-theory.md#probability-mass-function) is

$$
\boxed{P_n(x_1^n)
=\mathbb P(Y_1^n=x_1^n\mid Y_1^n\in B)
=\frac{Q^n(x_1^n)\mathbf1_{\{x_1^n\in B\}}}{Q^n(B)}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Conditionally on $X_1^n=x_1^n$, the [uniform](../../../continuous-probability-distribution.md#continuous-uniform-distribution) index $J$ selects the symbol $a$ with probability $\widehat P_{x_1^n}(a)$. The [law of total probability](../../../probability-theory.md#law-of-total-probability) therefore gives

$$
\overline P(a)
=\mathbb P(X_J=a)
=\sum_{x_1^n\in B}P_n(x_1^n)\widehat P_{x_1^n}(a)
=\sum_{x_1^n\in B}\frac{Q^n(x_1^n)}{Q^n(B)}\widehat P_{x_1^n}(a).
$$

**Thus $\overline P$ is the conditional mean type of a string in $B$.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $P_i$ be the marginal [probability distribution](../../../probability-theory.md#probability-distribution) of $X_i$. [Subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy) and the [concavity of information entropy](../../../information-theory.md#concavity-of-information-entropy) give

$$
H(X_1^n)\leq\sum_{i=1}^nH(P_i)
\leq nH\!\left(\frac1n\sum_{i=1}^nP_i\right).
$$

For each $a\in A$,

$$
\frac1n\sum_{i=1}^nP_i(a)
=\mathbb P(X_J=a)=\overline P(a),
$$

so $H(X_1^n)\leq nH(\overline P)$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Expand the logarithm of the [product measure](../../../probability-theory.md#product-measure) and exchange the finite sums:

$$
\begin{aligned}
\sum_{x_1^n\in B}P_n(x_1^n)\log_2Q^n(x_1^n)
&=\sum_{x_1^n\in B}P_n(x_1^n)\sum_{i=1}^n\log_2Q(x_i)\\
&=n\sum_{a\in A}\left\{\sum_{x_1^n\in B}P_n(x_1^n)\widehat P_{x_1^n}(a)\right\}\log_2Q(a)\\
&=n\sum_{a\in A}\overline P(a)\log_2Q(a),
\end{aligned}
$$

where part c identifies the expression in braces.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

On $B$, part b gives $\log_2P_n=\log_2Q^n-\log_2Q^n(B)$. Hence the [information entropy](../../../information-theory.md#information-entropy) of the conditional law satisfies

$$
H(X_1^n)
=-\sum_{x_1^n\in B}P_n(x_1^n)\log_2Q^n(x_1^n)
+\log_2Q^n(B).
$$

Parts d and e imply

$$
\begin{aligned}
\log_2Q^n(B)
&=H(X_1^n)+\sum_{x_1^n\in B}P_n(x_1^n)\log_2Q^n(x_1^n)\\
&\leq nH(\overline P)+n\sum_{a\in A}\overline P(a)\log_2Q(a)\\
&=-nD(\overline P\Vert Q).
\end{aligned}
$$

Exponentiation proves $Q^n(B)\leq2^{-nD(\overline P\Vert Q)}$.

## 3

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a binary [prefix code](../../../coding-theory.md#prefix-code) with length function $L_n:A^n\to\mathbb N$, the [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) is

$$
\boxed{\sum_{x_1^n\in A^n}2^{-L_n(x_1^n)}\leq1.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the direct half of the [code-distribution correspondence](../../../information-theory.md#code-distribution-correspondence), let $L$ be the length function of a binary prefix code and put

$$
K=\sum_x2^{-L(x)}\leq1,
\qquad
R(x)=\frac{2^{-L(x)}}K.
$$

Then $R$ is a [probability mass function](../../../probability-theory.md#probability-mass-function) and

$$
-\log_2R(x)=L(x)+\log_2K\leq L(x).
$$

Thus every prefix code determines a distribution whose ideal description lengths do not exceed the codeword lengths.

Conversely, given a probability mass function $R$, set

$$
L(x)=\left\lceil-\log_2R(x)\right\rceil
$$

for $R(x)>0$. Then $2^{-L(x)}\leq R(x)$, so the [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality) is satisfied. Its converse supplies a binary prefix code with these lengths, and

$$
-\log_2R(x)\leq L(x)<-\log_2R(x)+1.
$$

If real lengths are allowed, the ideal choice $L(x)=-\log_2R(x)$ satisfies Kraft with equality.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write $p(x)=\mathbb P(X_1^n=x)$, $a(x)=p(x)W(x)$, and

$$
A=\sum_xa(x)=\mathbb E[W(X_1^n)].
$$

On the support of $p$, define the [probability mass function](../../../probability-theory.md#probability-mass-function)

$$
R^*(x)=\frac{a(x)}A=\frac{p(x)W(x)}{\mathbb E[W(X_1^n)]}.
$$

For any real length function satisfying the [Kraft inequality](../../../coding-theory.md#kraft-mcmillan-inequality), put $K=\sum_x2^{-L(x)}\leq1$ and $R_L(x)=2^{-L(x)}/K$. The [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) gives

$$
\begin{aligned}
\sum_xa(x)L(x)
&=A\sum_xR^*(x)\{-\log_2R_L(x)-\log_2K\}\\
&=A\{H(R^*)+D(R^*\Vert R_L)-\log_2K\}\\
&\geq AH(R^*).
\end{aligned}
$$

Equality holds for the ideal weighted lengths

$$
L_n^*(x)=-\log_2R^*(x)
=\log_2\frac{\mathbb E[W(X_1^n)]}{p(x)W(x)}.
$$

Thus the smallest average weighted description length is

$$
\mathbb E[W(X_1^n)]
H\!\left(\frac{p(\mathord\cdot)W(\mathord\cdot)}{\mathbb E W(X_1^n)}\right).
$$

When $p$ has full support, the displayed $L_n^*$ attains this minimum. If some strings have zero probability, the same value is the infimum over finite lengths and is attained by the extended-real ideal assignment $L_n^*(x)=\infty$ there; finite codewords of arbitrarily large length approach it.

## 4

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $p_i=\mathbb P(X_i=1)$ and $\lambda=\sum_i p_i$. A relative-entropy form of the [Poisson approximation bound for dependent Bernoulli variables](../../../discrete-probability-distribution.md#poisson-approximation-bound-for-dependent-bernoulli-variables) is

$$
D_e(P_{S_n}\Vert\operatorname{Poisson}(\lambda))
\leq\sum_{i=1}^np_i^2
+\sum_{i=1}^nH_e(X_i)-H_e(X_1,\ldots,X_n).
$$

The last two terms form the [total correlation](../../../information-theory.md#total-correlation); they vanish when the Bernoulli variables are independent.

Here $D_e$ and $H_e$ use [natural logarithms](../../../calculus.md#natural-logarithm).

To prove the bound, let $Q_i$ be the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $p_i$ and let $Q=\bigotimes_iQ_i$. Expanding the [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) against this product law gives

$$
D_e(P_{X_1^n}\Vert Q)
=\sum_iD_e(\operatorname{Bernoulli}(p_i)\Vert\operatorname{Poisson}(p_i))
+\sum_iH_e(X_i)-H_e(X_1^n).
$$

The supplied one-dimensional estimate bounds the first sum by $\sum_i p_i^2$. Under the addition map, $P_{X_1^n}$ becomes $P_{S_n}$, while the [Sum of independent Poisson random variables](../../../discrete-probability-distribution.md#addition-of-independent-poisson-random-variables) under $Q$ has the Poisson distribution with mean $\lambda$. The [data processing inequality for relative entropy](../../../probability-and-statistics.md#data-processing-inequality-for-relative-entropy) proves the displayed result.

If a bound directly in the paper's unhalved total-variation norm is desired, [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality) also gives

$$
\boxed{\lVert P_{S_n}-\operatorname{Poisson}(\lambda)\rVert_1
\leq\sqrt{2\left\{\sum_i p_i^2+\sum_iH_e(X_i)-H_e(X_1^n)\right\}}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let

$$
S_n=\sum_{i=1}^nX_i^{(n)}.
$$

Here $S_n$ has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $(n,\lambda/n)$. Part a, now with independent coordinates, gives

$$
D_e(P_{S_n}\Vert\operatorname{Poisson}(\lambda))
\leq n(\lambda/n)^2=\frac{\lambda^2}{n}.
$$

By [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality), the probability mass functions therefore converge in total variation, and in particular $S_n$ [converges in distribution](../../../convergence-of-random-variables.md#convergence-in-distribution) to $Z\sim\operatorname{Poisson}(\lambda)$.

The joint probability of the observed row depends only on $S_n$:

$$
P_n(X_1^{(n)},\ldots,X_n^{(n)})
=\left(\frac\lambda n\right)^{S_n}
\left(1-\frac\lambda n\right)^{n-S_n}.
$$

Taking logarithms in any fixed base and choosing $c_n=\log n$ gives

$$
-\frac1{c_n}\log P_n(X_1^{(n)},\ldots,X_n^{(n)})
=a_nS_n+b_n,
$$

where

$$
a_n=\frac{\log(n/\lambda)+\log(1-\lambda/n)}{\log n}\longrightarrow1,
\qquad
b_n=-\frac{n\log(1-\lambda/n)}{\log n}\longrightarrow0.
$$

The convergence lemma supplied in the question now yields

$$
-\frac1{\log n}\log P_n(X_1^{(n)},\ldots,X_n^{(n)})
\xrightarrow{d}Z,
\qquad Z\sim\operatorname{Poisson}(\lambda).
$$

This sparse triangular array therefore has a random limiting normalized self-information rather than the constant limit in the usual [asymptotic equipartition property](../../../information-theory.md#asymptotic-equipartition-property).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
