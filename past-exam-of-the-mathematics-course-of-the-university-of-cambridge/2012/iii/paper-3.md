# Paper 3

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_3.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_3.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) $n$ is a finite sequence $\lambda_1\geq\cdots\geq\lambda_\ell>0$ with sum $n$; append zeros when comparing lengths. Its [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram) has cells $(i,j)$ with $1\leq j\leq\lambda_i$. A [Young tableau](../../../representation-theory-of-the-symmetric-group.md#young-tableau) is a bijective filling of these cells by $1,\ldots,n$. Write $R_t,C_t$ for its [row and column stabilizers](../../../representation-theory-of-the-symmetric-group.md#row-and-column-stabilizers-of-a-young-tableau), and fix the convention

$$
r_t=\sum_{r\in R_t}r,\qquad
c_t=\sum_{c\in C_t}\operatorname{sgn}(c)c,\qquad
h_t=c_tr_t.
$$

[Permutations](../../../combinatorics.md#permutation) act on entries on the left, with the rightmost factor acting first. This defines the [Young symmetrizer](../../../representation-theory-of-the-symmetric-group.md#young-symmetrizer) used throughout. In the [dictionary order on integer partitions](../../../representation-theory-of-the-symmetric-group.md#dictionary-order-on-integer-partitions), $\lambda>\mu$ means that at the first differing part $\lambda_i>\mu_i$; equality is allowed in $\geq$.

Suppose there is no row-column collision between $t$ of shape $\lambda$ and $u$ of shape $\mu$. Each column of $u$ contains at most one entry from each row of $t$. The first $k$ rows of $t$ therefore contain at most

$$
\sum_j\min(k,\mu'_j)=\sum_{i=1}^k\mu_i
$$

entries, where $\mu'_j$ is a column length. Thus $\sum_{i\leq k}\lambda_i\leq\sum_{i\leq k}\mu_i$ for every $k$: $\mu$ dominates $\lambda$ in [dominance order on partitions](../../../representation-theory-of-the-symmetric-group.md#dominance-order-on-partitions). If $\lambda\geq\mu$ in [dictionary order on integer partitions](../../../representation-theory-of-the-symmetric-group.md#dictionary-order-on-integer-partitions), a first strictly larger part would contradict the corresponding prefix inequality. Hence **$\lambda=\mu$**.

All the bounds must now be equalities. Every column $j$ of $u$ contains exactly one entry from row $i$ of $t$ whenever $i\leq\lambda'_j$. Choose $r_0\in R_t$ sending that entry to the entry of $t$ in cell $(i,j)$. These prescriptions are bijections within the rows. The columns of $r_0u$ then have exactly the same sets of entries as the columns of $t$, so $r_0u=c_0t$ for some $c_0\in C_t$. Consequently

$$
\boxed{u=r_0^{-1}c_0t,\quad r_0^{-1}\in R_t,\quad c_0\in C_t.}
$$

If a collision was present instead, its two entries supply the first alternative. This proves the [row-column collision lemma](../../../representation-theory-of-the-symmetric-group.md#row-column-collision-lemma), including the prescribed order of the two stabilizer factors.

We next prove the [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module) classification. By [Maschke's theorem](../../../representation-theory.md#maschke-s-theorem), the [group algebra](../../../associative-algebra.md#group-algebra) $A=\mathbb CS_n$ is a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra). Use the permitted basic quasi-idempotence of a [Young symmetrizer](../../../representation-theory-of-the-symmetric-group.md#young-symmetrizer),

$$
h_t^2=H_\lambda h_t,\qquad
H_\lambda=\prod_{(i,j)\in\lambda}(\lambda_i-j+\lambda'_j-i+1)\ne0,
$$

and put $e_t=h_t/H_\lambda$. The coefficient of $1$ in $h_t$ is one, because $R_t\cap C_t=\{1\}$, so $e_t\ne0$.

For $\pi\in S_n$, consider $r_t\pi c_t$. A collision between the rows of $t$ and the columns of $\pi t$ gives a [transposition](../../../combinatorics.md#transposition-permutation) $\tau\in R_t\cap\pi C_t\pi^{-1}$. Row symmetrization fixes $\tau$, whereas column antisymmetrization changes its sign, so $r_t\pi c_t=0$. If there is no collision, the proved lemma gives $\pi=rc$ with $r\in R_t,c\in C_t$, and

$$
r_t\pi c_t=\operatorname{sgn}(c)r_tc_t.
$$

It follows that $h_t\pi h_t$ is zero or $\operatorname{sgn}(c)H_\lambda h_t$. Since [permutations](../../../combinatorics.md#permutation) span $A$, **$e_tAe_t=\mathbb Ce_t$**. In a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra) this means that $e_t$ is a [primitive idempotent](../../../commutative-algebra.md#primitive-idempotent), so $Ae_t=Ah_t$ is an irreducible left module.

If $\lambda>\mu$ in [dictionary order on integer partitions](../../../representation-theory-of-the-symmetric-group.md#dictionary-order-on-integer-partitions), the collision lemma applied to every $\pi u$ gives $r_tA c_u=0$, and therefore $h_tA h_u=0$. Since

$$
\operatorname{Hom}_A(Ae_t,Ae_u)\cong e_tAe_u,
$$

the two [simple modules](../../../module-theory.md#irreducible-module) cannot be isomorphic. Conversely, [Young tableaux](../../../representation-theory-of-the-symmetric-group.md#young-tableau) of the same shape are related by a [permutation](../../../combinatorics.md#permutation), which conjugates their [Young symmetrizers](../../../representation-theory-of-the-symmetric-group.md#young-symmetrizer) and gives isomorphic [left ideals](../../../associative-algebra.md#left-ideal). Finally, the center of $\mathbb CS_n$ has the conjugacy-class sums as a basis. [Conjugacy classes](../../../group-theory.md#conjugacy-class) are indexed by cycle-type partitions, so its dimension is the number of partitions of $n$. The [Artin–Wedderburn theorem](../../../associative-algebra.md#artin-wedderburn-theorem) gives exactly that many simple-module isomorphism classes. We have already produced one for each partition. Thus **the $Ah_\lambda$ form a complete set of pairwise nonisomorphic [irreducible modules](../../../module-theory.md#irreducible-module)**.

## 2

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [standard Young tableau](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) has its entries increasing from left to right in each row and from top to bottom in each column. For the convention $h_t=c_tr_t$, use [column-reading order of standard Young tableaux](../../../representation-theory-of-the-symmetric-group.md#column-reading-order-of-standard-young-tableaux): read columns from left to right, each from top to bottom, and compare the resulting words lexicographically. This makes the requested product direction explicit. The order and the symmetrizer multiplication convention must be chosen together.

We prove the vanishing claim. Suppose the rows of $t$ and the columns of $u$ have no collision. The argument in Question 1 shows that every column of $u$ contains one entry from each eligible row of $t$. Its first column thus selects one entry from every row. Each selected entry is at least the first entry of that row in $t$. Sorting the selected entries, as the [standard tableau](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) $u$ does, gives a column componentwise at least the first column of $t$: increasing individual entries cannot decrease any order statistic. If the columns are equal, equality of their sums forces every selected entry to be that row's first entry. Delete this common column and repeat. At the first differing column, its first differing entry in $u$ is therefore larger; otherwise $u=t$. Thus absence of a collision implies $u\geq t$ in [column-reading order of standard Young tableaux](../../../representation-theory-of-the-symmetric-group.md#column-reading-order-of-standard-young-tableaux).

If $t>u$, there must instead be a [transposition](../../../combinatorics.md#transposition-permutation) in $R_t\cap C_u$. It fixes $r_t$ and negates $c_u$, giving $r_tc_u=0$. Hence

$$
\boxed{h_th_u=c_t(r_tc_u)r_u=0\qquad(t>u).}
$$

This is [triangular vanishing of Young-symmetrizer products](../../../representation-theory-of-the-symmetric-group.md#triangular-vanishing-of-young-symmetrizer-products); it does not assert vanishing in the opposite order.

Normalize to $e_t=h_t/H_\lambda$. List all [standard tableaux](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) in increasing shape [dictionary order on integer partitions](../../../representation-theory-of-the-symmetric-group.md#dictionary-order-on-integer-partitions), and within each shape in increasing [column-reading order of standard Young tableaux](../../../representation-theory-of-the-symmetric-group.md#column-reading-order-of-standard-young-tableaux). Then $e_ie_j=0$ for $i>j$, using Question 1 between different shapes and the result above within a shape. The [left ideals](../../../associative-algebra.md#left-ideal) $Ae_i$ have an internal [direct sum](../../../vector-space.md#direct-sum): if $\sum_i z_i=0$ with $z_i\in Ae_i$, multiply on the right by $e_1$ to get $z_1=0$, since $z_1e_1=z_1$ and every later $z_ie_1=0$. Repeat with $e_2,e_3,\ldots$. This proves directness without incorrectly treating all the [idempotents](../../../commutative-algebra.md#idempotent) as mutually orthogonal.

Let $f_\lambda$ count the [standard tableaux](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) of shape $\lambda$ and let $d_\lambda=\dim S^\lambda$. In the [regular representation](../../../representation-theory.md#regular-representation) a [simple module](../../../module-theory.md#irreducible-module) of dimension $d_\lambda$ occurs $d_\lambda$ times, by the [Artin–Wedderburn theorem](../../../associative-algebra.md#artin-wedderburn-theorem). The [direct sum](../../../vector-space.md#direct-sum) just constructed contains $f_\lambda$ copies of $S^\lambda$, so $f_\lambda\leq d_\lambda$ for every shape. We supply the needed counting identity independently of the dimension conclusion.

The [Robinson–Schensted correspondence](../../../representation-theory-of-the-symmetric-group.md#robinson-schensted-correspondence) bijects [permutations](../../../combinatorics.md#permutation) with pairs of [standard tableaux](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) of the same shape. Here is its [row insertion](../../../representation-theory-of-the-symmetric-group.md#row-insertion) construction and inverse. Insert the successive [permutation](../../../combinatorics.md#permutation) entries into an increasing row by replacing its first entry larger than the incoming entry, bumping that replaced entry into the next row; if no entry is larger, append at the row end. Continue until a new cell is created. Record the insertion time in that cell of a second tableau. For completeness, the successive bumped entries strictly increase, and their column indices weakly decrease: an entry below a bumped entry was originally larger, so the next replacement occurs no farther right. The entry newly placed in each row is smaller than the entry removed and larger than the entry above it. At a strictly earlier column, that last inequality follows from row increase in the preceding row; at the same column, it follows from the preceding bump. Hence the insertion tableau keeps increasing rows and columns. If a new cell is appended below the first row, the preceding bump guarantees that the row above reaches that column, so the shape stays a [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram). Recording times also increase in rows and columns, since every new cell is an outer corner of the current diagram. Thus both tableaux are standard at the end. Conversely, remove the cell with the largest recording label. Reverse its bumping path upward, replacing in each preceding row the rightmost entry smaller than the moving entry and moving the displaced entry upward. This recovers the last inserted letter; iterating recovers the entire [permutation](../../../combinatorics.md#permutation). The two rules undo one another at each row. Thus

$$
n!=\sum_{\lambda\vdash n}f_\lambda^2.
$$

Semisimplicity also gives $n!=\sum_\lambda d_\lambda^2$. Since $0\leq f_\lambda\leq d_\lambda$ termwise, equality of these sums forces $f_\lambda=d_\lambda$ for every shape. The internal [direct sum](../../../vector-space.md#direct-sum) has dimension $n!$ and hence fills $A$:

$$
\boxed{A=\bigoplus_{\lambda\vdash n}\ \bigoplus_{t\in\operatorname{SYT}(\lambda)}Ah_t,
\qquad \dim S^\lambda=\#\operatorname{SYT}(\lambda).}
$$

There is also a useful numerical form. Right multiplication by $e_t$ is an [idempotent](../../../commutative-algebra.md#idempotent) with image $Ae_t$. In the [permutation](../../../combinatorics.md#permutation) basis of $A$, each diagonal coefficient is the coefficient of $1$ in $e_t$, namely $1/H_\lambda$. Its trace equals its rank, so **$\dim S^\lambda=n!/H_\lambda$**. Together with the count just obtained this recovers the [hook-length formula](../../../representation-theory-of-the-symmetric-group.md#hook-length-formula).

## 3

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

On $T=V^{\otimes n}$, define the [permutation](../../../combinatorics.md#permutation) and diagonal actions by

$$
\sigma(v_1\otimes\cdots\otimes v_n)
=v_{\sigma^{-1}(1)}\otimes\cdots\otimes v_{\sigma^{-1}(n)},\qquad
g(v_1\otimes\cdots\otimes v_n)=gv_1\otimes\cdots\otimes gv_n.
$$

The inverse in the first formula gives a left action. Applying $g$ to every tensor factor and then reordering produces the same tensor as reordering and then applying $g$. Thus the two actions commute. The [Schur algebra](../../../lie-theory.md#schur-algebra) is

$$
\boxed{S_{\mathbb C}(m,n)=\operatorname{End}_{\mathbb CS_n}(T).}
$$

It is the [commutant of an operator algebra](../../../associative-algebra.md#commutant-of-an-operator-algebra) of the [permutation](../../../combinatorics.md#permutation) action.

To identify this commutant, use the multilinear isomorphism

$$
\operatorname{End}(T)\cong\operatorname{End}(V)^{\otimes n}.
$$

Conjugation by a [permutation](../../../combinatorics.md#permutation) reorders the factors on the right. Therefore the invariant subspace is the space of [symmetric tensors](../../../linear-algebra.md#symmetric-tensor) of degree $n$ in $\operatorname{End}(V)$. It is spanned by $a^{\otimes n}$. Indeed, the polarization identity

$$
\sum_{J\subseteq\{1,\ldots,n\}}(-1)^{n-|J|}
\left(\sum_{j\in J}a_j\right)^{\otimes n}
=\sum_{\sigma\in S_n}a_{\sigma(1)}\otimes\cdots\otimes a_{\sigma(n)}
$$

expresses every symmetrized elementary tensor as a [linear combination](../../../vector-space.md#linear-combination) of pure powers. Those symmetrized elementary tensors span the invariant subspace in [characteristic zero](../../../algebra.md#characteristic-zero).

One may restrict $a$ to invertible [endomorphisms](../../../algebra.md#endomorphism) without changing the span. For fixed $a$, the vector-valued [polynomial](../../../polynomial.md) $(a+tI)^{\otimes n}$ has degree at most $n$. Choose $n+1$ distinct values of $t$ away from the finitely many roots of $\det(a+tI)$. [Polynomial interpolation](../../../numerical-analysis.md#polynomial-interpolation) expresses its constant term $a^{\otimes n}$ as a [linear combination](../../../vector-space.md#linear-combination) of those invertible [tensor powers](../../../linear-algebra.md#tensor-power). Consequently

$$
S_{\mathbb C}(m,n)=\operatorname{span}_{\mathbb C}\{g^{\otimes n}:g\in\operatorname{GL}(V)\}.
$$

The span is an algebra, since products are $(gh)^{\otimes n}$.

The image $A_T$ of $\mathbb CS_n$ is semisimple, as a quotient of a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra). The [double-centralizer theorem for semisimple operator algebras](../../../associative-algebra.md#double-centralizer-theorem-for-semisimple-operator-algebras) gives $A_T''=A_T$. Since the preceding computation says that $A_T'$ is the span of the general linear action, the two actions are **mutual commutants**. More explicitly, [semisimple module](../../../module-theory.md#semisimple-module) decomposition gives

$$
\boxed{V^{\otimes n}\cong
\bigoplus_{\substack{\lambda\vdash n\\\ell(\lambda)\leq m}}
S^\lambda\otimes D_\lambda(V).}
$$

Here $D_\lambda(V)=\operatorname{Hom}_{S_n}(S^\lambda,T)$ is the multiplicity space, with its natural general linear action. The commutant algebra is the product of the full [endomorphism](../../../algebra.md#endomorphism) algebras of these multiplicity spaces. Hence each nonzero $D_\lambda$ is irreducible, and distinct spaces have nonisomorphic general linear representations, because the operators $g^{\otimes n}$ span that commutant. A primitive $e_t$ picks a one-dimensional factor from $S^\lambda$, so $e_tT$ is an equivalent realization of $D_\lambda$ as a [Schur module](../../../lie-theory.md#schur-module).

The range of shapes is exact. If $\lambda$ has more than $m$ rows, a column antisymmetrizes more than $m$ vectors and its action vanishes by $\Lambda^{m+1}V=0$. Conversely, for at most $m$ rows place the $i$th basis vector in every tensor position belonging to row $i$ of $t$. Row symmetrization multiplies this tensor by $\prod_i\lambda_i!$. Column antisymmetrization is nonzero, because all vectors within each column are distinct, and its different [permutations](../../../combinatorics.md#permutation) give distinct basis tensors. Thus $h_tT\ne0$. This proves the [length bound for a Schur module](../../../lie-theory.md#length-bound-for-a-schur-module) and the stated [Schur–Weyl duality](../../../lie-theory.md#schur-weyl-duality). For $n=0$, the empty partition and $V^{\otimes0}=\mathbb C$ give the trivial version.

## 4

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a partition $\nu$ with at most $m$ parts, let $D_\nu(V)$ be the [Schur module](../../../lie-theory.md#schur-module) constructed in Question 3, equivalently the image of a [Young symmetrizer](../../../representation-theory-of-the-symmetric-group.md#young-symmetrizer) on $V^{\otimes|\nu|}$. For a weakly decreasing integer tuple $\lambda$, put $k=\max(0,-\lambda_m)$ and $\nu=\lambda+k(1,\ldots,1)$. Define the [rational Schur module](../../../lie-theory.md#rational-schur-module) by

$$
\boxed{D_\lambda(V)=\det^{-k}\otimes D_\nu(V).}
$$

Here $\det^{-k}$ is the one-dimensional representation $g\mapsto\det(g)^{-k}$. This is rational, and it is irreducible under the permitted irreducibility assumption; for nonnegative $\lambda$ it is the original [polynomial](../../../polynomial.md) [Schur module](../../../lie-theory.md#schur-module). Larger shifts give the same module, as will also follow from the [character](../../../representation-theory.md#character-of-a-representation) formula below.

Write $s_r(x)=\sum_{i=1}^m x_i^r$ and $p_\alpha(x)=\prod_{r=1}^n s_r(x)^{\alpha_r}$. For a [permutation](../../../combinatorics.md#permutation) $\sigma$ of the given cycle type, the [trace of a permuted tensor power](../../../lie-theory.md#trace-of-a-permuted-tensor-power) is

$$
\operatorname{tr}_T(\sigma\xi^{\otimes n})
=\prod_{r=1}^n\operatorname{tr}(\xi^r)^{\alpha_r}=p_\alpha(x).
$$

In a tensor basis, the trace contracts the matrix entries of $\xi$ around each cycle of $\sigma$; a cycle of length $r$ contributes $\operatorname{tr}(\xi^r)$. This proof applies to nondiagonalizable [endomorphisms](../../../algebra.md#endomorphism) as well. The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) give $\operatorname{tr}(\xi^r)=s_r(x)$.

The [Schur–Weyl duality](../../../lie-theory.md#schur-weyl-duality) decomposition, on which $\sigma$ and $\xi^{\otimes n}$ act on the two respective factors, gives the same trace as

$$
\boxed{p_\alpha(x)=\sum_{\substack{\lambda\vdash n\\\ell(\lambda)\leq m}}
\chi^\lambda(\alpha)\phi_\lambda(\xi).}
$$

For a partition, the [character](../../../representation-theory.md#character-of-a-representation) extends polynomially to all [endomorphisms](../../../algebra.md#endomorphism) because the tensor-power action does. This extension is not asserted for determinant-twisted modules at singular matrices.

We now derive the [alternant character formula for the general linear group](../../../semisimple-lie-algebra.md#alternant-character-formula-for-the-general-linear-group). Put $\delta=(m-1,m-2,\ldots,0)$ and

$$
a_\beta(x)=\det(x_i^{\beta_j})_{1\leq i,j\leq m},\qquad
a_\delta(x)=\prod_{i<j}(x_i-x_j).
$$

Use the permitted symmetric-group [character](../../../representation-theory.md#character-of-a-representation) result, the [Frobenius alternant character formula](../../../combinatorics.md#frobenius-alternant-character-formula):

$$
\chi^\lambda(\alpha)=[x^{\lambda+\delta}]\bigl(a_\delta(x)p_\alpha(x)\bigr).
$$

It concerns [characters](../../../representation-theory.md#character-of-a-representation) of $S_n$, rather than assuming the [character](../../../representation-theory.md#character-of-a-representation) formula we seek for the general linear group. Substitute the proved trace identity and set

$$
c_{\lambda\mu}=[x^{\lambda+\delta}]\bigl(a_\delta\phi_\mu\bigr).
$$

Then $\chi^\lambda(\alpha)=\sum_\mu c_{\lambda\mu}\chi^\mu(\alpha)$ for every [conjugacy class](../../../group-theory.md#conjugacy-class). Independence of the irreducible symmetric-group [characters](../../../representation-theory.md#character-of-a-representation) forces $c_{\lambda\mu}=\delta_{\lambda\mu}$.

Each [character](../../../representation-theory.md#character-of-a-representation) $\phi_\mu$ on diagonal matrices is a symmetric homogeneous [polynomial](../../../polynomial.md) of degree $n$, since conjugation by [permutation](../../../combinatorics.md#permutation) matrices permutes its arguments. Thus $a_\delta\phi_\mu$ is alternating of degree $n+\binom m2$. Every [alternating polynomial](../../../polynomial.md#alternating-polynomial) of this degree has a unique expansion in alternants $a_{\lambda+\delta}$: a [monomial](../../../polynomial.md#monomial) with repeated exponents has zero coefficient, while each strictly decreasing nonnegative exponent vector is uniquely $\lambda+\delta$ for a partition $\lambda$ of $n$ with at most $m$ parts. Its coefficient at $x^{\lambda+\delta}$ is the coefficient of that alternant. The identities for $c_{\lambda\mu}$ therefore give $a_\delta\phi_\mu=a_{\mu+\delta}$. We have derived the [Weyl character formula](../../../semisimple-lie-algebra.md#weyl-character-formula)

$$
\boxed{\phi_\lambda(\operatorname{diag}(x_1,\ldots,x_m))
=\frac{\det(x_i^{\lambda_j+m-j})}{\det(x_i^{m-j})}.}
$$

For partitions the quotient is the [Schur polynomial](../../../combinatorics.md#schur-polynomial), with removable apparent singularities when [eigenvalues](../../../linear-operator-theory.md#eigenvalue) coincide. For arbitrary dominant integer tuples, multiply the formula for $\nu$ by $(x_1\cdots x_m)^{-k}$; this shifts every numerator exponent by $-k$ and yields the same boxed formula. The variables must then be nonzero. The expression also shows independence of the shift used to define the [determinant twist](../../../lie-theory.md#determinant-twist). Equality of [characters](../../../representation-theory.md#character-of-a-representation) identifies these [irreducible modules](../../../module-theory.md#irreducible-module): the group-algebra image on a [direct sum](../../../vector-space.md#direct-sum) of two irreducibles is finite-dimensional and semisimple, and its span of group operators detects the traces on every simple block.

Finally, the [character](../../../representation-theory.md#character-of-a-representation) of a [dual representation](../../../representation-theory.md#dual-representation) evaluates the original [character](../../../representation-theory.md#character-of-a-representation) at $x_i^{-1}$. Reverse the numerator's columns after making this substitution. The exponents become $-\lambda_{m+1-j}+1-j$. Factoring $(x_1\cdots x_m)^{-(m-1)}$ converts these into $\mu_j+m-j$ for $\mu_j=-\lambda_{m+1-j}$. The denominator undergoes the identical column reversal and factor, so both signs and factors cancel. Hence $\phi_\lambda(x^{-1})=\phi_\mu(x)$, and

$$
\boxed{D_\lambda(V)^*\cong D_{(-\lambda_m,-\lambda_{m-1},\ldots,-\lambda_1)}(V).}
$$

This tuple is again weakly decreasing, so it is precisely the required dominant label.

## 5

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [coordinate ring](../../../algebraic-geometry.md#coordinate-ring) is $\mathbb C[W]=\operatorname{Sym}(W^*)$. The induced action is contragredient on functions:

$$
(g\cdot p)(w)=p(\rho(g^{-1})w).
$$

It is a [group action](../../../group-theory.md#group-action) by degree-preserving algebra automorphisms, extending the dual action on linear [polynomial functions](../../../polynomial.md#polynomial-function). Its [polynomial invariant ring](../../../representation-theory.md#polynomial-invariant-ring) is

$$
\mathbb C[W]^G=\{p\in\mathbb C[W]:g\cdot p=p\text{ for every }g\in G\}.
$$

For a monic [polynomial](../../../polynomial.md) $f(t)=\prod_{i=1}^d(t-r_i)$, its [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) is $\operatorname{disc}(f)=\prod_{i<j}(r_i-r_j)^2$. This is symmetric in the roots, hence [polynomial](../../../polynomial.md) in the coefficients, and is zero exactly when a root is repeated.

For the [alternating group](../../../finite-group-theory.md#alternating-group) action, let $e_1,\ldots,e_n$ be the [elementary symmetric polynomials](../../../polynomial.md#elementary-symmetric-polynomial) and put $\Delta=\prod_{i<j}(X_i-X_j)$. If $p$ is $A_n$-invariant and $\tau$ is any [transposition](../../../combinatorics.md#transposition-permutation), decompose

$$
p=p_++p_-,\qquad p_+=\frac{p+\tau p}{2},\quad p_-=\frac{p-\tau p}{2}.
$$

Normality and index two of $A_n$ show that $p_+$ is symmetric and $p_-$ transforms by the sign [character](../../../representation-theory.md#character-of-a-representation) of $S_n$. Any [alternating polynomial](../../../polynomial.md#alternating-polynomial) vanishes when $X_i=X_j$, so every $X_i-X_j$ divides it. These pairwise nonassociate prime factors have product $\Delta$, so $p_-=\Delta q$ with $q$ symmetric. The [Fundamental theorem of symmetric polynomials](../../../polynomial.md#fundamental-theorem-of-symmetric-polynomials) yields

$$
\mathbb C[X_1,\ldots,X_n]^{A_n}
=\mathbb C[e_1,\ldots,e_n]\oplus\Delta\mathbb C[e_1,\ldots,e_n].
$$

The sum is direct, since a [polynomial](../../../polynomial.md) that is both symmetric and alternating is zero in [characteristic zero](../../../algebra.md#characteristic-zero). Also $\Delta^2=D(e_1,\ldots,e_n)$, where $D$ is the discriminant [polynomial](../../../polynomial.md) of

$$
t^n-e_1t^{n-1}+e_2t^{n-2}-\cdots+(-1)^ne_n.
$$

Thus, more precisely than the requested quotient assertion,

$$
\boxed{\mathbb C[X_1,\ldots,X_n]^{A_n}
\cong\mathbb C[T_1,\ldots,T_n,Z]/(Z^2-D(T_1,\ldots,T_n)).}
$$

Surjectivity follows from the direct-sum expression. Divide any putative kernel element by the monic quadratic in $Z$; its remainder is $a(T)+Zb(T)$. The [direct sum](../../../vector-space.md#direct-sum) forces $a(e)=b(e)=0$, and [algebraic independence](../../../algebra.md#algebraic-independence) of the $e_i$ gives $a=b=0$. Hence the displayed relation is the entire kernel. The argument also covers $n=2$, where $A_2$ is trivial.

Now let $G$ be finite with no nontrivial [linear characters](../../../representation-theory.md#linear-character), and write $R=\mathbb C[W]$, $S=R^G$. The [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $R$ is a [unique factorization domain](../../../algebra.md#unique-factorization-domain). Factor a nonzero invariant $f$ in $R$; invariance permutes the associate classes of its irreducible factors and makes their exponents constant on each orbit. For an orbit $\mathcal O$, choose representatives and form its [orbit product of polynomial factors](../../../representation-theory.md#orbit-product-of-polynomial-factors)

$$
q_{\mathcal O}=\prod_{p\in\mathcal O}p.
$$

For every $g$, $g\cdot q_{\mathcal O}=\theta(g)q_{\mathcal O}$ for a nonzero scalar $\theta(g)$. Applying two group elements proves that $\theta:G\to\mathbb C^\times$ is a homomorphism. The hypothesis forces $\theta=1$, so $q_{\mathcal O}\in S$.

This orbit product is prime in $S$. If it divides $ab$ with $a,b\in S$, one factor $p\in\mathcal O$ divides $a$ or $b$ in $R$. Invariance of that chosen [polynomial](../../../polynomial.md) makes every factor in the orbit divide it. Their product therefore divides it in $R$, and the quotient is invariant because numerator and denominator are invariant and cancellation is valid in the [integral domain](../../../commutative-algebra.md#integral-domain) $R$. Thus $q_{\mathcal O}$ divides $a$ or $b$ in $S$. Every nonzero $f\in S$ is a scalar times a product of these prime orbit products, and the only units of $S$ are nonzero constants, as they are units in $R$. Therefore **$\mathbb C[W]^G$ is a [unique factorization domain](../../../algebra.md#unique-factorization-domain)**. This gives a direct proof, without assuming a divisor-class-group theorem.

For a failure in [characteristic zero](../../../algebra.md#characteristic-zero), let the [cyclic group](../../../group.md#cyclic-group) of order two act on $\mathbb C^2$ by $-I$. Its coordinate invariants are

$$
S=\mathbb C[X^2,XY,Y^2]
\cong\mathbb C[a,b,c]/(ac-b^2).
$$

Every invariant [monomial](../../../polynomial.md#monomial) has even total degree: its exponents are either both even, or both odd, giving the indicated generators. Reducing powers of $b$ to at most one shows that $ac-b^2$ is the only relation, since $a^ic^j$ and $ba^ic^j$ map to distinct [monomials](../../../polynomial.md#monomial). The three quadratic invariants are irreducible in $S$: each nonconstant invariant has degree at least two, so a product of two nonunits has degree at least four. They are pairwise nonassociate, but

$$
\boxed{X^2Y^2=(X^2)(Y^2)=(XY)^2}
$$

gives two different irreducible factorizations. Hence **this invariant ring is not a [unique factorization domain](../../../algebra.md#unique-factorization-domain)**. The nontrivial sign [character](../../../representation-theory.md#character-of-a-representation) is precisely the kind of [character](../../../representation-theory.md#character-of-a-representation) excluded in the preceding theorem.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
