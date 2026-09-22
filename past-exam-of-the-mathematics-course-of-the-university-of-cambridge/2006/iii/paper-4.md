# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper4.pdf)

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
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [representation](../../../representation-theory.md#group-representation) over $F$ is a homomorphism $G\to\operatorname{GL}(V)$ on a [finite-dimensional vector space](../../../vector-space.md#finite-dimensional-vector-space). It is [irreducible](../../../representation-theory.md#irreducible-representation) if it has no nonzero proper [invariant subspace](../../../representation-theory.md#invariant-subspace), and has [absolute irreducibility of a group representation](../../../representation-theory.md#absolute-irreducibility-of-a-group-representation) if it remains [irreducible](../../../representation-theory.md#irreducible-representation) after every [field extension](../../../algebra.md#field-extension). A [representation over the rational numbers](../../../representation-theory.md#representation-over-the-rational-numbers) is one over $\mathbb Q$; an [ordinary character](../../../representation-theory.md#ordinary-character) is the [trace](../../../linear-algebra.md#matrix-trace) of a characteristic-zero [representation](../../../representation-theory.md#group-representation).

A [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) $n$ is a finite weakly decreasing sequence $\lambda=(\lambda_1,\lambda_2,\ldots)$ of positive integers of sum $n$, extended by zero parts when convenient. Its [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram) has $\lambda_i$ cells in row $i$; its [conjugate partition](../../../representation-theory-of-the-symmetric-group.md#conjugate-partition) $\lambda'$ has $\lambda'_j$ cells in column $j$. [Conjugacy classes](../../../group-theory.md#conjugacy-class) of $S_n$ are indexed by cycle lengths, hence by [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). The number of ordinary [irreducible characters](../../../representation-theory.md#irreducible-character) equals the number of [conjugacy classes](../../../group-theory.md#conjugacy-class); we now construct that many mutually distinct [representations over the rational numbers](../../../representation-theory.md#representation-over-the-rational-numbers).

A [Young tableau](../../../representation-theory-of-the-symmetric-group.md#young-tableau) $t$ of shape $\lambda$ bijectively labels its cells by $1,\ldots,n$. Its [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) $\{t\}$ remembers the set of labels in each distinguished row, not their order. The [Young permutation module](../../../representation-theory-of-the-symmetric-group.md#young-permutation-module) $M_F^\lambda$ is the [vector space](../../../vector-space.md) on these [tabloids](../../../representation-theory-of-the-symmetric-group.md#tabloid), with $S_n$ acting by relabeling. Its [tabloid bilinear form](../../../representation-theory-of-the-symmetric-group.md#tabloid-bilinear-form) makes the [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) basis orthonormal. Let $C_t$ be the subgroup permuting labels within each column and put

$$
\kappa_t=\sum_{g\in C_t}\operatorname{sgn}(g)g,\qquad e_t=\kappa_t\{t\},\qquad S_F^\lambda=\operatorname{span}_F\{e_t:t\text{ has shape }\lambda\}.
$$

Thus $e_t$ is a [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) and $S_F^\lambda$ is a [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module). Relabeling takes $e_t$ to $e_{gt}$, so any [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) generates the [module](../../../module-theory.md#module-mathematics). It is nonzero over every [field](../../../algebra.md#field): the coefficient of $\{t\}$ in $e_t$ is one, since the [row and column stabilizers of a Young tableau](../../../representation-theory-of-the-symmetric-group.md#row-and-column-stabilizers-of-a-young-tableau) intersect trivially.

Here is the elementary identity behind irreducibility. If a row of a [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) contains two entries from one column of $t$, their [transposition](../../../combinatorics.md#transposition-permutation) pairs and cancels the terms in $\kappa_t$, including in [characteristic](../../../algebra.md#characteristic-of-a-field) two. Otherwise, for a [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) of the same shape, its rows can be matched to those of $t$ by a column [permutation](../../../combinatorics.md#permutation), and $\kappa_t\{u\}=\pm e_t$. Looking at the coefficient of $\{t\}$ gives, for every $v\in M_F^\lambda$,

$$
\kappa_tv=\langle v,e_t\rangle e_t.
$$

Consequently a [submodule](../../../module-theory.md#submodule) $U$ of $M_F^\lambda$ either contains $S_F^\lambda$, if one of these pairings is nonzero, or lies in $(S_F^\lambda)^\perp$. This proves the [James submodule theorem](../../../representation-theory-of-the-symmetric-group.md#james-submodule-theorem) used below.

Over $\mathbb Q$, the restricted form on $S_\mathbb Q^\lambda$ is positive definite, so its [Gram determinant](../../../linear-algebra.md#gram-determinant) in a rational basis is nonzero. Extending scalars to any characteristic-zero [field](../../../algebra.md#field) preserves that nonzero [determinant](../../../linear-algebra.md#determinant) and hence keeps the restricted form a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form). The [James submodule theorem](../../../representation-theory-of-the-symmetric-group.md#james-submodule-theorem) applied to a [submodule](../../../module-theory.md#submodule) of $S^\lambda$ now forces it to be zero or the whole [module](../../../module-theory.md#module-mathematics). Therefore **$S_\mathbb Q^\lambda$ is absolutely [irreducible](../../../representation-theory.md#irreducible-representation)**, not merely [irreducible](../../../representation-theory.md#irreducible-representation) over $\mathbb Q$.

To distinguish shapes, the cancellation argument above works for a $\mu$-tabloid too. If $\kappa_t\{u\}\ne0$, its first $r$ rows contain at most $\min(r,\lambda'_j)$ entries from column $j$, so

$$
\sum_{i\le r}\mu_i\le\sum_j\min(r,\lambda'_j)=\sum_{i\le r}\lambda_i.
$$

Thus $\lambda$ dominates $\mu$. The operator $\kappa_t$ acts nontrivially on $S^\lambda$ because the restricted form is a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form). An isomorphism $S^\lambda\cong S^\mu$ would therefore imply $\lambda\unrhd\mu$, and reversing the roles gives equality of the [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). Counting [conjugacy classes](../../../group-theory.md#conjugacy-class) proves exhaustion. All matrices in a rational [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) basis have rational entries, giving the requested [representations over the rational numbers](../../../representation-theory.md#representation-over-the-rational-numbers).

For positive [characteristic](../../../algebra.md#characteristic-of-a-field) $p$, call a [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) a [regular partition](../../../representation-theory-of-the-symmetric-group.md#regular-partition) if no part is repeated $p$ or more times. Define

$$
R_F^\lambda=S_F^\lambda\cap(S_F^\lambda)^\perp,\qquad D_F^\lambda=S_F^\lambda/R_F^\lambda.
$$

The [James submodule theorem](../../../representation-theory-of-the-symmetric-group.md#james-submodule-theorem) shows that every proper [submodule](../../../module-theory.md#submodule) of $S_F^\lambda$ lies in $R_F^\lambda$. Whenever the restricted form is nonzero, $R_F^\lambda$ is proper and its quotient is simple.

We verify exactly when this happens. Let $m_j$ be the number of rows of length $j$. In the integral pairing $\langle e_s,e_t\rangle$, common [tabloids](../../../representation-theory-of-the-symmetric-group.md#tabloid) are acted on freely by [permutations](../../../combinatorics.md#permutation) of equal-length rows. Such a row [permutation](../../../combinatorics.md#permutation) has sign $\operatorname{sgn}(\pi)^j$ in both [polytabloids](../../../representation-theory-of-the-symmetric-group.md#polytabloid), so its contribution to the product of coefficients is unchanged. Each orbit has size $\prod_jm_j!$. Thus that integer divides every pairing. On the other hand, reverse each row of $t$ to obtain $t^*$. A [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) common to $e_t$ and $e_{t^*}$ can only interchange entries between rows of equal length. There are $m_j!$ independent choices in each of their $j$ columns, and the two signs agree. Hence

$$
\langle e_t,e_{t^*}\rangle=\prod_j(m_j!)^j.
$$

These two products have exactly the same prime divisors. All pairings vanish modulo $p$ precisely when some $m_j\ge p$. Therefore $D_F^\lambda\ne0$ exactly for $p$-regular $\lambda$.

For such a shape, the displayed pairing gives $\kappa_te_{t^*}=h e_t$ with $h\ne0$, and $e_t$ has nonzero image in $D^\lambda$. If $D^\lambda\cong D^\mu$, the same operator must act nontrivially on a quotient of $M^\mu$, forcing $\lambda\unrhd\mu$ by the cancellation argument. Interchanging the shapes proves $\lambda=\mu$.

For exhaustion over an [algebraic closure](../../../algebra.md#algebraic-closure) use the general [Brauer character basis theorem](../../../representation-theory.md#brauer-character-basis-theorem): the number of [simple modules](../../../module-theory.md#irreducible-module) over an algebraically closed [field](../../../algebra.md#field) of [characteristic](../../../algebra.md#characteristic-of-a-field) $p$ is the number of [conjugacy classes](../../../group-theory.md#conjugacy-class) of elements of order prime to $p$. Here these are the cycle [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) with no part divisible by $p$. The generating-function identity

$$
\prod_{j\ge1}(1+t^j+\cdots+t^{(p-1)j})
=\prod_{j\ge1}\frac{1-t^{pj}}{1-t^j}
=\prod_{p\nmid j}(1-t^j)^{-1}
$$

shows that their number equals the number of $p$-regular [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). We have already constructed that many distinct [simple modules](../../../module-theory.md#irreducible-module), so they exhaust all simples. The form, its radical and its quotient commute with [field extension](../../../algebra.md#field-extension), and the same simplicity proof holds after every extension. The [modules](../../../module-theory.md#module-mathematics) defined over the [prime field](../../../algebra.md#prime-field) are therefore absolutely [irreducible](../../../representation-theory.md#irreducible-representation) and form a split complete list over arbitrary $F$ as well. In summary,

$$
\boxed{\operatorname{Irr}(FS_n)=\{D_F^\lambda:\lambda\vdash n\text{ is }p\text{-regular}\}.}
$$

For [characteristic](../../../algebra.md#characteristic-of-a-field) zero the list is instead all $S_F^\lambda$. In positive [characteristic](../../../algebra.md#characteristic-of-a-field) a [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module) itself need not be [irreducible](../../../representation-theory.md#irreducible-representation); the radical quotient is essential.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [standard Young tableau](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) is a filling by $1,\ldots,n$, each used once, increasing along rows and down columns. A [semistandard Young tableau](../../../representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) is a filling by positive integers, weakly increasing along rows and strictly increasing down columns. Its content $\mu$ means that the entry $i$ occurs $\mu_i$ times. The [Kostka number](../../../representation-theory-of-the-symmetric-group.md#kostka-number) $K_{\lambda\mu}$ counts [semistandard tableaux](../../../representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) of shape $\lambda$ and content $\mu$. The [dominance order on partitions](../../../representation-theory-of-the-symmetric-group.md#dominance-order-on-partitions) is

$$
\lambda\unrhd\mu\quad\Longleftrightarrow\quad
\sum_{i\le r}\lambda_i\ge\sum_{i\le r}\mu_i\quad\text{for every }r.
$$

Strict dominance adds $\lambda\ne\mu$. The [Young permutation module](../../../representation-theory-of-the-symmetric-group.md#young-permutation-module) is $M^\mu=F\{\mu\text{-tabloids}\}=\operatorname{Ind}_{S_{\mu_1}\times S_{\mu_2}\times\cdots}^{S_n}\mathbf1$.

Let $D^\lambda$ be a [composition factor](../../../module-theory.md#composition-factor) of $M^\mu$. It occurs as a [submodule](../../../module-theory.md#submodule) of some quotient $M^\mu/U$, so its defining surjection $S^\lambda\to D^\lambda$ gives a nonzero map $\theta:S^\lambda\to M^\mu/U$. With $t^*$ the row reversal from Question 1, $\kappa_te_{t^*}=he_t$, $h\ne0$, and the cyclic generator cannot have zero image under $\theta$. Therefore $\kappa_t$ acts nontrivially on $M^\mu/U$, and hence on $M^\mu$. The column-cancellation argument proves $\lambda\unrhd\mu$.

When $\lambda=\mu$, the identity $\kappa_tv=\langle v,e_t\rangle e_t$ shows more: the image of every nonzero map $S^\mu\to M^\mu/U$ is $(S^\mu+U)/U$. In a [composition series](../../../finite-group-theory.md#composition-series) of $M^\mu$, a factor isomorphic to $D^\mu$ can thus occur only at the step where $S^\mu$ first becomes contained in the series term. Once contained, every later such map would have zero image. Since the quotient $D^\mu$ of the [submodule](../../../module-theory.md#submodule) $S^\mu$ certainly occurs when $\mu$ is regular, it occurs exactly once. If $\mu$ is not regular, no simple is indexed by $\mu$. Consequently **every other factor has a strictly dominating regular label**. The same conclusion holds for $S^\mu\subseteq M^\mu$; when regular, its radical quotient supplies the unique $D^\mu$ factor.

The integral standard-basis theorem says that the standard [polytabloids](../../../representation-theory-of-the-symmetric-group.md#polytabloid) form a basis over every [field](../../../algebra.md#field). Thus $\dim S_F^\mu=f^\mu$ is independent of [characteristic](../../../algebra.md#characteristic-of-a-field). In the [decomposition matrix](../../../representation-theory.md#decomposition-matrix-modular-representation-theory), rows are indexed by all ordinary shapes $\mu$ and columns by regular shapes $\lambda$:

$$
d_{\mu\lambda}=[S_F^\mu:D_F^\lambda],\qquad
\boxed{d_{\mu\lambda}=0\text{ unless }\lambda\unrhd\mu,\quad d_{\lambda\lambda}=1.}
$$

Ordering shapes by a common linear extension of dominance gives a rectangular triangular matrix, whose regular-row square submatrix is unitriangular. The standard basis also gives $f^\mu=\sum_\lambda d_{\mu\lambda}\dim D^\lambda$.

[Young's rule](../../../representation-theory-of-the-symmetric-group.md#young-s-rule) states that $M^\mu$ has a [Specht filtration](../../../representation-theory-of-the-symmetric-group.md#specht-filtration) with $K_{\lambda\mu}$ copies of $S^\lambda$. In [characteristic](../../../algebra.md#characteristic-of-a-field) zero this is a direct-sum decomposition into [irreducibles](../../../representation-theory.md#irreducible-representation). In positive [characteristic](../../../algebra.md#characteristic-of-a-field) these are Specht factors, not simple factors; rather

$$
[M^\mu:D^\alpha]=\sum_\lambda K_{\lambda\mu}d_{\lambda\alpha}.
$$

For content $\lambda$ and shape $\lambda$, entries at most $r$ must lie in the first $r$ rows, because columns strictly increase. Their number is exactly the size of those rows, so successive rows must be filled by their row number. Hence $K_{\lambda\lambda}=1$. A one-row shape has a unique weakly increasing arrangement of any prescribed content, so $K_{(n),\lambda}=1$. Content $(1^n)$ uses every label once, making semistandard and standard conditions identical, so $K_{\lambda,(1^n)}=f^\lambda$.

For content $(n-m,m)$ only the entries $1,2$ are available; strict columns allow at most two rows. In shape $(n-j,j)$ every bottom entry is $2$ and every entry above it is $1$. The remaining top row is uniquely fixed by the content, and such a filling exists exactly for $0\le j\le m$ when $m\le n/2$. [Young's rule](../../../representation-theory-of-the-symmetric-group.md#young-s-rule) therefore gives

$$
\boxed{[n-m][m]=\sum_{j=0}^m[n-j,j],}
$$

where multiplication denotes induction from the indicated [Young subgroup](../../../representation-theory-of-the-symmetric-group.md#young-subgroup), not pointwise multiplication of [characters](../../../representation-theory.md#character-of-a-representation) of the same group. The [dimension](../../../vector-space.md#dimension-vector-space) of this [permutation module](../../../representation-theory.md#permutation-module) is $\binom nm$. Subtracting the analogous identity with $m-1$ yields

$$
\boxed{\dim S^{(n-m,m)}=\binom nm-\binom n{m-1}
=\frac{n-2m+1}{n-m+1}\binom nm,}
$$

with $\binom n{-1}=0$ for $m=0$. This [dimension](../../../vector-space.md#dimension-vector-space) holds over every [field](../../../algebra.md#field).

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $n\ge2$, a [cycle type](../../../finite-group-theory.md#cycle-type) $\alpha\vdash n$ lies in $A_n$ exactly when $n-\ell(\alpha)$ is even. Its $S_n$ [conjugacy class](../../../group-theory.md#conjugacy-class) is either one $A_n$ class or two equal-sized classes. Splitting occurs exactly when its [centralizer](../../../group-theory.md#centralizer) in $S_n$ contains no odd [permutation](../../../combinatorics.md#permutation). An even-length cycle is itself odd; two equal odd-length cycles can be interchanged by an odd [permutation](../../../combinatorics.md#permutation). Conversely, for distinct odd cycle lengths the [centralizer](../../../group-theory.md#centralizer) is a product of cyclic groups of odd order, all contained in $A_n$. Thus **the classes that split are exactly the [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) into distinct odd parts**. Repeated fixed points count as repeated parts of length one.

For $n=1$ the group is trivial, with its single [trivial representation](../../../representation-theory.md#trivial-representation). Assume $n\ge2$ for the index-two argument that follows. For ordinary [representations](../../../representation-theory.md#group-representation) work over $\mathbb C$. Tensoring $S^\lambda$ by the [sign representation](../../../representation-theory-of-the-symmetric-group.md#sign-representation) gives $S^{\lambda'}$. The index-two restriction identity, obtained by [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity), is

$$
\left\langle\operatorname{Res}_{A_n}\chi^\lambda,\operatorname{Res}_{A_n}\chi^\mu\right\rangle
=\delta_{\lambda\mu}+\delta_{\lambda'\mu}.
$$

If $\lambda\ne\lambda'$, restriction is [irreducible](../../../representation-theory.md#irreducible-representation), and the conjugate pair gives the same [irreducible](../../../representation-theory.md#irreducible-representation). If $\lambda=\lambda'$, the norm is two, so restriction is the sum of two distinct [irreducibles](../../../representation-theory.md#irreducible-representation). An odd [permutation](../../../combinatorics.md#permutation) interchanges them, so both have degree $f^\lambda/2$. Every [irreducible](../../../representation-theory.md#irreducible-representation) of $A_n$ occurs in some such restriction: induce it to $S_n$ and choose an [irreducible](../../../representation-theory.md#irreducible-representation) constituent, then apply reciprocity. The displayed [inner product](../../../linear-algebra.md#inner-product) distinguishes all the listed constituents. Hence

$$
\boxed{\operatorname{Irr}(A_n)=\{V^{\{\lambda,\lambda'\}}:\lambda\ne\lambda'\}\ \cup\ \{V^{\lambda,+},V^{\lambda,-}:\lambda=\lambda'\}.}
$$

The first family has degree $f^\lambda$, the second degree $f^\lambda/2$. A choice of labels for the two split classes and constituents fixes the otherwise interchangeable signs.

The one-dimensional [representations](../../../representation-theory.md#group-representation) are [characters](../../../representation-theory.md#character-of-a-representation) of the [abelianization](../../../group-theory.md#abelianization). For $n\ge5$, simplicity and noncommutativity of $A_n$ make its [abelianization](../../../group-theory.md#abelianization) trivial. For $n=4$, its [commutator subgroup](../../../group-theory.md#commutator-subgroup) is the [Klein four-group](../../../finite-group-theory.md#klein-four-group) and its [abelianization](../../../group-theory.md#abelianization) is $C_3$, giving the three [characters](../../../representation-theory.md#character-of-a-representation) obtained by sending a quotient generator to $1,\omega,\omega^2$. For $n=3$, $A_3=C_3$ has the same three [characters](../../../representation-theory.md#character-of-a-representation); for $n=1,2$ the group is trivial and has just one. The two additional [linear characters](../../../representation-theory.md#linear-character) at $n=4$ are the split constituents of shape $(2,2)$; at $n=3$ they come from $(2,1)$.

Here is a [dimension](../../../vector-space.md#dimension-vector-space) argument that also proves the asserted uniqueness without assuming a classification of small [character](../../../representation-theory.md#character-of-a-representation) degrees. Write $f^\lambda$ for the number of [standard tableaux](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau). Removing the cell containing the largest label gives

$$
f^\lambda=\sum_{\mu\in\lambda^-}f^\mu.
$$

[Hook lengths](../../../representation-theory-of-the-symmetric-group.md#hook-length), or direct [Young tableau](../../../representation-theory-of-the-symmetric-group.md#young-tableau) counting, give the following small cases: for $S_5,S_6$ every non-linear degree is at least $4,5$, respectively. Among non-self-conjugate shapes excluding the row, column and standard pair, the minimum degree at $n=5,6,7$ is respectively $5,5,14$. The self-conjugate shapes at these sizes have half-degrees $3,8,10$, respectively, from $(3,1^2),(3,2,1),(4,1^3)$.

Inductively, for every $n\ge7$, a shape other than the row, column or standard pair has all its one-cell predecessors non-linear. If it has at least two removable corners, each predecessor has degree at least $n-2$, so its degree is at least $2(n-2)$. If it has only one corner, it is a nontrivial rectangle $(a^b)$. Remove that corner and then either of the two corners of $(a^{b-1},a-1)$. For $n\ge8$ these two size-$n-2$ shapes are non-linear, so its degree is at least $2(n-3)$. At $n=7$ there is no nontrivial rectangle. Together with the size-5 and size-6 checks this proves by induction that the standard pair is the only pair of shapes of degree $n-1$ for $n\ge7$, and that every other non-linear degree is larger.

We must additionally exclude a self-conjugate shape of degree $2(n-1)$, since its restriction splits. For $n\ge8$, if such a shape has at least three corners, the preceding lower bound gives $f^\lambda\ge3(n-2)>2(n-1)$. With two corners, its predecessors are a conjugate pair and are not standard shapes; the bounds just proved give $f^\lambda\ge4(n-4)>2(n-1)$. With one corner it is a square $(a^a)$. For $a\ge4$, the two size-$n-2$ predecessors obtained after two removals are nonstandard, giving $f^\lambda\ge4(n-5)>2(n-1)$. The remaining square $(3^3)$ has degree $42>16$ by the [hook-length formula](../../../representation-theory-of-the-symmetric-group.md#hook-length-formula). The size-7 self-conjugate case has degree $20>12$. This excludes both smaller split degrees and equality with the standard degree.

It follows that the lowest non-linear ordinary degree is **$3$ for $A_4$ and $n-1$ for every $n\ge6$**. For $A_1,A_2,A_3$ no non-linear [irreducible](../../../representation-theory.md#irreducible-representation) exists. The excluded case $A_5$ has lowest degree $3$, although its standard degree-$4$ [representation](../../../representation-theory.md#group-representation) is unique. At $A_6$ there are two degree-$5$ [irreducibles](../../../representation-theory.md#irreducible-representation), from the standard conjugate pair and the pair $(3,3),(2,2,2)$.

Finally, for every $n\ge7$ the preceding proof gives a unique degree-$n-1$ [irreducible](../../../representation-theory.md#irreducible-representation), namely the restriction of $S^{(n-1,1)}$. The small cases $n=4,5$ have unique degree $3,4$, respectively, and $A_2$ has its unique trivial degree-$1$ [representation](../../../representation-theory.md#group-representation). These prove exactly the requested uniqueness range; the omitted cases $n=3,6$ genuinely fail.

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use the [pair of partitions for a generalized Specht module](../../../representation-theory-of-the-symmetric-group.md#pair-of-partitions-for-a-generalized-specht-module) convention appropriate to [generalized Specht modules](../../../representation-theory-of-the-symmetric-group.md#generalized-specht-module). Put $a=\mu^\sharp$ and $b=\mu$. Here $b=(b_1,b_2,\ldots)$ is a sequence of nonnegative row lengths of total $n$, and $a$ is a proper [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) satisfying $0\le a_i\le b_i$ and $a_{i+1}\le a_i$. The row-length sequence $b$ is allowed to be a composition; it need not decrease. The first $a_i$ cells of row $i$ are marked. This construction is not an arbitrary pair of unrelated [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) and is not simply a skew diagram $b/a$.

A word has type $b$ if it contains $b_i$ occurrences of $i$. Read it from left to right. Every occurrence of $1$ is good; an occurrence of $i+1$ is good exactly when there have so far been more good occurrences of $i$ than good occurrences of $i+1$. Otherwise it is bad. Define

$$
s(a,b)=\{w:\operatorname{type}(w)=b,\ \#\text{good occurrences of }i\ge a_i\text{ for every }i\}.
$$

Thus $s(0,b)$ is the set of all words of type $b$, and $s(b,b)$ consists of [lattice words](../../../representation-theory-of-the-symmetric-group.md#lattice-word) when $b$ is a proper [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). Marking the whole first row makes no difference because every $1$ is good.

For a [Young tableau](../../../representation-theory-of-the-symmetric-group.md#young-tableau) $T$ with row lengths $b$, let $C_T^a$ permute labels within each column of its marked subdiagram, fixing all unmarked labels. Its generalized [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) and [generalized Specht module](../../../representation-theory-of-the-symmetric-group.md#generalized-specht-module) are

$$
\boxed{e_T^{a,b}=\sum_{g\in C_T^a}\operatorname{sgn}(g)\{gT\},\qquad
S^{a,b}=\operatorname{span}_F\{e_T^{a,b}\}\subseteq M^b.}
$$

In particular $S^{0,b}=M^b$ and $S^{b,b}=S^b$. The [Young tableau](../../../representation-theory-of-the-symmetric-group.md#young-tableau) shape in this definition must be the row sequence $b$.

We give the filtration argument, keeping its combinatorial and module-theoretic steps separate. Normalize $a_1=b_1$, and if $a\ne b$ choose the first row $c>1$ with $a_c<b_c$. Then $a_{c-1}=b_{c-1}$. Define $A_c(a,b)=(a+e_c,b)$ if $a_{c-1}>a_c$; otherwise the add branch is empty. Define $R_c(a,b)=(a,b')$ by moving the unmarked tail of row $c$ into row $c-1$:

$$
b'_c=a_c,\qquad b'_{c-1}=b_{c-1}+b_c-a_c,
$$

with other row lengths unchanged. Re-normalize the first marked row if necessary. The Basic Combinatorial Theorem supplies the counting and formal-character recursions

$$
|s(a,b)|=|s(A_c(a,b))|+|s(R_c(a,b))|,\qquad
[0]^{[a,b]}=[0]^{[A_c(a,b)]}+[0]^{[R_c(a,b)]}.
$$

At a terminal pair $(\nu,\nu)$ the formal term is $[\nu]$. Thus the second recursion specifies the Specht multiplicities by the terminal leaves, with repeated leaves counted separately.

Define an equivariant map $\psi:M^b\to M^{b'}$ by summing, on each [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid), over all choices of the $a_c$ labels retained in row $c$, moving the remaining labels to row $c-1$. Column cancellation gives

$$
\psi(S^{a,b})=S^{R_c(a,b)},\qquad
S^{A_c(a,b)}\subseteq S^{a,b}\cap\ker\psi.
$$

For the first identity, terms that put two marked labels of one column in the raised row cancel in pairs; the surviving marked antisymmetrizer is the one for the raised pair, and every target generator has a preimage. For the second, the extra marked cell makes such a collision unavoidable, so the sum vanishes. Also antisymmetrizing the extra cell expresses its generator as a sum of old generators, proving containment in $S^{a,b}$.

There is a characteristic-independent lower bound $\dim S^{a,b}\ge|s(a,b)|$. Given a word in $s(a,b)$, place the label $j$ in its letter's row: good occurrences fill that row from the left and bad occurrences fill it from the right. The marked cells form increasing column chains because each good $i+1$ has an earlier unmatched good $i$. Its generalized [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) has the original row-assignment [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) with coefficient one; every other term changes an earlier member of a marked chain. Ordering these row assignments gives a triangular coefficient matrix. The resulting vectors are independent over every [field](../../../algebra.md#field).

Start with $(0,v)$, where equality holds because the [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) basis is indexed by all words of type $v$. Any pair is reached from such a pair by a sequence of add and raise operations: reverse a raise by splitting a raised tail, and reverse an add by unmarking a cell; row by row these recover an entirely unmarked composition. Suppose equality holds at a pair. The map and [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) containment above give

$$
|s(a,b)|=\dim S^{a,b}\ge\dim S^{A_c(a,b)}+\dim S^{R_c(a,b)}
\ge|s(A_c(a,b))|+|s(R_c(a,b))|=|s(a,b)|.
$$

Every inequality is therefore equality. In particular the containment is the whole [kernel](../../../linear-algebra.md#kernel-of-a-linear-map), and

$$
0\longrightarrow S^{A_c(a,b)}\longrightarrow S^{a,b}\longrightarrow S^{R_c(a,b)}\longrightarrow0
$$

is exact. The process terminates because each add marks an extra cell and each raise decreases the total row index of unmarked cells. Induction from the terminal [Specht modules](../../../representation-theory-of-the-symmetric-group.md#specht-module), splicing their filtrations through these exact sequences, proves **a [Specht series](../../../representation-theory-of-the-symmetric-group.md#specht-filtration) with factors precisely $[0]^{[\mu^\sharp,\mu]}$**. No splitting of these sequences in positive [characteristic](../../../algebra.md#characteristic-of-a-field) is asserted.

Applying the same marking, raising and straightening procedure to the two sets of [column antisymmetrizers](../../../representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau) in $(S^\mu\boxtimes S^\lambda)\uparrow^{S_{r+s}}$, where $|\mu|=r$, $|\lambda|=s$, leaves the cells of $\mu$ fixed and records the added cells by their row labels from $\lambda$. The column relations require strict increase down columns, the row relations weak increase along rows, and the [good-letter matching in a tableau word](../../../representation-theory-of-the-symmetric-group.md#good-letter-matching-in-a-tableau-word) test requires a [lattice word](../../../representation-theory-of-the-symmetric-group.md#lattice-word). Thus the surviving terminal multiplicity is the number $c_{\mu\lambda}^\nu$ of [Semistandard Young tableaux](../../../representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) of [skew shape](../../../representation-theory-of-the-symmetric-group.md#skew-young-diagram) of shape $\nu/\mu$ and content $\lambda$ whose word, read right-to-left along successive rows from top to bottom, has at least as many $i$'s as $(i+1)$'s in every prefix. The same triangular leading-tabloid argument identifies each quotient with $S^\nu$. Consequently the [Littlewood–Richardson rule](../../../representation-theory-of-the-symmetric-group.md#littlewood-richardson-rule) is

$$
\boxed{[\mu][\lambda]=\sum_{\nu\vdash r+s}c_{\mu\lambda}^\nu[\nu].}
$$

It describes ordinary [irreducible](../../../representation-theory.md#irreducible-representation) constituents in [characteristic](../../../algebra.md#characteristic-of-a-field) zero and [Specht filtration](../../../representation-theory-of-the-symmetric-group.md#specht-filtration) factors over arbitrary $F$.

For induction by one letter, content $(1)$ permits exactly one added cell and each multiplicity is one. A [Specht series](../../../representation-theory-of-the-symmetric-group.md#specht-filtration) for the requested induced [module](../../../module-theory.md#module-mathematics) has successive quotients, ordered by addable nodes from bottom to top,

$$
\boxed{S^{(4,2,2,1,1)},\quad S^{(4,2,2,2)},\quad S^{(4,3,2,1)},\quad S^{(5,2,2,1)}.}
$$

Equivalently there is $0=N_0\subset N_1\subset N_2\subset N_3\subset N_4=S^{(4,2,2,1)}\uparrow^{S_{10}}$ with these four quotients in order. Their [dimensions](../../../vector-space.md#dimension-vector-space) $567,300,768,525$ sum to $2160=10\cdot216$, the [dimension](../../../vector-space.md#dimension-vector-space) of the induced [module](../../../module-theory.md#module-mathematics).

## 5

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Use the induction product of symmetric-group [characters](../../../representation-theory.md#character-of-a-representation): for $a\ge0$, $[a]$ is the trivial [character](../../../representation-theory.md#character-of-a-representation) of $S_a$, $[0]$ is the unit and $[a]=0$ for $a<0$. Products mean induction of external [tensor products](../../../linear-algebra.md#tensor-product). The determinantal form is

$$
\boxed{[\lambda]=\det\bigl([\lambda_i-i+j]\bigr)_{1\le i,j\le r},}
$$

where $r\ge\ell(\lambda)$. Each [determinant](../../../linear-algebra.md#determinant) term is a virtual [character](../../../representation-theory.md#character-of-a-representation) of $S_n$, because its indices sum to $n$.

Here is a proof. The [Frobenius characteristic map](../../../combinatorics.md#frobenius-characteristic-map) sends $[a]$ to the [complete homogeneous symmetric function](../../../combinatorics.md#complete-homogeneous-symmetric-polynomial) $h_a$, and induction products to multiplication. By [Young's rule](../../../representation-theory-of-the-symmetric-group.md#young-s-rule) its value on $[\lambda]$ is the [Schur function](../../../combinatorics.md#schur-polynomial) $s_\lambda$, the generating function of [semistandard tableaux](../../../representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) of shape $\lambda$. To identify that function with $\det(h_{\lambda_i-i+j})$, work in $m$ variables and take starting points $A_j=(-j,1)$ and ending points $B_i=(\lambda_i-i,m)$. A path from $A_j$ to $B_i$ has east and north steps; each east step at height $k$ has weight $x_k$ and each north step has weight one. Its east-step count is $\lambda_i-i+j$, so its weight sum is $h_{\lambda_i-i+j}$. Expanding the [determinant](../../../linear-algebra.md#determinant) sums signed systems of paths with permuted endpoints. For a system with an intersection, exchange the two tails after the first intersection. This preserves its monomial weight and reverses the endpoint [permutation](../../../combinatorics.md#permutation)'s sign, so all intersecting systems cancel in pairs. Nonintersecting systems necessarily have the identity endpoint [permutation](../../../combinatorics.md#permutation) and correspond precisely to weak rows with strictly increasing columns, namely [semistandard tableaux](../../../representation-theory-of-the-symmetric-group.md#semistandard-young-tableau) of shape $\lambda$. Their signs are positive. This proves $s_\lambda=\det(h_{\lambda_i-i+j})$, the [Jacobi–Trudi identity](../../../combinatorics.md#jacobi-trudi-identity), and injectivity of the [Frobenius characteristic map](../../../combinatorics.md#frobenius-characteristic-map) gives the [character](../../../representation-theory.md#character-of-a-representation) formula above. The path sum may be taken in finitely many variables first and then stabilized, so no infinite formal sum is required in the argument.

A removable [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook), or border strip, of length $k$ is a connected skew diagram $\lambda/\nu$ of $k$ cells with no $2\times2$ square, where removal leaves a [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). Its leg length is the number of occupied rows minus one. The [Murnaghan–Nakayama rule](../../../representation-theory-of-the-symmetric-group.md#murnaghan-nakayama-rule) states

$$
\boxed{\chi^\lambda(k,\rho)=\sum_{\nu:\lambda/\nu\text{ is a }k\text{-rim hook}}
(-1)^{\operatorname{leg}(\lambda/\nu)}\chi^\nu(\rho).}
$$

A proof sketch follows directly from the alternant form of [Schur functions](../../../combinatorics.md#schur-polynomial). Multiply an alternant by $p_k=\sum_jx_j^k$. In each term one alternant exponent increases by $k$. Equal exponents cancel; otherwise reordering the exponents contributes the sign of the number crossed. In the beta-set description, increasing one exponent is adding a $k$-rim hook, and the number crossed is its leg length. Therefore $p_ks_\nu=\sum_\lambda(-1)^{\operatorname{leg}(\lambda/\nu)}s_\lambda$. Taking its adjoint in the [Hall inner product of symmetric functions](../../../combinatorics.md#hall-inner-product-of-symmetric-functions), where [Schur functions](../../../combinatorics.md#schur-polynomial) are orthonormal and [power-sum symmetric polynomials](../../../combinatorics.md#power-sum-symmetric-polynomial) have squared norm $z_\rho$, reads off the value at a $k$-cycle and the remaining [cycle type](../../../finite-group-theory.md#cycle-type). This gives the stated rule and explains its sign.

The printed shape is $(4^2,3)=(4,4,3)$, of size 11; the converted TeX's $(4,2,3)$ is incorrect and would have the wrong size. There are two removable length-5 [rim hooks](../../../representation-theory-of-the-symmetric-group.md#rim-hook). They leave $(3,2,1)$ with leg length 2 and $(4,2)$ with leg length 1. Thus

$$
\chi^{(4,4,3)}(5,4,2)=\chi^{(3,2,1)}(4,2)-\chi^{(4,2)}(4,2).
$$

The staircase $(3,2,1)$ has no removable length-4 [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook), so its term is zero. The unique removable length-4 [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook) of $(4,2)$ leaves $(1,1)$ and has leg length 1. The remaining length-2 [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook) in $(1,1)$ also has leg length 1, giving $\chi^{(4,2)}(4,2)=(-1)(-1)=1$. Hence

$$
\boxed{\chi^{(4,4,3)}(5,4,2)=-1.}
$$

As a separate [determinant](../../../linear-algebra.md#determinant) check, the only term whose row sizes can be unions of cycles of lengths $5,4,2$ is the [transposition](../../../combinatorics.md#transposition-permutation) term with sizes $(4,5,2)$. Its [permutation character](../../../representation-theory.md#permutation-character) has value one and its [determinant](../../../linear-algebra.md#determinant) sign is negative.

Taking $k=1$ in the [Murnaghan–Nakayama rule](../../../representation-theory-of-the-symmetric-group.md#murnaghan-nakayama-rule) removes a single corner and every leg length is zero. Evaluating on a [permutation](../../../combinatorics.md#permutation) fixing the distinguished point therefore gives

$$
\operatorname{Res}^{S_n}_{S_{n-1}}\chi^\lambda=\sum_{\nu\in\lambda^-}\chi^\nu.
$$

This is the [restriction branching rule for a symmetric group](../../../representation-theory-of-the-symmetric-group.md#restriction-branching-rule-for-a-symmetric-group); ordinary [semisimple representation](../../../representation-theory.md#semisimple-representation) theory converts the [character](../../../representation-theory.md#character-of-a-representation) equality into a direct-sum decomposition. [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity) gives the corresponding add-one-cell induction rule.

For a positive prime $p$, the [weight of a partition](../../../representation-theory-of-the-symmetric-group.md#weight-of-a-partition) $\lambda$ at prime modulus $p$, denoted $w$, is the number of length-$p$ [rim hooks](../../../representation-theory-of-the-symmetric-group.md#rim-hook) removed in reaching its [partition core](../../../representation-theory-of-the-symmetric-group.md#core-of-a-partition) $\kappa$, so $n=|\kappa|+pw$. On a prime-modulus [partition abacus](../../../representation-theory-of-the-symmetric-group.md#abacus-of-a-partition) write its [partition quotient](../../../representation-theory-of-the-symmetric-group.md#quotient-of-a-partition) as $(\lambda^{(0)},\ldots,\lambda^{(p-1)})$ and put $w_i=|\lambda^{(i)}|$, with $\sum_iw_i=w$. Removing a length-$p$ [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook) removes one corner from one quotient [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). Complete removal sequences therefore number

$$
N_p(\lambda)=\binom{w}{w_0,\ldots,w_{p-1}}\prod_{i=0}^{p-1}f^{\lambda^{(i)}}
=\frac{w!}{\prod_iH_{\lambda^{(i)}}},
$$

where $H_\alpha$ is the [hook product of a partition](../../../representation-theory-of-the-symmetric-group.md#hook-product-of-a-partition) and $H_\varnothing=1$. Each component's [standard tableaux](../../../representation-theory-of-the-symmetric-group.md#standard-young-tableau) encode its possible removal orders, and the multinomial coefficient interleaves the components.

All these sequences have the same total sign $\varepsilon_p(\lambda)$. To see this, label the beads on each runner in their preserved order. Each slide crosses exactly the beads counted by its rim-hook leg. Its sign is the change in the total order of bead labels, and the product telescopes to the [permutation](../../../combinatorics.md#permutation) from the initial ordering to the final packed-core ordering, independently of the slides chosen. Repeating the [Murnaghan–Nakayama rule](../../../representation-theory-of-the-symmetric-group.md#murnaghan-nakayama-rule) on the $w$ distinguished $p$-cycles gives

$$
\boxed{\chi^\lambda(\pi\rho)=\varepsilon_p(\lambda)N_p(\lambda)\chi^\kappa(\pi).}
$$

Here $\pi$ acts on the complementary $n-pw$ letters; no $p$-regularity hypothesis on $\pi$ is necessary. If its [cycle type](../../../finite-group-theory.md#cycle-type) contains a part divisible by $p$, the [partition core](../../../representation-theory-of-the-symmetric-group.md#core-of-a-partition) [character](../../../representation-theory.md#character-of-a-representation) is zero, since its [partition abacus](../../../representation-theory-of-the-symmetric-group.md#abacus-of-a-partition) admits no hook removal of a length divisible by $p$. For $w=0$ the coefficient and sign are one.

## 6

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For a cell $(i,j)$ in the [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram) of $\lambda$, its [hook of a Young diagram](../../../representation-theory-of-the-symmetric-group.md#hook-of-a-young-diagram) consists of that cell, the cells to its right in row $i$ and the cells below it in column $j$. Its length is

$$
h_{ij}=\lambda_i-j+\lambda'_j-i+1.
$$

A removable [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook) is a connected border strip $\lambda/\mu$ containing no $2\times2$ square, whose removal leaves a [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram). Its leg length is the number of rows it meets minus one. The [hook graph](../../../representation-theory-of-the-symmetric-group.md#hook-graph-of-a-partition) is the [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram) labeled at each cell by $h_{ij}$; here “graph” means this labeled array, not a graph of possible hook-walk moves.

Choose $l\ge\ell(\lambda)$, pad with zeros and form the [beta numbers](../../../representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition)

$$
\boxed{\beta_i=\lambda_i+l-i,\qquad i=1,\ldots,l.}
$$

They are distinct nonnegative integers in decreasing order and recover $\lambda_i=\beta_i-l+i$. For $l=\ell(\lambda)$ they equal the first-column [hook lengths](../../../representation-theory-of-the-symmetric-group.md#hook-length), since $h_{i1}=\lambda_i+l-i$. If $l$ is increased, old [beta numbers](../../../representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition) shift upward by one and a new bead at zero is inserted.

For a prime-modulus [partition abacus](../../../representation-theory-of-the-symmetric-group.md#abacus-of-a-partition) arrange the nonnegative positions in $p$ runners: position $pq+r$ lies at level $q$ on runner $r$, $0\le r<p$. Put beads at the [beta numbers](../../../representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition) and leave the other positions empty. Replacing a bead at $b$ by a bead at a vacant $b-k\ge0$ removes a [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook) of length $k$; its leg length is the number of beads strictly between these positions. This follows by tracing the boundary of the diagram: bead positions record vertical steps and gaps record horizontal steps, and exchanging one bead and gap removes the intervening border strip. In particular a removable $p$-hook is exactly a bead that can slide up one place on its own runner.

The [partition core](../../../representation-theory-of-the-symmetric-group.md#core-of-a-partition) at modulus $p$ is the result of sliding beads up until there are no gaps above any bead on a runner. If runner $r$ initially has $b_r$ beads, its final occupied levels must be $0,1,\ldots,b_r-1$, independently of slide order. Thus its packed [beta set](../../../representation-theory-of-the-symmetric-group.md#beta-set-of-a-partition), and hence its core [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer), is unique. Increasing the number of [beta numbers](../../../representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition) merely re-expresses the same boundary by shifting positions and adding the new initial bead; the packed configuration represents the same [partition of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer). This proves well-definedness both with respect to removal order and to the chosen padding. The number of slides is

$$
w_p(\lambda)=\frac{|\lambda|-|\operatorname{core}_p\lambda|}{p}.
$$

The [partition quotient](../../../representation-theory-of-the-symmetric-group.md#quotient-of-a-partition) components record how far each runner's beads lie above their packed positions, giving the hook-removal interpretation used in Question 5.

A [block of a group algebra](../../../representation-theory.md#block-of-a-group-algebra) in [characteristic](../../../algebra.md#characteristic-of-a-field) $p$ for $FS_n$ is a two-sided ideal $B=FS_ne$ for a [primitive central idempotent](../../../associative-algebra.md#primitive-central-idempotent) $e$, meaning a nonzero [central idempotent](../../../associative-algebra.md#central-idempotent) that is not a sum of two nonzero orthogonal [central idempotents](../../../associative-algebra.md#central-idempotent). The identity is the sum of these block [idempotents](../../../commutative-algebra.md#idempotent) and the [group algebra](../../../associative-algebra.md#group-algebra) is their direct product. An [indecomposable module](../../../module-theory.md#indecomposable-module) $V$ belongs to $B$ when $eV=V$, equivalently every other block [idempotent](../../../commutative-algebra.md#idempotent) acts as zero. Indeed $V=\bigoplus_e eV$; indecomposability makes exactly one summand nonzero.

The [Nakayama block theorem](../../../representation-theory.md#nakayama-block-theorem), historically called the Nakayama Conjecture, states

$$
\boxed{S_F^\lambda\text{ and }S_F^\mu\text{ belong to the same }p\text{-block}
\iff\operatorname{core}_p(\lambda)=\operatorname{core}_p(\mu).}
$$

Equivalently the [ordinary characters](../../../representation-theory.md#ordinary-character) assigned to one modular block have a common [partition core](../../../representation-theory-of-the-symmetric-group.md#core-of-a-partition) at modulus $p$. Its [simple modules](../../../module-theory.md#irreducible-module) are the $D^\lambda$ with regular $\lambda$ having that core. Only cores $\kappa$ for which $n-|\kappa|$ is a nonnegative multiple of $p$ occur. The block weight is $(n-|\kappa|)/p$; a core alone determines the block at this fixed degree.

One route to the proof separates the combinatorial core invariant from the algebraic center invariant. Let $c_r(\lambda)$ be the number of cells of residue $r=j-i\pmod p$. A length-$p$ [rim hook](../../../representation-theory-of-the-symmetric-group.md#rim-hook) has one cell of every residue: along its border strip the contents are consecutive integers. Therefore removal subtracts one from every $c_r$. More precisely, choose the number $l$ of [beta numbers](../../../representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition) divisible by $p$ and write the runner charges as $q_r=b_r-l/p$. Reading the boundary, or adding a cell and checking its two changed beta positions, gives

$$
q_r=c_r-c_{r+1}\qquad(r\bmod p).
$$

The charges determine the packed runners and hence the core. For fixed $n$, two equal cores have the same weight, so their full residue multisets are equal. Conversely equal residue multisets give equal charges and the same core. This establishes

$$
\operatorname{core}_p\lambda=\operatorname{core}_p\mu\iff (c_0(\lambda),\ldots,c_{p-1}(\lambda))=(c_0(\mu),\ldots,c_{p-1}(\mu))
$$

for [partitions of an integer](../../../representation-theory-of-the-symmetric-group.md#partition-of-an-integer) of the same integer. The fixed-degree condition matters.

For the center invariant, use the commuting [Jucys–Murphy elements](../../../representation-theory-of-the-symmetric-group.md#jucys-murphy-element) $J_k=\sum_{i<k}(i\ k)$, with $J_1=0$. In the [Young seminormal form](../../../representation-theory-of-the-symmetric-group.md#young-seminormal-form) basis, $J_k$ has eigenvalue equal to the content of the cell containing $k$. A [symmetric polynomial](../../../polynomial.md#symmetric-polynomial) in them therefore acts on $S^\lambda$ as the same scalar for every [Young tableau](../../../representation-theory-of-the-symmetric-group.md#young-tableau): its value on the multiset of all contents of $\lambda$. The integral Specht lattice makes this a scalar identity before modular reduction, so modulo $p$ these central scalars depend only on the residue multiset, and every [composition factor](../../../module-theory.md#composition-factor) inherits them.

The substantive center theorem used in this proof is that the center of the symmetric-group algebra, integrally and over a [field](../../../algebra.md#field), consists of [symmetric polynomials](../../../polynomial.md#symmetric-polynomial) in the [Jucys–Murphy elements](../../../representation-theory-of-the-symmetric-group.md#jucys-murphy-element). Centrality of elementary [symmetric polynomials](../../../polynomial.md#symmetric-polynomial) follows from

$$
\prod_{k=1}^n(t+J_k)=\sum_{g\in S_n}t^{\#\text{cycles}(g)}g;
$$

the coefficients are central class-sum combinations. The reverse inclusion requires the integral triangular class-sum argument: expand symmetric monomials in the $J_k$ as products of [transpositions](../../../combinatorics.md#transposition-permutation), group the leading terms by reduced [cycle type](../../../finite-group-theory.md#cycle-type), and eliminate these leading [class sums](../../../associative-algebra.md#conjugacy-class-sum) in the resulting unitriangular order. The integral coefficients, with no division by multiples of $p$, are crucial; knowing the center only over $\mathbb Q$ would not prove the modular assertion. This is the central algebraic ingredient of this proof route.

Thus equal residue multisets yield equal [characters](../../../representation-theory.md#character-of-a-representation) of the entire modular center. Different residue multisets are separated already by the coefficients of the central [polynomial](../../../polynomial.md) $\prod_k(t+J_k)$: its scalar on the shape $\lambda$ reduces to $\prod_r(t+r)^{c_r(\lambda)}$, whose unique factorization records the multiplicities exactly, even in [characteristic](../../../algebra.md#characteristic-of-a-field) $p$. In a finite-dimensional split algebra, two [simple modules](../../../module-theory.md#irreducible-module) are in the same block exactly when their central [characters](../../../representation-theory.md#character-of-a-representation) agree: the center of each block is local, while different block [idempotents](../../../commutative-algebra.md#idempotent) separate different blocks. It follows that equal cores give one block and different cores give distinct blocks. This proves both directions rather than just observing that core is constant on known blocks.

Finally, each ordinary Specht lattice has a single reduced central [character](../../../representation-theory.md#character-of-a-representation), so all constituents of its reduction lie in that one block. Question 1 supplies every [simple module](../../../module-theory.md#irreducible-module) and its label; the regular labels therefore identify all the simples in each core block. The constructions use integer coefficients and absolutely [irreducible](../../../representation-theory.md#irreducible-representation) prime-field [modules](../../../module-theory.md#module-mathematics), so the block description descends to the arbitrary characteristic-$p$ [field](../../../algebra.md#field) in the question. This completes the main steps of the block proof without presupposing semisimplicity in positive [characteristic](../../../algebra.md#characteristic-of-a-field).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
