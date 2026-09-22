# Paper 101

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20101%20updated.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20101%20updated.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)

## 1

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Tensor-hom adjunction](../../../module-theory.md#tensor-hom-adjunction) is the natural isomorphism

$$
\Phi_{M,N,P}:\operatorname{Hom}_R(M\otimes_RN,P)
\longrightarrow
\operatorname{Hom}_R\bigl(M,\operatorname{Hom}_R(N,P)\bigr).
$$

For an [R-module homomorphism](../../../module-theory.md#module-homomorphism) $f$, it is given explicitly by

$$
\Phi(f)(m)(n)=f(m\otimes n).
$$

Conversely, an $R$-linear map $g:M\to\operatorname{Hom}_R(N,P)$ determines the [balanced map](../../../module-theory.md#balanced-map) $(m,n)\mapsto g(m)(n)$, so the [universal property of the tensor product of modules](../../../module-theory.md#universal-property-of-the-tensor-product-of-modules) gives

$$
\Phi^{-1}(g)(m\otimes n)=g(m)(n).
$$

These formulas are inverse to each other because pure tensors generate the [tensor product of modules](../../../module-theory.md#tensor-product-of-modules).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $u:M'\to M$ be an [R-module homomorphism](../../../module-theory.md#module-homomorphism). Naturality in the left argument means that precomposition by $u\otimes1_N$ on the left corresponds under the [Tensor-hom adjunction](../../../module-theory.md#tensor-hom-adjunction) to precomposition by $u$ on the right. For $f:M\otimes_RN\to P$,

$$
\begin{aligned}
\Phi_{M',N,P}\bigl(f\circ(u\otimes1_N)\bigr)(m')(n)
&=f\bigl(u(m')\otimes n\bigr)\\
&=\Phi_{M,N,P}(f)\bigl(u(m')\bigr)(n).
\end{aligned}
$$

**Thus the naturality square commutes pointwise on every $m'\in M'$ and $n\in N$.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

**No.** Let $Q$ be the [quiver](../../../algebra.md#quiver) $1\to2$ over a field $k$, and take the [representation of a quiver](../../../algebra.md#representation-of-a-quiver)

$$
k\xrightarrow{1_k}k.
$$

An [endomorphism](../../../algebra.md#endomorphism) is a pair of scalar maps $(a,b)$ satisfying $b=a$, so its [endomorphism ring](../../../module-theory.md#endomorphism-ring) is $k$. Every nonzero endomorphism is therefore an [isomorphism](../../../algebra.md#isomorphism), making this representation a [brick module](../../../module-theory.md#brick-module). It nevertheless has the proper nonzero subrepresentation $0\to k$, so it is not an [irreducible module](../../../module-theory.md#irreducible-module).

Equivalently, this is a nonsimple module over the [path algebra](../../../algebra.md#path-algebra) $kQ$ whose endomorphism ring is a division ring.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Write the nonsplit [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
0\longrightarrow L\xrightarrow{j}M\xrightarrow{q}N\longrightarrow0.
$$

For an endomorphism $g:M\to M$, the composite $qgj:L\to N$ vanishes because $\operatorname{Hom}_R(L,N)=0$. Hence $g$ restricts to an endomorphism $f$ of $L$ and induces an endomorphism $h$ of $N$, giving a [commutative diagram](../../../homology.md#commutative-diagram) of short exact sequences.

Because $L$ and $N$ are [brick modules](../../../module-theory.md#brick-module), each of $f,h$ is either zero or an isomorphism. If both are isomorphisms, the [short five lemma](../../../module-theory.md#short-five-lemma) makes $g$ an isomorphism. If both vanish, $g$ factors successively through $N$ and through $L$, hence through a map $N\to L$; this map is zero, so $g=0$.

The mixed cases would split the sequence. If $f$ is invertible and $h=0$, then $qg=0$, so $g=j\alpha$ for some $\alpha:M\to L$; the identity $\alpha j=f$ makes $f^{-1}\alpha$ a retraction of $j$. If $f=0$ and $h$ is invertible, then $gj=0$, so $g=\beta q$; the identity $q\beta=h$ makes $\beta h^{-1}$ a section of $q$. Both contradict nonsplitting. Thus every endomorphism of $M$ is zero or invertible, and $M$ is a brick.

## 2

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [minimal primary decomposition](../../../commutative-algebra.md#minimal-primary-decomposition) is an expression

$$
I=Q_1\cap\cdots\cap Q_s
$$

in which every $Q_i$ is a [primary ideal](../../../commutative-algebra.md#primary-ideal), the prime ideals $\sqrt{Q_i}$ are pairwise distinct, and the decomposition is irredundant: deleting any $Q_i$ changes the intersection.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Second uniqueness theorem for primary decomposition](../../../commutative-algebra.md#second-uniqueness-theorem-for-primary-decomposition) says that in a minimal primary decomposition of an ideal in a [Noetherian ring](../../../algebra.md#noetherian-ring), every primary component belonging to an isolated prime is unique. Here an isolated prime is a minimal member of the set $\{\sqrt{Q_i}\}$.

Let $\mathfrak p=\sqrt{Q_i}$ be isolated and apply [localization at a prime ideal](../../../commutative-algebra.md#localization-at-a-prime-ideal). If $j\ne i$, minimality of $\mathfrak p$ gives $\sqrt{Q_j}\nsubseteq\mathfrak p$, so some element of $Q_j$ becomes a unit in $R_{\mathfrak p}$. Consequently

$$
IR_{\mathfrak p}=Q_iR_{\mathfrak p}.
$$

Because $Q_i$ is $\mathfrak p$-primary, multiplication by any $s\notin\mathfrak p$ cannot carry an element outside $Q_i$ into $Q_i$. Therefore

$$
Q_i=Q_iR_{\mathfrak p}\cap R=IR_{\mathfrak p}\cap R.
$$

The right side depends only on $I$ and $\mathfrak p$, proving uniqueness.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**No.** Take the [Noetherian ring](../../../algebra.md#noetherian-ring) $R=k[x]$, the finitely generated $R$-module

$$
M=R\oplus R/(x),
$$

and $N=0$. Its [annihilator of a module](../../../module-theory.md#annihilator-of-a-module) is

$$
\operatorname{Ann}_R(M)=0,
$$

which is a [prime ideal](../../../commutative-algebra.md#prime-ideal) and hence a [primary ideal](../../../commutative-algebra.md#primary-ideal). But with $r=x$ and $m=(0,\overline1)$ we have $m\ne0$ and $rm=0$, while $x^kM\ne0$ for every $k$ because the free summand survives. Thus $N$ is not a [primary submodule](../../../module-theory.md#primary-submodule).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Pass to $A=R/I$. It is enough to prove that the zero ideal of $A[t]$ is primary. The zero ideal of $A$ is primary, so every [zero divisor](../../../mathematics.md#zero-divisor) of $A$ is [nilpotent element](../../../commutative-algebra.md#nilpotent).

Suppose $fg=0$ in $A[t]$ with $g\ne0$. By [McCoy theorem](../../../commutative-algebra.md#mccoy-theorem), some nonzero $a\in A$ satisfies $af=0$. Hence every coefficient of $f$ is a zero divisor and therefore nilpotent. There are only finitely many coefficients, so the ideal they generate is nilpotent; consequently some power of $f$ is zero. This proves that $(0)$ is primary in $A[t]$, and the [coefficientwise quotient of a polynomial ring](../../../commutative-algebra.md#coefficientwise-quotient-of-a-polynomial-ring)

$$
R[t]/I^e\cong(R/I)[t]
$$

shows that $I^e$ is primary.

## 3

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Going-down theorem](../../../commutative-algebra.md#going-down-theorem) states: let $R\subseteq A$ be an [integral extension](../../../commutative-algebra.md#integral-extension) of [integral domains](../../../commutative-algebra.md#integral-domain), with $R$ integrally closed in its [fraction field](../../../commutative-algebra.md#field-of-fractions). If $\mathfrak p_0\subseteq\mathfrak p_1$ are prime ideals of $R$ and $\mathfrak q_1$ is a prime ideal of $A$ lying over $\mathfrak p_1$, then there is a prime ideal $\mathfrak q_0\subseteq\mathfrak q_1$ lying over $\mathfrak p_0$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $K=\operatorname{Frac}R$, let

$$
f(T)=T^d+a_{d-1}T^{d-1}+\cdots+a_0
$$

be the [minimal polynomial of an algebraic element](../../../galois-theory.md#minimal-polynomial-of-an-algebraic-element) $y$ over $K$, and let $B$ be the integral closure of $R$ in a finite normal extension containing all roots of $f$. Since $y$ is integral over $R$ and $R$ is [integrally closed domain](../../../commutative-algebra.md#integrally-closed-domain), every $a_i$ belongs to $R$.

Write $y=\sum_jp_jz_j$ with $p_j\in\mathfrak p$ and $z_j\in A$. Every $K$-embedding into the normal extension fixes the $p_j$ and sends each $z_j$ to an element integral over $R$. Thus every conjugate of $y$ lies in the extended ideal $\mathfrak pB$. Each nonleading coefficient of $f$ is, up to sign, an [elementary symmetric polynomial](../../../polynomial.md#elementary-symmetric-polynomial) in those conjugates, so it lies in $\mathfrak pB\cap R$.

For an [integral extension](../../../commutative-algebra.md#integral-extension), extension followed by contraction preserves a prime ideal:

$$
\mathfrak pB\cap R=\mathfrak p.
$$

Indeed, the determinant trick gives $r^m\in\mathfrak p$ for $r\in\mathfrak pB\cap R$, and primality then gives $r\in\mathfrak p$. Hence $a_i\in\mathfrak p$ for every $i<d$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

As an $A'$-algebra, $A\otimes_RA'$ is generated by the elements $a\otimes1$. If $a$ obeys a monic relation

$$
a^d+r_{d-1}a^{d-1}+\cdots+r_0=0
$$

over $R$, then $a\otimes1$ obeys the same monic relation after applying the structure map $R\to A'$. Thus every generator is an [integral element](../../../commutative-algebra.md#integral-element). The [subalgebra generated by finitely many integral elements](../../../commutative-algebra.md#subalgebra-generated-by-finitely-many-integral-elements) is finite as a module, and therefore integral; each tensor involves only finitely many generators. Hence $A\otimes_RA'$ is integral over $A'$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

If the coefficients of $p$ are integral over $R$, they generate a finite $R$-algebra $B$. Then $B[t_1,\ldots,t_n]$ is a finite $R[t_1,\ldots,t_n]$-module, so every one of its elements, including $p$, is integral.

Conversely, use the fact that the [integral closure of a graded ring is graded](../../../commutative-algebra.md#integral-closure-of-a-graded-ring-is-graded). Give $A[t_1,\ldots,t_n]$ its $\mathbb N^n$-grading and regard $R[t_1,\ldots,t_n]$ as a graded subring. If $p$ is integral, each homogeneous component $a_\alpha t^\alpha$ is integral. Applying the evaluation homomorphism $t_1=\cdots=t_n=1$ shows that every coefficient $a_\alpha$ is integral over $R$.

## 4

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [inverse limit](../../../module-theory.md#inverse-limit) is the submodule of the direct product consisting of compatible families:

$$
\varprojlim_{i\in I}N_i
=\left\{(x_i)\in\prod_{i\in I}N_i:
g_{ij}(x_j)=x_i\text{ whenever }i\le j\right\}.
$$

Its projection to $N_i$ sends $(x_j)$ to $x_i$; these projections satisfy the [universal property of an inverse limit](../../../module-theory.md#universal-property-of-an-inverse-limit).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Two decreasing [filtrations of a module](../../../module-theory.md#filtration-of-a-module) $(M_n)$ and $(M'_n)$ are equivalent when each contains a fixed shift of the other: there are $a,b\ge0$ such that

$$
M_{n+a}\subseteq M'_n,
\qquad
M'_{n+b}\subseteq M_n
$$

for every $n\ge0$.

For an $I$-filtration, $IM_n\subseteq M_{n+1}$, so $I^nM_0\subseteq M_n$. If it is stable from $s$ onward, then

$$
M_{s+n}=I^nM_s\subseteq I^nM_0.
$$

It is therefore equivalent to the [I-adic filtration](../../../module-theory.md#i-adic-filtration). Any two stable $I$-filtrations are consequently equivalent to each other.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

**No.** Give $R=k[x]$ the [x-adic filtration](../../../module-theory.md#x-adic-filtration) $R_n=(x^n)$, take $M=R$, and let $N=(x)$. At $n=1$ the intersection filtration gives

$$
M_1\cap N=(x),
$$

whereas the induced filtration of $N$ gives

$$
R_1N=(x^2).
$$

**Thus intersection with a [submodule](../../../module-theory.md#submodule) need not equal the induced filtration.**

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

**Yes.** Scalar multiplication in the [quotient module](../../../module-theory.md#quotient-module) gives directly

$$
R_n(M/N)=\{r(m+N):r\in R_n,m\in M\}
=(R_nM+N)/N=(M_n+N)/N.
$$

**Hence the displayed filtration is precisely the induced filtration.**

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Work modulo $I$. Put

$$
C=R/(I+J),
$$

and let $A$ be the image of $I'/I$ in $C$. The separating condition $I'=I'\cap(I+J)$ modulo $I$ says that $I'/I\to C$ is injective, so we may regard $A$ as a submodule of $C$.

Since $r\in\sqrt{(I:I')}$, some power $r^q$ annihilates $A$. Apply the [Artin-Rees lemma](../../../module-theory.md#artin-rees-lemma) to $A\subseteq C$ and the principal ideal $(r)$. There is $s$ such that for every $m\ge s$,

$$
A\cap r^mC=r^{m-s}(A\cap r^sC).
$$

For $m\ge s+q$, the right side is zero. Pulling the equality $A\cap r^mC=0$ back to $R$ gives

$$
I'\cap(I+J+(r^m))=I,
$$

as required.

## 5

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

For an $\mathfrak m$-primary ideal $I$ in a [Noetherian local ring](../../../algebra.md#noetherian-local-ring), the function

$$
n\longmapsto\operatorname{length}_R(R/I^n)
$$

agrees for all sufficiently large $n$ with a polynomial in $n$. This is the [Hilbert-Samuel polynomial](../../../commutative-algebra.md#hilbert-samuel-polynomial), also called here the characteristic polynomial of $I$. Using $R/I^{n+1}$ instead merely shifts its variable.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

Suppose $I$ has $s$ generators. Its [associated graded ring](../../../commutative-algebra.md#associated-graded-ring)

$$
\operatorname{gr}_I(R)=\bigoplus_{n\ge0}I^n/I^{n+1}
$$

is generated in degree one by their initial forms, so there is a graded surjection

$$
(R/I)[X_1,\ldots,X_s]\twoheadrightarrow\operatorname{gr}_I(R).
$$

Because $I$ is $\mathfrak m$-primary, $R/I$ has finite [length of a module](../../../module-theory.md#length-of-a-module). The degree-$n$ piece on the left has length

$$
\operatorname{length}(R/I)\binom{n+s-1}{s-1},
$$

so $\operatorname{length}(I^n/I^{n+1})$ grows with degree at most $s-1$. Summing these lengths shows that $\operatorname{length}(R/I^n)$ has polynomial degree at most $s$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The weighted [Hilbert series](../../../commutative-algebra.md#hilbert-series) of $K[x,y,t_1,\ldots,t_n]$ is

$$
\frac1{(1-z)^2\prod_{i=1}^n(1-z^i)}.
$$

The homogeneous polynomial $x^k-y^k$ has degree $k$ and is a [non-zero-divisor](../../../mathematics.md#non-zero-divisor), so quotienting by it multiplies the series by $1-z^k$. Therefore the requested [Poincare series of a graded module](../../../commutative-algebra.md#poincare-series-of-a-graded-module) is

$$
\boxed{P_R(z)=\frac{1-z^k}{(1-z)^2\prod_{i=1}^n(1-z^i)}.}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

Let $P=p_1\cdots p_n$ and $A=\mathbb Z/P\mathbb Z=R_0$. By the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem), $A\cong\prod_i\mathbb F_{p_i}$, so $\operatorname{length}_A(A)=n$.

If a positive-degree monomial contains both $t_i$ and $t_j$ with $i\ne j$, then it vanishes: [Bezout identity](../../../algebra.md#bezout-identity) gives $u p_i+v p_j=1$, while both $p_i$ and $p_j$ annihilate that monomial. Thus the degree-$d$ component for $d\ge1$ is

$$
R_d\cong\bigoplus_{i=1}^n A/(p_i),
$$

and every summand has length one. Hence every $R_d$ has length $n$, including $d=0$, and

$$
\boxed{P_R(z)=\sum_{d\ge0}nz^d=\frac{n}{1-z}.}
$$

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

The denominator has degree one, independently of the number $n$ of variables. This reflects the fact that all mixed monomials vanish and each component of the ring supports only one polynomial direction; equivalently, the [Krull dimension](../../../commutative-algebra.md#krull-dimension) of this graded ring is one.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
