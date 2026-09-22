# Mathematics I

↑ **Parent:** [Prelims](../prelims.md)

Source: [released examination PDF, bundle pages 1–4](https://www.whatdotheyknow.com/request/bsc_mathematics_prelims_and_part/response/2784209/attach/3/202409%20817%20annex.pdf#page=1).

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
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [A](#2/c/ii/a)
        - [Solution](#2/c/ii/a/solution)
      - [B](#2/c/ii/b)
        - [Solution](#2/c/ii/b/solution)
      - [C](#2/c/ii/c)
        - [Solution](#2/c/ii/c/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
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
    - [iv](#6/a/iv)
      - [Solution](#6/a/iv/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
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

For the [linear map](../../../vector-space.md#linear-map) $T:V\to W$, its [image of a linear map](../../../vector-space.md#image-of-a-linear-map) and [kernel of a linear map](../../../kernel-of-a-linear-map.md) are

$$
\boxed{\operatorname{im}T=\{T(v):v\in V\},\qquad\ker T=\{v\in V:T(v)=0\}.}
$$

Both contain the [zero vector](../../../vector-space.md#zero-vector), since $T(0)=0$. If $y_1=T(v_1)$ and $y_2=T(v_2)$ belong to the [image of a linear map](../../../vector-space.md#image-of-a-linear-map), then for any [real numbers](../../../arithmetic.md#real-number) $a,b$,

$$
ay_1+by_2=T(av_1+bv_2)\in\operatorname{im}T.
$$

Thus $\operatorname{im}T$ is a [vector subspace](../../../vector-space.md#vector-subspace) of $W$. If $u_1,u_2\in\ker T$, then

$$
T(au_1+bu_2)=aT(u_1)+bT(u_2)=0,
$$

so $\ker T$ is a [vector subspace](../../../vector-space.md#vector-subspace) of $V$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [rank of a linear map](../../../vector-space.md#rank-of-a-linear-map) and [nullity of a linear map](../../../kernel-of-a-linear-map.md#nullity-of-a-linear-map) are

$$
r(T)=\dim\operatorname{im}T,\qquad n(T)=\dim\ker T.
$$

The [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) states that

$$
\boxed{r(T)+n(T)=\dim V=n.}
$$

To prove it, choose a [basis](../../../vector-space.md#basis) $u_1,\ldots,u_k$ of the [kernel of a linear map](../../../kernel-of-a-linear-map.md) and use [basis extension](../../../vector-space.md#basis-extension) to obtain a [basis](../../../vector-space.md#basis)

$$
u_1,\ldots,u_k,v_1,\ldots,v_{n-k}
$$

of $V$. The [vectors](../../../vector-space.md#vector) $T(v_1),\ldots,T(v_{n-k})$ [span](../../../vector-space.md#linear-span) the [image of a linear map](../../../vector-space.md#image-of-a-linear-map): applying $T$ to an arbitrary [linear combination](../../../vector-space.md#linear-combination) of the displayed [basis](../../../vector-space.md#basis) removes all the $u_i$ terms. They are also [linearly independent](../../../vector-space.md#linear-independence). Indeed,

$$
\sum_j a_jT(v_j)=0\quad\Longrightarrow\quad\sum_j a_jv_j\in\ker T,
$$

so $\sum_j a_jv_j=\sum_i b_iu_i$ for some [scalars](../../../vector-space.md#scalar) $b_i$. The [linear independence](../../../vector-space.md#linear-independence) of the extended [basis](../../../vector-space.md#basis) forces every $a_j$ and $b_i$ to vanish. Consequently $r(T)=n-k$ and $n(T)=k$, proving the identity. The same argument covers an empty [basis](../../../vector-space.md#basis) when one of these [dimensions](../../../vector-space.md#dimension-vector-space) is zero.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Here $\dim V=2$. By the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem), $r(T)+n(T)=2$, and a [dimension](../../../vector-space.md#dimension-vector-space) is a nonnegative integer. All three possibilities occur:

$$
\boxed{\begin{array}{c|c}
(r(T),n(T))&T(x,y)\\\hline
(0,2)&(0,0,0)\\
(1,1)&(x,0,0)\\
(2,0)&(x,y,0)
\end{array}}
$$

The [images of a linear map](../../../vector-space.md#image-of-a-linear-map) in these examples have [dimensions](../../../vector-space.md#dimension-vector-space) $0,1,2$, respectively, while the corresponding [kernel of a linear map](../../../kernel-of-a-linear-map.md) is $\mathbb R^2$, $\{(0,y):y\in\mathbb R\}$ and $\{0\}$. The identity above excludes all other pairs.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

If $TS=\operatorname{id}_W$, every $w\in W$ would satisfy $w=T(Sw)$, so $T$ would be a [surjective linear map](../../../vector-space.md#surjective-linear-map). But its [image of a linear map](../../../vector-space.md#image-of-a-linear-map) has [dimension](../../../vector-space.md#dimension-vector-space) at most $\dim V=2$, whereas $\dim W=3$. Therefore **no such $S$ exists**. This is the obstruction to a [right inverse](../../../function.md#right-inverse): $T$ cannot reach every target [vector](../../../vector-space.md#vector).

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The necessary and sufficient condition is

$$
\boxed{\ker T=\{0\}.}
$$

For necessity, if $ST=\operatorname{id}_V$ and $v\in\ker T$, then $v=S(Tv)=S(0)=0$.

For sufficiency, let $e_1,e_2$ be a [basis](../../../vector-space.md#basis) of $V$ and suppose the [kernel of a linear map](../../../kernel-of-a-linear-map.md) is trivial. The [vectors](../../../vector-space.md#vector) $Te_1,Te_2$ are [linearly independent](../../../vector-space.md#linear-independence), since $aTe_1+bTe_2=0$ implies $ae_1+be_2\in\ker T$. Extend them to a [basis](../../../vector-space.md#basis) $Te_1,Te_2,w_3$ of $W$. Define a [linear map](../../../vector-space.md#linear-map) $S$ by

$$
S(Te_1)=e_1,\qquad S(Te_2)=e_2,\qquad S(w_3)=0.
$$

Then $ST$ agrees with the [identity operator](../../../vector-space.md#identity-operator) on a [basis](../../../vector-space.md#basis), hence on all of $V$. Thus a [left inverse](../../../function.md#left-inverse) exists precisely when $T$ is [injective](../../../algebra.md#injective-function); this is the [linear left inverse criterion](../../../vector-space.md#linear-left-inverse-criterion).

## 2

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

An [elementary row operation](../../../numerical-linear-algebra.md#elementary-row-operation) is one of three reversible changes: interchange two rows; multiply one row by a nonzero [scalar](../../../vector-space.md#scalar); or add a [scalar multiple](../../../vector-space.md#scalar-multiple) of one row to a different row. Their inverses are, respectively, the same interchange, multiplication by the reciprocal, and addition of the negative [scalar multiple](../../../vector-space.md#scalar-multiple).

Applied to an [augmented matrix](../../../linear-algebra.md#augmented-matrix), these changes interchange [linear equations](../../../linear-algebra.md#linear-equation), rescale an equation by a nonzero factor, or add a multiple of one equation to another. Every old solution satisfies the new equations. Applying the inverse [elementary row operation](../../../numerical-linear-algebra.md#elementary-row-operation) gives the converse, so **the solution set is unchanged** at every step. Equivalently, all the operations together give

$$
[\widetilde A\mid\widetilde b]=E[A\mid b],\qquad\widetilde Ax=\widetilde b\iff EAx=Eb\iff Ax=b,
$$

where $E$ is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), a product of [elementary matrices](../../../numerical-linear-algebra.md#elementary-matrix).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Writing the unknown [vector](../../../vector-space.md#vector) as $(x,y,z)^T$, the first two [linear equations](../../../linear-algebra.md#linear-equation) give $x=z-1$ and $y=z-\beta$. Substitution into the third gives

$$
-(z-1)-(z-\beta)+\alpha z=1,\qquad(\alpha-2)z=-\beta.
$$

Thus, when $\alpha\ne2$, put $t=-\beta/(\alpha-2)$. There is exactly one solution:

$$
\boxed{(x,y,z)=(t-1,t-\beta,t),\qquad t=-\frac{\beta}{\alpha-2}.}
$$

When $\alpha=2$, the remaining equation is $0=-\beta$. Hence

$$
\boxed{\begin{aligned}
\alpha=2,\ \beta\ne0&:\quad\varnothing,\\
\alpha=2,\ \beta=0&:\quad\{(-1,0,0)+t(1,1,1):t\in\mathbb R\}.
\end{aligned}}
$$

The second case is an [affine line in a vector space](../../../vector-space.md#affine-line-in-a-vector-space), so it contains infinitely many solutions. These cases exhaust all [real numbers](../../../arithmetic.md#real-number) $\alpha,\beta$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

A [system of linear equations](../../../linear-algebra.md#system-of-linear-equations) $T_\alpha x=b$ is solvable exactly when $b\in\operatorname{im}T_\alpha$. If $x_0$ is one solution, then

$$
T_\alpha x=b\iff T_\alpha(x-x_0)=0,
$$

so its solution set is $x_0+\ker T_\alpha$, a translate of the [kernel of a linear map](../../../kernel-of-a-linear-map.md).

For $\alpha\ne2$, the [matrix](../../../vector-space.md#matrix) is an [invertible matrix](../../../linear-algebra.md#invertible-matrix), and

$$
\boxed{\operatorname{im}T_\alpha=\mathbb R^3,\qquad\ker T_\alpha=\{0\}.}
$$

Every $b$ is in the [image of a linear map](../../../vector-space.md#image-of-a-linear-map) and has exactly one preimage. For $\alpha=2$, its first two columns [span](../../../vector-space.md#linear-span) the [image of a linear map](../../../vector-space.md#image-of-a-linear-map), while the corresponding [homogeneous linear system](../../../linear-algebra.md#homogeneous-linear-system) gives the [kernel of a linear map](../../../kernel-of-a-linear-map.md):

$$
\boxed{\operatorname{im}T_2=\{(u,v,w):u-v+w=0\},\qquad\ker T_2=\operatorname{span}\{(1,1,1)\}.}
$$

The prescribed $b=(-1,\beta,1)^T$ satisfies the displayed condition precisely when $\beta=0$. If $\beta\ne0$, it lies outside the [image of a linear map](../../../vector-space.md#image-of-a-linear-map) and there is no solution. If $\beta=0$, it lies in the [image of a linear map](../../../vector-space.md#image-of-a-linear-map), and the nonzero [kernel of a linear map](../../../kernel-of-a-linear-map.md) supplies infinitely many solutions.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/a">A</h5>

↑ **Parent:** [Ii](#2/c/ii)

<h6 id="2/c/ii/a/solution">Solution</h6>

↑ **Parent:** [A](#2/c/ii/a)

For $\alpha\ne2$, $A'=I_3$, whose [row space](../../../vector-space.md#row-space) is $\mathbb R^3=\operatorname{im}T_\alpha$. For $\alpha=2$, [elementary row operations](../../../numerical-linear-algebra.md#elementary-row-operation) give the [reduced row echelon form](../../../numerical-linear-algebra.md#reduced-row-echelon-form)

$$
A'=\begin{pmatrix}1&0&-1\\0&1&-1\\0&0&0\end{pmatrix}.
$$

Its [row space](../../../vector-space.md#row-space) is $\{(u,v,w):u+v+w=0\}$, whereas the [image of a linear map](../../../vector-space.md#image-of-a-linear-map) is $\{(u,v,w):u-v+w=0\}$. These differ: $(0,1,-1)$ belongs to the former but not the latter. Thus **(A) is true exactly when $\alpha\ne2$**. Rows are being identified with [vectors](../../../vector-space.md#vector) in $\mathbb R^3$ in this comparison.

<h5 id="2/c/ii/b">B</h5>

↑ **Parent:** [Ii](#2/c/ii)

<h6 id="2/c/ii/b/solution">Solution</h6>

↑ **Parent:** [B](#2/c/ii/b)

Every [elementary column operation](../../../vector-space.md#elementary-column-operation) preserves the [linear span](../../../vector-space.md#linear-span) of the columns: each new column is a [linear combination](../../../vector-space.md#linear-combination) of the old columns, and the inverse operation supplies the reverse inclusion. Thus the [column space](../../../vector-space.md#column-space) of $A''$ equals that of $A$, which is precisely the [image of a linear map](../../../vector-space.md#image-of-a-linear-map) $T_\alpha$. Consequently **(B) is true for every $\alpha\in\mathbb R$**.

<h5 id="2/c/ii/c">C</h5>

↑ **Parent:** [Ii](#2/c/ii)

<h6 id="2/c/ii/c/solution">Solution</h6>

↑ **Parent:** [C](#2/c/ii/c)

For $\alpha\ne2$, both reduced forms are $I_3$, so $A''=(A')^T$. At $\alpha=2$, the [reduced column echelon form](../../../vector-space.md#reduced-column-echelon-form) is the [transpose](../../../vector-space.md#transpose) of the [reduced row echelon form](../../../numerical-linear-algebra.md#reduced-row-echelon-form) of $A^T$, giving

$$
A''=\begin{pmatrix}1&0&0\\0&1&0\\-1&1&0\end{pmatrix},\qquad
(A')^T=\begin{pmatrix}1&0&0\\0&1&0\\-1&-1&0\end{pmatrix}.
$$

For example, $C_2\mapsto-C_2$ followed by $C_3\mapsto C_3+C_1-C_2$, using the updated second column, produces the displayed $A''$ directly. Its third column is zero. The two [matrices](../../../vector-space.md#matrix) differ, so **(C) is true exactly when $\alpha\ne2$**. Taking a [transpose](../../../vector-space.md#transpose) exchanges the kind of reduction, but also replaces the original $A$ by $A^T$; it does not generally identify the two reduced forms of $A$ itself.

## 3

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Choose the [rotation](../../../riemannian-geometry.md#rotation-mathematics) taking $e_1$ to $e_2$, $e_2$ to $-e_1$ and $e_3$ to itself. The columns of the [matrix of a linear map](../../../vector-space.md#matrix-representation-of-a-linear-map) are these images of the [standard basis](../../../vector-space.md#standard-basis), so

$$
\boxed{A=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}.}
$$

This fixes the orientation used throughout this question.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Using the convention $\chi_T(x)=\det(xI-A)$, the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is

$$
\boxed{\chi_T(x)=(x-1)\det\begin{pmatrix}x&1\\-1&x\end{pmatrix}=(x-1)(x^2+1).}
$$

Since $x^2+1>0$ for every $x\in\mathbb R$, the only [eigenvalue](../../../linear-operator-theory.md#eigenvalue) over the [real numbers](../../../arithmetic.md#real-number) is $1$. Solving $(A-I)v=0$ gives

$$
\boxed{E_1=\ker(A-I)=\operatorname{span}\{(0,0,1)\}.}
$$

Thus the only [eigenspace](../../../linear-operator-theory.md#eigenspace) over the [real numbers](../../../arithmetic.md#real-number) is the axis of the [rotation](../../../riemannian-geometry.md#rotation-mathematics).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The two nonzero proper [invariant subspaces](../../../representation-theory.md#invariant-subspace) are

$$
\boxed{U=\operatorname{span}\{e_3\},\qquad W=\operatorname{span}\{e_1,e_2\}.}
$$

Both are preserved by the [rotation](../../../riemannian-geometry.md#rotation-mathematics). To show there are no others, note that

$$
P=\frac{I+T^2}{2},\qquad P(x,y,z)=(0,0,z)
$$

is the [linear projection](../../../vector-space.md#projection-linear-algebra) onto $U$, and $I-P$ is the [linear projection](../../../vector-space.md#projection-linear-algebra) onto $W$. Every [invariant subspace](../../../representation-theory.md#invariant-subspace) $L$ is preserved by $I,T^2$, and hence by both of these [linear projections](../../../vector-space.md#projection-linear-algebra). Therefore

$$
L=(L\cap U)\oplus(L\cap W).
$$

Because $U$ has [dimension](../../../vector-space.md#dimension-vector-space) one, $L\cap U$ is either $0$ or $U$. If $L\cap W$ contains a nonzero $v=(a,b,0)$, it also contains $Tv=(-b,a,0)$. These two [vectors](../../../vector-space.md#vector) are [linearly independent](../../../vector-space.md#linear-independence), because their two-dimensional [determinant](../../../multilinear-algebra.md#determinant) is $a^2+b^2>0$. They [span](../../../vector-space.md#linear-span) $W$, so $L\cap W$ is either $0$ or $W$. The only possibilities for $L$ are therefore $0,U,W,V$.

Finally every $(x,y,z)$ has the unique decomposition $(0,0,z)+(x,y,0)$, with one summand in each of $U,W$. Hence

$$
\boxed{V=U\oplus W.}
$$

This also illustrates how [invariant subspaces of a quarter-turn in three dimensions](../../../representation-theory.md#invariant-subspaces-of-a-quarter-turn-in-three-dimensions) can be classified by [linear projections](../../../vector-space.md#projection-linear-algebra).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Over the [complex numbers](../../../complex-analysis.md#complex-number), the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) splits into three distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), $1,i,-i$. Direct multiplication gives the [eigenvectors](../../../linear-operator-theory.md#eigenvector)

$$
v_1=\begin{pmatrix}0\\0\\1\end{pmatrix},\qquad
v_i=\begin{pmatrix}1\\-i\\0\end{pmatrix},\qquad
v_{-i}=\begin{pmatrix}1\\i\\0\end{pmatrix},
\qquad Av_1=v_1,\quad Av_i=iv_i,\quad Av_{-i}=-iv_{-i}.
$$

They are [linearly independent](../../../vector-space.md#linear-independence): the last two have two-dimensional [determinant](../../../multilinear-algebra.md#determinant) $2i\ne0$ in the first two coordinates, and the first has nonzero third coordinate. Thus

$$
\boxed{\mathcal B=(v_1,v_i,v_{-i}),\qquad[T']_{\mathcal B}=\operatorname{diag}(1,i,-i).}
$$

This is a [basis](../../../vector-space.md#basis) of [eigenvectors](../../../linear-operator-theory.md#eigenvector) of $\mathbb C^3$, proving that $T'$ has a [diagonalizable matrix](../../../linear-operator-theory.md#diagonalizable-matrix).

## 4

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The prescribed form is a sum of products of real [polynomial evaluations](../../../polynomial.md#polynomial-evaluation). It is a [symmetric bilinear form](../../../bilinear-form.md#symmetric-bilinear-form), since each evaluation is a [linear map](../../../vector-space.md#linear-map). Also

$$
\langle f,f\rangle=\frac{f(-1)^2+f(0)^2+f(1)^2}{3}\geq0.
$$

Equality forces $f(-1)=f(0)=f(1)=0$. A nonzero [polynomial](../../../polynomial.md) of [degree of a polynomial](../../../polynomial.md#degree-of-a-polynomial) at most two cannot have three distinct [roots of a polynomial](../../../polynomial.md#root-of-a-polynomial), by the [root bound for a polynomial](../../../polynomial.md#lagrange-root-bound-over-a-field). Thus equality holds only for the zero [polynomial](../../../polynomial.md), establishing [positive definiteness](../../../bilinear-form.md#positive-definiteness). Therefore **the form is a real [inner product](../../../inner-product.md)**, and $V$ is an [inner product space](../../../inner-product.md#inner-product-space). This is a [discrete sampling inner product on polynomial spaces](../../../inner-product.md#discrete-sampling-inner-product-on-polynomial-spaces).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

The relevant [inner products](../../../inner-product.md) are

$$
\langle1,x\rangle=\frac{-1+0+1}{3}=0,\qquad
\langle1,1\rangle=1,\qquad\langle x,x\rangle=\frac23.
$$

Hence $1$ and $x$ are [orthogonal vectors](../../../inner-product.md#orthogonal-vectors). Dividing by their [norms](../../../normed-vector-space.md#norm) gives the [orthonormal basis](../../../inner-product.md#orthonormal-basis)

$$
\boxed{f=1,\qquad g=\sqrt{\frac32}\,x}
$$

of their [linear span](../../../vector-space.md#linear-span) $U$.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For any [orthonormal basis](../../../inner-product.md#orthonormal-basis) $f,g$ of $U$, [bilinearity](../../../multilinear-algebra.md#bilinearity) gives

$$
\begin{aligned}
\langle f,h\rangle
&=\langle f,x^2\rangle-\langle f,x^2\rangle\langle f,f\rangle-\langle g,x^2\rangle\langle f,g\rangle=0,\\
\langle g,h\rangle
&=\langle g,x^2\rangle-\langle f,x^2\rangle\langle g,f\rangle-\langle g,x^2\rangle\langle g,g\rangle=0.
\end{aligned}
$$

Together with $\langle f,g\rangle=0$, these identities prove **pairwise [orthogonality](../../../inner-product.md#orthogonal-vectors)**. The construction subtracts the [orthogonal projection onto a finite-dimensional subspace](../../../inner-product.md#orthogonal-projection-onto-a-finite-dimensional-subspace) $U$ from $x^2$, leaving the [orthogonal projection residual](../../../inner-product.md#orthogonal-projection-residual).

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

Use $f,g$ from [i](#4/b/i). Their [inner products](../../../inner-product.md) with $x^2$ are

$$
\langle f,x^2\rangle=\frac23,\qquad
\langle g,x^2\rangle=\sqrt{\frac32}\,\frac{-1+0+1}{3}=0.
$$

Thus $h=x^2-2/3$. Its values at $-1,0,1$ are $1/3,-2/3,1/3$, so

$$
\|h\|^2=\frac13\left(\frac19+\frac49+\frac19\right)=\frac29.
$$

By [ii](#4/b/ii) the three [polynomials](../../../polynomial.md) are [orthogonal vectors](../../../inner-product.md#orthogonal-vectors), and normalizing $h$ gives

$$
\boxed{\mathcal B=\left(1,\sqrt{\frac32}\,x,\frac{3x^2-2}{\sqrt2}\right).}
$$

This [orthonormal set](../../../inner-product.md#orthonormal-set) is a [basis](../../../vector-space.md#basis) of the three-dimensional [vector space](../../../vector-space.md) $V$. It is the result of the [Gram-Schmidt process](../../../inner-product.md#gram-schmidt-process) applied to $1,x,x^2$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

If $T$ is an [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) and $e_1,e_2,e_3$ is an [orthonormal basis](../../../inner-product.md#orthonormal-basis), then

$$
\langle Te_i,Te_j\rangle=\langle e_i,e_j\rangle=\delta_{ij}.
$$

The images form an [orthonormal set](../../../inner-product.md#orthonormal-set), hence are [linearly independent](../../../vector-space.md#linear-independence) and form an [orthonormal basis](../../../inner-product.md#orthonormal-basis) in [dimension](../../../vector-space.md#dimension-vector-space) three.

Conversely, suppose the images $Te_1,Te_2,Te_3$ of one chosen [orthonormal basis](../../../inner-product.md#orthonormal-basis) form an [orthonormal basis](../../../inner-product.md#orthonormal-basis). Write $u=\sum_i a_ie_i$ and $v=\sum_j b_je_j$. By [linearity](../../../vector-space.md#linearity) of $T$ and [bilinearity](../../../multilinear-algebra.md#bilinearity),

$$
\langle Tu,Tv\rangle=\sum_{i,j}a_ib_j\langle Te_i,Te_j\rangle
=\sum_i a_ib_i=\langle u,v\rangle.
$$

Thus **mapping one [orthonormal basis](../../../inner-product.md#orthonormal-basis) to an [orthonormal basis](../../../inner-product.md#orthonormal-basis) is equivalent to preserving every [inner product](../../../inner-product.md)**. In the converse, a single chosen [orthonormal basis](../../../inner-product.md#orthonormal-basis) suffices.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Put $p=(3x^2-2)/\sqrt2$ and use the [orthonormal basis](../../../inner-product.md#orthonormal-basis) $\mathcal B=(1,\sqrt{3/2}\,x,p)$ from [iii](#4/b/iii). The columns of the given [matrix](../../../vector-space.md#matrix) give

$$
T(1)=-\sqrt2+\frac3{\sqrt2}x^2=p,\qquad T(x)=x,\qquad T(x^2)=-\sqrt2+\sqrt2x^2.
$$

Consequently

$$
T(p)=\frac{3T(x^2)-2T(1)}{\sqrt2}=-1.
$$

The images of $\mathcal B$ are therefore $(p,\sqrt{3/2}\,x,-1)$, again an [orthonormal basis](../../../inner-product.md#orthonormal-basis). By [i](#4/c/i), **$T$ is an [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation)**. Its [matrix](../../../vector-space.md#matrix) in this [orthonormal basis](../../../inner-product.md#orthonormal-basis) is

$$
\boxed{[T]_{\mathcal B}=\begin{pmatrix}0&0&-1\\0&1&0\\1&0&0\end{pmatrix}.}
$$

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

**$A$ is not an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix).** Its first column has squared [Euclidean norm](../../../normed-vector-space.md#euclidean-norm)

$$
(-\sqrt2)^2+0^2+(3/\sqrt2)^2=\frac{13}{2}\ne1,
$$

so $A^TA\ne I$. The reason this is compatible with [ii](#4/c/ii) is that $1,x,x^2$ is not an [orthonormal basis](../../../inner-product.md#orthonormal-basis) for the given [inner product](../../../inner-product.md). Its [Gram matrix](../../../inner-product.md#gram-matrix) is

$$
G=\begin{pmatrix}1&0&2/3\\0&2/3&0\\2/3&0&2/3\end{pmatrix},\qquad
\langle u,v\rangle=[u]^TG[v].
$$

The correct condition on this [matrix representation of a linear map](../../../vector-space.md#matrix-representation-of-a-linear-map) is

$$
\boxed{A^TGA=G,}
$$

which follows either by direct multiplication or by the [inner product](../../../inner-product.md) preservation just proved. This is the rule for an [orthogonal transformation in a nonorthonormal basis](../../../linear-algebra.md#orthogonal-transformation-in-a-nonorthonormal-basis).

## 5

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

For a [subgroup](../../../group.md#subgroup) $H$ of $G$, the [left coset](../../../group-theory.md#left-coset) represented by $g$ is

$$
\boxed{gH=\{gh:h\in H\}.}
$$

Suppose two [left cosets](../../../group-theory.md#left-coset) intersect. There are $h_1,h_2\in H$ such that $g_1h_1=g_2h_2$, so

$$
g_1=g_2h_2h_1^{-1}.
$$

Because $H$ is a [subgroup](../../../group.md#subgroup), $h_2h_1^{-1}\in H$. Thus, for every $h\in H$, $g_1h=g_2(h_2h_1^{-1}h)\in g_2H$, proving $g_1H\subseteq g_2H$. Interchanging the two representatives gives the reverse inclusion. Therefore **two [left cosets](../../../group-theory.md#left-coset) are equal or disjoint**.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

[Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states that if $H$ is a [subgroup](../../../group.md#subgroup) of a [finite group](../../../group.md#finite-group) $G$, then

$$
\boxed{|G|=[G:H]|H|,\qquad |H|\mid|G|,}
$$

where the [index of a subgroup](../../../group.md#index-of-a-subgroup) $[G:H]$ is the number of distinct [left cosets](../../../group-theory.md#left-coset).

Every $g\in G$ lies in $gH$, since $g=ge$. By [i](#5/a/i), distinct [left cosets](../../../group-theory.md#left-coset) are disjoint, so these [sets](../../../set.md) form a [partition of a set](../../../set.md#partition-of-a-set) $G$. Each has [cardinality](../../../cardinal-number.md#cardinality) $|H|$: the [function](../../../function.md) $h\mapsto gh$ from $H$ to $gH$ is a [bijection](../../../function.md#bijection), with inverse $gh\mapsto h$, by cancellation in a [group](../../../group.md). Counting the elements in this finite [partition of a set](../../../set.md#partition-of-a-set) gives $|G|=[G:H]|H|$, proving the theorem.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

The [order of a group element](../../../group-theory.md#order-of-a-group-element) $g$ is the smallest positive integer $d$ with $g^d=e$. Such an integer exists in a [finite group](../../../group.md#finite-group): two powers in $e,g,g^2,\ldots$ must agree, and cancellation gives a positive power equal to $e$.

By minimality, $e,g,\ldots,g^{d-1}$ are distinct. Every integer power of $g$ is one of them, by division of its exponent by $d$. They form the [cyclic subgroup](../../../group.md#cyclic-subgroup)

$$
\langle g\rangle=\{e,g,\ldots,g^{d-1}\},\qquad|\langle g\rangle|=d.
$$

Applying [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) to this [subgroup](../../../group.md#subgroup) gives

$$
\boxed{o(g)=|\langle g\rangle|\mid|G|.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

For $a\in A$, the element $a=ae$ belongs to both $A$ and $aA$. The assumed equal-or-disjoint property therefore gives $aA=A$.

If $a,b\in A$, then $ab\in aA=A$, so $A$ is closed under multiplication. Also $e\in A=aA$, so some $c\in A$ satisfies $ac=e$. Therefore $c=a^{-1}\in A$. Along with the given [identity element](../../../algebraic-operation.md#identity-element), closure and existence of [inverse elements](../../../algebraic-operation.md#inverse-element) establish that **$A$ is a [subgroup](../../../group.md#subgroup) of $G$**. This is the [subgroup test](../../../group.md#subgroup-test). The proof even works without assuming that $G$ is finite.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Choose $b_0\in B$ and put $H=b_0^{-1}B$. Then $e\in H$. For any $g_1,g_2\in G$,

$$
g_1H=(g_1b_0^{-1})B,\qquad g_2H=(g_2b_0^{-1})B,
$$

so these translates are equal or disjoint by the assumed property of $B$. Applying [i](#5/b/i) shows that $H$ is a [subgroup](../../../group.md#subgroup). Thus

$$
\boxed{B=b_0H,\qquad H=b_0^{-1}B\leq G.}
$$

This proves that $B$ is a [left coset](../../../group-theory.md#left-coset). Together with [i](#5/a/i), it gives the [equal-or-disjoint translates characterize cosets](../../../group-theory.md#equal-or-disjoint-translates-characterize-cosets) criterion.

## 6

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

Let $|G|=p$, with $p$ a [prime number](../../../prime-number.md), and choose $g\ne e$. By [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), the [order of a group element](../../../group-theory.md#order-of-a-group-element) $g$ divides $p$ and is greater than one. It is therefore $p$, and $G=\langle g\rangle$. Hence **a [group](../../../group.md) of prime [cardinality](../../../cardinal-number.md#cardinality) is a [cyclic group](../../../group.md#cyclic-group)**.

The converse is false: the [cyclic group](../../../group.md#cyclic-group) $C_4$ has four elements, and $4$ is not a [prime number](../../../prime-number.md).

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

If $G=\langle g\rangle$, any two elements are $g^a,g^b$, and

$$
g^ag^b=g^{a+b}=g^{b+a}=g^bg^a.
$$

Thus **every [cyclic group](../../../group.md#cyclic-group) is an [abelian group](../../../group.md#abelian-group)**.

For the converse, the [Klein four-group](../../../finite-group-theory.md#klein-four-group) $C_2\times C_2$ is an [abelian group](../../../group.md#abelian-group), with componentwise multiplication. Each nonidentity element has [order of a group element](../../../group-theory.md#order-of-a-group-element) two, so none generates its four elements. It is therefore not a [cyclic group](../../../group.md#cyclic-group).

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

The hypothesis implies $x^{-1}=x$ for every $x\in G$, including $e$. For $a,b\in G$,

$$
ab=(ab)^{-1}=b^{-1}a^{-1}=ba.
$$

Thus **$G$ is an [abelian group](../../../group.md#abelian-group)**. This is the [group of exponent two is abelian](../../../group.md#group-of-exponent-two-is-abelian) argument.

The converse is false: the [cyclic group](../../../group.md#cyclic-group) $C_3$ is an [abelian group](../../../group.md#abelian-group), but its two nonidentity elements have [order of a group element](../../../group-theory.md#order-of-a-group-element) three.

<h4 id="6/a/iv">iv</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/a/iv)

Choose distinct $a,b\ne e$, possible because $|G|>2$. By [iii](#6/a/iii), $a$ and $b$ commute, and $a^2=b^2=e$. The four elements

$$
H=\{e,a,b,ab\}
$$

are distinct: $ab=e$ would give $a=b$, while $ab=a$ or $ab=b$ would make $b=e$ or $a=e$. Commutativity and $a^2=b^2=e$ show that products stay in $H$, and every element is its own inverse. More explicitly,

$$
\boxed{C_2\times C_2\longrightarrow H,\qquad(i,j)\longmapsto a^ib^j\quad(i,j\in\{0,1\})}
$$

is a [group isomorphism](../../../algebra.md#group-isomorphism), with addition of exponents modulo two. Hence $G$ contains a [subgroup](../../../group.md#subgroup) isomorphic to the [Klein four-group](../../../finite-group-theory.md#klein-four-group).

The converse is false. The [direct product of groups](../../../group-theory.md#direct-product-of-groups) $C_2\times C_2\times C_3$ contains $C_2\times C_2\times\{e\}$, but it has elements of [order of a group element](../../../group-theory.md#order-of-a-group-element) three. Thus the existence of the specified [subgroup](../../../group.md#subgroup) does not force every nonidentity element to have [order of a group element](../../../group-theory.md#order-of-a-group-element) two.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The complete classification up to [group isomorphism](../../../algebra.md#group-isomorphism) is

$$
\boxed{\begin{array}{c|l}
|G|&G\\\hline
1&C_1\\
2&C_2\\
3&C_3\\
4&C_4,\ C_2\times C_2\\
5&C_5\\
6&C_6,\ S_3
\end{array}}
$$

Here $C_1$ is the [trivial group](../../../group.md#trivial-group). The [prime number](../../../prime-number.md) cases follow from [i](#6/a/i). For four elements, an element of [order of a group element](../../../group-theory.md#order-of-a-group-element) four generates $C_4$. If there is none, [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) makes every nonidentity element have [order of a group element](../../../group-theory.md#order-of-a-group-element) two. Then [iv](#6/a/iv) produces a four-element [subgroup](../../../group.md#subgroup), which must be all of $G$, giving the [Klein four-group](../../../finite-group-theory.md#klein-four-group).

For six elements, an element of [order of a group element](../../../group-theory.md#order-of-a-group-element) six gives $C_6$. Suppose there is none. If there were no element of [order of a group element](../../../group-theory.md#order-of-a-group-element) three either, all nonidentity elements would have [order of a group element](../../../group-theory.md#order-of-a-group-element) two. Part [iv](#6/a/iv) would then produce a [subgroup](../../../group.md#subgroup) of [cardinality](../../../cardinal-number.md#cardinality) four, contradicting [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). Thus choose $a$ of [order of a group element](../../../group-theory.md#order-of-a-group-element) three. There is also an [involution](../../../group-theory.md#involution) $b$: otherwise the five nonidentity elements could be paired into distinct pairs $\{g,g^{-1}\}$, impossible for an odd number of elements.

The [subgroup](../../../group.md#subgroup) $H=\langle a\rangle$ has [index of a subgroup](../../../group.md#index-of-a-subgroup) two, so it is a [normal subgroup](../../../group-theory.md#normal-subgroup). Indeed, for $g\notin H$, both $gH$ and $Hg$ are the complement of $H$, and for $g\in H$ both equal $H$. Consequently $bab^{-1}$ is either $a$ or $a^{-1}$. The first possibility makes $a,b$ commute, and $ab$ then has [order of a group element](../../../group-theory.md#order-of-a-group-element) six: $(ab)^k=e$ forces $a^k=b^{-k}\in\langle a\rangle\cap\langle b\rangle=\{e\}$, so both $3$ and $2$ divide $k$. This contradicts our assumption. Therefore

$$
bab^{-1}=a^{-1}.
$$

Every element is uniquely $a^i$ or $a^ib$, with $0\leq i<3$, and the relation $ba=a^{-1}b$ determines all their products. Sending $a$ to $(123)$ and $b$ to $(12)$ gives a [group isomorphism](../../../algebra.md#group-isomorphism) with the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_3$. This completes the classification of [groups of order at most six](../../../finite-group-theory.md#groups-of-order-at-most-six).

Of these [groups](../../../group.md), **exactly $C_1,C_2,C_3,C_4,C_2\times C_2,S_3$ embed in $S_4$**. Concrete [subgroups](../../../group.md#subgroup) are

$$
\{e\},\quad\langle(12)\rangle,\quad\langle(123)\rangle,\quad
\langle(1234)\rangle,\quad
\{e,(12)(34),(13)(24),(14)(23)\},\quad
\{\sigma\in S_4:\sigma(4)=4\}.
$$

There is no $C_5$ [subgroup](../../../group.md#subgroup), since $5$ does not divide $24$. There is no $C_6$ [subgroup](../../../group.md#subgroup) either: the [order of a group element](../../../group-theory.md#order-of-a-group-element) in a [symmetric group](../../../finite-group-theory.md#symmetric-group) is the [least common multiple](../../../divisibility.md#least-common-multiple) of the lengths in its [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition), and on four letters the only possibilities are $1,2,3,4$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Label the vertices of a [regular tetrahedron](../../../euclidean-geometry.md#regular-tetrahedron) $1,2,3,4$, and include all its [Euclidean isometries](../../../riemannian-geometry.md#euclidean-isometry), both [rotations](../../../riemannian-geometry.md#rotation-mathematics) and [reflections](../../../linear-algebra.md#reflection-mathematics). The following list describes every [subgroup](../../../group.md#subgroup) of [cardinality](../../../cardinal-number.md#cardinality) at most six, allowing arbitrary relabelling of the vertices. The numbers count actual [subgroups](../../../group.md#subgroup), rather than just their [group isomorphism](../../../algebra.md#group-isomorphism) types.

- **One trivial [subgroup](../../../group.md#subgroup)** contains only the [identity element](../../../algebraic-operation.md#identity-element).
- **Six reflection [subgroups](../../../group.md#subgroup) $C_2$** are generated by a [transposition](../../../combinatorics.md#transposition-permutation), for example $(12)$. Its mirror plane contains vertices $3,4$ and the midpoint of the opposite edge $12$.
- **Three half-turn [subgroups](../../../group.md#subgroup) $C_2$** are generated by a product of two disjoint [transpositions](../../../combinatorics.md#transposition-permutation), for example $(12)(34)$. The [rotation](../../../riemannian-geometry.md#rotation-mathematics) axis joins the midpoints of the opposite edges $12$ and $34$.
- **Four [cyclic subgroups](../../../group.md#cyclic-subgroup) $C_3$** consist of the three [rotations](../../../riemannian-geometry.md#rotation-mathematics) about an axis joining a vertex to the centre of its opposite face. For example, $\langle(123)\rangle$ fixes vertex $4$.
- **Three [cyclic subgroups](../../../group.md#cyclic-subgroup) $C_4$** are generated by an [improper orthogonal transformation](../../../linear-algebra.md#improper-orthogonal-transformation): a quarter-turn about an axis through opposite edge midpoints, composed with a [reflection](../../../linear-algebra.md#reflection-mathematics) in the perpendicular plane through the centre. For $\langle(1234)\rangle$, the axis joins the midpoints of edges $13$ and $24$. Its square is the half-turn $(13)(24)$.
- **One rotational [Klein four-group](../../../finite-group-theory.md#klein-four-group)** consists of the [identity element](../../../algebraic-operation.md#identity-element) and the three half-turns about opposite-edge midpoint axes:$$
  \{e,(12)(34),(13)(24),(14)(23)\}.
  $$
- **Three further [Klein four-groups](../../../finite-group-theory.md#klein-four-group)** arise from a pair of opposite edges. For edges $12,34$, the [subgroup](../../../group.md#subgroup) is$$
  \{e,(12),(34),(12)(34)\}.
  $$

  It contains two [reflections](../../../linear-algebra.md#reflection-mathematics) in perpendicular planes and their product, the half-turn about the line where those planes meet. It preserves each of the two opposite edges as a [set](../../../set.md).
- **Four [subgroups](../../../group.md#subgroup) $S_3$** are the [stabilizer subgroups](../../../group-action.md#stabilizer-subgroup) of individual vertices. Each contains three [rotations](../../../riemannian-geometry.md#rotation-mathematics) about the vertex-to-opposite-face axis and three [reflections](../../../linear-algebra.md#reflection-mathematics) in planes containing that axis. For the fixed vertex $4$, this is every [permutation](../../../combinatorics.md#permutation) of $1,2,3$.

Here is why this is exhaustive. Part [b](#6/b) leaves only the [trivial group](../../../group.md#trivial-group), $C_2,C_3,C_4,C_2\times C_2,S_3$. The [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) gives exactly the two listed kinds of [involutions](../../../group-theory.md#involution), the three-cycles, and the four-cycles, accounting for all the [cyclic subgroups](../../../group.md#cyclic-subgroup). In a [Klein four-group](../../../finite-group-theory.md#klein-four-group), the nonidentity elements commute. If it contains $(12)$, any other nonidentity element must be a commuting [involution](../../../group-theory.md#involution), hence $(34)$ or $(12)(34)$; either choice yields the displayed opposite-edge [subgroup](../../../group.md#subgroup). If it has no [transposition](../../../combinatorics.md#transposition-permutation), its three nonidentity elements must be all three double [transpositions](../../../combinatorics.md#transposition-permutation), yielding the rotational [subgroup](../../../group.md#subgroup).

Finally, an $S_3$ [subgroup](../../../group.md#subgroup) has a unique [cyclic subgroup](../../../group.md#cyclic-subgroup) of [cardinality](../../../cardinal-number.md#cardinality) three. Its two three-cycles fix the same unique vertex. Every element of the $S_3$ [subgroup](../../../group.md#subgroup) preserves this vertex, since [conjugation](../../../group-action.md#conjugation) preserves that unique [cyclic subgroup](../../../group.md#cyclic-subgroup). Thus it is the full [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) of that vertex. The counts in the list are consequently exhaustive, giving

$$
\boxed{1+6+3+4+3+1+3+4=25\text{ subgroups of order at most }6.}
$$

The two kinds of $C_2$ and the two kinds of [Klein four-groups](../../../finite-group-theory.md#klein-four-group) have different geometric behavior despite having the same abstract [group isomorphism](../../../algebra.md#group-isomorphism) type within each pair. This is the distinction recorded by the [small subgroups of tetrahedral symmetry](../../../finite-group-theory.md#small-subgroups-of-tetrahedral-symmetry).

## 7

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

A left [group action](../../../group-action.md) of $G$ on a [set](../../../set.md) $S$ is a [function](../../../function.md) $G\times S\to S$, written $(g,s)\mapsto g\cdot s$, satisfying

$$
\boxed{e\cdot s=s,\qquad(gh)\cdot s=g\cdot(h\cdot s)}
$$

for all $g,h\in G$, $s\in S$. The [orbit of a group action](../../../group-action.md#orbit-group-theory) through $s$ and the [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) of $s$ are, respectively,

$$
\boxed{G\cdot s=\{g\cdot s:g\in G\},\qquad G_s=\{g\in G:g\cdot s=s\}.}
$$

The [identity element](../../../algebraic-operation.md#identity-element) belongs to $G_s$. If $g,h\in G_s$, then $(gh)\cdot s=g\cdot(h\cdot s)=g\cdot s=s$, so $gh\in G_s$. If $g\in G_s$, applying $g^{-1}$ to $g\cdot s=s$ gives $s=g^{-1}\cdot s$, so $g^{-1}\in G_s$. These facts prove that the [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) is a [subgroup](../../../group.md#subgroup) of $G$.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

The [orbit-stabilizer theorem](../../../group-action.md#orbit-stabilizer-theorem) identifies the [orbit of a group action](../../../group-action.md#orbit-group-theory) of $s$ with the [set](../../../set.md) of [left cosets](../../../group-theory.md#left-coset) of $G_s$. Explicitly, there is a [bijection](../../../function.md#bijection)

$$
\boxed{G/G_s\longrightarrow G\cdot s,\qquad gG_s\longmapsto g\cdot s.}
$$

Here $G/G_s$ denotes a [set](../../../set.md) of [cosets](../../../group-theory.md#coset); it is not asserted to be a [quotient group](../../../group-theory.md#quotient-group). To prove the identification, observe that

$$
gG_s=hG_s\iff h^{-1}g\in G_s
\iff(h^{-1}g)\cdot s=s
\iff g\cdot s=h\cdot s.
$$

This equivalence proves both well-definedness and [injectivity](../../../algebra.md#injective-function). Every element of the [orbit of a group action](../../../group-action.md#orbit-group-theory) has the form $g\cdot s$, proving [surjectivity](../../../algebra.md#surjective-function).

In particular, for a [finite group](../../../group.md#finite-group), the [cardinalities](../../../cardinal-number.md#cardinality) satisfy

$$
\boxed{|G\cdot s|=[G:G_s]=\frac{|G|}{|G_s|},\qquad|G|=|G\cdot s|\,|G_s|.}
$$

The last equality follows from [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) applied to the [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

The [orbits of a group action](../../../group-action.md#orbit-group-theory) form a [partition of a set](../../../set.md#partition-of-a-set) $S$: every element lies in its own [orbit of a group action](../../../group-action.md#orbit-group-theory), and two intersecting [orbits of a group action](../../../group-action.md#orbit-group-theory) coincide because each point can be moved back and then forward using [inverse elements](../../../algebraic-operation.md#inverse-element). By the [orbit-stabilizer theorem](../../../group-action.md#orbit-stabilizer-theorem), each [orbit of a group action](../../../group-action.md#orbit-group-theory) has [cardinality](../../../cardinal-number.md#cardinality) dividing $8$, so its size is $1,2,4$ or $8$.

If every [orbit of a group action](../../../group-action.md#orbit-group-theory) had size $2,4$ or $8$, their sizes would add to an even number, contrary to $|S|=17$. Therefore there is a one-element [orbit of a group action](../../../group-action.md#orbit-group-theory), say $\{s'\}$. Every $g\in G$ sends $s'$ into this same singleton, so

$$
\boxed{g\cdot s'=s'\quad\text{for every }g\in G.}
$$

Thus $s'$ is a [fixed point of a group action](../../../group-action.md#fixed-point-of-a-group-action). In fact the number of [fixed points of a group action](../../../group-action.md#fixed-point-of-a-group-action) is odd, since all other [orbits of a group action](../../../group-action.md#orbit-group-theory) have even [cardinality](../../../cardinal-number.md#cardinality).

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

For a [free group action](../../../group-action.md#free-group-action), every [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) is $\{e\}$. By the [orbit-stabilizer theorem](../../../group-action.md#orbit-stabilizer-theorem), every [orbit of a group action](../../../group-action.md#orbit-group-theory) has [cardinality](../../../cardinal-number.md#cardinality) $|G|$. Hence the two [free group actions](../../../group-action.md#free-group-action) have the same number

$$
r=\frac{|S|}{|G|}
$$

of [orbits of a group action](../../../group-action.md#orbit-group-theory). Choose one representative $s_i$ from each $\cdot$ [orbit of a group action](../../../group-action.md#orbit-group-theory) and one representative $t_i$ from each $*$ [orbit of a group action](../../../group-action.md#orbit-group-theory), and match them using $1\leq i\leq r$.

Every $s\in S$ has a unique expression $s=g\cdot s_i$. The [orbit of a group action](../../../group-action.md#orbit-group-theory) determines $i$, and the [free group action](../../../group-action.md#free-group-action) property determines $g$: if $g\cdot s_i=h\cdot s_i$, then $(h^{-1}g)\cdot s_i=s_i$, forcing $g=h$. Therefore the rule

$$
\boxed{f(g\cdot s_i)=g*t_i}
$$

defines a [function](../../../function.md) $f:S\to S$ without ambiguity. For $h\in G$,

$$
f\bigl(h\cdot(g\cdot s_i)\bigr)
=f\bigl((hg)\cdot s_i\bigr)
=(hg)*t_i
=h*(g*t_i)
=h*f(g\cdot s_i),
$$

which proves the required identity for every $s$.

Indeed, $f$ is a [bijection](../../../function.md#bijection): its inverse is $g*t_i\mapsto g\cdot s_i$, well defined because the second is also a [free group action](../../../group-action.md#free-group-action). If $S$ is empty, the unique empty [function](../../../function.md) already satisfies the identity. Thus the result holds in every case, and proves the stronger statement that [free finite actions with equal cardinality are isomorphic](../../../group-action.md#free-finite-actions-with-equal-cardinality-are-isomorphic).

## ↑ Ancestors (9)

1. [Prelims](../prelims.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Oxford](../../../past-exam-of-the-mathematics-course-of-the-university-of-oxford.md)
4. [Mathematics course of the University of Oxford](../../../university-of-oxford.md#mathematics-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../../university-of-oxford.md)
8. [List of universities](../../../README.md#list-of-universities)
9. [Codex Wiki](../../../README.md)
