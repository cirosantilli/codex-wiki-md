# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper4.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Use the defining property of the [Frobenius complement](../../../group.md#frobenius-complement): $H\cap H^x=\{1\}$ whenever $x\notin H$. The [induced character](../../../representation-theory.md#induced-character) formula, extended linearly to any [class function](../../../representation-theory.md#class-function), is

$$
\theta^G(g)=\frac1{|H|}\sum_{x\in G:\ x^{-1}gx\in H}\theta(x^{-1}gx).
$$

For $h\in H\setminus\{1\}$, a summand requires $h\in H\cap xHx^{-1}$. The Frobenius intersection property forces $x\in H$. All $|H|$ remaining terms equal $\theta(h)$ since $\theta$ is a [class function](../../../representation-theory.md#class-function) on $H$, so $\theta^G(h)=\theta(h)$. At the identity,

$$
\theta^G(1)=[G:H]\theta(1)=0=\theta(1).
$$

Together these give

$$
\boxed{(\theta^G)_H=\theta.}
$$

The zero identity value is essential: at nonidentity elements the intersection argument already gives the equality, whereas induction multiplies the identity value by the subgroup index.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

We prove closure of $N$ through [character kernels](../../../representation-theory.md#kernel-of-a-character), rather than assuming that a conjugacy-invariant set is a subgroup. Let $\eta\in\operatorname{Irr}(H)\setminus\{1_H\}$, write $d=\eta(1)$, and define the [generalised character](../../../representation-theory.md#virtual-character)

$$
\Psi_\eta=(\eta-d1_H)^G+d1_G.
$$

Here $1_H,1_G$ are the [trivial characters](../../../representation-theory.md#trivial-character). Since $(\eta-d1_H)(1)=0$, part (i) gives $(\Psi_\eta)_H=\eta$ and $\Psi_\eta(1)=d$. Put $\vartheta=\eta-d1_H$. By [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity) and [character orthogonality](../../../representation-theory.md#character-orthogonality),

$$
\langle\vartheta^G,\vartheta^G\rangle_G=\langle\vartheta,(\vartheta^G)_H\rangle_H=\langle\vartheta,\vartheta\rangle_H=1+d^2,\qquad \langle\vartheta^G,1_G\rangle_G=-d.
$$

Consequently

$$
\langle\Psi_\eta,\Psi_\eta\rangle_G=(1+d^2)-2d^2+d^2=1.
$$

To justify the resulting irreducibility, write any [generalised character](../../../representation-theory.md#virtual-character) as an integer combination $\sum_\chi a_\chi\chi$ of [irreducible characters](../../../representation-theory.md#irreducible-character). Its squared norm is $\sum a_\chi^2$, so norm one makes it $\chi$ or $-\chi$ for one irreducible $\chi$. Positive degree rules out the negative sign. Thus $\Psi_\eta$ is an [irreducible character](../../../representation-theory.md#irreducible-character), an instance of the fact that [positive-degree norm-one virtual characters are irreducible](../../../representation-theory.md#positive-degree-norm-one-virtual-characters-are-irreducible).

If $x\in N\setminus\{1\}$, no conjugate of $x$ lies in $H$, so the induction formula gives $\vartheta^G(x)=0$. At $1$ it is also zero. Hence $\Psi_\eta(x)=d$ for all $x\in N$. For a finite-group representation we may choose an invariant positive Hermitian form, making every representing matrix unitary. Its trace equals its dimension only when all its unit-modulus eigenvalues are $1$. Thus the [kernel of a character](../../../representation-theory.md#kernel-of-a-character) is $\{g:\Psi_\eta(g)=\Psi_\eta(1)\}$, and $N\subseteq\ker\Psi_\eta$.

Conversely, if $g\notin N$, then $g$ is conjugate to some $h\in H\setminus\{1\}$. The character of the [regular representation](../../../representation-theory.md#regular-representation) of $H$ is

$$
\rho_H=\sum_{\eta\in\operatorname{Irr}(H)}\eta(1)\eta,\qquad \rho_H(1)=|H|,\qquad \rho_H(h)=0.
$$

If every nontrivial $\eta$ satisfied $\eta(h)=\eta(1)$, the sum at $h$ would instead equal $\sum\eta(1)^2=|H|$, a contradiction. Choose an $\eta$ for which these values differ. Since $\Psi_\eta$ restricts to $\eta$, it has $\Psi_\eta(g)=\eta(h)\ne d$, so $g\notin\ker\Psi_\eta$. Therefore

$$
\boxed{N=\bigcap_{\eta\in\operatorname{Irr}(H)\setminus\{1_H\}}\ker\Psi_\eta\triangleleft G.}
$$

This proves the [Frobenius kernel theorem](../../../group.md#frobenius-kernel-theorem)'s subgroup assertion. The definition also gives $N\cap H=\{1\}$. Using the permitted cardinality $|N|=[G:H]$, normality ensures $NH$ is a subgroup and

$$
|NH|=\frac{|N||H|}{|N\cap H|}=|G|,\qquad \boxed{NH=G\quad\text{and}\quad G=N\rtimes H.}
$$

Thus $N$ is the [Frobenius kernel](../../../group.md#frobenius-kernel), and $H$ supplies the complementary factor.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Let $V$ afford the [irreducible character](../../../representation-theory.md#irreducible-character) $\chi$. The positive [character inner product](../../../representation-theory.md#character-inner-product) $\langle\chi_H,1_H\rangle_H$ is the multiplicity of the [trivial representation](../../../representation-theory.md#trivial-representation) in $V$ restricted to $H$, so there is a nonzero vector $v$ fixed by every element of $H$. Since $N\subseteq\ker\chi$, every element of $N$ acts as the identity on all of $V$. By $G=NH$, every element of $G$ therefore fixes $v$.

The line $\mathbb Cv$ is a nonzero [invariant subspace](../../../representation-theory.md#invariant-subspace) of the [irreducible representation](../../../representation-theory.md#irreducible-representation) $V$, so it must equal $V$. The action on this line is trivial, proving

$$
\boxed{\chi=1_G.}
$$

The hypothesis on the [kernel of a character](../../../representation-theory.md#kernel-of-a-character) is what makes an $H$-fixed vector into a $G$-fixed vector.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

First show $C_N(h)=\{1\}$. If $z\in N$ commutes with $h$ and $z\ne1$, then $z\notin H$ because $N\cap H=\{1\}$. But $z^{-1}hz=h$, so the nonidentity element $h$ lies in $H\cap H^z$, contradicting the [Frobenius complement](../../../group.md#frobenius-complement) property. Thus conjugation by $h$ has no nonidentity fixed element in the [Frobenius kernel](../../../group.md#frobenius-kernel).

Normality of $N$ makes

$$
f_h:N\longrightarrow N,\qquad f_h(y)=h^{-1}y^{-1}hy
$$

well-defined. If $f_h(a)=f_h(b)$, cancellation gives $a^{-1}ha=b^{-1}hb$, and hence $ba^{-1}$ commutes with $h$. Since $ba^{-1}\in N$ and $C_N(h)=\{1\}$, we obtain $a=b$. The map is injective, and an injection of a finite set into itself is surjective. Consequently

$$
\boxed{\text{For every }x\in N\text{ there exists a unique }y\in N\text{ with }[h,y]=x.}
$$

This is the [commutator bijection from a fixed-point-free automorphism](../../../group.md#commutator-bijection-from-a-fixed-point-free-automorphism), applied to $\alpha(y)=h^{-1}yh$.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Because $N$ is an [abelian group](../../../group.md#abelian-group), every $\varphi\in\operatorname{Irr}(N)$ is a [linear character](../../../representation-theory.md#linear-character), hence a homomorphism to $\mathbb C^\times$. Its [inertia group of a character](../../../representation-theory.md#inertia-group-of-a-character) contains $N$, whose inner conjugations act trivially on $N$. Write an arbitrary $g\in G$ as $g=nh$ with $n\in N$ and $h\in H$, using $G=NH$. Conjugation by $n$ does not affect $\varphi$, so $g$ stabilizes $\varphi$ if and only if $h$ does.

Suppose $h\ne1$ stabilizes $\varphi$. Then $\varphi(h^{-1}yh)=\varphi(y)$ for every $y\in N$, and its multiplicativity gives

$$
\varphi([h,y])=\varphi(h^{-1}y^{-1}hy)=\varphi(h^{-1}yh)^{-1}\varphi(y)=1.
$$

Part (iv) makes $y\mapsto[h,y]$ surjective onto $N$, so $\varphi(x)=1$ for every $x\in N$. This would be the [trivial character](../../../representation-theory.md#trivial-character), contrary to the hypothesis. Therefore no nonidentity $h\in H$ stabilizes $\varphi$, and

$$
\boxed{I_G(\varphi)=N\qquad(\varphi\ne1_N).}
$$

The argument uses both abelianness, to make $\varphi$ multiplicative, and the fixed-point-free commutator bijection.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

We use complex representations. By [Maschke's theorem](../../../representation-theory.md#maschke-s-theorem), restriction to any finite subgroup is a [semisimple module](../../../module-theory.md#semisimple-module), so it has a canonical [isotypic decomposition](../../../module-theory.md#isotypic-decomposition). In particular, the $\theta$-[isotypic component](../../../module-theory.md#isotypic-component) $W_\theta$ is the sum of all copies of the irreducible $N$-module with character $\theta$. The central [character idempotent](../../../associative-algebra.md#character-idempotent)

$$
e_\theta=\frac{\theta(1)}{|N|}\sum_{n\in N}\theta(n^{-1})n
$$

projects onto this component. These projections preserve every $N$-submodule, which consequently decomposes as the [direct sum](../../../vector-space.md#direct-sum) of its intersections with the [isotypic components](../../../module-theory.md#isotypic-component).

Let $W$ afford $\xi\in\operatorname{Irr}(T\mid\theta)$. The component $W_\theta$ is nonzero. Since $T=I_G(\theta)$ fixes $\theta$, it preserves $W_\theta$. Irreducibility of $W$ as a $T$-module therefore gives $W=W_\theta$: its restriction to $N$ consists entirely of copies of $\theta$.

Form the [induced representation](../../../representation-theory.md#induced-representation)

$$
V=\mathbb C[G]\otimes_{\mathbb C[T]}W=\bigoplus_{g\in\mathcal R}g\otimes W,
$$

where $\mathcal R$ represents the left cosets $G/T$. Because $N\triangleleft G$, for $n\in N$ we have

$$
n(g\otimes w)=g\otimes(g^{-1}ng)w.
$$

Thus $g\otimes W$ is $N$-isotypic of type $\theta^g$, where $\theta^g(n)=\theta(g^{-1}ng)$. These types are distinct for distinct cosets $gT$, precisely by the definition of the [inertia group of a character](../../../representation-theory.md#inertia-group-of-a-character) $T$.

Let $Y$ be a nonzero $G$-submodule of $V$. Its [isotypic decomposition](../../../module-theory.md#isotypic-decomposition) as an $N$-module shows that it meets some $g\otimes W$ nontrivially. Acting by $g^{-1}$ gives $Y\cap(1\otimes W)\ne0$. This intersection is a $T$-submodule of the irreducible $W$, hence equals $1\otimes W$. The $G$-translates of that component span $V$, so $Y=V$. The induced representation is therefore irreducible, and its restriction contains $\theta$. Its [induced character](../../../representation-theory.md#induced-character) satisfies

$$
\boxed{\xi^G\in\operatorname{Irr}(G\mid\theta).}
$$

This proves the irreducibility assertion directly from [isotypic components](../../../module-theory.md#isotypic-component); no form of the correspondence being proved has been assumed.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $V$ be an irreducible $G$-module with character $\chi\in\operatorname{Irr}(G\mid\theta)$, and let $W=V_\theta\ne0$ be its $\theta$-[isotypic component](../../../module-theory.md#isotypic-component). It is invariant under the [inertia group of a character](../../../representation-theory.md#inertia-group-of-a-character) $T$. The sum of its $G$-translates is a nonzero $G$-submodule, so irreducibility makes it all of $V$. Translates associated with different cosets $gT$ have distinct $N$-types and hence form a [direct sum](../../../vector-space.md#direct-sum):

$$
V=\bigoplus_{g\in\mathcal R}gW.
$$

To see that $W$ is irreducible over $T$, let $0\ne W_0\subseteq W$ be a $T$-submodule. Then $\sum_{g\in\mathcal R}gW_0$ is a nonzero $G$-submodule of $V$, hence equals $V$. Its $\theta$-isotypic part is exactly $W_0$, whereas the corresponding part of $V$ is $W$. Thus $W_0=W$.

Let $\xi$ be the [irreducible character](../../../representation-theory.md#irreducible-character) of $W$ as a $T$-module. It lies over $\theta$, and the natural map of [induced representations](../../../representation-theory.md#induced-representation)

$$
\mathbb C[G]\otimes_{\mathbb C[T]}W\longrightarrow V,\qquad g\otimes w\longmapsto gw
$$

is an isomorphism: it identifies each summand with the corresponding $gW$, and these summands are direct and exhaust $V$. Consequently $\chi=\xi^G$, proving surjectivity of induction on the stated sets.

For injectivity, the construction in (a) shows that the $\theta$-isotypic component of $\operatorname{Ind}_T^G W$ is exactly $1\otimes W$, with its original $T$-action. Isomorphic induced $G$-modules therefore have isomorphic intrinsic $\theta$-components as $T$-modules. Since complex representations with the same character are isomorphic, $\xi_1^G=\xi_2^G$ forces $\xi_1=\xi_2$. Hence the [Clifford correspondence](../../../representation-theory.md#clifford-correspondence) is the bijection

$$
\boxed{\operatorname{Irr}(T\mid\theta)\xrightarrow{\ \xi\mapsto\xi^G\ }\operatorname{Irr}(G\mid\theta),}
$$

whose inverse takes the character of the $\theta$-isotypic component.

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

An [M-group](../../../group.md#monomial-group) is a finite group for which every [irreducible character](../../../representation-theory.md#irreducible-character) is induced from a [linear character](../../../representation-theory.md#linear-character) of some subgroup. Let $L\triangleleft K$ have both $L$ and $K/L$ abelian, and fix an irreducible $K$-module $V$ with character $\chi$. Since $L$ is abelian, $V_L$ has a linear constituent. Choose, among all pairs $(A,\varphi)$ with $L\subseteq A\subseteq K$ and a [linear character](../../../representation-theory.md#linear-character) $\varphi$ occurring in $\chi_A$, one for which $|A|$ is maximal.

Every subgroup containing $L$ is normal in $K$: its image in the abelian quotient $K/L$ is normal, and it is the full preimage of that image. Thus $A\triangleleft K$, so the [inertia group of a character](../../../representation-theory.md#inertia-group-of-a-character) $I_K(\varphi)$ is defined and contains $A$.

Suppose $x\in I_K(\varphi)\setminus A$. The nonzero $\varphi$-[isotypic component](../../../module-theory.md#isotypic-component) $V_\varphi$ is preserved by $x$, and every $a\in A$ acts there as the scalar $\varphi(a)$ because $\varphi(1)=1$. The finite-order operator representing $x$ is diagonalizable over $\mathbb C$; choose an eigenvector $0\ne v\in V_\varphi$. Then $\mathbb Cv$ is invariant under both $A$ and $x$, hence under $D=\langle A,x\rangle$. This line affords a [linear character](../../../representation-theory.md#linear-character) $\psi$ of $D$ with $\psi_A=\varphi$. Since it is a subrepresentation of $V_D$, it is a constituent of $\chi_D$. But $D$ strictly contains $A$ and still contains $L$, contradicting maximality.

Therefore $I_K(\varphi)=A$. Apply the [Clifford correspondence](../../../representation-theory.md#clifford-correspondence) with [normal subgroup](../../../group-theory.md#normal-subgroup) $A$. Its inertia group is $A$ itself, and $\operatorname{Irr}(A\mid\varphi)=\{\varphi\}$, so the unique irreducible $K$-character lying over $\varphi$ is $\varphi^K$. In particular,

$$
\boxed{\chi=\varphi^K,\qquad\varphi(1)=1.}
$$

Since $\chi$ was arbitrary, every [irreducible character](../../../representation-theory.md#irreducible-character) is a [monomial character](../../../representation-theory.md#monomial-character), proving that [finite metabelian groups are monomial](../../../group-theory.md#finite-metabelian-groups-are-monomial):

$$
\boxed{\text{Every finite metabelian group is an M-group}.}
$$

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For [integer partitions](../../../combinatorics.md#integer-partition) $\lambda,\mu$ of $n$, padded by zero parts, the [dominance order on partitions](../../../representation-theory-of-the-symmetric-group.md#dominance-order-on-partitions) is

$$
\boxed{\lambda\unrhd\mu\iff\sum_{i=1}^r\lambda_i\geq\sum_{i=1}^r\mu_i\quad\text{for every }r\geq1.}
$$

A $\lambda$-tableau fills the [Young diagram](../../../representation-theory-of-the-symmetric-group.md#young-diagram) of $\lambda$ with $1,\ldots,n$, each once. A [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) $[t]$ remembers the sets of entries in each row, ignoring their order within that row. The [Young permutation module](../../../representation-theory-of-the-symmetric-group.md#young-permutation-module) $M^\lambda=\mathbb CX_\lambda$ has these [tabloids](../../../representation-theory-of-the-symmetric-group.md#tabloid) as basis, with $S_n$ acting by permuting the entries.

The [row and column stabilizers](../../../representation-theory-of-the-symmetric-group.md#row-and-column-stabilizers-of-a-young-tableau) $R_t,C_t$ independently permute entries within the rows and columns of $t$. The [column antisymmetrizer](../../../representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau) is $\kappa_t=\sum_{c\in C_t}\operatorname{sgn}(c)c$, and $e_t=\kappa_t[t]$ is the associated [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid). Since $C_{gt}=gC_tg^{-1}$ and conjugation preserves permutation sign,

$$
\kappa_{gt}=g\kappa_tg^{-1},\qquad e_{gt}=\kappa_{gt}[gt]=g\kappa_t[t],\qquad \boxed{ge_t=e_{gt}.}
$$

Thus the [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module) is the submodule

$$
\boxed{S^\lambda=\operatorname{span}_{\mathbb C}\{e_t:t\text{ is a }\lambda\text{-tableau}\}\subseteq M^\lambda.}
$$

Every tableau is $gt$ for a fixed $t$, so any single $e_t$ generates it under $S_n$. Also $C_t\cap R_t=\{1\}$, since a permutation preserving both rows and columns must fix every cell. The [tabloids](../../../representation-theory-of-the-symmetric-group.md#tabloid) $[ct]$ for $c\in C_t$ are consequently distinct, and $e_t$ has coefficient $1$ at $[t]$; in particular $e_t\ne0$.

We use the following precise [column antisymmetrizer](../../../representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau) facts. If some row of a $\mu$-tableau $s$ contains two entries from one column of $t$, the transposition interchanging them pairs equal [tabloids](../../../representation-theory-of-the-symmetric-group.md#tabloid) with opposite signs in $\kappa_t[s]$, so $\kappa_t[s]=0$. Otherwise each row of $s$ meets each column of $t$ at most once. The first $r$ rows of $s$ therefore contain at most $\min(r,\lambda'_j)$ entries from column $j$ of $t$, whence

$$
\sum_{i=1}^r\mu_i\leq\sum_j\min(r,\lambda'_j)=\sum_{i=1}^r\lambda_i.
$$

This states and explains [dominance from a nonzero column antisymmetrizer](../../../representation-theory-of-the-symmetric-group.md#dominance-from-a-nonzero-column-antisymmetrizer): $\kappa_t[s]\ne0$ implies $\lambda\unrhd\mu$.

When $\mu=\lambda$, the [nonzero column antisymmetrizer criterion](../../../representation-theory-of-the-symmetric-group.md#nonzero-column-antisymmetrizer-criterion) says more: either $\kappa_t[s]=0$, or a column permutation takes $[s]$ to $[t]$, and $\kappa_t[s]=\pm e_t$. Thus $\kappa_tM^\lambda=\mathbb Ce_t$. This follows by matching the row positions within each column when all intersections have size at most one; the equal row and column sizes force the Ferrers incidence pattern.

For the [inner product](../../../linear-algebra.md#inner-product), use the positive Hermitian extension of the orthonormal [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) basis, linear in its first argument. It has the supplied self-adjointness of $\kappa_t$. Its orthogonal complement of $S^\lambda$ agrees with that obtained from the complex [tabloid bilinear form](../../../representation-theory-of-the-symmetric-group.md#tabloid-bilinear-form), since the spanning [polytabloids](../../../representation-theory-of-the-symmetric-group.md#polytabloid) have real coefficients. Because the coefficient of $[t]$ in $e_t$ is $1$, self-adjointness and the one-dimensional image give the useful identity

$$
\boxed{\kappa_tu=\langle u,e_t\rangle e_t\qquad(u\in M^\lambda).}
$$

Indeed, the scalar multiplying $e_t$ is the $[t]$-coefficient of $\kappa_tu$, which is $\langle\kappa_tu,[t]\rangle=\langle u,\kappa_t[t]\rangle=\langle u,e_t\rangle$.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Suppose first that $U$ is not contained in $(S^\lambda)^\perp$. Since [polytabloids](../../../representation-theory-of-the-symmetric-group.md#polytabloid) span $S^\lambda$, there exist $u\in U$ and a tableau $t$ with $\langle u,e_t\rangle\ne0$. The [column antisymmetrizer](../../../representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau) identity from the preliminaries gives

$$
\kappa_tu=\langle u,e_t\rangle e_t\in U.
$$

Therefore $e_t\in U$. Because $U$ is an $S_n$-submodule, it contains all translates $ge_t=e_{gt}$, and these span the [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module). Hence $S^\lambda\subseteq U$. If the initial supposition fails, $U\subseteq(S^\lambda)^\perp$. This proves the [James submodule theorem](../../../representation-theory-of-the-symmetric-group.md#james-submodule-theorem)

$$
\boxed{U\supseteq S^\lambda\quad\text{or}\quad U\subseteq(S^\lambda)^\perp.}
$$

Now let $W$ be a submodule of $S^\lambda$. Apply the dichotomy to $W\subseteq M^\lambda$. Either $W=S^\lambda$, or $W\subseteq S^\lambda\cap(S^\lambda)^\perp$. Positivity of the Hermitian form gives $S^\lambda\cap(S^\lambda)^\perp=\{0\}$: a vector in this intersection has squared norm zero. The same intersection is zero for the bilinear form by the agreement of complements explained above. Since $S^\lambda\ne0$, the only submodules are $0$ and itself. Therefore

$$
\boxed{S^\lambda\text{ is simple over }\mathbb C.}
$$

This use of characteristic zero and nondegeneracy is why the conclusion does not automatically extend to every modular [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Let $0\ne f:S^\lambda\to M^\mu$ be a module homomorphism. Since $S^\lambda$ is simple, $f$ is injective. Fix a $\lambda$-tableau $t$; its nonzero [polytabloid](../../../representation-theory-of-the-symmetric-group.md#polytabloid) $e_t$ then has $f(e_t)\ne0$. The sign sum in the column group satisfies

$$
\kappa_t^2=|C_t|\kappa_t,
$$

because every coefficient in the square receives $|C_t|$ equal contributions. Thus $\kappa_te_t=|C_t|e_t$, and equivariance gives

$$
\kappa_tf(e_t)=f(\kappa_te_t)=|C_t|f(e_t)\ne0.
$$

The [column antisymmetrizer](../../../representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau) therefore acts nontrivially on $M^\mu$, so some basis [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid) $[s]$ has $\kappa_t[s]\ne0$. The stated [dominance from a nonzero column antisymmetrizer](../../../representation-theory-of-the-symmetric-group.md#dominance-from-a-nonzero-column-antisymmetrizer) yields

$$
\boxed{\operatorname{Hom}_{\mathbb CS_n}(S^\lambda,M^\mu)\ne0\Longrightarrow\lambda\unrhd\mu.}
$$

For $\mu=\lambda$, the same calculation forces $f(e_t)=|C_t|^{-1}\kappa_tf(e_t)$ into the one-dimensional space $\mathbb Ce_t$. Write $f(e_t)=ce_t$. Since $e_t$ generates the [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module), equivariance gives $f(ge_t)=cge_t$ for every $g$, so $f$ is $c$ times the inclusion $S^\lambda\hookrightarrow M^\lambda$. That inclusion is nonzero, hence

$$
\boxed{\dim\operatorname{Hom}_{\mathbb CS_n}(S^\lambda,M^\lambda)=1.}
$$

As a useful consequence, if $S^\lambda\cong S^\mu$, their inclusions into $M^\lambda,M^\mu$ give dominance both ways. Antisymmetry of the [dominance order on partitions](../../../representation-theory-of-the-symmetric-group.md#dominance-order-on-partitions) then gives $\lambda=\mu$, so different partitions produce nonisomorphic simple modules.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The preceding parts give a simple [Specht module](../../../representation-theory-of-the-symmetric-group.md#specht-module) for each partition and show that different partitions give nonisomorphic simples. The [conjugacy classes](../../../group-theory.md#conjugacy-class) of $S_n$ are indexed by partitions of $n$, namely cycle types. We use the standard finite-group character theorem: the number of irreducible complex characters equals the number of [conjugacy classes](../../../group-theory.md#conjugacy-class), and they form an orthonormal basis of complex [class functions](../../../representation-theory.md#class-function). Consequently the $\chi^\lambda$ are the complete list of [irreducible characters](../../../representation-theory.md#irreducible-character) of $S_n$.

By [Maschke's theorem](../../../representation-theory.md#maschke-s-theorem), the [Young permutation module](../../../representation-theory-of-the-symmetric-group.md#young-permutation-module) $M^\mu$ decomposes as a [direct sum](../../../vector-space.md#direct-sum) of these simple modules. For a semisimple complex module, [Schur lemma](../../../representation-theory.md#schur-s-lemma) makes the multiplicity of a simple module equal to the dimension of the homomorphism space from that simple; [character orthogonality](../../../representation-theory.md#character-orthogonality) identifies the same number with the [character inner product](../../../representation-theory.md#character-inner-product). Hence

$$
M^\mu\cong\bigoplus_{\lambda\vdash n}(S^\lambda)^{\oplus a_{\lambda\mu}},\qquad a_{\lambda\mu}=\dim\operatorname{Hom}_{\mathbb CS_n}(S^\lambda,M^\mu)=\langle\xi^\mu,\chi^\lambda\rangle\in\mathbb Z_{\geq0}.
$$

Part (ii) makes $a_{\lambda\mu}=0$ unless $\lambda\unrhd\mu$, and gives $a_{\mu\mu}=1$. Taking characters proves

$$
\boxed{\xi^\mu=\sum_{\lambda\unrhd\mu}\langle\xi^\mu,\chi^\lambda\rangle\chi^\lambda,\qquad\langle\xi^\mu,\chi^\mu\rangle=1.}
$$

Thus the permutation-character decomposition is triangular in the [dominance order on partitions](../../../representation-theory-of-the-symmetric-group.md#dominance-order-on-partitions), with diagonal multiplicity one. These are the dominance and diagonal-multiplicity consequences of [Young's rule](../../../representation-theory-of-the-symmetric-group.md#young-s-rule), obtained here without assuming its full multiplicity formula.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The [permutation character](../../../representation-theory.md#permutation-character) $\xi^\mu(g)$ is the number of $\mu$-[tabloids](../../../representation-theory-of-the-symmetric-group.md#tabloid) fixed by $g$, since the trace of a permutation matrix counts fixed basis elements. It is therefore an integer. Arrange the partitions in decreasing lexicographic order. If $\lambda$ strictly dominates $\mu$, the first part at which they differ is larger for $\lambda$, so this ordering places $\lambda$ before $\mu$.

For the first partition $(n)$, there is just one [tabloid](../../../representation-theory-of-the-symmetric-group.md#tabloid), and $\chi^{(n)}=\xi^{(n)}=1_{S_n}$ is integer-valued. At a general partition $\mu$, the decomposition in (iii) can be rearranged as

$$
\chi^\mu=\xi^\mu-\sum_{\substack{\lambda\unrhd\mu\\\lambda\ne\mu}}a_{\lambda\mu}\chi^\lambda,\qquad a_{\lambda\mu}\in\mathbb Z_{\geq0}.
$$

By induction, all characters in the sum are already integer-valued; the [permutation character](../../../representation-theory.md#permutation-character) and all coefficients are also integral. Thus $\chi^\mu$ is integer-valued. Finite induction proves that [symmetric-group characters are integer-valued](../../../representation-theory-of-the-symmetric-group.md#symmetric-group-characters-are-integer-valued):

$$
\boxed{\chi^\lambda(g)\in\mathbb Z\qquad(g\in S_n,\ \lambda\vdash n).}
$$

The diagonal coefficient one is essential: it lets us solve for $\chi^\mu$ without division, preserving integrality.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

Take $g=(1\ 2\ \cdots\ n)$. Since $n\equiv3\pmod4$ is odd, its sign is $(-1)^{n-1}=1$, so $g\in A_n$. Define $s$ to fix $1$ and reverse the other cyclic labels: it interchanges $2$ with $n$, $3$ with $n-1$, and so on. Then $sgs^{-1}=g^{-1}$, while

$$
\operatorname{sgn}(s)=(-1)^{(n-1)/2}=-1.
$$

The [centralizer](../../../group-theory.md#centralizer) of an $n$-cycle in $S_n$ is $\langle g\rangle$: a commuting permutation is determined by the image of one point, and that image fixes the corresponding power of the cycle. All its elements are even, because $g$ is even. Any other conjugator taking $g$ to $g^{-1}$ differs from $s$ by a [centralizer](../../../group-theory.md#centralizer) element and therefore remains odd. Thus $g$ and $g^{-1}$ are not conjugate in $A_n$. This is the parity obstruction described by [inversion of an odd cycle in an alternating group](../../../group-theory.md#inversion-of-an-odd-cycle-in-an-alternating-group).

For any complex character of a finite group, a unitary realization gives

$$
\theta(g^{-1})=\overline{\theta(g)}.
$$

If every $\theta\in\operatorname{Irr}(A_n)$ had real value at $g$, all these characters would take equal values on $g$ and $g^{-1}$. But [irreducible characters separate conjugacy classes](../../../representation-theory.md#irreducible-characters-separate-conjugacy-classes): they form a basis of [class functions](../../../representation-theory.md#class-function), so equality of every irreducible value would also give equality of the class indicator functions. The two distinct [conjugacy classes](../../../group-theory.md#conjugacy-class) cannot have that property. Consequently

$$
\boxed{\text{There is }\theta\in\operatorname{Irr}(A_n)\text{ with }\theta((1\ 2\ \cdots\ n))\notin\mathbb R.}
$$

In other words, these alternating groups are not [ambivalent groups](../../../group.md#ambivalent-group), even though all symmetric-group [irreducible characters](../../../representation-theory.md#irreducible-character) are integer-valued.

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

In character theory, a [p-elementary group](../../../group.md#p-elementary-group) is a finite group isomorphic to $P\times C$, where $P$ is a $p$-group and $C$ is cyclic of order coprime to $p$. Either factor may be trivial. An [elementary group](../../../group.md#elementary-group) is p-elementary for at least one prime $p$; it need not be an elementary [abelian group](../../../group.md#abelian-group).

A [generalised character](../../../representation-theory.md#virtual-character) means an integer linear combination of irreducible complex characters. [Brauer's characterisation of characters](../../../representation-theory.md#brauer-s-characterization-of-characters) states that a complex [class function](../../../representation-theory.md#class-function) $f$ on a finite group $G$ is a [generalised character](../../../representation-theory.md#virtual-character) if and only if $f_E$ is a [generalised character](../../../representation-theory.md#virtual-character) for every elementary subgroup $E\leq G$. Equivalently,

$$
\boxed{f\in\mathbb Z\operatorname{Irr}(G)\iff\langle f_E,\alpha\rangle_E\in\mathbb Z\text{ for every elementary }E\leq G\text{ and }\alpha\in\operatorname{Irr}(E).}
$$

An ordinary character additionally requires nonnegative coefficients in its global irreducible decomposition. We use the virtual-character criterion just stated.

For the extension construction, set $d=\theta(1)$. The [determinant character](../../../representation-theory.md#determinant-character) $\det\theta$ is linear. Since its extension $\mu$ has the same value $1$ at the identity, $\mu$ is also a [linear character](../../../representation-theory.md#linear-character). For any $g\in G$, the subgroup $J_g=N\langle g\rangle$ has cyclic quotient $J_g/N$, hence a solvable quotient. The invariant character $\theta$ has degree coprime to $[J_g:N]$, since this index divides $[G:N]$, and $\mu_{J_g}$ extends its determinant. The permitted [coprime-degree determinant extension theorem](../../../representation-theory.md#coprime-degree-determinant-extension-theorem) therefore gives a unique character $\chi_g\in\operatorname{Irr}(J_g)$ with

$$
(\chi_g)_N=\theta,\qquad\det\chi_g=\mu_{J_g}.
$$

Define a function on $G$ by $f(g)=\chi_g(g)$. We next verify that these individually defined values form a compatible [class function](../../../representation-theory.md#class-function).

If $x\in G$, conjugation carries $J_g$ to $J_{xgx^{-1}}$. Transporting $\chi_g$ by this conjugation gives a character extending $\theta$, because $\theta$ is $G$-invariant, and with determinant $\mu$ restricted to the conjugate subgroup, because $\mu$ is a [class function](../../../representation-theory.md#class-function). Uniqueness identifies the transported character with $\chi_{xgx^{-1}}$. Consequently $f(xgx^{-1})=f(g)$.

Now take an elementary subgroup $E\leq G$ and let $J=NE$. A finite $p$-group is solvable, a cyclic group is solvable, and a direct product of [solvable groups](../../../group-theory.md#solvable-group) is solvable. Thus $E$ is solvable, and so is $J/N\cong E/(E\cap N)$. Again the index $[J:N]$ divides $[G:N]$, so the same extension theorem gives $\chi_J\in\operatorname{Irr}(J)$ extending $\theta$ with determinant $\mu_J$.

For $g\in E$, we have $J_g\leq J$. The restriction $(\chi_J)_{J_g}$ is irreducible: an [invariant subspace](../../../representation-theory.md#invariant-subspace) for $J_g$ would be invariant for $N$, whose restriction already affords the irreducible $\theta$. Its determinant is $\mu_{J_g}$. By uniqueness on $J_g$, it equals $\chi_g$. Therefore

$$
f_E=(\chi_J)_E,
$$

an ordinary character and hence a [generalised character](../../../representation-theory.md#virtual-character) of $E$. [Brauer's characterisation of characters](../../../representation-theory.md#brauer-s-characterization-of-characters) now makes $f$ a [generalised character](../../../representation-theory.md#virtual-character) of $G$. If $n\in N$, then $J_n=N$ and $\chi_n=\theta$, so $f(n)=\theta(n)$. We have proved, by [gluing determinant-normalized character extensions](../../../representation-theory.md#gluing-determinant-normalized-character-extensions),

$$
\boxed{\chi:=f\text{ is a generalised character of }G,\qquad\chi_N=\theta.}
$$

Only the intermediate quotients $J_g/N$ and $NE/N$ were required to be solvable; no solvability assumption on $G/N$ has been added.

For the prime-set assertion, let $E=P\times C$ be p-elementary, and split the cyclic group as $C=C_\pi\times C_{\pi'}$, where each factor has the indicated prime divisors in its order. If $p\in\pi$, put $E_\pi=P\times C_\pi$ and $E_{\pi'}=C_{\pi'}$. If $p\notin\pi$, put $E_\pi=C_\pi$ and $E_{\pi'}=P\times C_{\pi'}$. In both cases the factors commute, have trivial intersection and have orders with disjoint prime spectra. This proves the [prime-set decomposition of elementary groups](../../../group.md#prime-set-decomposition-of-elementary-groups)

$$
\boxed{E=E_\pi\times E_{\pi'},\qquad E_\pi\text{ a }\pi\text{-group},\quad E_{\pi'}\text{ a }\pi'\text{-group}.}
$$

Here a [pi-group](../../../group.md#pi-group) has order divisible only by primes in $\pi$, and a [pi-element](../../../group.md#pi-element) has such an element order; the identity qualifies for both complementary prime sets.

Finally, suppose $K$ satisfies the given element-order condition. The sets $A,B$ are unions of [conjugacy classes](../../../group-theory.md#conjugacy-class) and are disjoint, because membership in both would force every prime divisor of the element order into $\pi\cap\pi'=\varnothing$, hence force order $1$. Let $E\leq K$ be elementary and use $E=E_\pi\times E_{\pi'}$. If both factors were nontrivial, choose $a\ne1$ in the first and $b\ne1$ in the second. They commute and have coprime orders, so $ab$ has order $|a||b|$, containing primes from both $\pi$ and $\pi'$. It would belong to neither $A$ nor $B$ nor $\{1\}$, contrary to the hypothesis. Thus every elementary subgroup is entirely a [pi-group](../../../group.md#pi-group) or entirely a complementary-prime group.

Write $m=|K|_\pi$ and $r=|K|_{\pi'}$ for the two prime parts of $|K|$, so $|K|=mr$ and $\gcd(m,r)=1$. The [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) supplies an integer $D$ satisfying

$$
D\equiv1\pmod m,\qquad D\equiv0\pmod r.
$$

Define the [class function](../../../representation-theory.md#class-function)

$$
f(1)=D,\qquad f(a)=1\ (a\in A),\qquad f(b)=0\ (b\in B).
$$

For an elementary $\pi$-subgroup $E$, its order divides $m$. Let $\rho_E$ be the character of its [regular representation](../../../representation-theory.md#regular-representation), equal to $|E|$ at $1$ and zero elsewhere. Then

$$
f_E=1_E+\frac{D-1}{|E|}\rho_E,
$$

with integral coefficient because $D\equiv1\pmod{|E|}$. For an elementary $\pi'$-subgroup, its order divides $r$, and

$$
f_E=\frac{D}{|E|}\rho_E
$$

again has integral coefficient. The trivial subgroup satisfies either formula. Every elementary restriction is therefore a [generalised character](../../../representation-theory.md#virtual-character). A second application of [Brauer's characterisation of characters](../../../representation-theory.md#brauer-s-characterization-of-characters) proves

$$
\boxed{\xi:=f\text{ is a generalised character of }K,\qquad\xi(a)=1\ (a\in A),\quad\xi(b)=0\ (b\in B).}
$$

The freely chosen identity value, fixed by the two congruences, makes the restrictions integral. This construction also covers the cases $\pi=\varnothing$, $\pi'=\varnothing$, or $K=\{1\}$, using modulus-one congruences where appropriate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
