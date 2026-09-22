# Paper 108

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_108.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_108.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Assume first that $\mu(A\cap T^{-n}A)=0$ for every $n\geq1$. For $n>m$ the [measure-preserving transformation](../../../measure-theory.md#measure-preserving-transformation) property gives

$$
\mu(T^{-m}A\cap T^{-n}A)=\mu(A\cap T^{-(n-m)}A)=0.
$$

Thus the sets $T^{-n}A$, $n\geq0$, are pairwise disjoint and all have measure $\mu(A)>0$, impossible in a probability space. Hence

$$
\boxed{\mu(A\cap T^{-n}A)>0\text{ for some }n>0.}
$$

The [Poincaré recurrence theorem](../../../measure-theory.md#poincare-recurrence-theorem) states that almost every $x\in A$ returns to $A$ infinitely often. Let

$$
E=\{x\in A:T^nx\notin A\text{ for every }n\geq1\}.
$$

The sets $T^{-n}E$ are pairwise disjoint: if $x$ belonged to the $m$th and $n$th inverse images with $m<n$, then $T^mx\in E$ would return to $E\subseteq A$ after $n-m$ steps. Invariance and finiteness therefore give $\mu(E)=0$. A point of $A$ with only finitely many returns belongs, after its last return, to some $T^{-k}E$. The countable union of these null sets is null, proving the theorem.

Now let $S\subseteq\mathbb Z$ have $d^*(S)>0$. Put $x=\mathbf1_S\in\{0,1\}^{\mathbb Z}$ and let $\sigma$ be the bilateral shift. Choose intervals $I_j$ with $|I_j|\to\infty$ and $|S\cap I_j|/|I_j|\to d^*(S)$. A weak-star limit of

$$
\mu_j=\frac1{|I_j|}\sum_{m\in I_j}\delta_{\sigma^m x}
$$

exists on the compact shift space. Boundary terms show that the limit $\mu$ is $\sigma$-invariant. For the cylinder $A=\{y:y_0=1\}$,

$$
\mu(A)=d^*(S)>0.
$$

The stated polynomial recurrence theorem supplies $n>0$ with $\mu(A\cap\sigma^{-|P(n)|}A)>0$. Hence that cylinder intersection meets the orbit closure of $x$; because it is open, some shift $\sigma^m x$ lies in it. Therefore $m,m+|P(n)|\in S$. Orient these two integers according to the sign of $P(n)$ to obtain

$$
\boxed{a,b\in S\quad\text{and}\quad b-a=P(n).}
$$

This is the [Furstenberg correspondence principle](../../../measure-theory.md#furstenberg-correspondence-principle).

## 2

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The statement $D\!\operatorname{-lim}a_n=a$ means [convergence in density of a sequence](../../../measure-theory.md#convergence-in-density-of-a-sequence): for every $\varepsilon>0$, the proportion of $n\leq N$ with $|a_n-a|\geq\varepsilon$ tends to zero. The statement $C\!\operatorname{-lim}a_n=a$ means [Cesaro convergence of a sequence](../../../measure-theory.md#cesaro-convergence-of-a-sequence), $N^{-1}\sum_{n=1}^Na_n\to a$.

Suppose $|a_n-a|\leq M$. Splitting into the indices where $|a_n-a|<\varepsilon$ and its complement gives

$$
\frac1N\sum_{n=1}^N|a_n-a|
\leq\varepsilon+M\frac{|\{n\leq N:|a_n-a|\geq\varepsilon\}|}{N}.
$$

Thus density convergence implies Cesaro convergence of the absolute deviations to zero. Conversely, the [Markov inequality](../../../probability-inequality.md#markov-inequality) gives

$$
\frac{|\{n\leq N:|a_n-a|\geq\varepsilon\}|}{N}
\leq\frac1{\varepsilon N}\sum_{n=1}^N|a_n-a|,
$$

proving the reverse implication.

The [product characterization of weak mixing](../../../measure-theory.md#product-characterization-of-weak-mixing) says that if $T$ is weakly mixing, then $T\times S$ is ergodic exactly when $S$ is ergodic; in particular, ergodicity of $T\times T$ characterizes weak mixing.

Suppose $U_Tf=\lambda f$. Unitarity of the [Koopman operator](../../../measure-theory.md#koopman-operator) gives $|\lambda|=1$. Weak mixing implies ergodicity, so $|f|$ is almost everywhere constant. On the product,

$$
F(x,y)=f(x)\overline{f(y)}
$$

is invariant under $T\times T$. Since the square is ergodic, $F$ is constant, which forces $f$ to be constant almost everywhere. Thus **there are no nonconstant Koopman eigenfunctions**.

Finally use the density-one correlation characterization of a [weakly mixing measure-preserving transformation](../../../measure-theory.md#weakly-mixing-measure-preserving-transformation). For each positive-measure pair $(A,B)$, the integers $n$ for which $\mu(T^{-n}A\cap B)>0$ form a density-one set after discarding finitely many terms; the corresponding sets for $(A,B)$ and $(A,C)$ therefore intersect, proving simultaneous hitting. Conversely, the simultaneous-hitting property is precisely the [simultaneous hitting characterization of weak mixing](../../../measure-theory.md#simultaneous-hitting-characterization-of-weak-mixing), so it implies weak mixing.

## 3

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a finite measurable partition $\xi$,

$$
H_\mu(\xi)=-\sum_{A\in\xi}\mu(A)\log\mu(A).
$$

Its [conditional entropy of finite measurable partitions](../../../measure-theory.md#conditional-entropy-of-finite-measurable-partitions) relative to $\eta$ is

$$
H_\mu(\xi\mid\eta)
=\sum_{B\in\eta}\mu(B)
\left[-\sum_{A\in\xi}\mu(A\mid B)\log\mu(A\mid B)\right].
$$

The concavity of $-t\log t$, equivalently [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy), gives

$$
\boxed{H_\mu(\xi\mid\eta)\leq H_\mu(\xi).}
$$

The atoms of $T^{-1}\xi$ are $T^{-1}A$ with the same measures as the atoms $A$ of $\xi$. Hence $\boxed{H_\mu(T^{-1}\xi)=H_\mu(\xi)}$.

Set

$$
a_N=H_\mu\left(\bigvee_{n=0}^{N-1}T^{-n}\xi\right).
$$

The chain rule and invariance give $a_{N+M}\leq a_N+a_M$, so $(a_N)$ is a [subadditive sequence](../../../real-analysis.md#subadditive-sequence). Therefore

$$
h_\mu(T,\xi)=\lim_{N\to\infty}\frac{a_N}{N}
=\inf_{N\geq1}\frac{a_N}{N}.
$$

The [Kolmogorov-Sinai entropy](../../../measure-theory.md#kolmogorov-sinai-entropy) is $h_\mu(T)=\sup_\xi h_\mu(T,\xi)$ over finite partitions.

Taking $F=\{0,\ldots,N-1\}$ immediately shows that the infimum over arbitrary finite $F$ is at most $h_\mu(T,\xi)$. For the reverse inequality, apply [Shearer's inequality](../../../information-theory.md#shearer-s-inequality) to translates of a fixed finite $F$ inside a long interval. Every interior coordinate is covered $|F|$ times, while only $O(\max F)$ boundary coordinates are lost. Subadditivity bounds the boundary contribution; division by the interval length and passage to the limit give

$$
h_\mu(T,\xi)\leq\frac1{|F|}H_\mu\left(\bigvee_{n\in F}T^{-n}\xi\right).
$$

Taking the infimum proves

$$
\boxed{h_\mu(T,\xi)=\inf_{\varnothing\ne F\subseteq\mathbb Z_{\geq0}\text{ finite}}
\frac1{|F|}H_\mu\left(\bigvee_{n\in F}T^{-n}\xi\right).}
$$

## 4

↑ **Parent:** [Paper 108](paper-108.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a finite partition $\xi$, put

$$
\mathcal F_n(\xi)=\bigvee_{k=n}^{\infty}T^{-k}\xi.
$$

The system is [K-mixing](../../../measure-theory.md#k-mixing) when every measurable $A$ becomes uniformly asymptotically independent of this remote future:

$$
\sup_{B\in\mathcal F_n(\xi)}|\mu(A\cap B)-\mu(A)\mu(B)|\longrightarrow0.
$$

Taking $\xi=\{B,X\setminus B\}$ makes $T^{-n}B\in\mathcal F_n(\xi)$, so

$$
\mu(A\cap T^{-n}B)\longrightarrow\mu(A)\mu(B).
$$

Thus **K-mixing implies mixing**.

The [tail sigma-algebra of a measurable partition](../../../measure-theory.md#tail-sigma-algebra-of-a-measurable-partition) is

$$
\mathcal T(\xi)=\bigcap_{n\geq0}\mathcal F_n(\xi).
$$

By the [reverse martingale convergence theorem](../../../martingale.md#reverse-martingale-convergence-theorem),

$$
\mathbb E[\mathbf1_A\mid\mathcal F_n(\xi)]
\longrightarrow
\mathbb E[\mathbf1_A\mid\mathcal T(\xi)]
$$

in $L^1$. The uniform independence in the definition of K-mixing is equivalent to the limit being the constant $\mu(A)$ for every $A$. This holds exactly when every $\mathcal T(\xi)$-measurable set has measure zero or one. Hence the system is K-mixing if and only if every finite partition has trivial tail sigma-algebra.

Let $\mathcal P=\{A:h_\mu(T,\xi_A)=0\}$. Complements preserve the binary partition. If $A,B\in\mathcal P$, then $\xi_{A\cup B}$ is coarser than $\xi_A\vee\xi_B$, so subadditivity gives zero entropy rate. Thus $\mathcal P$ is an algebra. For $A=\bigcup_{j\geq1}A_j$, let $A^{(m)}=\bigcup_{j\leq m}A_j$. The entropy metric continuity bound

$$
|h_\mu(T,\xi_A)-h_\mu(T,\xi_{A^{(m)}})|
\leq H_\mu(\xi_A\mid\xi_{A^{(m)}})+H_\mu(\xi_{A^{(m)}}\mid\xi_A)
$$

tends to zero because $\mu(A\mathbin\triangle A^{(m)})\to0$. Hence $A\in\mathcal P$, proving that $\mathcal P$ is a sigma-algebra: the [Pinsker sigma-algebra](../../../measure-theory.md#pinsker-sigma-algebra).

If $A$ belongs modulo null sets to $\mathcal T(\xi)$ for a finite $\xi$, remote-future approximations make the entropy rate of $\xi_A$ zero. Conversely, if $h_\mu(T,\xi_A)=0$, the conditional-entropy formula for entropy rate gives

$$
H_\mu\left(\xi_A\,middle|\,\bigvee_{n=1}^{\infty}T^{-n}\xi_A\right)=0.
$$

Thus $A$ is measurable modulo null sets from its strict future. Iterating this fact makes it measurable from every remote future, so $A\in\mathcal T(\xi_A)$ modulo null sets. Therefore

$$
\boxed{A\in\mathcal P\iff
\exists\text{ finite }\xi\ \exists A'\in\mathcal T(\xi):
\mu(A\mathbin\triangle A')=0.}
$$

This is the [Tail characterization of the Pinsker sigma-algebra](../../../measure-theory.md#tail-characterization-of-the-pinsker-sigma-algebra).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
