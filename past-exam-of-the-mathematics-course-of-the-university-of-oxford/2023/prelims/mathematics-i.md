# Mathematics I

↑ **Parent:** [Prelims](../prelims.md)

Source: [released examination PDF, pages 180–184](https://www.whatdotheyknow.com/request/request_for_mathematics_examinat/response/3129786/attach/3/FOI%20202507%20740%20Data.pdf#page=180).

Solutions cover all seven questions, including every optional question. The module label is I, with M1 used for Mathematics and Computer Science; the formal paper code is A10138W1. Throughout Question 4, [diagonalisable matrices](../../../linear-operator-theory.md#diagonalizable-matrix) are understood over the [real numbers](../../../arithmetic.md#real-number).

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
    - [v](#3/a/v)
      - [Solution](#3/a/v/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
    - [iv](#3/b/iv)
      - [Solution](#3/b/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
    - [iv](#5/a/iv)
      - [Solution](#5/a/iv/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
    - [iv](#5/b/iv)
      - [Solution](#5/b/iv/solution)
    - [v](#5/b/v)
      - [Solution](#5/b/v/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
    - [iv](#6/b/iv)
      - [Solution](#6/b/iv/solution)
    - [v](#6/b/v)
      - [Solution](#6/b/v/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
- [7](#7)
  - [a](#7/a)
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
    - [iii](#7/a/iii)
      - [Solution](#7/a/iii/solution)
    - [iv](#7/a/iv)
      - [Solution](#7/a/iv/solution)
  - [b](#7/b)
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)

## 1

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [a](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [i](#1/a/i)

The three [elementary row operations](../../../numerical-linear-algebra.md#elementary-row-operation) on an $m\times n$ [real matrix](../../../vector-space.md#real-matrix) are:

- Interchange two distinct rows: $R_i\leftrightarrow R_j$.
- Multiply one row by a nonzero [real number](../../../arithmetic.md#real-number): $R_i\leftarrow cR_i$, with $c\ne0$.
- Add a [scalar multiple](../../../vector-space.md#scalar-multiple) of one row to a different row: $R_i\leftarrow R_i+cR_j$, with $i\ne j$.

Each operation changes whole rows, so it acts on every column by the same rule. Each can be undone by an [elementary row operation](../../../numerical-linear-algebra.md#elementary-row-operation).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [a](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#1/a/ii)

For an $m\times n$ [matrix](../../../vector-space.md#matrix), the corresponding [elementary matrices](../../../numerical-linear-algebra.md#elementary-matrix) are $m\times m$, because the operation is implemented by left [matrix multiplication](../../../vector-space.md#matrix-multiplication). Apply the desired [elementary row operation](../../../numerical-linear-algebra.md#elementary-row-operation) to the [identity matrix](../../../vector-space.md#identity-matrix) $I_m$. Writing $E_{ij}$ for the [matrix unit](../../../vector-space.md#matrix-unit) with its only nonzero entry, $1$, in position $(i,j)$ gives:

$$
\begin{aligned}
P_{ij}&=I_m-E_{ii}-E_{jj}+E_{ij}+E_{ji},
& P_{ij}^{-1}&=P_{ij},\\
D_i(c)&=I_m+(c-1)E_{ii},
& D_i(c)^{-1}&=D_i(c^{-1})\quad(c\ne0),\\
L_{ij}(c)&=I_m+cE_{ij},
& L_{ij}(c)^{-1}&=L_{ij}(-c)\quad(i\ne j).
\end{aligned}
$$

Indeed, these [matrix products](../../../vector-space.md#matrix-product) interchange rows $i,j$, scale row $i$, and add $c$ times row $j$ to row $i$, respectively. The displayed inverses undo precisely those operations. Algebraically, $E_{ij}^2=0$ when $i\ne j$, so $(I_m+cE_{ij})(I_m-cE_{ij})=I_m$; the other two inverse identities follow immediately from their row actions. Thus every [elementary matrix](../../../numerical-linear-algebra.md#elementary-matrix) is an [invertible matrix](../../../linear-algebra.md#invertible-matrix).

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [a](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [iii](#1/a/iii)

Perform the [elementary row operations](../../../numerical-linear-algebra.md#elementary-row-operation) $R_2\leftarrow R_2+2R_1$ and $R_3\leftarrow R_3-R_1$, then $R_2\leftarrow R_2/2$, $R_1\leftarrow R_1-R_2$, and finally $R_1\leftarrow R_1+R_3$, $R_2\leftarrow R_2-3R_3$:

$$
\begin{pmatrix}1&1&2\\-2&0&2\\1&1&3\end{pmatrix}
\longrightarrow
\begin{pmatrix}1&1&2\\0&2&6\\0&0&1\end{pmatrix}
\longrightarrow
\begin{pmatrix}1&0&-1\\0&1&3\\0&0&1\end{pmatrix}
\longrightarrow I_3.
$$

Consequently the [reduced row echelon form](../../../numerical-linear-algebra.md#reduced-row-echelon-form) is $I_3$. Applying the same operations to the augmented column $b=(b_1,b_2,b_3)^T$ gives

$$
\boxed{v=\begin{pmatrix}
b_3-b_1-\tfrac12b_2\\
4b_1+\tfrac12b_2-3b_3\\
b_3-b_1
\end{pmatrix}.}
$$

Thus **every** $b\in\mathbb R^3$ admits exactly one solution. This follows because the [elementary row operations](../../../numerical-linear-algebra.md#elementary-row-operation) preserve the solution set of the augmented [linear system](../../../linear-algebra.md#system-of-linear-equations), and the reduced coefficient [matrix](../../../vector-space.md#matrix) is the [identity matrix](../../../vector-space.md#identity-matrix).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [b](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [i](#1/b/i)

If $A$ is a [strictly upper triangular matrix](../../../linear-algebra.md#strictly-upper-triangular-matrix), then $A_{ij}=0$ unless $j-i\ge1$. We prove by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) that

$$
(A^k)_{ij}=0\qquad\text{whenever }j-i<k.
$$

The assertion for $k=1$ is the definition. In the [matrix multiplication](../../../vector-space.md#matrix-multiplication) formula

$$
(A^{k+1})_{ij}=\sum_{\ell=1}^n(A^k)_{i\ell}A_{\ell j},
$$

a nonzero summand would require $\ell-i\ge k$ and $j-\ell\ge1$, hence $j-i\ge k+1$. This proves the induction step. Since $j-i\le n-1$ for all entries, $\boxed{A^n=0}$. In particular, every [strictly upper triangular matrix](../../../linear-algebra.md#strictly-upper-triangular-matrix) is a [nilpotent matrix](../../../linear-operator-theory.md#nilpotent-matrix).

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [b](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#1/b/ii)

Write $A=I_3+N$, where

$$
N=\begin{pmatrix}0&a&b\\0&0&c\\0&0&0\end{pmatrix},\qquad
N^2=\begin{pmatrix}0&0&ac\\0&0&0\\0&0&0\end{pmatrix},\qquad N^3=0.
$$

The [binomial theorem for commuting matrices](../../../binomial-coefficient.md#binomial-theorem-for-commuting-matrices) applies because $I_3N=NI_3$. All terms of degree at least three vanish, so for every positive [integer](../../../integer.md) $n$,

$$
\boxed{A^n=I_3+nN+\binom n2N^2
=\begin{pmatrix}
1&na&nb+\dfrac{n(n-1)}2ac\\
0&1&nc\\
0&0&1
\end{pmatrix}.}
$$

The same expression directly gives $A$ when $n=1$, so no small exponent is excluded.

## 2

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [a](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [i](#2/a/i)

A [vector space](../../../vector-space.md) over a [field](../../../algebra.md#field) $\mathbb F$ is a set $V$ with [vector addition](../../../vector-space.md#vector-addition) $V\times V\to V$ and [scalar multiplication](../../../vector-space.md#scalar-multiplication) $\mathbb F\times V\to V$ satisfying the following [vector space axioms](../../../vector-space.md#vector-space-axioms). Under [vector addition](../../../vector-space.md#vector-addition), $V$ is an [abelian group](../../../group.md#abelian-group): addition is associative and commutative, there is a [zero vector](../../../vector-space.md#zero-vector) $0_V$, and each $v$ has an additive inverse $-v$. For all $a,b\in\mathbb F$ and $u,v\in V$,

$$
a(u+v)=au+av,\qquad (a+b)v=av+bv,\qquad
(ab)v=a(bv),\qquad 1_{\mathbb F}v=v.
$$

The operations are defined for every indicated pair and take their values in $V$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [a](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#2/a/ii)

A map $T:V\to W$ between [vector spaces](../../../vector-space.md) over the same [field](../../../algebra.md#field) $\mathbb F$ is a [linear map](../../../vector-space.md#linear-map) precisely when it preserves [vector addition](../../../vector-space.md#vector-addition) and [scalar multiplication](../../../vector-space.md#scalar-multiplication):

$$
T(u+v)=T(u)+T(v),\qquad T(av)=aT(v)
\quad(u,v\in V,\ a\in\mathbb F).
$$

Equivalently, $T(au+bv)=aT(u)+bT(v)$ for all $u,v\in V$ and $a,b\in\mathbb F$.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [a](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [iii](#2/a/iii)

Every $v\in V$ has a unique [basis](../../../vector-space.md#basis) expansion $v=\sum_{i=1}^n a_iv_i$. Define the [linear functional](../../../dual-space.md#linear-functional)

$$
\boxed{T\left(\sum_{i=1}^n a_iv_i\right)=\sum_{i=1}^n a_i\mu_i.}
$$

Uniqueness of the [coordinates](../../../vector-space.md#coordinate-linear-algebra) makes this definition well defined. The [coordinates](../../../vector-space.md#coordinate-linear-algebra) of a sum or a [scalar multiple](../../../vector-space.md#scalar-multiple) are the corresponding sums or [scalar multiples](../../../vector-space.md#scalar-multiple) of the [coordinates](../../../vector-space.md#coordinate-linear-algebra), so this formula defines a [linear map](../../../vector-space.md#linear-map). It has $T(v_i)=\mu_i$. Conversely, any [linear map](../../../vector-space.md#linear-map) with those values must satisfy the same formula by [linearity](../../../vector-space.md#linearity), proving uniqueness.

If the [finite field](../../../algebra.md#finite-field) $\mathbb F$ has $q$ elements, each of the $n$ values $\mu_i$ can be chosen independently in $q$ ways. The number of [linear maps](../../../vector-space.md#linear-map) $V\to\mathbb F$ is therefore $\boxed{q^n}$, including the zero [linear map](../../../vector-space.md#linear-map).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [b](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [i](#2/b/i)

Use [basis extension](../../../vector-space.md#basis-extension) to choose a [basis](../../../vector-space.md#basis) $(v,v_2,\ldots,v_n)$ of the [vector space](../../../vector-space.md) $V$ over the [finite field](../../../algebra.md#finite-field) $\mathbb F_p=\mathbb Z_p$. The condition $T(v)=0$ fixes the first value of a [linear functional](../../../dual-space.md#linear-functional); its remaining $n-1$ values are arbitrary. There are $p^{n-1}$ such [linear maps](../../../vector-space.md#linear-map), exactly one of which is zero. Hence the required number is

$$
\boxed{p^{n-1}-1.}
$$

For $n=1$ this is zero, as it should be: vanishing at a [basis vector](../../../vector-space.md#basis-vector) then forces the entire [linear functional](../../../dual-space.md#linear-functional) to vanish.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [b](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#2/b/ii)

Put $L=\operatorname{span}\{v\}$. Every two-dimensional [vector subspace](../../../vector-space.md#vector-subspace) containing $v$ is $W=\operatorname{span}\{v,w\}$ for some $w\notin L$. There are $p^n-p$ choices for $w$ in $V$. Within any one such $W$, exactly $p^2-p$ choices of $w\in W\setminus L$ yield that same $W$: each forms a [linearly independent](../../../vector-space.md#linear-independence) pair with $v$, and that pair is a [basis](../../../vector-space.md#basis) of $W$.

These sets of choices partition $V\setminus L$, because $w$ determines $\operatorname{span}\{v,w\}$ uniquely. Thus the number is

$$
\boxed{\frac{p^n-p}{p^2-p}=\frac{p^{n-1}-1}{p-1}.}
$$

Equivalently these [vector subspaces](../../../vector-space.md#vector-subspace) correspond to the one-dimensional [vector subspaces](../../../vector-space.md#vector-subspace) of the [quotient vector space](../../../vector-space.md#quotient-vector-space) $V/L$. For $n=1$ there are none and the formula gives zero.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [b](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [iii](#2/b/iii)

If $T'=\lambda T$ with $\lambda\ne0$, then $T'(x)=0$ if and only if $T(x)=0$, so their [kernels](../../../kernel-of-a-linear-map.md) agree. Conversely, suppose both nonzero [linear functionals](../../../dual-space.md#linear-functional) have [kernel](../../../kernel-of-a-linear-map.md) $K$. Choose $u$ with $T(u)=1$, by scaling a [vector](../../../vector-space.md#vector) on which $T$ is nonzero. For each $x\in V$,

$$
x=T(x)u+\bigl(x-T(x)u\bigr),\qquad x-T(x)u\in K.
$$

Therefore $T'(x)=T(x)T'(u)$. Moreover $T'(u)\ne0$, since $u\notin K$. Thus $\boxed{T'=T'(u)T}$, with a nonzero [scalar](../../../vector-space.md#scalar).

Every nonzero [linear functional](../../../dual-space.md#linear-functional) $V\to\mathbb F_p$ is surjective, so its [kernel](../../../kernel-of-a-linear-map.md) has [dimension](../../../vector-space.md#dimension-vector-space) $n-1$ by the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem). Conversely, every [hyperplane](../../../vector-space.md#hyperplane) $K$ is such a [kernel](../../../kernel-of-a-linear-map.md): extend a [basis](../../../vector-space.md#basis) of $K$ by one [vector](../../../vector-space.md#vector) $u$, and assign value zero on that [basis](../../../vector-space.md#basis) and value one on $u$. Hence the [hyperplanes](../../../vector-space.md#hyperplane) containing $v$ are exactly the [kernels](../../../kernel-of-a-linear-map.md) of the $p^{n-1}-1$ nonzero [linear functionals](../../../dual-space.md#linear-functional) counted above. Each [kernel](../../../kernel-of-a-linear-map.md) occurs for exactly $p-1$ of them, its distinct nonzero [scalar multiples](../../../vector-space.md#scalar-multiple). The required number is

$$
\boxed{\frac{p^{n-1}-1}{p-1}.}
$$

## 3

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [a](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [i](#3/a/i)

For the [linear map](../../../vector-space.md#linear-map) $T_A:x\mapsto Ax$ on the [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space) $\mathbb R^n$, the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) implies that injectivity and surjectivity are equivalent. Consequently $T_A$ is invertible if and only if $\ker T_A=\{0\}$.

Using the permitted equivalence between invertibility and a nonzero [determinant](../../../multilinear-algebra.md#determinant), we obtain

$$
\det A=0
\iff T_A\text{ is not invertible}
\iff\ker T_A\ne\{0\}
\iff \exists v\ne0:\ Av=0.
$$

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [a](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#3/a/ii)

We use the [monic polynomial](../../../polynomial.md#monic-polynomial) convention for the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) of an $n\times n$ [matrix](../../../vector-space.md#matrix):

$$
\boxed{\chi_A(t)=\det(tI_n-A).}
$$

It has degree $n$, since the only contribution to the coefficient of $t^n$ in the [determinant](../../../multilinear-algebra.md#determinant) is the product of the $n$ diagonal terms $t$. The alternative convention $\det(A-tI_n)=(-1)^n\chi_A(t)$ has the same [polynomial roots](../../../polynomial.md#root-of-a-polynomial).

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [a](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [iii](#3/a/iii)

A [scalar](../../../vector-space.md#scalar) $\lambda$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $A$ if and only if there is a nonzero [vector](../../../vector-space.md#vector) $v$ with $Av=\lambda v$. By the preceding [kernel](../../../kernel-of-a-linear-map.md) criterion,

$$
Av=\lambda v\text{ for some }v\ne0
\iff (\lambda I_n-A)v=0\text{ for some }v\ne0
\iff\det(\lambda I_n-A)=0.
$$

The last condition is $\chi_A(\lambda)=0$, exactly the definition of a [polynomial root](../../../polynomial.md#root-of-a-polynomial). For a [real matrix](../../../vector-space.md#real-matrix), this proves the assertion for real [eigenvalues](../../../linear-operator-theory.md#eigenvalue); the same proof over the [complex numbers](../../../complex-analysis.md#complex-number) gives the usual complex version.

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [a](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [iv](#3/a/iv)

Write $B=[b_1,\ldots,b_n]$. Since $AB=[Ab_1,\ldots,Ab_n]$ and $b\mapsto Ab$ is a [linear map](../../../vector-space.md#linear-map), the [multilinearity](../../../multilinear-algebra.md#multilinearity) of the [determinant](../../../multilinear-algebra.md#determinant) gives, for any column position $j$,

$$
D(b_1,\ldots,\alpha u+\beta w,\ldots,b_n)
=\alpha D(b_1,\ldots,u,\ldots,b_n)
+\beta D(b_1,\ldots,w,\ldots,b_n).
$$

If $b_i=b_j$ for $i\ne j$, the corresponding columns $Ab_i,Ab_j$ also agree, so $D(B)=0$. Thus $D$ is an [alternating multilinear map](../../../multilinear-algebra.md#alternating-multilinear-map) of the columns of $B$, even when $A$ is not invertible.

<h4 id="3/a/v">v</h4>

↑ **Parent:** [a](#3/a)

<h5 id="3/a/v/solution">Solution</h5>

↑ **Parent:** [v](#3/a/v)

We have $D(I_n)=\det A$. Define a function of the columns of $B$ by

$$
F(B)=D(B)+(1-\det A)\det B.
$$

It is an [alternating multilinear map](../../../multilinear-algebra.md#alternating-multilinear-map), because both summands are, and $F(I_n)=\det A+1-\det A=1$. Hence $F$ is a normalized [determinantal function](../../../multilinear-algebra.md#determinantal-function). By the asserted uniqueness of the [determinant](../../../multilinear-algebra.md#determinant), $F(B)=\det B$ for every $B$. Rearranging yields

$$
\boxed{\det(AB)=\det A\det B.}
$$

This argument also covers $\det A=0$ without dividing by it.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [b](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [i](#3/b/i)

Take the nonzero [vector](../../../vector-space.md#vector) $\mathbf1=(1,\ldots,1)^T$. Its $i$th image entry under [matrix multiplication](../../../vector-space.md#matrix-multiplication) is the sum of row $i$:

$$
(A\mathbf1)_i=\sum_{j=1}^n A_{ij}=\lambda.
$$

Thus $A\mathbf1=\lambda\mathbf1$, exhibiting $\mathbf1$ as an [eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\boxed{\lambda}$.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [b](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#3/b/ii)

Yes. The sums of the columns of $A$ are the sums of the rows of its [transpose](../../../vector-space.md#transpose) $A^T$. By the previous argument, $A^T\mathbf1=\lambda\mathbf1$, so $\det(\lambda I_n-A^T)=0$. The [determinant](../../../multilinear-algebra.md#determinant) is unchanged by [transpose](../../../vector-space.md#transpose), giving

$$
\det(\lambda I_n-A)
=\det\bigl((\lambda I_n-A)^T\bigr)
=\det(\lambda I_n-A^T)=0.
$$

Therefore $\boxed{\lambda\text{ is an eigenvalue of }A}$. The [vector](../../../vector-space.md#vector) $\mathbf1$ need not itself be an [eigenvector](../../../linear-operator-theory.md#eigenvector) of $A$ in the column-sum case.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [b](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [iii](#3/b/iii)

If $A$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), then

$$
BA=A^{-1}(AB)A.
$$

If instead $B$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), then

$$
AB=B^{-1}(BA)B.
$$

Thus in either case $AB$ and $BA$ are [similar matrices](../../../linear-algebra.md#matrix-similarity). Explicitly, whenever $Y=P^{-1}XP$ and $Xu=\lambda u$ with $u\ne0$, one has $Y(P^{-1}u)=\lambda P^{-1}u$ and $P^{-1}u\ne0$. Applying the same argument with $P^{-1}$ in place of $P$ proves equality of the sets of [eigenvalues](../../../linear-operator-theory.md#eigenvalue), including zero.

<h4 id="3/b/iv">iv</h4>

↑ **Parent:** [b](#3/b)

<h5 id="3/b/iv/solution">Solution</h5>

↑ **Parent:** [iv](#3/b/iv)

The same [matrix similarity](../../../linear-algebra.md#matrix-similarity) preserves being a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix). If $S^{-1}(AB)S=D$ is a [diagonal matrix](../../../linear-algebra.md#diagonal-matrix), then

$$
(A^{-1}S)^{-1}(BA)(A^{-1}S)
=S^{-1}A(BA)A^{-1}S
=S^{-1}(AB)S=D.
$$

Therefore $BA$ is a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) whenever $AB$ is, and the converse follows by interchanging $A,B$. Thus they are either both [diagonalisable matrices](../../../linear-operator-theory.md#diagonalizable-matrix) or neither is. In fact the previous part shows that one invertible factor suffices.

## 4

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [a](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [i](#4/a/i)

The real [spectral theorem](../../../hilbert-space.md#spectral-theorem) states that a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) has an [orthonormal basis](../../../inner-product.md#orthonormal-basis) of real [eigenvectors](../../../linear-operator-theory.md#eigenvector), and hence is a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix). Here is a proof in this setting.

For $n\ge1$, the [quadratic form](../../../quadratic-form.md) $q(x)=x^TAx$ attains a maximum on the [unit sphere](../../../topology.md#unit-sphere), by [compactness](../../../topology.md#compact-space) and the [extreme value theorem](../../../real-analysis.md#extreme-value-theorem). Choose a unit maximizer $u$ and put $\lambda=u^TAu$. For any $w\perp u$, the [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) along $u+tw$ has a maximum at $t=0$, so

$$
0=\left.\frac{d}{dt}\frac{(u+tw)^TA(u+tw)}{\|u+tw\|^2}\right|_{t=0}
=2w^TAu.
$$

The last equality uses $A=A^T$ and $u^Tw=0$. Thus $Au$ is orthogonal to every $w\perp u$, so $Au=\lambda u$.

The [orthogonal complement](../../../hilbert-space.md#orthogonal-complement) $u^\perp$ is an [invariant subspace](../../../representation-theory.md#invariant-subspace), because for $x\perp u$,

$$
u^TAx=(Au)^Tx=\lambda u^Tx=0.
$$

The [restriction](../../../function.md#restriction-mathematics) of $A$ to $u^\perp$ is again symmetric with respect to the induced [inner product](../../../inner-product.md). By [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on [dimension](../../../vector-space.md#dimension-vector-space), it has an [orthonormal basis](../../../inner-product.md#orthonormal-basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector); adjoining $u$ gives one for $\mathbb R^n$. If $Q$ has those [basis vectors](../../../vector-space.md#basis-vector) as columns, then $Q^TAQ$ is a real [diagonal matrix](../../../linear-algebra.md#diagonal-matrix) and $Q^{-1}=Q^T$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [a](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#4/a/ii)

Let $A$ be a [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix). For every real [vector](../../../vector-space.md#vector) $x$, the real [scalar](../../../vector-space.md#scalar) $x^TAx$ equals its own [transpose](../../../vector-space.md#transpose), but

$$
x^TAx=(x^TAx)^T=x^TA^Tx=-x^TAx.
$$

Hence $x^TAx=0$. If $Av=\lambda v$ is a real [eigenvector](../../../linear-operator-theory.md#eigenvector) equation with $v\ne0$, it follows that

$$
0=v^TAv=\lambda v^Tv,
$$

so $\lambda=0$. If $A$ is a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) over $\mathbb R$, it has a real [basis](../../../vector-space.md#basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector), all with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) zero. Thus $A$ vanishes on a [basis](../../../vector-space.md#basis) and $\boxed{A=0_n}$.

The [field](../../../algebra.md#field) matters: a nonzero real [skew-symmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) can be a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) over the [complex numbers](../../../complex-analysis.md#complex-number), for example $\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $i,-i$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [b](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [i](#4/b/i)

The [matrix units](../../../vector-space.md#matrix-unit) $E_{ij}$, $1\le i,j\le n$, form a [basis](../../../vector-space.md#basis) of $M_n(\mathbb R)$: each [matrix](../../../vector-space.md#matrix) has the unique expression $A=\sum_{i,j}a_{ij}E_{ij}$. There are $n^2$ of them, so

$$
\boxed{\dim M_n(\mathbb R)=n^2.}
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [b](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#4/b/ii)

Take the [vector subspace](../../../vector-space.md#vector-subspace) of [skew-symmetric matrices](../../../linear-algebra.md#skew-symmetric-matrix),

$$
K=\{A\in M_n(\mathbb R):A^T=-A\}.
$$

It is closed under [vector addition](../../../vector-space.md#vector-addition) and [scalar multiplication](../../../vector-space.md#scalar-multiplication), and a [basis](../../../vector-space.md#basis) is

$$
\{E_{ij}-E_{ji}:1\le i<j\le n\}.
$$

Indeed, its diagonal entries vanish, and its entries below the diagonal are forced by those above it. Hence $\boxed{\dim K=\binom n2}$. Part (a)(ii) proves that the only [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix) in $K$ is $0_n$.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [b](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [iii](#4/b/iii)

Let $S$ be the [vector subspace](../../../vector-space.md#vector-subspace) of [symmetric matrices](../../../linear-algebra.md#symmetric-matrix). A [basis](../../../vector-space.md#basis) consists of $E_{ii}$ for $1\le i\le n$ and $E_{ij}+E_{ji}$ for $i<j$, so

$$
\dim S=n+\binom n2=\frac{n(n+1)}2.
$$

The [dimension formula for a sum of subspaces](../../../vector-space.md#dimension-formula-for-a-sum-of-subspaces) now gives

$$
\begin{aligned}
\dim(V\cap S)
&=\dim V+\dim S-\dim(V+S)\\
&\ge\dim V+\frac{n(n+1)}2-n^2\\
&=\dim V-\binom n2>0.
\end{aligned}
$$

Choose $0\ne A\in V\cap S$. It belongs to $V$ and is a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), so part (a)(i) makes it a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix). The preceding example shows that the strict threshold is sharp.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [c](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [i](#4/c/i)

Write $r=(r_1,\ldots,r_n)^T$. The [linear map](../../../vector-space.md#linear-map) represented by $A$ has the form

$$
Ax=(r^Tx)e_i.
$$

The [image of a linear map](../../../vector-space.md#image-of-a-linear-map) here is contained in the one-dimensional [linear span](../../../vector-space.md#linear-span) of $e_i$, so its [matrix rank](../../../vector-space.md#matrix-rank) is at most one. The [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) yields

$$
\boxed{\dim\ker A=n-\operatorname{rank}A\ge n-1.}
$$

Thus the solution space of $Ax=0$, namely the zero [eigenspace](../../../linear-operator-theory.md#eigenspace) when zero is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue), contains at least $n-1$ [linearly independent vectors](../../../vector-space.md#linear-independence). If $r=0$ its [dimension](../../../vector-space.md#dimension-vector-space) is $n$; otherwise it is $n-1$. When $n=1$ the asserted lower bound is zero, even if zero is not an [eigenvalue](../../../linear-operator-theory.md#eigenvalue).

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [c](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [ii](#4/c/ii)

Since $Ae_i=r_ie_i$, the [vector](../../../vector-space.md#vector) $e_i$ is an [eigenvector](../../../linear-operator-theory.md#eigenvector) with nonzero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $r_i$. The assumption $r_i\ne0$ also makes $r\ne0$, so the [kernel](../../../kernel-of-a-linear-map.md) has [dimension](../../../vector-space.md#dimension-vector-space) $n-1$. Choose its [basis](../../../vector-space.md#basis) $u_1,\ldots,u_{n-1}$.

The [vector](../../../vector-space.md#vector) $e_i$ is outside this [kernel](../../../kernel-of-a-linear-map.md). Hence $(u_1,\ldots,u_{n-1},e_i)$ is a [basis](../../../vector-space.md#basis) of $\mathbb R^n$ consisting of [eigenvectors](../../../linear-operator-theory.md#eigenvector), with corresponding [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $0,\ldots,0,r_i$. In that [basis](../../../vector-space.md#basis), $A$ is the [diagonal matrix](../../../linear-algebra.md#diagonal-matrix)

$$
\boxed{\operatorname{diag}(0,\ldots,0,r_i).}
$$

This proves that $A$ is a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix), including the case $n=1$.

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [c](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [iii](#4/c/iii)

Yes. Consider the following $n^2$ [matrices](../../../vector-space.md#matrix):

$$
\boxed{\mathcal B=\{E_{ii}:1\le i\le n\}
\ \cup\ \{E_{ii}+E_{ij}:1\le i,j\le n,\ i\ne j\}.}
$$

Each has only row $i$ nonzero and has $i$th diagonal entry $1$, so part (c)(ii) proves that it is a [diagonalisable matrix](../../../linear-operator-theory.md#diagonalizable-matrix). The collection is a [spanning set](../../../vector-space.md#spanning-set), because it contains every $E_{ii}$ and

$$
E_{ij}=(E_{ii}+E_{ij})-E_{ii}\qquad(i\ne j).
$$

Thus it spans the [matrix unit](../../../vector-space.md#matrix-unit) [basis](../../../vector-space.md#basis). A [spanning set](../../../vector-space.md#spanning-set) of $n^2$ [vectors](../../../vector-space.md#vector) in an $n^2$-dimensional [vector space](../../../vector-space.md) is a [basis](../../../vector-space.md#basis). Alternatively, in a vanishing [linear combination](../../../vector-space.md#linear-combination) of $\mathcal B$, each off-diagonal entry first forces its own coefficient to be zero, and then each diagonal entry forces the remaining coefficient to be zero.

## 5

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [a](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [i](#5/a/i)

In the [finite field](../../../algebra.md#finite-field) $\mathbb Z_3=\{0,1,2\}$, perform ordinary addition and multiplication and then take the remainder modulo $3$. The tables are

$$
\begin{array}{c|ccc}
+&0&1&2\\\hline
0&0&1&2\\
1&1&2&0\\
2&2&0&1
\end{array}
\qquad
\begin{array}{c|ccc}
\cdot&0&1&2\\\hline
0&0&0&0\\
1&0&1&2\\
2&0&2&1
\end{array}.
$$

The nonzero elements have multiplicative inverses $1^{-1}=1$ and $2^{-1}=2$.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [a](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#5/a/ii)

Parametrize the [matrices](../../../vector-space.md#matrix) by

$$
h(a,b,c)=\begin{pmatrix}1&a&b\\0&1&c\\0&0&1\end{pmatrix},
\qquad a,b,c\in\mathbb Z_3.
$$

Direct [matrix multiplication](../../../vector-space.md#matrix-multiplication) gives

$$
h(a,b,c)h(a',b',c')
=h(a+a',\ b+b'+ac',\ c+c').
$$

This proves closure. The [identity matrix](../../../vector-space.md#identity-matrix) is $h(0,0,0)$, and the formula

$$
\boxed{h(a,b,c)^{-1}=h(-a,\ ac-b,\ -c)}
$$

gives both a left and a right inverse, as substitution in the product formula verifies. Thus each element is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), and the [subgroup test](../../../group.md#subgroup-test) shows that $H$ is a [subgroup](../../../group.md#subgroup) of $\operatorname{GL}_3(\mathbb Z_3)$. It is the [unitriangular group](../../../group-theory.md#unitriangular-group) $\operatorname{UT}_3(\mathbb F_3)$ and has $3^3=27$ elements.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [a](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [iii](#5/a/iii)

The identity is the [identity matrix](../../../vector-space.md#identity-matrix)

$$
\boxed{e=h(0,0,0)=I_3=\begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}.}
$$

Left or right [matrix multiplication](../../../vector-space.md#matrix-multiplication) by it preserves every entry, as is also immediate from the product formula above.

<h4 id="5/a/iv">iv</h4>

↑ **Parent:** [a](#5/a)

<h5 id="5/a/iv/solution">Solution</h5>

↑ **Parent:** [iv](#5/a/iv)

Take $x=h(1,0,0)=I_3+E_{12}$ and $y=h(0,0,1)=I_3+E_{23}$. Their [matrix products](../../../vector-space.md#matrix-product) are

$$
xy=\begin{pmatrix}1&1&1\\0&1&1\\0&0&1\end{pmatrix},
\qquad
yx=\begin{pmatrix}1&1&0\\0&1&1\\0&0&1\end{pmatrix}.
$$

They differ in the $(1,3)$ entry because $E_{12}E_{23}=E_{13}$ whereas $E_{23}E_{12}=0$. Therefore $xy\ne yx$, and $\boxed{H\text{ is a non-abelian group}}$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [b](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [i](#5/b/i)

If $G$ is an [abelian group](../../../group.md#abelian-group), its elements commute, so for all $x,y\in G$,

$$
T(xy)=(xy)^3=xyxyxy=x^3y^3=T(x)T(y).
$$

Thus $\boxed{T\text{ is a group homomorphism}}$. Also $T(e)=e^3=e$, as required.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [b](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#5/b/ii)

Use the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_3$, composing [permutations](../../../combinatorics.md#permutation) from right to left. Set $x=(12)$ and $y=(23)$. Each is a [transposition](../../../combinatorics.md#transposition-permutation), so $x^3=x$ and $y^3=y$, whereas $xy=(123)$ has [order of a group element](../../../group-theory.md#order-of-a-group-element) three. Consequently

$$
T(xy)=(123)^3=e,\qquad T(x)T(y)=(12)(23)=(123)\ne e.
$$

Thus the cubing map on $S_3$ is not a [group homomorphism](../../../group-theory.md#group-homomorphism).

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [b](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [iii](#5/b/iii)

Assume $T$ is a [group homomorphism](../../../group-theory.md#group-homomorphism). For any $a,b\in G$, expanding $(ab)^3=a^3b^3$ and cancelling the initial $a$ and final $b$ gives the useful identity

$$
\boxed{(ba)^2=a^2b^2.}\qquad\text{(1)}
$$

We also need a consequence of compatibility with [conjugation](../../../group-action.md#conjugation). Calculate the cube of $gzg^{-1}$ in two ways:

$$
gz^3g^{-1}=(gzg^{-1})^3
=T(g)T(z)T(g)^{-1}=g^3z^3g^{-3}.
$$

Cancelling shows $g^2z^3=z^3g^2$. Thus the square of every element of $G$ commutes with every element of the [image of a group homomorphism](../../../group-theory.md#image-of-a-group-homomorphism) $J=T(G)$.

Now take any $x,y\in J$. In particular $x^2y=yx^2$. Applying (1) to $x,y$ and then using this commutation gives

$$
yxyx=x^2y^2,
\qquad
xyx=y^{-1}x^2y^2=x^2y,
\qquad
yx=xy.
$$

This proves the [abelian image of a cubing homomorphism](../../../group-theory.md#abelian-image-of-a-cubing-homomorphism) property. Since the [image of a group homomorphism](../../../group-theory.md#image-of-a-group-homomorphism) is a [subgroup](../../../group.md#subgroup), $\boxed{T(G)\text{ is an abelian group}}$.

<h4 id="5/b/iv">iv</h4>

↑ **Parent:** [b](#5/b)

<h5 id="5/b/iv/solution">Solution</h5>

↑ **Parent:** [iv](#5/b/iv)

If $T$ is a surjective [group homomorphism](../../../group-theory.md#group-homomorphism), then $G=T(G)$, which is an [abelian group](../../../group.md#abelian-group) by the preceding part.

If $T$ is an injective [group homomorphism](../../../group-theory.md#group-homomorphism), then for all $a,b\in G$,

$$
T(ab)=T(a)T(b)=T(b)T(a)=T(ba),
$$

because $T(a),T(b)$ lie in the [abelian group](../../../group.md#abelian-group) $T(G)$. Injectivity gives $ab=ba$. Hence $\boxed{G\text{ is abelian in either case}}$.

<h4 id="5/b/v">v</h4>

↑ **Parent:** [b](#5/b)

<h5 id="5/b/v/solution">Solution</h5>

↑ **Parent:** [v](#5/b/v)

Yes: use the [non-abelian group](../../../group.md#non-abelian-group) $H$ from part (a). Every element is $I_3+N$ for a [strictly upper triangular matrix](../../../linear-algebra.md#strictly-upper-triangular-matrix) $N$ with $N^3=0$. In the [finite field](../../../algebra.md#finite-field) $\mathbb Z_3$, the [binomial theorem for commuting matrices](../../../binomial-coefficient.md#binomial-theorem-for-commuting-matrices) gives

$$
(I_3+N)^3=I_3+3N+3N^2+N^3=I_3.
$$

Thus $\boxed{T(h)=I_3\text{ for all }h\in H}$. This constant identity-valued map is a [group homomorphism](../../../group-theory.md#group-homomorphism), since $T(xy)=I_3=T(x)T(y)$. Part (a)(iv) already proves that $H$ is not an [abelian group](../../../group.md#abelian-group). Here $T$ is neither injective nor surjective, consistently with the preceding part.

## 6

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [a](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [i](#6/a/i)

The set $S_n$ is nonempty because $n\in S_n$. By the [well-ordering principle](../../../arithmetic.md#well-ordering-principle-for-the-natural-numbers) for the [natural numbers](../../../arithmetic.md#natural-number), it has a least element $p$. In particular $p>1$ and $p$ divides $n$.

If $p$ were not a [prime number](../../../prime-number.md), it would have a positive [integer divisor](../../../divisibility.md#divisor) $d$ with $1<d<p$. Since $d$ divides $p$ and $p$ divides $n$, [divisibility](../../../divisibility.md) is transitive and $d$ divides $n$. This would put $d$ in $S_n$, contradicting the minimality of $p$. Hence $\boxed{p\text{ is prime}}$.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [a](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#6/a/ii)

Neither $1$ nor $-1$ is divisible by a [prime number](../../../prime-number.md), so both lie outside $U$. On the other hand, $0\in2\mathbb Z\subseteq U$. If an [integer](../../../integer.md) $z$ has $|z|>1$, part (a)(i) supplies a [prime number](../../../prime-number.md) $p$ dividing the positive [integer](../../../integer.md) $|z|$; the same $p$ divides $z$, so $z\in p\mathbb Z\subseteq U$. These cases exhaust $\mathbb Z$, proving

$$
\boxed{\mathbb Z\setminus U=\{-1,1\}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [b](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [i](#6/b/i)

For every $g\in G$, left multiplication gives a [bijection](../../../function.md#bijection)

$$
H\longrightarrow gH,\qquad h\longmapsto gh,
$$

whose inverse is $x\mapsto g^{-1}x$. Hence every [left coset](../../../group-theory.md#left-coset) has the same [cardinality](../../../cardinal-number.md#cardinality) as $H$. If $H$ is an [infinite set](../../../set.md#infinite-set), every [left coset](../../../group-theory.md#left-coset) is infinite; if $H$ is a [finite set](../../../set.md#finite-set), every [left coset](../../../group-theory.md#left-coset) is finite. These are the only possibilities.

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [b](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#6/b/ii)

Suppose $H$ were finite, say $|H|=r$. There are at most $n$ [left cosets](../../../group-theory.md#left-coset), each with $r$ elements by part (i), and they partition $G$. Hence $G$ would be a [finite set](../../../set.md#finite-set) with at most $nr$ elements. This contradicts the assumption that $G$ is an [infinite group](../../../group.md#infinite-group). Therefore $\boxed{H\text{ is infinite}}$.

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [b](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [iii](#6/b/iii)

Every [left coset](../../../group-theory.md#left-coset) $kH$ with $k\in K$ is also a [left coset](../../../group-theory.md#left-coset) of $H$ in $G$. Moreover equality of two such [cosets](../../../group-theory.md#coset) means the same thing in $K$ and in $G$:

$$
kH=k'H\iff k'^{-1}k\in H.
$$

Thus the map from the set of [left cosets](../../../group-theory.md#left-coset) of $H$ in $K$ to the set of [left cosets](../../../group-theory.md#left-coset) of $H$ in $G$, taking $kH$ to itself, is injective. Consequently the [index of a subgroup](../../../group.md#index-of-a-subgroup) satisfies

$$
\boxed{|K/H|\le|G/H|\le n.}
$$

These are sets of [cosets](../../../group-theory.md#coset); no [normal subgroup](../../../group-theory.md#normal-subgroup) assumption is needed.

<h4 id="6/b/iv">iv</h4>

↑ **Parent:** [b](#6/b)

<h5 id="6/b/iv/solution">Solution</h5>

↑ **Parent:** [iv](#6/b/iv)

Define a map between sets of [left cosets](../../../group-theory.md#left-coset) by

$$
\Phi:G/(H\cap K)\longrightarrow(G/H)\times(G/K),
\qquad g(H\cap K)\longmapsto(gH,gK).
$$

It is well defined: replacing $g$ by $gu$ for $u\in H\cap K$ changes neither component. It is injective because

$$
gH=g'H\text{ and }gK=g'K
\iff g'^{-1}g\in H\cap K
\iff g(H\cap K)=g'(H\cap K).
$$

The [Cartesian product](../../../set-theory.md#cartesian-product) on the right has at most $nm$ elements. Therefore

$$
\boxed{|G/(H\cap K)|\le|G/H|\,|G/K|\le nm.}
$$

This proves the basic bound for a [finite intersection of finite-index subgroups](../../../group.md#finite-intersection-of-finite-index-subgroups).

<h4 id="6/b/v">v</h4>

↑ **Parent:** [b](#6/b)

<h5 id="6/b/v/solution">Solution</h5>

↑ **Parent:** [v](#6/b/v)

Put $L=\bigcap_{i=1}^kH_i$. Repeated application of part (iv), or [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $k$, gives

$$
|G/L|\le\prod_{i=1}^k n_i<\infty.
$$

Part (ii) therefore implies that $L$ is an [infinite set](../../../set.md#infinite-set). If $G\setminus U$ is nonempty, choose $g\notin U$. We claim its [left coset](../../../group-theory.md#left-coset) $gL$ is wholly outside $U$. If $g\ell\in H_i$ for some $\ell\in L$, then $\ell\in H_i$ and closure under products and inverses would give $g=(g\ell)\ell^{-1}\in H_i$, a contradiction.

Thus $gL\subseteq G\setminus U$. Part (i) makes $gL$ infinite, so the complement is infinite. If there is no such $g$, the complement is empty. This proves the [complement of a finite union of finite-index subgroups](../../../group.md#complement-of-a-finite-union-of-finite-index-subgroups) property:

$$
\boxed{G\setminus(H_1\cup\cdots\cup H_k)\text{ is empty or infinite}.}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [c](#6/c)

Suppose there were only finitely many [prime numbers](../../../prime-number.md), say $p_1,\ldots,p_k$. Work in the [infinite group](../../../group.md#infinite-group) $(\mathbb Z,+)$ and set $H_i=p_i\mathbb Z$. The [left cosets](../../../group-theory.md#left-coset) are the $p_i$ residue classes modulo $p_i$, so each $H_i$ is a [finite-index subgroup](../../../group.md#finite-index-subgroup), with $|\mathbb Z/H_i|=p_i$.

By part (b)(v), $\mathbb Z\setminus\bigcup_i p_i\mathbb Z$ is empty or infinite. But part (a)(ii) identifies it as the nonempty two-element set $\{-1,1\}$. This contradiction proves [Euclid's theorem](../../../prime-number.md#euclid-s-theorem):

$$
\boxed{\text{There are infinitely many prime numbers}.}
$$

## 7

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [a](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [i](#7/a/i)

Conjugating a [cycle](../../../finite-group-theory.md#permutation-cycle) simply relabels its entries. With [permutations](../../../combinatorics.md#permutation) composed from right to left,

$$
\rho(a_1\ a_2\ \cdots\ a_\ell)\rho^{-1}
=(\rho(a_1)\ \rho(a_2)\ \cdots\ \rho(a_\ell)).
$$

This follows by applying each side to $\rho(a_j)$ and to points outside the displayed [cycle](../../../finite-group-theory.md#permutation-cycle). Consequently [conjugation](../../../group-action.md#conjugation) preserves the lengths in the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition), including fixed points, and therefore preserves [cycle type](../../../finite-group-theory.md#cycle-type).

Conversely, suppose two [permutations](../../../combinatorics.md#permutation) have the same [cycle type](../../../finite-group-theory.md#cycle-type). Pair their [cycles](../../../finite-group-theory.md#permutation-cycle) of equal length, including their one-cycles. Define a [bijection](../../../function.md#bijection) $\rho$ by mapping the entries of each [cycle](../../../finite-group-theory.md#permutation-cycle) of the first [permutation](../../../combinatorics.md#permutation), in their cyclic order, to the entries of the paired [cycle](../../../finite-group-theory.md#permutation-cycle) of the second. Because the [cycles](../../../finite-group-theory.md#permutation-cycle) partition $\{1,\ldots,n\}$, these assignments combine into a [permutation](../../../combinatorics.md#permutation). The displayed identity then conjugates the first [permutation](../../../combinatorics.md#permutation) to the second. Thus they are [conjugate group elements](../../../group-action.md#conjugate-group-elements) exactly when their [cycle types](../../../finite-group-theory.md#cycle-type) agree.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [a](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [ii](#7/a/ii)

Let the lengths in the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) of $\tau$ be $\ell_1,\ldots,\ell_s$, with fixed points contributing length one. Disjoint [cycles](../../../finite-group-theory.md#permutation-cycle) commute, and $\tau^m=e$ if and only if every [cycle](../../../finite-group-theory.md#permutation-cycle) raised to $m$ is the identity, equivalently $\ell_j$ divides $m$ for every $j$. Hence the [order of a group element](../../../group-theory.md#order-of-a-group-element) is

$$
\boxed{\operatorname{ord}(\tau)=\operatorname{lcm}(\ell_1,\ldots,\ell_s).}
$$

In particular, the identity has order one.

<h4 id="7/a/iii">iii</h4>

↑ **Parent:** [a](#7/a)

<h5 id="7/a/iii/solution">Solution</h5>

↑ **Parent:** [iii](#7/a/iii)

For $0\le k\le\lfloor n/2\rfloor$, first select an ordered list of $2k$ distinct entries. There are $n!/(n-2k)!$ lists. Pair consecutive entries to obtain

$$
(a_1a_2)(a_3a_4)\cdots(a_{2k-1}a_{2k}).
$$

Each product of $k$ disjoint [transpositions](../../../combinatorics.md#transposition-permutation) is counted $2^k k!$ times: each pair has two orientations, and the $k$ pairs can be ordered in $k!$ ways. There is no other duplication, by uniqueness of the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition). Therefore

$$
\boxed{|T_k|=\frac{n!}{2^k k!(n-2k)!}.}
$$

If $2k>n$, there are no such [permutations](../../../combinatorics.md#permutation). For $k=0$, $T_0=\{e\}$.

<h4 id="7/a/iv">iv</h4>

↑ **Parent:** [a](#7/a)

<h5 id="7/a/iv/solution">Solution</h5>

↑ **Parent:** [iv](#7/a/iv)

For distinct $i,j\ne1$, direct [conjugation](../../../group-action.md#conjugation) gives

$$
(ij)=(1i)(1j)(1i).
$$

Thus the given star [transpositions](../../../combinatorics.md#transposition-permutation) generate every [transposition](../../../combinatorics.md#transposition-permutation). Every [cycle](../../../finite-group-theory.md#permutation-cycle) can in turn be expressed as

$$
(a_1a_2\cdots a_\ell)
=(a_1a_\ell)(a_1a_{\ell-1})\cdots(a_1a_2).
$$

By the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition), every [permutation](../../../combinatorics.md#permutation) is a product of [cycles](../../../finite-group-theory.md#permutation-cycle), hence of [transpositions](../../../combinatorics.md#transposition-permutation), hence of the given star [transpositions](../../../combinatorics.md#transposition-permutation). Therefore

$$
\boxed{\langle(12),(13),\ldots,(1n)\rangle=S_n.}
$$

For $n=1$, the empty [generating set of a group](../../../group.md#generating-set-of-a-group) generates the [trivial group](../../../group.md#trivial-group) $S_1$.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [b](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [i](#7/b/i)

Assume first $n\ge2$. All [transpositions](../../../combinatorics.md#transposition-permutation) form a single [conjugacy class](../../../group-action.md#conjugacy-class) $T_1$. A [group automorphism](../../../algebra.md#group-automorphism) preserves [order of a group element](../../../group-theory.md#order-of-a-group-element), so the image of a [transposition](../../../combinatorics.md#transposition-permutation) is a nonidentity [involution](../../../group-theory.md#involution). By the order formula, its [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) contains only one-cycles and two-cycles, with at least one two-cycle. Thus it lies in some $T_k$, where $1\le k\le\lfloor n/2\rfloor$.

Moreover an [automorphism](../../../algebra.md#automorphism) maps the entire [conjugacy class](../../../group-action.md#conjugacy-class) onto the [conjugacy class](../../../group-action.md#conjugacy-class) of the image: for a fixed [transposition](../../../combinatorics.md#transposition-permutation) $t$,

$$
\phi(gtg^{-1})=\phi(g)\phi(t)\phi(g)^{-1},
$$

and $\phi(g)$ runs over all of $S_n$ by surjectivity. Part (a)(i) identifies that latter [conjugacy class](../../../group-action.md#conjugacy-class) as $T_k$. Hence $\boxed{\phi(T_1)=T_k}$, with equality rather than just inclusion. If $n=1$, $T_1$ is empty and the equality holds trivially with $k=1$.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [b](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [ii](#7/b/ii)

For $n\ge2$ with $n\ne6$, bijectivity of $\phi$ and the previous part imply

$$
\frac{n!}{2^k k!(n-2k)!}=|T_k|=|T_1|=\frac{n(n-1)}2.
$$

The supplied numerical fact forces $k=1$. Thus $\phi$ permutes the [transpositions](../../../combinatorics.md#transposition-permutation).

Suppose $n\ge3$, and write $s_r=\phi((1r))$ for $r=2,\ldots,n$. These are distinct [transpositions](../../../combinatorics.md#transposition-permutation). For $r\ne t$, the product $(1r)(1t)$ has [order of a group element](../../../group-theory.md#order-of-a-group-element) three, so $s_rs_t$ also has order three. Two distinct [transpositions](../../../combinatorics.md#transposition-permutation) have this property precisely when their two-element sets of moved points meet in one point: disjoint ones have a product of order two, whereas ones sharing one point have a three-cycle as product. The two-element [support of a permutation](../../../finite-group-theory.md#support-of-a-permutation) associated with each $s_r$ therefore meets that of every other $s_t$.

We now show that they have a common point. Choose two; the [support of a permutation](../../../finite-group-theory.md#support-of-a-permutation) is $\{a,b\}$ for one and $\{a,c\}$ for the other, where $a,b,c$ are distinct. Any further two-element set meeting both either contains $a$ or is $\{b,c\}$. If $\{b,c\}$ occurs, any two-element set meeting all three must itself be one of $\{a,b\},\{a,c\},\{b,c\}$: a set containing $a$ must also contain $b$ or $c$, and a set omitting $a$ must contain both $b,c$. Hence a pairwise-intersecting family with no common point consists of exactly those three edges of a triangle.

For $n\ge5$, there are $n-1\ge4$ distinct $s_r$, ruling out that triangle. For $n=3$, the two sets already have a common point. For $n=4$, the triangle alternative would make all three $s_r$ fix the fourth point. They would then generate a proper [subgroup](../../../group.md#subgroup) of $S_4$, contrary to surjectivity of $\phi$ and part (a)(iv), which imply that the $s_r$ generate $S_4$. Thus in every case $n\ge3$ there is a common point $a$, and we may write

$$
s_r=(a\ b_r)\qquad(2\le r\le n).
$$

The $b_r$ are distinct and different from $a$, so they exhaust the remaining $n-1$ points. Define a [permutation](../../../combinatorics.md#permutation) $\sigma$ by

$$
\sigma(a)=1,\qquad \sigma(b_r)=r.
$$

Then

$$
\sigma^{-1}(1r)\sigma
=(\sigma^{-1}(1)\ \sigma^{-1}(r))
=(a\ b_r)=\phi((1r)).
$$

The two [group homomorphisms](../../../group-theory.md#group-homomorphism) $\tau\mapsto\phi(\tau)$ and $\tau\mapsto\sigma^{-1}\tau\sigma$ agree on a [generating set of a group](../../../group.md#generating-set-of-a-group), so agree on every product of its elements, hence throughout $S_n$:

$$
\boxed{\phi(\tau)=\sigma^{-1}\tau\sigma\qquad(\tau\in S_n).}
$$

Finally, $S_1$ is trivial and $S_2$ has a unique nonidentity element, so every [automorphism](../../../algebra.md#automorphism) of either is the identity and we can take $\sigma=e$. This completes all degrees $n\ne6$ and proves that every such [automorphism](../../../algebra.md#automorphism) is an [inner automorphism](../../../group-theory.md#inner-automorphism).

## ↑ Ancestors (9)

1. [Prelims](../prelims.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Oxford](../../../past-exam-of-the-mathematics-course-of-the-university-of-oxford.md)
4. [Mathematics course of the University of Oxford](../../../university-of-oxford.md#mathematics-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../../university-of-oxford.md)
8. [List of universities](../../../README.md#list-of-universities)
9. [Codex Wiki](../../../README.md)
