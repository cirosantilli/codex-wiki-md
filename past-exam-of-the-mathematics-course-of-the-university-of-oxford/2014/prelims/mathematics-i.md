# Mathematics I

↑ **Parent:** [Prelims](../prelims.md)

Solutions to all seven questions of the [University of Oxford](../../../university-of-oxford.md) undergraduate Prelims Mathematics I examination, sat on 23 June 2014. The cover also identifies the shared mathematics and computer science paper as M1. Source: [released examination archive](https://www.whatdotheyknow.com/request/maths_papers_2/response/1850333/attach/3/FOI%2020210708%201%20Data.zip?cookie_passthrough=1), member `FOI-20210708-1 - Data/4243.pdf`, printed pages 1–4. Question statements are omitted. A bounded exact-paper availability check found no advertised full or partial answers; the published even-year policy explicitly establishes coverage back to at least 2016, rather than establishing this 2014 paper's availability.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
- [7](#7)
  - [a](#7/a)
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
  - [b](#7/b)
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)

## 1

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a finite set $S=\{s_1,\ldots,s_k\}$ of [vectors](../../../vector-space.md#vector) in a real [vector space](../../../vector-space.md), its [span](../../../vector-space.md#linear-span) is the set of all [linear combinations](../../../vector-space.md#linear-combination):

$$
\boxed{\operatorname{Sp}(S)=\left\{\sum_{i=1}^ka_is_i:a_i\in\mathbb R\right\}.}
$$

The [span](../../../vector-space.md#linear-span) of the empty set is $\{0\}$. The set $S$ is [linearly independent](../../../vector-space.md#linear-independence) if $\sum_i a_is_i=0$ implies $a_i=0$ for every $i$. It is a [spanning set](../../../vector-space.md#spanning-set) for $V$ if $\operatorname{Sp}(S)=V$. A [basis](../../../vector-space.md#basis) is both a [linearly independent](../../../vector-space.md#linear-independence) set and a [spanning set](../../../vector-space.md#spanning-set).

For [basis extension](../../../vector-space.md#basis-extension), start with the given [linearly independent](../../../vector-space.md#linear-independence) set. If it does not span $V$, choose $v\notin\operatorname{Sp}(S)$ and adjoin it. The enlarged set remains [linearly independent](../../../vector-space.md#linear-independence): a relation $av+\sum_i a_is_i=0$ with $a\ne0$ would express $v$ as a [linear combination](../../../vector-space.md#linear-combination) of $S$, a contradiction; if $a=0$, independence of $S$ forces all other coefficients to be zero.

Repeat whenever the current [span](../../../vector-space.md#linear-span) is proper. Each step increases the set's size by one, while the allowed bound says its size cannot exceed $\dim V$. Thus the process terminates with a [linearly independent](../../../vector-space.md#linear-independence) set spanning $V$, hence a [basis](../../../vector-space.md#basis) containing the original set. This also covers an initially empty set and the zero-dimensional [vector space](../../../vector-space.md).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Choose a [basis](../../../vector-space.md#basis) $u_1,\ldots,u_r$ of $U$, extend it to a [basis](../../../vector-space.md#basis) $u_1,\ldots,u_r,w_1,\ldots,w_s$ of $W$, and extend again to a [basis](../../../vector-space.md#basis) of $V$ by adding $v_1,\ldots,v_t$. Define

$$
\boxed{W'=\operatorname{span}\{u_1,\ldots,u_r,v_1,\ldots,v_t\}.}
$$

Every member of the full [basis](../../../vector-space.md#basis) lies in $W$ or $W'$, so the [sum of vector subspaces](../../../vector-space.md#sum-of-vector-subspaces) is $W+W'=V$. If $x\in W\cap W'$, express it in both displayed [bases](../../../vector-space.md#basis). Uniqueness of the coordinates in the full [basis](../../../vector-space.md#basis) forces its $w_j$ and $v_j$ coefficients to vanish. Thus $x\in U$. The reverse inclusion is built into the construction, proving $W\cap W'=U$. This is a [subspace supplement with a prescribed intersection](../../../vector-space.md#subspace-supplement-with-a-prescribed-intersection).

For the matrix example, let

$$
J=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad
I=\begin{pmatrix}1&0\\0&1\end{pmatrix}.
$$

The [skew-symmetric matrices](../../../linear-algebra.md#skew-symmetric-matrix) are exactly $U=\operatorname{span}\{J\}$, and the traceless [matrices](../../../vector-space.md#matrix) form $W$. A suitable answer is

$$
\boxed{W'=\operatorname{span}\{I,J\}
=\left\{\begin{pmatrix}a&b\\-b&a\end{pmatrix}:a,b\in\mathbb R\right\}.}
$$

The [matrix trace](../../../linear-algebra.md#matrix-trace) of $aI+bJ$ is $2a$, so $W\cap W'=\operatorname{span}\{J\}=U$. Every $2\times2$ real [matrix](../../../vector-space.md#matrix) has the decomposition

$$
A=\left(A-\frac{\operatorname{tr}A}{2}I\right)+\frac{\operatorname{tr}A}{2}I,
$$

whose first term lies in $W$ and second in $W'$. Therefore $W+W'=M_2(\mathbb R)$, as required.

## 2

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a [linear map](../../../vector-space.md#linear-map) $T:V\to V$, its [kernel of a linear map](../../../kernel-of-a-linear-map.md) and [image of a linear map](../../../vector-space.md#image-of-a-linear-map) are

$$
\ker T=\{v\in V:T(v)=0\},\qquad\operatorname{im}T=\{T(v):v\in V\}.
$$

Its [nullity of a linear map](../../../kernel-of-a-linear-map.md#nullity-of-a-linear-map) is $n(T)=\dim\ker T$, and its [rank of a linear map](../../../vector-space.md#rank-of-a-linear-map) is $r(T)=\dim\operatorname{im}T$.

Choose a [basis](../../../vector-space.md#basis) $u_1,\ldots,u_k$ of $\ker T$ and extend it to a [basis](../../../vector-space.md#basis) $u_1,\ldots,u_k,v_1,\ldots,v_m$ of $V$. The [vectors](../../../vector-space.md#vector) $T(v_1),\ldots,T(v_m)$ span $\operatorname{im}T$, because applying $T$ to an arbitrary [linear combination](../../../vector-space.md#linear-combination) of the full [basis](../../../vector-space.md#basis) eliminates the $u_i$ terms. They are also [linearly independent](../../../vector-space.md#linear-independence): if $\sum_jb_jT(v_j)=0$, then $\sum_jb_jv_j\in\ker T$, so $\sum_jb_jv_j=\sum_i a_i u_i$ for some coefficients. Independence of the extended [basis](../../../vector-space.md#basis) forces all $a_i,b_j$ to vanish.

Consequently $r(T)=m$, $n(T)=k$ and $\dim V=k+m$. This proves the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem):

$$
\boxed{\dim V=r(T)+n(T).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Restrict $S$ to the [vector subspace](../../../vector-space.md#vector-subspace) $W=\operatorname{im}T$. This restriction has [kernel of a linear map](../../../kernel-of-a-linear-map.md) $W\cap\ker S$ and [image of a linear map](../../../vector-space.md#image-of-a-linear-map) $S(W)=\operatorname{im}(ST)$. The [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) on $W$ therefore gives

$$
r(ST)=r(T)-\dim(\operatorname{im}T\cap\ker S).
$$

Apply the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) to $T$ and $ST$ on $V$ to obtain the exact [nullity of a composition](../../../kernel-of-a-linear-map.md#nullity-of-a-composition) identity:

$$
n(ST)=n(T)+\dim(\operatorname{im}T\cap\ker S).
$$

Since the intersection is a [vector subspace](../../../vector-space.md#vector-subspace) of $\ker S$, its [dimension](../../../vector-space.md#dimension-vector-space) is at most $n(S)$. Hence

$$
\boxed{n(ST)\leq n(T)+n(S).}
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The [image of a linear map](../../../vector-space.md#image-of-a-linear-map) $\operatorname{im}(ST)=S(\operatorname{im}T)$ lies inside $\operatorname{im}S$. Therefore $r(ST)\leq r(S)$. Also $S$ restricted to $\operatorname{im}T$ cannot have [rank of a linear map](../../../vector-space.md#rank-of-a-linear-map) greater than its domain's [dimension](../../../vector-space.md#dimension-vector-space), so $r(ST)\leq\dim\operatorname{im}T=r(T)$. Thus

$$
\boxed{r(ST)\leq\min\{r(S),r(T)\}.}
$$

Equivalently, apply the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) to that restriction: $r(ST)=r(T)-\dim(\operatorname{im}T\cap\ker S)\leq r(T)$. This proof keeps track of the intermediate [vector subspace](../../../vector-space.md#vector-subspace), rather than assuming an invertible factor.

## 3

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An [elementary row operation](../../../numerical-linear-algebra.md#elementary-row-operation) is one of three operations: interchange two rows, multiply one row by a nonzero [scalar](../../../vector-space.md#scalar), or add a scalar multiple of one row to a different row. Each operation is reversed by another operation of the same kind.

Performing such an operation on an $m\times n$ [matrix](../../../vector-space.md#matrix) $A$ is equivalent to left multiplication by the $m\times m$ [elementary matrix](../../../numerical-linear-algebra.md#elementary-matrix) obtained by applying that operation to the [identity matrix](../../../vector-space.md#identity-matrix). Each [elementary matrix](../../../numerical-linear-algebra.md#elementary-matrix) is invertible, with inverse corresponding to the reverse operation. Thus a sequence of operations gives

$$
B=E_kE_{k-1}\cdots E_1A,
\qquad
\boxed{B=PA,\quad P=E_k\cdots E_1\text{ invertible}.}
$$

For square [matrices](../../../vector-space.md#matrix), if $A$ were invertible, then $B=PA$ would have inverse $A^{-1}P^{-1}$. Hence **if $B$ is singular, $A$ must be singular as well**. In fact the two are invertible together, because $A=P^{-1}B$ gives the converse.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Solve $Ax=b$ for a general right-hand side $b=(b_1,b_2,b_3,b_4)^T$. Subtracting the fourth equation from the second gives $x_3=b_2-b_4$. The first and fourth then give

$$
x_1=b_1-b_2+b_4-x_4,\qquad x_2=b_4-x_4.
$$

Substitution into the third equation reduces the remaining condition to

$$
(t-2)x_4=b_3-b_1-b_4.
$$

If $t\ne2$, every right-hand side therefore has a unique solution, and collecting its four coefficients yields the [matrix inverse](../../../matrix-inverse.md)

$$
\boxed{A^{-1}=\frac1{t-2}
\begin{pmatrix}
t-1&2-t&-1&t-1\\
1&0&-1&t-1\\
0&t-2&0&2-t\\
-1&0&1&-1
\end{pmatrix},\qquad t\ne2.}
$$

For $t=2$, the nonzero [vector](../../../vector-space.md#vector) $(-1,-1,0,1)^T$ lies in the [kernel of a linear map](../../../kernel-of-a-linear-map.md) represented by $A$, so $A$ is singular. Hence **$A$ is invertible exactly when $t\ne2$**. The same calculation gives $\det A=t-2$; the formula above can also be checked by multiplying its numerator by $A$ to obtain $(t-2)I$.

## 4

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

A real number $\lambda$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $A$ if there is a nonzero [vector](../../../vector-space.md#vector) $v$ with $Av=\lambda v$; such a $v$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) for $\lambda$. The nonzero condition is essential.

For distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_1,\ldots,\lambda_r$, choose corresponding nonzero [eigenvectors](../../../linear-operator-theory.md#eigenvector) $v_1,\ldots,v_r$. Prove their [linear independence](../../../vector-space.md#linear-independence) by induction on $r$. The claim for one vector is immediate. Given a relation $\sum_{i=1}^r a_iv_i=0$, apply $A-\lambda_rI$ to get

$$
\sum_{i=1}^{r-1}a_i(\lambda_i-\lambda_r)v_i=0.
$$

By the induction hypothesis, every coefficient here is zero. Distinctness gives $a_i=0$ for $i<r$, and the original relation then gives $a_r=0$ since $v_r\ne0$. Thus the [eigenvectors](../../../linear-operator-theory.md#eigenvector) are [linearly independent](../../../vector-space.md#linear-independence).

With $n$ distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue), the $n$ real [eigenvectors](../../../linear-operator-theory.md#eigenvector) form a [basis](../../../vector-space.md#basis) of $\mathbb R^n$. Put them into the columns of $P$. Then $P$ is invertible and

$$
AP=P\operatorname{diag}(\lambda_1,\ldots,\lambda_n),
\qquad
\boxed{P^{-1}AP=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

This proves [diagonalizability](../../../linear-operator-theory.md#diagonalizable-matrix) directly.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Suppose $A^T=A$. For [eigenvectors](../../../linear-operator-theory.md#eigenvector) $v_i,v_j$ with distinct real [eigenvalues](../../../linear-operator-theory.md#eigenvalue), symmetry gives

$$
\lambda_i v_i^Tv_j=(Av_i)^Tv_j=v_i^TA^Tv_j=v_i^TAv_j
=\lambda_jv_i^Tv_j.
$$

Thus $(\lambda_i-\lambda_j)v_i^Tv_j=0$, and the [eigenvectors](../../../linear-operator-theory.md#eigenvector) are [orthogonal](../../../inner-product.md#orthogonal-vectors). Divide each by its nonzero [Euclidean norm](../../../normed-vector-space.md#euclidean-norm) to obtain an [orthonormal basis](../../../inner-product.md#orthonormal-basis). The [matrix](../../../vector-space.md#matrix) $P$ having these normalized columns satisfies $P^TP=I$, so it is an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) and $P^{-1}=P^T$. As in part (a),

$$
\boxed{P^TAP=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

This proves the needed [orthogonal diagonalization](../../../linear-algebra.md#orthogonal-diagonalization-of-a-real-symmetric-matrix) from symmetry and distinct [eigenvalues](../../../linear-operator-theory.md#eigenvalue), without invoking an unproved [spectral theorem](../../../hilbert-space.md#spectral-theorem).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For the given symmetric [matrix](../../../vector-space.md#matrix), $(1,1)^T$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $1$, and $(1,-1)^T$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $27$. Normalize them to obtain

$$
P=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},\qquad
A=P\begin{pmatrix}1&0\\0&27\end{pmatrix}P^T.
$$

Take the real cube roots of the two diagonal entries and transform back:

$$
\boxed{C=P\begin{pmatrix}1&0\\0&3\end{pmatrix}P^T
=\begin{pmatrix}2&-1\\-1&2\end{pmatrix}.}
$$

It is a real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), and $C^3=P\operatorname{diag}(1,27)P^T=A$ because $P^TP=I$. Direct multiplication also gives $C^2=\begin{pmatrix}5&-4\\-4&5\end{pmatrix}$ and then $C^3=\begin{pmatrix}14&-13\\-13&14\end{pmatrix}$.

## 5

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Among the $|G|+1$ powers $e,g,g^2,\ldots,g^{|G|}$ in the finite [group](../../../group.md) $G$, the [pigeonhole principle](../../../combinatorics.md#pigeonhole-principle) forces two to be equal: $g^i=g^j$ with $0\leq i<j\leq|G|$. Multiply by $g^{-i}$ to obtain

$$
\boxed{g^{j-i}=e,\qquad j-i>0.}
$$

This proves the existence of a positive power equal to the [identity element](../../../algebraic-operation.md#identity-element), without presupposing the [order of a group element](../../../group-theory.md#order-of-a-group-element).

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

The [order of a group element](../../../group-theory.md#order-of-a-group-element) $o(g)$ is the least positive integer $n$ for which $g^n=e$, whose existence follows from part (i). If $g^k=e$, use the [Euclidean division](../../../integer.md#euclidean-division) to write $k=qn+r$, where $0\leq r<n$. Then

$$
e=g^k=(g^n)^qg^r=g^r.
$$

Minimality of $n$ forces $r=0$. Thus

$$
\boxed{o(g)\mid k.}
$$

The argument also works for negative $k$, using integer powers and the same remainder convention.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

[Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states that for a [subgroup](../../../group.md#subgroup) $H$ of a finite [group](../../../group.md) $G$,

$$
|G|=[G:H]|H|,
$$

where $[G:H]$ is the [index of a subgroup](../../../group.md#index-of-a-subgroup), the number of its [left cosets](../../../group-theory.md#left-coset). In particular, $|H|$ divides $|G|$.

The [cyclic subgroup](../../../group.md#cyclic-subgroup) $\langle g\rangle$ consists of the distinct elements $e,g,\ldots,g^{n-1}$, where $n=o(g)$. Every power reduces to one of these by the [Euclidean division](../../../integer.md#euclidean-division), and a repetition among them would contradict minimality of $n$. Thus $|\langle g\rangle|=o(g)$. Applying [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) gives

$$
\boxed{o(g)\mid|G|.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $n=o(g)$. A [group homomorphism](../../../group-theory.md#group-homomorphism) preserves powers and the [identity element](../../../algebraic-operation.md#identity-element), so

$$
\phi(g)^n=\phi(g^n)=\phi(e)=e_H.
$$

The preceding divisibility property gives

$$
\boxed{o(\phi(g))\mid o(g).}
$$

Now assume $\phi$ is surjective and choose $h\in H$ of order $m$. Take a preimage $g$ of $h$, and write $o(g)=mr$, as the divisibility result permits. The element $g^r$ has order exactly $m$: its $m$th power is $e$, while $(g^r)^s=e$ implies $mr\mid rs$, hence $m\mid s$. Therefore **$G$ contains an element of order $m$**, namely $g^r$.

The preimage $g$ itself need not have order $m$; taking the suitable power is the essential step. The constructed element need not map to the original $h$. This proves that [element orders in a finite quotient occur in the original group](../../../group-theory.md#element-orders-in-a-finite-quotient-occur-in-the-original-group).

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

A [group homomorphism](../../../group-theory.md#group-homomorphism) from an additive [cyclic group](../../../group.md#cyclic-group) $\mathbb Z_n$ is determined by the image $a$ of $1$, subject exactly to $a^n=e$ in multiplicative notation, or $na=0$ in an additive target.

For $\mathbb Z_{18}\to\mathbb Z_{15}$, the relation is $18a\equiv0\pmod{15}$, equivalently $3a\equiv0\pmod{15}$. The possibilities are $a=0,5,10$, and each defines a [homomorphism between cyclic groups](../../../group-theory.md#homomorphism-between-cyclic-groups). Thus there are **three** such maps, an instance of the [number of homomorphisms between finite cyclic groups](../../../group-theory.md#number-of-homomorphisms-between-finite-cyclic-groups).

For $\mathbb Z_9\to S_4$, the image of $1$ must be a [permutation](../../../combinatorics.md#permutation) whose [order of a group element](../../../group-theory.md#order-of-a-group-element) divides $9$. A [permutation](../../../combinatorics.md#permutation) on four symbols can have order $1,2,3$ or $4$, so the allowed images are the identity and the [three-cycles](../../../finite-group-theory.md#three-cycle). There are $\binom43(3-1)!=8$ [three-cycles](../../../finite-group-theory.md#three-cycle): choose their three symbols and one of the two cyclic orientations. Hence there are **nine** maps.

Finally, each [transposition](../../../combinatorics.md#transposition-permutation) in $S_5$ has order $2$, so its image in $\mathbb Z_5$ must have order dividing both $2$ and $5$, and is therefore the identity. Every [permutation](../../../combinatorics.md#permutation) is a product of [transpositions](../../../combinatorics.md#transposition-permutation), so every element must map to the identity. There is **one** map. In the order asked, the counts are

$$
\boxed{3,\qquad9,\qquad1.}
$$

## 6

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

A [subgroup](../../../group.md#subgroup) $N$ of $G$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) if conjugation by every element preserves it:

$$
\boxed{gNg^{-1}=N\quad\text{for every }g\in G.}
$$

Equivalently, $gN=Ng$ for every $g\in G$. Here equality means equality of sets; it does not require each individual element of $N$ to commute with every element of $G$.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

The [center of a group](../../../group-theory.md#center-of-a-group) consists of its elements commuting with every element. First check it is a [subgroup](../../../group.md#subgroup). The [identity element](../../../algebraic-operation.md#identity-element) is central. If $a,b\in Z(G)$ and $x\in G$, then $b^{-1}$ commutes with $x$ and

$$
(ab^{-1})x=a(xb^{-1})=x(ab^{-1}).
$$

Thus $ab^{-1}\in Z(G)$, proving closure under the subgroup criterion. Moreover, if $z\in Z(G)$, then $xzx^{-1}=z$ for every $x\in G$. Hence conjugation fixes the center elementwise, so

$$
\boxed{xZ(G)x^{-1}=Z(G)\quad(x\in G).}
$$

Therefore the [center of a group](../../../group-theory.md#center-of-a-group) is a [normal subgroup](../../../group-theory.md#normal-subgroup).

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

If $g\in Z(G)$, it commutes with each $x\in G$, so $x^{-1}gx=g$. Its [conjugacy class](../../../group-action.md#conjugacy-class) is therefore $C(g)=\{g\}$.

Conversely, if $C(g)=\{g\}$, then $x^{-1}gx=g$ for every $x$. Multiplication by $x$ on the left gives $gx=xg$ for every $x$, which is exactly membership in the [center of a group](../../../group-theory.md#center-of-a-group). Thus

$$
\boxed{g\in Z(G)\iff C(g)=\{g\}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

[Conjugation](../../../group-action.md#conjugation) of a [permutation](../../../combinatorics.md#permutation) relabels each symbol by the inverse conjugating permutation. Specifically,

$$
\boxed{\tau^{-1}(a_1a_2\cdots a_n)\tau
=(\tau^{-1}(a_1)\ \tau^{-1}(a_2)\ \cdots\ \tau^{-1}(a_n)).}
$$

To verify the direction of the inverse, apply the left side to $\tau^{-1}(a_j)$: $\tau$ first takes it to $a_j$, the original cycle takes it to $a_{j+1}$, and $\tau^{-1}$ takes it to $\tau^{-1}(a_{j+1})$, with cyclic indexing. Any symbols fixed by the original [permutation](../../../combinatorics.md#permutation) are similarly relabelled and remain fixed. More generally, conjugate every cycle of a disjoint-cycle decomposition in this way; disjointness is preserved because $\tau^{-1}$ is a [bijection](../../../function.md#bijection).

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

By the preceding relabelling formula, every conjugate of $(123)$ is a [three-cycle](../../../finite-group-theory.md#three-cycle), and any [three-cycle](../../../finite-group-theory.md#three-cycle) on four symbols can be obtained by a suitable relabelling. Therefore

$$
\boxed{C((123))=\{(123),(132),(124),(142),(134),(143),(234),(243)\}.}
$$

There are eight elements, agreeing with the count $\binom43\cdot2$.

Likewise, conjugation preserves the pattern of two disjoint [transpositions](../../../combinatorics.md#transposition-permutation), and every partition of four symbols into two pairs is realized by relabelling. Thus

$$
\boxed{C((12)(34))=\{(12)(34),(13)(24),(14)(23)\}.}
$$

These have the respective [cycle types](../../../finite-group-theory.md#cycle-type) $(3,1)$ and $(2,2)$ in the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_4$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Suppose $\sigma\ne e$. Choose a symbol $i$ moved by $\sigma$ and write $j=\sigma(i)\ne i$. Since $n\geq3$, choose a third symbol $k$ distinct from $i,j$. Let $\tau=(jk)$, a [transposition](../../../combinatorics.md#transposition-permutation) that fixes $i$. Then

$$
(\tau^{-1}\sigma\tau)(i)=\tau^{-1}(\sigma(i))=\tau^{-1}(j)=k\ne j=\sigma(i).
$$

Thus $\tau^{-1}\sigma\tau\ne\sigma$, proving that the [conjugacy class](../../../group-action.md#conjugacy-class) of any nonidentity [permutation](../../../combinatorics.md#permutation) has more than one element. By part (a)(iii), no such [permutation](../../../combinatorics.md#permutation) lies in the [center of a group](../../../group-theory.md#center-of-a-group). The identity always does, so

$$
\boxed{Z(S_n)=\{e\}\quad(n\geq3).}
$$

The restriction on $n$ is necessary: $S_2$ is an [abelian group](../../../group.md#abelian-group) and equals its own center.

## 7

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

A left [group action](../../../group-action.md) of $G$ on a set $S$ is a function $\phi:G\times S\to S$ satisfying

$$
\boxed{\phi(e,s)=s,\qquad\phi(gh,s)=\phi(g,\phi(h,s))}
$$

for all $s\in S$ and $g,h\in G$. Writing $g\cdot s=\phi(g,s)$, these are $e\cdot s=s$ and $(gh)\cdot s=g\cdot(h\cdot s)$. No commutativity is assumed, so the order of composition matters.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

The [group action](../../../group-action.md) law gives

$$
\phi_g\circ\phi_{g^{-1}}=\phi_e=\operatorname{id}_S,
\qquad
\phi_{g^{-1}}\circ\phi_g=\operatorname{id}_S.
$$

Thus $\phi_g$ is a [bijection](../../../function.md#bijection) with inverse $\phi_{g^{-1}}$, hence a [permutation](../../../combinatorics.md#permutation) of $S$. Also, for every $s$,

$$
\phi_{gh}(s)=\phi(g,\phi(h,s))=(\phi_g\circ\phi_h)(s).
$$

Therefore the assignment $\Phi(g)=\phi_g$ takes values in the [symmetric group](../../../finite-group-theory.md#symmetric-group) $\operatorname{Sym}(S)$ and satisfies

$$
\boxed{\Phi(gh)=\Phi(g)\Phi(h).}
$$

It is a [group homomorphism](../../../group-theory.md#group-homomorphism), with the group product on the right interpreted as composition of [permutations](../../../combinatorics.md#permutation).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

Define $g\cdot(g_1H)=(gg_1)H$ on the set of [left cosets](../../../group-theory.md#left-coset). It is well-defined: if $g_1H=g_2H$, then $g_2=g_1h$ for some $h\in H$, so $(gg_2)H=(gg_1h)H=(gg_1)H$. The identity fixes each coset, and associativity in $G$ gives

$$
g\cdot(h\cdot(g_1H))=(ghg_1)H=(gh)\cdot(g_1H).
$$

Hence this is a left [group action](../../../group-action.md), and part (a) supplies its [group homomorphism](../../../group-theory.md#group-homomorphism) $\Phi:G\to\operatorname{Sym}(S)$.

An element of the [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) $\Phi$ fixes every coset, in particular $H$ itself. Thus $g\in\ker\Phi$ implies $gH=H$, which implies $g\in H$. Therefore

$$
\boxed{\ker\Phi\leq H.}
$$

The subgroup symbol is justified because a [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is a [subgroup](../../../group.md#subgroup), and the argument proves containment.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

By [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), the [index of a subgroup](../../../group.md#index-of-a-subgroup) is $[G:H]=75/25=3$. Thus the set of [left cosets](../../../group-theory.md#left-coset) has three elements, and the preceding [group action](../../../group-action.md) yields a [group homomorphism](../../../group-theory.md#group-homomorphism) $\Phi:G\to S_3$ after labelling them.

Its image is a [subgroup](../../../group.md#subgroup) of $S_3$, so its order divides $6$. By the [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem), $|\operatorname{im}\Phi|=|G|/|\ker\Phi|$ also divides $75$. Hence its order divides $\gcd(6,75)=3$, giving possibilities $1$ and $3$. The action on cosets is [transitive](../../../set-theory.md#transitive-relation): $g_2g_1^{-1}$ sends $g_1H$ to $g_2H$. It cannot be the trivial action on a three-element set, so the image does not have order $1$. Therefore

$$
\boxed{|\operatorname{im}\Phi|=3.}
$$

It follows that $|\ker\Phi|=75/3=25$. Part (b)(i) gives $\ker\Phi\leq H$, and $|H|=25$; equal finite orders force equality. A [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) is a [normal subgroup](../../../group-theory.md#normal-subgroup), so

$$
\boxed{H=\ker\Phi\mathrel{\trianglelefteq}G.}
$$

This is an instance of the fact that a [subgroup of index the smallest prime divisor is normal](../../../group.md#subgroup-of-index-the-smallest-prime-divisor-is-normal).

## ↑ Ancestors (9)

1. [Prelims](../prelims.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Oxford](../../../past-exam-of-the-mathematics-course-of-the-university-of-oxford.md)
4. [Mathematics course of the University of Oxford](../../../university-of-oxford.md#mathematics-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../../university-of-oxford.md)
8. [List of universities](../../../README.md#list-of-universities)
9. [Codex Wiki](../../../README.md)
