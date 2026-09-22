# Mathematics I

↑ **Parent:** [Prelims](../prelims.md)

Source: [released examination PDF, bundle pages 10–14](https://www.whatdotheyknow.com/request/bsc_mathematics_prelims_and_part/response/2784209/attach/3/202409%20817%20annex.pdf#page=10).

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
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
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
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
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
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
    - [iv](#6/b/iv)
      - [Solution](#6/b/iv/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)
    - [iii](#6/c/iii)
      - [Solution](#6/c/iii/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)
    - [iii](#7/b/iii)
      - [Solution](#7/b/iii/solution)

## 1

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [vectors](../../../vector-space.md#vector) are [linearly independent](../../../vector-space.md#linear-independence) if

$$
\sum_{j=1}^n a_jv_j=0,\quad a_j\in\mathbb R
\quad\Longrightarrow\quad a_1=\cdots=a_n=0.
$$

They [span](../../../vector-space.md#linear-span) $V$ if every $v\in V$ is a [linear combination](../../../vector-space.md#linear-combination) $v=\sum_{j=1}^n a_jv_j$ with real [coefficients](../../../vector-space.md#coefficient). They form a [basis](../../../vector-space.md#basis) of $V$ if they are [linearly independent](../../../vector-space.md#linear-independence) and [span](../../../vector-space.md#linear-span) $V$. Equivalently, every $v\in V$ has exactly one such representation: existence is the [spanning set](../../../vector-space.md#spanning-set) condition, and subtracting two representations shows that uniqueness is precisely [linear independence](../../../vector-space.md#linear-independence).

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [Steinitz exchange lemma](../../../vector-space.md#steinitz-exchange-lemma) states that if $u_1,\ldots,u_r$ are [linearly independent](../../../vector-space.md#linear-independence) and $w_1,\ldots,w_s$ [span](../../../vector-space.md#linear-span) a [vector space](../../../vector-space.md) $V$, then $r\leq s$ and some $r$ of the $w_j$ can be replaced by $u_1,\ldots,u_r$ while preserving the [spanning set](../../../vector-space.md#spanning-set) property.

Here is the exchange argument. Suppose that after $k$ replacements, a [spanning set](../../../vector-space.md#spanning-set) is

$$
u_1,\ldots,u_k,w_{k+1},\ldots,w_s,
$$

where the remaining $w_j$ have been relabelled if necessary. Express $u_{k+1}$ as a [linear combination](../../../vector-space.md#linear-combination) of this family. At least one remaining $w_j$ has a nonzero [coefficient](../../../vector-space.md#coefficient); otherwise $u_{k+1}$ belongs to the [span](../../../vector-space.md#linear-span) of $u_1,\ldots,u_k$, contradicting [linear independence](../../../vector-space.md#linear-independence). Relabel this entry $w_{k+1}$. Solving for $w_{k+1}$ shows that it lies in the [span](../../../vector-space.md#linear-span) of

$$
u_1,\ldots,u_{k+1},w_{k+2},\ldots,w_s.
$$

The new family therefore still [spans](../../../vector-space.md#linear-span) $V$. Starting at $k=0$ repeats this step until all $r$ independent [vectors](../../../vector-space.md#vector) have been inserted. If $r>s$, after $s$ steps the next $u_{s+1}$ would lie in the [span](../../../vector-space.md#linear-span) of $u_1,\ldots,u_s$, a contradiction. Thus $r\leq s$, and the construction proves the replacement assertion as well.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Put $w_1=v_1$ and $w_j=v_j-v_1$ for $j\geq2$. Since $v_1=w_1$ and $v_j=w_j+w_1$, the two families have the same [linear span](../../../vector-space.md#linear-span). Moreover,

$$
\sum_{j=1}^n a_jw_j
=\left(a_1-\sum_{j=2}^n a_j\right)v_1+\sum_{j=2}^n a_jv_j.
$$

If the $v_j$ are [linearly independent](../../../vector-space.md#linear-independence), a vanishing expression forces $a_j=0$ for $j\geq2$ and then $a_1=0$. Conversely,

$$
\sum_{j=1}^n b_jv_j
=\left(\sum_{j=1}^n b_j\right)w_1+\sum_{j=2}^n b_jw_j,
$$

so [linear independence](../../../vector-space.md#linear-independence) of the $w_j$ forces all $b_j=0$. Thus both the [spanning set](../../../vector-space.md#spanning-set) condition and [linear independence](../../../vector-space.md#linear-independence) are equivalent for the two families, proving the desired equivalence of [bases](../../../vector-space.md#basis).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $u=(a,b)^T$, $v=(c,d)^T$ and $\Delta=ad-bc$. If $xu+yv=0$, then

$$
ax+cy=0,\qquad bx+dy=0.
$$

Eliminating $y$ gives $\Delta x=0$, and eliminating $x$ gives $\Delta y=0$. Hence $\Delta\ne0$ implies [linear independence](../../../vector-space.md#linear-independence).

For the converse, suppose $\Delta=0$. If $u=0$, the family already contains the [zero vector](../../../vector-space.md#zero-vector) and is [linearly dependent](../../../vector-space.md#linear-dependence). If $a\ne0$, the equality $ad=bc$ gives $v=(c/a)u$. If $a=0$ but $u\ne0$, then $b\ne0$ and $bc=0$ forces $c=0$, so $v=(d/b)u$. Both cases give a nontrivial [linear relation](../../../vector-space.md#linear-relation). Therefore

$$
\boxed{u,v\text{ are linearly independent}\iff ad-bc\ne0.}
$$

This is the two-dimensional [determinant](../../../multilinear-algebra.md#determinant) criterion, proved directly without assuming that criterion.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Subtracting the first [vector](../../../vector-space.md#vector) from each of the other two preserves the [basis](../../../vector-space.md#basis) property by [iii](#1/a/iii). The resulting family is

$$
e_1,\quad(0,\alpha,\alpha^2)^T,\quad(0,\beta,\beta^2)^T.
$$

Its last two [vectors](../../../vector-space.md#vector) belong to the plane with first coordinate zero. By [b](#1/b), they are [linearly independent](../../../vector-space.md#linear-independence) there precisely when

$$
\alpha\beta^2-\beta\alpha^2=\alpha\beta(\beta-\alpha)\ne0.
$$

In that case their two-dimensional [span](../../../vector-space.md#linear-span) is the whole plane, and adjoining $e_1$ gives a [basis](../../../vector-space.md#basis) of $\mathbb R^3$. If the displayed expression vanishes, a nontrivial [linear relation](../../../vector-space.md#linear-relation) among those two [vectors](../../../vector-space.md#vector) prevents a [basis](../../../vector-space.md#basis). Thus

$$
\boxed{\alpha\ne0,\quad\beta\ne0,\quad\alpha\ne\beta.}
$$

## 2

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

By definition, the [image of a linear map](../../../vector-space.md#image-of-a-linear-map) $T_A$ is

$$
\operatorname{im}T_A=\{A\mathbf x:\mathbf x\in\mathbb R^m\}.
$$

Consequently $\mathbf b\in\operatorname{im}T_A$ means exactly that some $\mathbf x\in\mathbb R^m$ satisfies $A\mathbf x=\mathbf b$. This is precisely the existence of a solution of the [linear system](../../../linear-algebra.md#system-of-linear-equations).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Suppose $\mathbf x_0$ is one solution. By [linearity](../../../vector-space.md#linearity),

$$
A\mathbf x=\mathbf b
\iff A(\mathbf x-\mathbf x_0)=0
\iff\mathbf x-\mathbf x_0\in\ker T_A.
$$

Thus the [solution set of a linear system](../../../linear-algebra.md#solution-set-of-a-linear-system) is exactly $\mathbf x_0+\ker T_A$. It has one member if the [kernel](../../../kernel-of-a-linear-map.md) is $\{0\}$. Conversely, if there is a unique solution and $\mathbf z\in\ker T_A$, then $\mathbf x_0+\mathbf z$ is also a solution, forcing $\mathbf z=0$. Combining this with [i](#2/a/i) gives

$$
\boxed{\text{unique solution}\iff\mathbf b\in\operatorname{im}T_A\text{ and }\ker T_A=\{0\}.}
$$

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

If $\mathbf b$ is outside the [image of a linear map](../../../vector-space.md#image-of-a-linear-map) $T_A$, there is no solution. Otherwise choose $\mathbf x_0$ with $A\mathbf x_0=\mathbf b$. By [ii](#2/a/ii), a zero [kernel](../../../kernel-of-a-linear-map.md) gives a unique solution. If the [kernel](../../../kernel-of-a-linear-map.md) contains a nonzero [vector](../../../vector-space.md#vector) $\mathbf z$, all

$$
\mathbf x_0+t\mathbf z,\qquad t\in\mathbb R,
$$

are solutions. They are distinct, since $(t-s)\mathbf z=0$ forces $t=s$. Hence there are infinitely many. These alternatives exhaust all possibilities.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

**No.** Here $A$ has more rows than columns, which does not force a nonzero [kernel](../../../kernel-of-a-linear-map.md). For example, with $m=1$, $n=2$,

$$
A=\begin{pmatrix}1\\0\end{pmatrix},\qquad
\mathbf b=\begin{pmatrix}0\\0\end{pmatrix},
$$

the [linear system](../../../linear-algebra.md#system-of-linear-equations) has the unique solution $x=0$. With the same $A$ and $\mathbf b=(0,1)^T$ it has no solution at all.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**No.** Take $A=I_m$ and $\mathbf b=0$. The [homogeneous linear system](../../../linear-algebra.md#homogeneous-linear-system) then has only the solution $\mathbf x=0$. Homogeneity ensures existence, but infinitely many solutions would additionally require a nonzero [kernel](../../../kernel-of-a-linear-map.md).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

**No.** The [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) gives

$$
\dim\ker T_A=m-\operatorname{rank}T_A\geq m-n>0,
$$

but this guarantees infinitely many solutions only when the [linear system](../../../linear-algebra.md#system-of-linear-equations) is consistent. For a counterexample take

$$
n=1,\quad m=2,\quad A=\begin{pmatrix}0&0\end{pmatrix},\quad\mathbf b=(1).
$$

There is no solution, since the left side always vanishes.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

**Yes.** A [surjective](../../../algebra.md#surjective-function) $T_A$ has $\operatorname{im}T_A=\mathbb R^n$, so every $\mathbf b$ is attained. Its [rank of a linear map](../../../vector-space.md#rank-of-a-linear-map) is $n$, and the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) gives

$$
\dim\ker T_A=m-n>0.
$$

The [solution set of a linear system](../../../linear-algebra.md#solution-set-of-a-linear-system) is therefore a translate of a nonzero [vector subspace](../../../vector-space.md#vector-subspace), containing infinitely many solutions as in [iii](#2/a/iii).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The first two equations give $x_1=1-2x_3$ and $x_2=2-5x_3$. Substitution into the third gives

$$
(\lambda-5)x_3=\mu-2.
$$

This equation is inconsistent exactly when its left side is identically zero and its right side is nonzero. Therefore

$$
\boxed{\text{no solution}\iff\lambda=5,\quad\mu\ne2.}
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

The elimination in [i](#2/c/i) determines $x_3$ uniquely exactly when $\lambda\ne5$. The other two coordinates are then also fixed. Explicitly,

$$
\boxed{\lambda\ne5:\quad
\mathbf x=\begin{pmatrix}
1-2(\mu-2)/(\lambda-5)\\
2-5(\mu-2)/(\lambda-5)\\
(\mu-2)/(\lambda-5)
\end{pmatrix}.}
$$

For $\lambda=5$, the reduced equation is either inconsistent or leaves $x_3$ free, so a unique solution is impossible.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

By [i](#2/c/i), a free choice of $x_3$ is possible precisely when $\lambda=5$ and $\mu=2$. Thus

$$
\boxed{\text{infinitely many solutions}\iff(\lambda,\mu)=(5,2).}
$$

The complete [solution set of a linear system](../../../linear-algebra.md#solution-set-of-a-linear-system) is

$$
\boxed{\mathbf x=\begin{pmatrix}1\\2\\0\end{pmatrix}
+t\begin{pmatrix}-2\\-5\\1\end{pmatrix},\quad t\in\mathbb R.}
$$

The direction [vector](../../../vector-space.md#vector) spans the [kernel](../../../kernel-of-a-linear-map.md), and the displayed [straight line](../../../euclidean-geometry.md#straight-line) is the entire [solution set of a linear system](../../../linear-algebra.md#solution-set-of-a-linear-system).

## 3

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [preimage](../../../set-theory.md#preimage) is

$$
T^{-1}(X)=\{u\in U:T(u)\in X\}.
$$

It contains $0$, and if $u,v$ belong to it and $a,b\in\mathbb R$, then $T(au+bv)=aT(u)+bT(v)\in X$, since $X$ is a [vector subspace](../../../vector-space.md#vector-subspace). Thus $T^{-1}(X)$ is a [vector subspace](../../../vector-space.md#vector-subspace). It contains the [kernel](../../../kernel-of-a-linear-map.md) of $T$ because $0\in X$.

To establish the [dimension of the preimage of a vector subspace](../../../set-theory.md#dimension-of-the-preimage-of-a-vector-subspace) formula without assuming the theorem to be deduced, choose a [basis](../../../vector-space.md#basis) $k_1,\ldots,k_{n_T}$ of $\ker T$ and a [basis](../../../vector-space.md#basis) $y_1,\ldots,y_d$ of $X\cap\operatorname{im}T$, where $d=\dim(X\cap\operatorname{im}T)$. For each $j$, choose $u_j\in U$ with $T(u_j)=y_j$. These $u_j$ lie in $T^{-1}(X)$.

The family $k_1,\ldots,k_{n_T},u_1,\ldots,u_d$ is [linearly independent](../../../vector-space.md#linear-independence): applying $T$ to a vanishing [linear combination](../../../vector-space.md#linear-combination) forces all $u_j$ [coefficients](../../../vector-space.md#coefficient) to vanish by [linear independence](../../../vector-space.md#linear-independence) of the $y_j$, and then all remaining [coefficients](../../../vector-space.md#coefficient) vanish by [linear independence](../../../vector-space.md#linear-independence) of the $k_i$. It also [spans](../../../vector-space.md#linear-span) $T^{-1}(X)$: for $u$ in that [preimage](../../../set-theory.md#preimage), write $T(u)=\sum_j b_jy_j$. Then $u-\sum_j b_ju_j\in\ker T$, so it is a [linear combination](../../../vector-space.md#linear-combination) of the $k_i$. Consequently

$$
\boxed{\dim T^{-1}(X)=\dim(X\cap\operatorname{im}T)+n_T.}
$$

Set $X=V$. Then $T^{-1}(V)=U$ and $V\cap\operatorname{im}T=\operatorname{im}T$, giving the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem):

$$
\boxed{\dim U=r_T+n_T.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Since $S'$ is the [restriction](../../../function.md#restriction-mathematics) of $S$ to $\operatorname{im}T$,

$$
\operatorname{im}(ST)=\{S(Tu):u\in U\}
=\{S(v):v\in\operatorname{im}T\}=\operatorname{im}S'.
$$

This [image of a linear map](../../../vector-space.md#image-of-a-linear-map) is contained in $\operatorname{im}S$, so $r_{ST}\leq r_S$. Also, applying $S$ to a [basis](../../../vector-space.md#basis) of $\operatorname{im}T$ gives a [spanning set](../../../vector-space.md#spanning-set) for $\operatorname{im}S'$, of size $r_T$. Thus $r_{ST}\leq r_T$, and

$$
\boxed{r_{ST}\leq\min(r_S,r_T).}
$$

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

For $u\in U$, the [vector](../../../vector-space.md#vector) $Tu$ already belongs to $\operatorname{im}T$, so

$$
STu=0\iff S'(Tu)=0\iff Tu\in\ker S'.
$$

Therefore $\ker(ST)=T^{-1}(\ker S')$. Since $\ker S'=\ker S\cap\operatorname{im}T$, its intersection with $\operatorname{im}T$ is itself. Applying [a](#3/a) with $X=\ker S'$ yields

$$
\boxed{n_{ST}=n_{S'}+n_T\leq n_S+n_T.}
$$

The inequality follows from the inclusion $\ker S'\subseteq\ker S$ and monotonicity of [dimension](../../../vector-space.md#dimension-vector-space) for [vector subspaces](../../../vector-space.md#vector-subspace).

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

By [i](#3/b/i) and [ii](#3/b/ii),

$$
r_{ST}+n_{ST}=r_{S'}+n_{S'}+n_T.
$$

The [domain of a function](../../../function.md#domain-of-a-function) of $S'$ is $\operatorname{im}T$. Its [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) gives $r_{S'}+n_{S'}=\dim\operatorname{im}T=r_T$. Applying the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) for $T$ now gives

$$
\boxed{r_{ST}+n_{ST}=r_T+n_T=\dim U,}
$$

which is exactly the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) for the [function composition](../../../function.md#function-composition) $ST$.

## 4

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Choose an [ordered basis](../../../vector-space.md#ordered-basis) $\mathcal B$ of $V$ and let $A=[T]_{\mathcal B}$. Define the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) by

$$
\boxed{\chi_T(x)=\det(xI-A).}
$$

If a different [basis](../../../vector-space.md#basis) gives $B=P^{-1}AP$ for an [invertible matrix](../../../linear-algebra.md#invertible-matrix) $P$, multiplicativity of the [determinant](../../../multilinear-algebra.md#determinant) gives

$$
\det(xI-B)=\det\bigl(P^{-1}(xI-A)P\bigr)
=\det(P^{-1})\det(xI-A)\det P
=\det(xI-A).
$$

Thus the definition is independent of the chosen [basis](../../../vector-space.md#basis). The alternate convention $\det(A-xI)$ differs by the constant factor $(-1)^{\dim V}$ and gives the same roots.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

A real number $\lambda$ is an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $T$ if $Tv=\lambda v$ for some nonzero [vector](../../../vector-space.md#vector) $v\in V$. Its [eigenspace](../../../linear-operator-theory.md#eigenspace) is

$$
E_\lambda=\{v\in V:Tv=\lambda v\}=\ker(T-\lambda I).
$$

It is a [vector subspace](../../../vector-space.md#vector-subspace) because it contains $0$ and $T(av+bw)=aTv+bTw=\lambda(av+bw)$ whenever $v,w\in E_\lambda$ and $a,b\in\mathbb R$.

If $v\in E_\lambda\cap E_\mu$, then $\lambda v=Tv=\mu v$, so $(\lambda-\mu)v=0$. Since $\lambda\ne\mu$, this forces $v=0$. Therefore

$$
\boxed{E_\lambda\cap E_\mu=\{0\}.}
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The definition of an [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and the [kernel](../../../kernel-of-a-linear-map.md) criterion for a singular [square matrix](../../../vector-space.md#square-matrix) give

$$
\begin{aligned}
\lambda\text{ is an eigenvalue}
&\iff\ker(T-\lambda I)\ne\{0\}\\
&\iff\lambda I-A\text{ is not invertible}\\
&\iff\det(\lambda I-A)=0\\
&\iff\chi_T(\lambda)=0.
\end{aligned}
$$

For the second equivalence, a [linear map](../../../vector-space.md#linear-map) from a finite-dimensional [vector space](../../../vector-space.md) to itself has zero [kernel](../../../kernel-of-a-linear-map.md) exactly when its [rank of a linear map](../../../vector-space.md#rank-of-a-linear-map) is the full [dimension](../../../vector-space.md#dimension-vector-space), by the [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem), and therefore exactly when it is invertible. This proves both directions.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

If $T^2=I$, every $v\in V$ has the decomposition

$$
v=\frac{v+Tv}{2}+\frac{v-Tv}{2},
$$

whose first term belongs to $E_1$ and second to $E_{-1}$. Their intersection is zero by [ii](#4/a/ii), so $V=E_1\oplus E_{-1}$ is a [direct sum](../../../vector-space.md#direct-sum). Choosing [bases](../../../vector-space.md#basis) of the two [eigenspaces](../../../linear-operator-theory.md#eigenspace) gives a diagonal [matrix](../../../vector-space.md#matrix) with entries $1$ and $-1$.

Since $T^2\ne T$ while $T^2=I$, we have $T\ne I$. Thus $\dim E_{-1}$ is $1$, $2$, or $3$. Reordering the [basis](../../../vector-space.md#basis) gives exactly

$$
\boxed{-I_3,\qquad\operatorname{diag}(1,1,-1),\qquad
\operatorname{diag}(1,-1,-1).}
$$

For $-I_3$, $T$ is **point inversion through the origin**. For $\operatorname{diag}(1,1,-1)$, it fixes the plane $E_1$ pointwise and reverses the complementary line $E_{-1}$: if $v=p+\ell$ in this [direct sum](../../../vector-space.md#direct-sum), then $Tv=p-\ell$. For $\operatorname{diag}(1,-1,-1)$, it fixes the line $E_1$ pointwise and reverses the complementary plane $E_{-1}$.

These are instances of [oblique symmetry of complementary subspaces](../../../group-theory.md#oblique-symmetry-of-complementary-subspaces), allowing oblique [eigenspaces](../../../linear-operator-theory.md#eigenspace). They are a Euclidean [reflection in a hyperplane](../../../linear-algebra.md#reflection-in-a-hyperplane) and a [rotation in three dimensions](../../../linear-algebra.md#rotation-in-three-dimensions) through $\pi$ about a line, respectively, when the two [eigenspaces](../../../linear-operator-theory.md#eigenspace) are perpendicular. The hypotheses do not require an [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) or an [orthonormal basis](../../../inner-product.md#orthonormal-basis), so that additional metric property cannot be inferred just from the displayed diagonal forms.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For this [tripotent linear operator](../../../vector-space.md#tripotent-linear-operator), the relation $T^3=T$ gives $T(T^2-I)=0$. Since $T^2\ne I$, there is $v$ with $(T^2-I)v\ne0$, and that nonzero [vector](../../../vector-space.md#vector) belongs to $\ker T$. Hence $n_T\geq1$. Also $T\ne0$, because $T=0$ would imply $T^2=T$. The [rank-nullity theorem](../../../kernel-of-a-linear-map.md#rank-nullity-theorem) in [dimension](../../../vector-space.md#dimension-vector-space) three therefore gives

$$
\boxed{n_T\in\{1,2\}.}
$$

Now suppose $n_T=2$. Then $\operatorname{im}T$ is a line. On this line, $T^2$ is the [identity operator](../../../vector-space.md#identity-operator): if $y=Tx$, then $T^2y=T^3x=Tx=y$. Consequently $T$ acts on this line by a [scalar](../../../vector-space.md#scalar) $c$ satisfying $c^2=1$. If $c=1$, then $T^2x=Tx$ for every $x$, contrary to $T^2\ne T$. Thus $c=-1$.

Choose a nonzero $w\in\operatorname{im}T$, so $Tw=-w$. It does not belong to $\ker T$. A [basis](../../../vector-space.md#basis) $k_1,k_2$ of $\ker T$, followed by $w$, is therefore a [basis](../../../vector-space.md#basis) of $V$, in which

$$
\boxed{[T]_{(k_1,k_2,w)}=\begin{pmatrix}0&0&0\\0&0&0\\0&0&-1\end{pmatrix}.}
$$

## 5

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [transposition](../../../combinatorics.md#transposition-permutation) in the [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_n$ exchanges two distinct symbols and fixes all others. A [permutation cycle](../../../finite-group-theory.md#permutation-cycle) $(a_1\ a_2\ \cdots\ a_k)$ sends $a_j$ to $a_{j+1}$, sends $a_k$ to $a_1$, and fixes the other symbols. Its entries are distinct. For $k=1$ this is the identity [permutation](../../../combinatorics.md#permutation).

A [group element](../../../group.md#group-element) has [order of a group element](../../../group-theory.md#order-of-a-group-element) $k$ if $k$ is the least positive integer for which its $k$th power is the [identity element](../../../algebraic-operation.md#identity-element). For the displayed [permutation cycle](../../../finite-group-theory.md#permutation-cycle), its $j$th power sends $a_i$ forward $j$ places, with subscripts read modulo $k$. Hence the $k$th power fixes every symbol, whereas for $0<j<k$ the image of $a_1$ is different from $a_1$. Thus its [order of a group element](../../../group-theory.md#order-of-a-group-element) is exactly $k$, including $k=1$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

For each symbol $a$, iterate the [permutation](../../../combinatorics.md#permutation) $\sigma$. Since the symbol set is finite, some iterate repeats. Applying an inverse power of $\sigma$ shows that the first return is to $a$ itself, giving

$$
a,\sigma(a),\ldots,\sigma^{k-1}(a),\qquad\sigma^k(a)=a,
$$

with the displayed symbols distinct. This is a [permutation cycle](../../../finite-group-theory.md#permutation-cycle). If two such lists share a symbol, applying powers of $\sigma$ shows that they contain exactly the same symbols. Hence these [group orbits](../../../group-action.md#orbit-group-theory) form a [partition of a set](../../../set.md#partition-of-a-set) $\{1,\ldots,n\}$. On each [group orbit](../../../group-action.md#orbit-group-theory), $\sigma$ acts as the corresponding [permutation cycle](../../../finite-group-theory.md#permutation-cycle), and these [disjoint permutation cycles](../../../finite-group-theory.md#disjoint-permutation-cycles) multiply to $\sigma$.

The [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) is **unique up to reordering the cycles and cyclically rotating the entries within each cycle**, with fixed points optionally omitted. Indeed, each cycle must consist of one of the uniquely determined [group orbits](../../../group-action.md#orbit-group-theory), and its successive entries must follow the action of $\sigma$.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

With products acting from right to left, a [permutation cycle](../../../finite-group-theory.md#permutation-cycle) satisfies

$$
(a_1\ a_2\ \cdots\ a_k)
=(a_1\ a_k)(a_1\ a_{k-1})\cdots(a_1\ a_2).
$$

The right side sends $a_1$ to $a_2$, each $a_j$ to $a_{j+1}$ for $2\leq j<k$, and $a_k$ to $a_1$, while fixing all other symbols. This verifies the formula. Applying it to every cycle in the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) expresses any [permutation](../../../combinatorics.md#permutation) as a product of [transpositions](../../../combinatorics.md#transposition-permutation). The identity is represented by the empty product.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

Suppose $\sigma$ has [order of a group element](../../../group-theory.md#order-of-a-group-element) two. On a cycle of length $k$, $\sigma^2$ moves each entry two places. Since $\sigma^2=e$, every such $k$ divides two, so $k=1$ or $k=2$. After omitting the fixed points, the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) is therefore a product of [disjoint permutation cycles](../../../finite-group-theory.md#disjoint-permutation-cycles) of length two, which are [transpositions](../../../combinatorics.md#transposition-permutation). There is at least one, because $\sigma\ne e$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

If a [permutation](../../../combinatorics.md#permutation) has disjoint cycle lengths $d_1,\ldots,d_t$, then its $k$th power is the identity exactly when every $d_j$ divides $k$. Thus its [order of a permutation](../../../combinatorics.md#order-of-a-permutation) is $\operatorname{lcm}(d_1,\ldots,d_t)$.

Suppose $n=p^r$ is a [prime power](../../../prime-number.md#prime-power) and $\sigma\in S_n$ has order $n$. Each $d_j$ divides $p^r$, so is a power of $p$. Their [least common multiple](../../../divisibility.md#least-common-multiple) is therefore their maximum, forcing some $d_j=p^r=n$. This cycle already uses all $n$ symbols, so $\sigma$ is an $n$-cycle.

Conversely, if $n>1$ is not a [prime power](../../../prime-number.md#prime-power), choose a prime-power factor $a=p^r$ containing the full power of one [prime divisor](../../../prime-number.md#prime-factor) of $n$, and put $b=n/a$. Then $a,b>1$, they are [coprime](../../../divisibility.md#coprime-integers), and $ab=n$. Moreover

$$
ab-a-b=(a-1)(b-1)-1\geq0,
$$

so $a+b\leq n$. We can therefore take disjoint cycles of lengths $a$ and $b$ in $S_n$, fixing all remaining symbols. Their product has [order of a permutation](../../../combinatorics.md#order-of-a-permutation) $\operatorname{lcm}(a,b)=ab=n$, but it is not an $n$-cycle. This proves the [prime-power characterization by full permutation cycles](../../../finite-group-theory.md#prime-power-characterization-by-full-permutation-cycles):

$$
\boxed{\text{every element of order }n\text{ in }S_n\text{ is an }n\text{-cycle}\iff n=p^r.}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Acting separately on disjoint sets of four and eight symbols embeds the [direct product of groups](../../../group-theory.md#direct-product-of-groups) $S_4\times S_8$ into $S_{12}$. The action is injective since fixing all twelve symbols forces both factors to be identities.

For the lower bound, $S_4$ contains a cycle of order four and $S_8$ contains disjoint cycles of lengths five and three, whose product has order fifteen. The corresponding element of $S_4\times S_8$ has [order of a group element](../../../group-theory.md#order-of-a-group-element) $\operatorname{lcm}(4,15)=60$. Every isomorphic subgroup of $S_n$ must therefore contain a [permutation](../../../combinatorics.md#permutation) of order sixty. We can bound the [minimum number of symbols for a permutation of prescribed order](../../../combinatorics.md#minimum-number-of-symbols-for-a-permutation-of-prescribed-order) directly here.

In the [disjoint cycle decomposition](../../../finite-group-theory.md#disjoint-cycle-decomposition) of such a [permutation](../../../combinatorics.md#permutation), all cycle lengths divide $60$, and their [least common multiple](../../../divisibility.md#least-common-multiple) must contain the factors $4$, $3$, and $5$. If these factors occur in three distinct cycles, those cycles use at least $4+3+5=12$ symbols. If two occur in the same cycle, that cycle has length at least their product: combining $4,3$ costs at least $12$, combining $4,5$ costs at least $20$, and combining $3,5$ costs at least $15$. Each possibility already requires at least twelve symbols. Thus $n\geq12$, and

$$
\boxed{n_{\min}=12.}
$$

## 6

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

[Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states that for a [subgroup](../../../group.md#subgroup) $K$ of a [finite group](../../../group.md#finite-group) $G$,

$$
|G|=[G:K]|K|;
$$

in particular, $|K|$ divides $|G|$. Here $[G:K]$ is the [subgroup index](../../../group.md#index-of-a-subgroup), the number of left [cosets](../../../group-theory.md#coset) of $K$.

The [order of a group element](../../../group-theory.md#order-of-a-group-element) $g\in G$ is the least positive integer $k$ such that $g^k=e$. It exists because $G$ is finite. The [cyclic subgroup](../../../group.md#cyclic-subgroup) $\langle g\rangle$ consists of exactly $e,g,\ldots,g^{k-1}$, so has order $k$. Applying [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) to this [subgroup](../../../group.md#subgroup) gives

$$
\boxed{o(g)\mid|G|.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

A map $\phi:G\to G$ is a [group isomorphism](../../../algebra.md#group-isomorphism) if it is a [bijection](../../../function.md#bijection) and a [group homomorphism](../../../group-theory.md#group-homomorphism), meaning

$$
\phi(xy)=\phi(x)\phi(y)\qquad(x,y\in G).
$$

Such a map from a [group](../../../group.md) to itself is an [group automorphism](../../../algebra.md#group-automorphism). Its inverse is also a [group homomorphism](../../../group-theory.md#group-homomorphism): if $u=\phi(x)$ and $v=\phi(y)$, then $\phi^{-1}(uv)=xy=\phi^{-1}(u)\phi^{-1}(v)$.

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Write $C_p=\langle g\rangle$. A [group homomorphism](../../../group-theory.md#group-homomorphism) from this [cyclic group](../../../group.md#cyclic-group) is determined by the image of $g$, because $\phi(g^j)=\phi(g)^j$. Each choice $\phi(g)=g^a$, with $a=0,\ldots,p-1$, gives a well-defined [group homomorphism](../../../group-theory.md#group-homomorphism). It is an [group automorphism](../../../algebra.md#group-automorphism) exactly when $g^a$ generates $C_p$.

For a [prime number](../../../prime-number.md) $p$, every $a=1,\ldots,p-1$ is [coprime](../../../divisibility.md#coprime-integers) to $p$, so the powers of $g^a$ run through all of $C_p$. The choice $a=0$ gives the trivial [group homomorphism](../../../group-theory.md#group-homomorphism) and fails to be bijective. Consequently

$$
\boxed{|\operatorname{Aut}(C_p)|=p-1.}
$$

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

For $h\in H$, define $\pi(h)(n)=hnh^{-1}$. Since $N$ is a [normal subgroup](../../../group-theory.md#normal-subgroup), this sends $N$ into itself. It preserves multiplication, and its inverse is conjugation by $h^{-1}$, so it is an [group automorphism](../../../algebra.md#group-automorphism) of $N$. Moreover

$$
\pi(h_1h_2)(n)=h_1h_2n h_2^{-1}h_1^{-1}
=\bigl(\pi(h_1)\circ\pi(h_2)\bigr)(n).
$$

Thus $\pi:H\to\operatorname{Aut}(N)$ is a [group homomorphism](../../../group-theory.md#group-homomorphism), induced by the [group action](../../../group-action.md) of [conjugation](../../../group-action.md#conjugation).

If $\pi$ is trivial, every element of $H$ commutes with every element of $N$. Hence

$$
F:N\times H\longrightarrow G,\qquad F(n,h)=nh
$$

is a [group homomorphism](../../../group-theory.md#group-homomorphism), since $(n_1h_1)(n_2h_2)=n_1n_2h_1h_2$. Its [image of a group homomorphism](../../../group-theory.md#image-of-a-group-homomorphism) is a [subgroup](../../../group.md#subgroup) containing both $N$ and $H$, and every product $nh$ lies in $\langle N,H\rangle$, so its image is exactly $\langle N,H\rangle$. If $nh=e$, then $n=h^{-1}\in N\cap H=\{e\}$, so $n=h=e$. Thus $F$ is injective and gives

$$
\boxed{\langle N,H\rangle\cong N\times H.}
$$

<h4 id="6/b/iv">iv</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/b/iv)

The [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) of $H$ for this [conjugation](../../../group-action.md#conjugation) [group action](../../../group-action.md) is its [normalizer](../../../group-action.md#normalizer)

$$
\operatorname{Stab}(H)=N_G(H)=\{g\in G:gHg^{-1}=H\}.
$$

If it is all of $G$, the equality $gHg^{-1}=H$ holds for every $g\in G$, which is precisely the definition of a [normal subgroup](../../../group-theory.md#normal-subgroup).

If instead $\operatorname{Stab}(H)=H$, the [orbit-stabilizer theorem](../../../group-action.md#orbit-stabilizer-theorem) says that the [group orbit](../../../group-action.md#orbit-group-theory) of $H$ has size $[G:H]$. Every conjugate $gHg^{-1}$ is isomorphic to $H$, with [group isomorphism](../../../algebra.md#group-isomorphism) $h\mapsto ghg^{-1}$, so this [group orbit](../../../group-action.md#orbit-group-theory) is a [subset](../../../set.md#subset) of $\Omega$. Therefore

$$
\boxed{|\Omega|\geq[G:H].}
$$

The [group action](../../../group-action.md) need not be transitive on all of $\Omega$; this one [group orbit](../../../group-action.md#orbit-group-theory) supplies the lower bound.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

By [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), every nonidentity [group element](../../../group.md#group-element) has order $5$, $7$, or $35$. If some element has order $35$, its seventh and fifth powers have orders $5$ and $7$, respectively, and we are done.

Otherwise every nonidentity element has order $5$ or $7$. Distinct [subgroups](../../../group.md#subgroup) of a given [prime number](../../../prime-number.md) order intersect only in the identity: a shared nonidentity element generates both. If there were no element of order $5$, the $34$ nonidentity elements would therefore partition into sets of six, the nonidentity elements of the [cyclic subgroups](../../../group.md#cyclic-subgroup) of order seven. This would force $6\mid34$, a contradiction. If there were no element of order $7$, the analogous partition into sets of four would force $4\mid34$, again a contradiction. Thus **elements of both orders exist**.

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

Let $P$ and $Q$ be [subgroups](../../../group.md#subgroup) of orders five and seven, which exist by [i](#6/c/i). Their [normalizers](../../../group-action.md#normalizer) contain $P$ and $Q$, respectively. By [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), $N_G(P)$ has order $5$ or $35$, and $N_G(Q)$ has order $7$ or $35$. If either has order $35$, its [subgroup](../../../group.md#subgroup) is normal by [iv](#6/b/iv).

Suppose neither is normal. Then [iv](#6/b/iv) gives at least seven distinct [subgroups](../../../group.md#subgroup) of order five and at least five distinct [subgroups](../../../group.md#subgroup) of order seven. Distinct [subgroups](../../../group.md#subgroup) of the same prime order intersect only in the identity, and a [subgroup](../../../group.md#subgroup) of order five and one of order seven also intersect only in the identity by [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). Thus $G$ would have at least

$$
7(5-1)+5(7-1)=58
$$

nonidentity elements, contradicting $|G|-1=34$. Hence **at least one of $P,Q$ is a normal subgroup**.

<h4 id="6/c/iii">iii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/c/iii)

Choose a [normal subgroup](../../../group-theory.md#normal-subgroup) $N$ of prime order $p\in\{5,7\}$ as in [ii](#6/c/ii), and choose a [subgroup](../../../group.md#subgroup) $H$ of the other prime order $q$. Their intersection is trivial by [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). Both are [cyclic groups](../../../group.md#cyclic-group), and [ii](#6/b/ii) gives $|\operatorname{Aut}(N)|=p-1$.

The [image of a group homomorphism](../../../group-theory.md#image-of-a-group-homomorphism) $\pi:H\to\operatorname{Aut}(N)$ from [iii](#6/b/iii) has order dividing $q$, because its [kernel of a group homomorphism](../../../group-theory.md#kernel-of-a-group-homomorphism) partitions $H$ into equally sized [cosets](../../../group-theory.md#coset). Its order also divides $p-1$ by [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). But

$$
\gcd(7,4)=\gcd(5,6)=1,
$$

so $\pi$ is trivial in either case. By [iii](#6/b/iii), $\langle N,H\rangle\cong C_p\times C_q$ has order $pq=35$ and therefore equals $G$.

If $n$ and $h$ generate $N$ and $H$, the element $(n,h)$ has order $\operatorname{lcm}(p,q)=pq=35$, since its $k$th power is the identity exactly when both $p$ and $q$ divide $k$. Thus this [direct product of groups](../../../group-theory.md#direct-product-of-groups) is cyclic, and

$$
\boxed{G\cong C_{35}.}
$$

## 7

↑ **Parent:** [Mathematics I](mathematics-i.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

A left [group action](../../../group-action.md) is a map $a:G\times X\to X$ satisfying

$$
a(e,x)=x,\qquad a(gh,x)=a\bigl(g,a(h,x)\bigr)
\quad(g,h\in G,\ x\in X).
$$

Define $\rho_a(g):X\to X$ by $\rho_a(g)(x)=a(g,x)$. The action axioms give

$$
\rho_a(g)\circ\rho_a(g^{-1})=\rho_a(e)=\operatorname{id}_X
=\rho_a(g^{-1})\circ\rho_a(g).
$$

Hence each $\rho_a(g)$ is a [bijection](../../../function.md#bijection), with inverse $\rho_a(g^{-1})$, and belongs to the [symmetric group](../../../finite-group-theory.md#symmetric-group) $\operatorname{Sym}(X)$. Finally,

$$
\rho_a(gh)(x)=a(gh,x)=a\bigl(g,a(h,x)\bigr)
=\bigl(\rho_a(g)\circ\rho_a(h)\bigr)(x),
$$

so $\rho_a:G\to\operatorname{Sym}(X)$ is a [group homomorphism](../../../group-theory.md#group-homomorphism).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

For $X\in\operatorname{SO}_3(\mathbb R)$, the defining identity $X^TX=I$ gives

$$
\|Xv\|^2=v^TX^TXv=v^Tv=\|v\|^2.
$$

Thus an [orthogonal transformation](../../../linear-algebra.md#orthogonal-transformation) preserves the [Euclidean norm](../../../normed-vector-space.md#euclidean-norm) and sends the [unit sphere](../../../topology.md#unit-sphere) to itself. Restricting the given [group action](../../../group-action.md) to this invariant set preserves both action axioms.

If $XN=N$, the first column of $X$ is $N=e_1$. The other columns are [unit vectors](../../../vector-space.md#unit-vector) perpendicular to it, so the first row is also $(1,0,0)$. Hence $X=\operatorname{diag}(1,B)$ with $B^TB=I_2$ and $\det B=1$. Conversely, every such [matrix](../../../vector-space.md#matrix) lies in $G$ and fixes $N$. Since every element of the [special orthogonal group in two dimensions](../../../linear-algebra.md#special-orthogonal-group-in-two-dimensions) has the planar [rotation matrix](../../../linear-algebra.md#rotation-matrix) form, the [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) is

$$
\boxed{H=\left\{R_\theta=
\begin{pmatrix}
1&0&0\\
0&\cos\theta&-\sin\theta\\
0&\sin\theta&\cos\theta
\end{pmatrix}:\theta\in\mathbb R\right\}\cong\operatorname{SO}_2(\mathbb R).}
$$

Geometrically these are exactly the [rotations in three dimensions](../../../linear-algebra.md#rotation-in-three-dimensions) about the first coordinate axis.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

Let $v\in S$. Choose a [unit vector](../../../vector-space.md#unit-vector) $u$ perpendicular to $v$, and put $w=v\times u$. The [cross product](../../../vector-space.md#cross-product) identities show that $(v,u,w)$ is an [orthonormal basis](../../../inner-product.md#orthonormal-basis) with positive orientation: $u\times(v\times u)=v$, so

$$
\det\begin{pmatrix}v&u&w\end{pmatrix}
=v\cdot(u\times w)=v\cdot v=1.
$$

Thus the [matrix](../../../vector-space.md#matrix) $A_v$ with these columns belongs to the [special orthogonal group](../../../linear-algebra.md#special-orthogonal-group) $G$ and satisfies $A_vN=v$. For any $v,z\in S$, the element $A_zA_v^{-1}$ sends $v$ to $z$. Therefore the [group action](../../../group-action.md) on the [unit sphere](../../../topology.md#unit-sphere) is **transitive**.

<h4 id="7/b/iii">iii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/b/iii)

For any integer $n\geq1$, let $R=R_{2\pi/n}$ in the [stabilizer subgroup](../../../group-action.md#stabilizer-subgroup) from [i](#7/b/i). Since $R_\theta R_\phi=R_{\theta+\phi}$ and $R_\theta=I$ exactly when $\theta\in2\pi\mathbb Z$, this [rotation matrix](../../../linear-algebra.md#rotation-matrix) has order exactly $n$. Therefore

$$
\boxed{\langle R_{2\pi/n}\rangle\cong C_n}
$$

is a [subgroup](../../../group.md#subgroup) of $G$ of order $n$, including the trivial case $n=1$.

For infinitely many non-Abelian examples, let $n\geq3$, retain $R=R_{2\pi/n}$, and take the half-turn

$$
J=\operatorname{diag}(-1,1,-1)\in G.
$$

Direct multiplication gives $J^2=I$ and $JRJ=R^{-1}$. Every word in $R,J$ therefore reduces to $R^k$ or $R^kJ$, $0\leq k<n$. The $R^k$ are distinct, as are the $R^kJ$, and no element from the first family equals one from the second: they send $N$ to $N$ and $-N$, respectively. Hence $\langle R,J\rangle$ has exactly $2n$ elements and is a [dihedral group](../../../finite-group-theory.md#dihedral-group).

It is non-Abelian because $R\ne R^{-1}$ for $n\geq3$, so $JR\ne RJ$. Different values of $n$ give different [group orders](../../../group.md#order-of-a-finite-group), and therefore different [subgroups](../../../group.md#subgroup). Thus **$G$ has infinitely many non-Abelian subgroups**, already among its finite [subgroups](../../../group.md#subgroup).

## ↑ Ancestors (9)

1. [Prelims](../prelims.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Oxford](../../../past-exam-of-the-mathematics-course-of-the-university-of-oxford.md)
4. [Mathematics course of the University of Oxford](../../../university-of-oxford.md#mathematics-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../../university-of-oxford.md)
8. [List of universities](../../../README.md#list-of-universities)
9. [Codex Wiki](../../../README.md)
