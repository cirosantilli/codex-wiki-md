# Paper 224

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20224.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20224.pdf)

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

Suppose $X\to Y\to Z$ is a [Markov chain](../../../markov-process.md#markov-chain), so $I(X;Z\mid Y)=0$. The [chain rule for mutual information](../../../information-theory.md#chain-rule-for-mutual-information) gives

$$
I(X;Y,Z)=I(X;Y)+I(X;Z\mid Y)=I(X;Y)
$$

and also

$$
I(X;Y,Z)=I(X;Z)+I(X;Y\mid Z)\geq I(X;Z),
$$

because [conditional mutual information](../../../information-theory.md#conditional-mutual-information) is nonnegative. Therefore $I(X;Z)\leq I(X;Y)$. Similarly,

$$
I(X,Y;Z)=I(Y;Z)+I(X;Z\mid Y)=I(Y;Z)
$$

while $I(X,Y;Z)=I(X;Z)+I(Y;Z\mid X)\geq I(X;Z)$, so $I(X;Z)\leq I(Y;Z)$. These are the two [data processing inequalities](../../../information-theory.md#data-processing-inequality). In particular, applying any deterministic function or [Markov kernel](../../../markov-process.md#markov-kernel) to either argument cannot increase [mutual information](../../../information-theory.md#mutual-information).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Independence makes

$$
X\longrightarrow X+Y\longrightarrow X+Y+Z
$$

a [Markov chain](../../../markov-process.md#markov-chain). The [data processing inequality for mutual information](../../../information-theory.md#data-processing-inequality) therefore gives $I(X;X+Y+Z)\leq I(X;X+Y)$. Translation by the known value of $X$ is a [bijection](../../../function.md#bijection), so [conditional entropy](../../../information-theory.md#conditional-entropy) and independence give

$$
I(X;X+Y+Z)=H(X+Y+Z)-H(Y+Z),
$$

and $I(X;X+Y)=H(X+Y)-H(Y)$. Rearranging proves the stated [entropy submodularity for three independent sums](../../../information-theory.md#entropy-submodularity-for-three-independent-sums):

$$
H(X+Y+Z)+H(Y)\leq H(X+Y)+H(Y+Z).
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Because the [Entropic Ruzsa distance](../../../information-theory.md#entropic-ruzsa-distance) depends only on marginal distributions, take $X,Y,Z$ independent with the required marginals. Since $X-Z=(X-Y)+(Y-Z)$ is a function of $(X-Y,Y-Z)$, the [data processing inequality for mutual information](../../../information-theory.md#data-processing-inequality) yields

$$
I\bigl(X;(X-Y,Y-Z)\bigr)\geq I(X;X-Z).
$$

The map $(X,X-Y,Y-Z)\mapsto(X,Y,Z)$ is a [bijection](../../../function.md#bijection). Using independence and the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy), the left side is

$$
H(X-Y,Y-Z)-H(Y)-H(Z),
$$

whereas the right side is $H(X-Z)-H(Z)$. Hence

$$
H(X-Z)+H(Y)\leq H(X-Y,Y-Z)
\leq H(X-Y)+H(Y-Z),
$$

where the final step is [subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy). Substituting this inequality into the definition of $d_R$ gives the [Entropic Ruzsa triangle inequality](../../../information-theory.md#entropic-ruzsa-triangle-inequality)

$$
\boxed{d_R(X,Z)\leq d_R(X,Y)+d_R(Y,Z).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Let $X_1,X_2,Y$ be independent, with $X_1,X_2$ distributed as $X$. Apply part (b) to $X_1,-Y,X_2$:

$$
H(X_1+X_2-Y)+H(Y)\leq2H(X-Y).
$$

Adding an [independent random variable](../../../random-variable.md#independent-random-variables) cannot decrease [information entropy](../../../information-theory.md#information-entropy), so

$$
H(X_1+X_2)+H(Y)\leq2H(X-Y).
$$

In terms of [Entropic Ruzsa distance](../../../information-theory.md#entropic-ruzsa-distance), this is $d_R(X,-X)\leq2d_R(X,Y)$. The [Entropic Ruzsa triangle inequality](../../../information-theory.md#entropic-ruzsa-triangle-inequality) and invariance under simultaneous negation now give

$$
d_R(X,-Y)
\leq d_R(X,-X)+d_R(-X,-Y)
\leq2d_R(X,Y)+d_R(X,Y),
$$

which is the [Entropic Ruzsa sum-difference inequality](../../../information-theory.md#entropic-ruzsa-sum-difference-inequality).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For independent $X,Y$, expand the [Entropic Ruzsa sum-difference inequality](../../../information-theory.md#entropic-ruzsa-sum-difference-inequality) from part (d):

$$
H(X+Y)-\frac12H(X)-\frac12H(Y)
\leq3\left(H(X-Y)-\frac12H(X)-\frac12H(Y)\right).
$$

Collecting the [information entropy](../../../information-theory.md#information-entropy) terms gives

$$
H(X+Y)+H(X)+H(Y)\leq3H(X-Y).
$$

Replacing $Y$ by $-Y$ interchanges sum and difference and preserves $H(Y)$, yielding the requested orientation

$$
\boxed{H(X-Y)+H(X)+H(Y)\leq3H(X+Y).}
$$

## 2

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $P\ne Q$ be [probability mass functions](../../../probability-theory.md#probability-mass-function) on a finite [alphabet](../../../information-theory.md#alphabet), with $P$ absolutely continuous with respect to $Q$. A decision region $B_n$ accepts the null law $P^{\otimes n}$. Write

$$
\alpha_n=P^{\otimes n}(B_n^c),\qquad
\beta_n=Q^{\otimes n}(B_n)
$$

for its type-I and type-II errors. [Stein's lemma](../../../information-theory.md#stein-s-lemma-information-theory) states that for every fixed $0<\varepsilon<1$,

$$
\lim_{n\to\infty}-\frac1n\log
\inf_{B_n:\,\alpha_n\leq\varepsilon}\beta_n
=D(P\Vert Q),
$$

where logarithms and [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) use base two.

For achievability, let

$$
B_n=\left\{x_1^n:\frac1n\log
\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\geq D(P\Vert Q)-\eta\right\}.
$$

Under $P^{\otimes n}$, the normalized log-likelihood ratio converges in probability to $D(P\Vert Q)$ by the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers), so $alpha_n\to0$. On $B_n$, $Q^{\otimes n}\leq2^{-n(D(P\Vert Q)-\eta)}P^{\otimes n}$, whence $\beta_n\leq2^{-n(D(P\Vert Q)-\eta)}$.

For the converse, let

$$
A_n=\left\{x_1^n:\frac1n\log
\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
\leq D(P\Vert Q)+\eta\right\}.
$$

Again $P^{\otimes n}(A_n)\to1$. If $alpha_n\leq\varepsilon$, then

$$
\beta_n\geq Q^{\otimes n}(B_n\cap A_n)
\geq2^{-n(D(P\Vert Q)+\eta)}P^{\otimes n}(B_n\cap A_n).
$$

The final factor has positive lower limit at least $1-\varepsilon$. Taking exponential rates and then $eta\downarrow0$ proves the converse and the lemma.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Neyman-Pearson decision region](../../../information-theory.md#neyman-pearson-decision-region) accepting $P^{\otimes n}$ is

$$
B_n(t)=\left\{x_1^n:
\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}\geq t
\right\},
$$

with randomization on the boundary when needed. If $R=\widehat P_{x_1^n}$ is the [type](../../../information-theory.md#type-information-theory) of the observed string, then

$$
\frac1n\log\frac{P^{\otimes n}(x_1^n)}{Q^{\otimes n}(x_1^n)}
=D(R\Vert Q)-D(R\Vert P).
$$

Thus the equivalent [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) form is

$$
\boxed{B_n(t)=\{x_1^n:D(\widehat P_{x_1^n}\Vert Q)
-D(\widehat P_{x_1^n}\Vert P)\geq n^{-1}\log t\}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let

$$
\mathcal C_\delta=\{R:D(R\Vert P)\leq\delta\},
\qquad
D(\delta)=\min_{R\in\mathcal C_\delta}D(R\Vert Q).
$$

The minimum exists because the probability simplex is compact. Let $R^*$ be the [information projection](../../../information-theory.md#information-projection) of $Q$ onto the closed [convex set](../../../mathematical-optimization.md#convex-set) $\mathcal C_\delta$. Its Pythagorean inequality says that every $R\in\mathcal C_\delta$ satisfies

$$
D(R\Vert Q)-D(R\Vert R^*)\geq D(R^*\Vert Q)=D(\delta).
$$

For a string $x_1^n$ of [type](../../../information-theory.md#type-information-theory) $R\in\mathcal C_\delta$, this gives

$$
\frac{Q^{\otimes n}(x_1^n)}{(R^*)^{\otimes n}(x_1^n)}
=2^{-n[D(R\Vert Q)-D(R\Vert R^*)]}
\leq2^{-nD(\delta)}.
$$

Summing over the decision region $B_n$ proves the exact bound

$$
\boxed{e_1^{(n)}=Q^{\otimes n}(B_n)
\leq2^{-nD(\delta)}(R^*)^{\otimes n}(B_n)
\leq2^{-nD(\delta)}.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Here $e_2^{(n)}=P^{\otimes n}(B_n^c)$. The [method of types](../../../information-theory.md#method-of-types) gives at most $(n+1)^{|A|}$ possible values of [type](../../../information-theory.md#type-information-theory), and a type class $T_R$ has

$$
P^{\otimes n}(T_R)\leq2^{-nD(R\Vert P)}.
$$

Every [type](../../../information-theory.md#type-information-theory) in $B_n^c$ has $D(R\Vert P)>\delta$, so

$$
e_2^{(n)}
\leq(n+1)^{|A|}2^{-n\delta}.
$$

The polynomial prefactor has zero exponential rate. Therefore

$$
\boxed{\limsup_{n\to\infty}\frac1n\log e_2^{(n)}\leq-\delta.}
$$

## 3

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For nonnegative numbers $a_i,b_i$, put $a=\sum_i a_i$ and $b=\sum_i b_i$. The [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality) is

$$
\sum_i a_i\log\frac{a_i}{b_i}\geq a\log\frac ab,
$$

with $0\log(0/b)=0$ and the usual extended-value convention when a denominator vanishes. Equality holds precisely when $a_i/b_i$ is constant over the indices with $a_i>0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $K(y\mid x)$ be a [Markov kernel](../../../markov-process.md#markov-kernel), and let $P_Y=PK$, $Q_Y=QK$ be the output [probability distributions](../../../probability-theory.md#probability-distribution). Applying the [log-sum inequality](../../../probability-and-statistics.md#log-sum-inequality) for each $y$ to $a_x=P(x)K(y\mid x)$ and $b_x=Q(x)K(y\mid x)$ gives

$$
\sum_xP(x)K(y\mid x)\log\frac{P(x)}{Q(x)}
\geq P_Y(y)\log\frac{P_Y(y)}{Q_Y(y)}.
$$

Summing over $y$ and using $\sum_yK(y\mid x)=1$ yields the [data processing inequality for relative entropy](../../../probability-and-statistics.md#data-processing-inequality-for-relative-entropy)

$$
\boxed{D(PK\Vert QK)\leq D(P\Vert Q).}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The elementary [logarithm inequality](../../../calculus.md#logarithm-inequality) $\log_2u\leq(\log_2e)(u-1)$ gives

$$
D(P\Vert Q)
\leq(\log e)\sum_xP(x)\left(\frac{P(x)}{Q(x)}-1\right).
$$

Since $\sum_x(P(x)-Q(x))=0$,

$$
\sum_xP(x)\frac{P(x)-Q(x)}{Q(x)}
=\sum_x\frac{(P(x)-Q(x))^2}{Q(x)}
=\chi^2(P\Vert Q).
$$

This proves $D(P\Vert Q)\leq(\log e)\chi^2(P\Vert Q)$, relating [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) to [chi-squared divergence](../../../probability-and-statistics.md#chi-squared-divergence).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Writing $P,Q$ for the laws of $X,Y$, respectively, and using [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) for the concave [natural logarithm](../../../calculus.md#natural-logarithm),

$$
\begin{aligned}
\mathbb E_Pg-D_e(P\Vert Q)
&=\sum_xP(x)\log_e\frac{e^{g(x)}Q(x)}{P(x)}\\
&\leq\log_e\sum_xP(x)\frac{e^{g(x)}Q(x)}{P(x)}\\
&=\log_e\mathbb E_Qe^{g(Y)}.
\end{aligned}
$$

This is the lower-bound half of the [Gibbs variational principle for relative entropy](../../../probability-and-statistics.md#gibbs-variational-principle-for-relative-entropy).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $Z=\mathbb E_Qe^g$ and define the exponentially tilted [probability mass function](../../../probability-theory.md#probability-mass-function)

$$
P^*(x)=\frac{Q(x)e^{g(x)}}Z.
$$

For this choice every ratio $e^{g(x)}Q(x)/P^*(x)$ equals $Z$, so equality holds in the [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) used in part (d). Hence

$$
\log_e\mathbb E_Qe^g
=\sup_P\{\mathbb E_Pg-D_e(P\Vert Q)\},
$$

and $P^*$ is the maximizer. This is the finite-alphabet [Gibbs variational principle for relative entropy](../../../probability-and-statistics.md#gibbs-variational-principle-for-relative-entropy).

## 4

↑ **Parent:** [Paper 224](paper-224.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For $\mu>0$, let $Q$ be the [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution)

$$
Q(k)=\frac1{1+\mu}\left(\frac\mu{1+\mu}\right)^k,
\qquad k\geq0.
$$

If $P$ is the law of $X$, [Gibbs inequality](../../../probability-and-statistics.md#gibbs-inequality) gives

$$
0\leq D(P\Vert Q)
=-H(X)+\log(1+\mu)+\mu\log\frac{1+\mu}{\mu}.
$$

Therefore

$$
H(X)\leq\log(1+\mu)+\mu\log\frac{1+\mu}{\mu}
=(1+\mu)h\left(\frac1{1+\mu}\right).
$$

For $\mu=0$, the nonnegative random variable $X$ is zero almost surely and both sides vanish. This proves that the [maximum entropy distribution on the nonnegative integers](../../../information-theory.md#maximum-entropy-distribution-on-the-nonnegative-integers) with fixed [expected value](../../../probability-theory.md#expected-value) is geometric.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Order the symbols so that $p_1\geq p_2\geq\cdots$. For each $l\geq0$, there are exactly $2^l$ binary strings of length $l$, while precisely the indices

$$
2^l\leq i\leq2^{l+1}-1
$$

satisfy $\lfloor\log i\rfloor=l$. Assign those $2^l$ symbols bijectively to the strings of length $l$. The resulting map is an [injective function](../../../algebra.md#injective-function) and hence a [one-to-one source code](../../../information-theory.md#one-to-one-source-code), with $L^*(x_i)=\lfloor\log i\rfloor$. Assigning shorter available words to more probable symbols also shows that this is an [optimal one-to-one binary code](../../../information-theory.md#optimal-one-to-one-binary-code).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Monotonicity of the ordered probabilities gives $ip_i\leq\sum_{j\leq i}p_j\leq1$, so $\log i\leq-\log p_i$. Consequently

$$
\mathbb E[L^*(X)]
=\sum_ip_i\lfloor\log i\rfloor
\leq\sum_ip_i\log i
\leq H(X).
$$

Given $L^*(X)=l$, the source symbol can take at most $2^l$ values. The [maximum entropy distribution on a finite set](../../../information-theory.md#maximum-entropy-distribution-on-a-finite-set) is uniform, hence

$$
H(X\mid L^*(X)=l)\leq\log2^l=l.
$$

Averaging this [conditional entropy](../../../information-theory.md#conditional-entropy) inequality proves

$$
\boxed{H(X\mid L^*(X))\leq\mathbb E[L^*(X)].}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Put $L=L^*(X)$ and $\mu=\mathbb E L$. Since $L$ is a function of $X$, the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) and part (c) give

$$
H(X)=H(L)+H(X\mid L)\leq H(L)+\mu.
$$

Part (a), applied to the nonnegative integer-valued random variable $L$, yields

$$
H(L)\leq(1+\mu)h\left(\frac1{1+\mu}\right)
=\log(1+\mu)+\mu\log\left(1+\frac1\mu\right).
$$

The [logarithm inequality](../../../calculus.md#logarithm-inequality) $\log(1+t)\leq t\log e$ implies $\mu\log(1+1/\mu)\leq\log e$. Thus

$$
H(X)\leq\mu+\log(1+\mu)+\log e.
$$

Part (c) also gives $\mu\leq H(X)$, so monotonicity of the [logarithm](../../../calculus.md#logarithm) lets us replace $\log(1+\mu)$ by $\log(H(X)+1)$. Rearranging proves

$$
\boxed{\mathbb E[L^*(X)]
\geq H(X)-\log[H(X)+1]-\log e.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
