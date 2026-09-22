# Paper 138

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_138.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_138.pdf)

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
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $N=\sum_{g\in G}g$ be the [group norm element](../../../associative-algebra.md#group-norm-element). This is a nonzero vector in the [group algebra](../../../associative-algebra.md#group-algebra) $kG$, and $kN$ is a trivial [submodule](../../../module-theory.md#submodule) of its left regular [module](../../../module-theory.md#module-mathematics). If $kG$ were a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra), this [submodule](../../../module-theory.md#submodule) would have a $kG$-linear projection $\pi:kG\to kN$. Write $\pi(1)=cN$. Since $gN=N$ for every $g$, we would have

$$
\pi(N)=\sum_{g\in G}g\pi(1)=|G|cN=0,
$$

whereas a projection onto $kN$ satisfies $\pi(N)=N\ne0$. Thus $\boxed{kG\text{ is not semisimple}}$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $q=p^n$. A finitely generated [module](../../../module-theory.md#module-mathematics) over $A=k[X]/(X^q)$ is finite-dimensional over $k$, and multiplication by $X$ is a [nilpotent linear map](../../../linear-operator-theory.md#nilpotent-linear-map) $T$ with $T^q=0$. Its [Jordan normal form](../../../linear-operator-theory.md#jordan-normal-form) exists over $k$ because its minimal polynomial is a power of $X$. Each [Jordan block](../../../linear-operator-theory.md#jordan-block) has size $r\le q$ and is the [cyclic module](../../../module-theory.md#cyclic-module) $M_r=k[X]/(X^r)$. Hence

$$
M\cong\bigoplus_{r=1}^{q}M_r^{\oplus m_r}.
$$

A [submodule](../../../module-theory.md#submodule) of $M_r$ is an ideal of $k[X]/(X^r)$, and its inverse image is an ideal of the [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) $k[X]$ containing $(X^r)$. The only possibilities are $(X^j)$ with $0\le j\le r$. Thus all [submodules](../../../module-theory.md#submodule) form the chain

$$
M_r\supset XM_r\supset\cdots\supset X^{r-1}M_r\supset0.
$$

Every successive quotient is the one-dimensional [simple module](../../../module-theory.md#irreducible-module) on which $X$ acts as zero. This is its unique [composition series](../../../finite-group-theory.md#composition-series), so $M_r$ is a [uniserial module](../../../module-theory.md#uniserial-module) and is an [indecomposable representation](../../../representation-theory.md#indecomposable-representation): two nonzero direct summands would be incomparable [submodules](../../../module-theory.md#submodule). Only $M_1$ is simple.

For $G=\langle g\rangle$ of order $q$, the [group algebra](../../../associative-algebra.md#group-algebra) satisfies

$$
kG\cong k[T]/(T^q-1)\cong k[X]/(X^q),\qquad X=g-1,
$$

since $(T-1)^q=T^q-1$ in [characteristic](../../../algebra.md#characteristic-of-a-field) $p$. Consequently, up to isomorphism, $\boxed{M_1,\ldots,M_{p^n}}$ are precisely the finite-dimensional indecomposable modules, and $\boxed{M_1\text{ is the unique simple module}}$. The finite-dimensional convention follows from the finite-generation hypothesis; “exactly” counts isomorphism classes.

## 2

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The roots-of-unity criterion for a [splitting field for finite group representations](../../../representation-theory.md#splitting-field-for-finite-group-representations) says that the assumed $m$th [roots of unity](../../../algebra.md#root-of-unity) make $k$ a splitting [field](../../../algebra.md#field) for $G$. Fix a multiplicative identification of the group $\mu_m(k)$ with the complex $m$th [roots of unity](../../../algebra.md#root-of-unity). For a [p-regular element](../../../representation-theory.md#p-regular-element) $g$, its order divides $m$; the operator $\rho(g)$ is diagonalizable because $X^{|g|}-1$ has distinct roots in $k$. If its [eigenvalues](../../../linear-operator-theory.md#eigenvalue), counted with multiplicity, are $\lambda_1,\ldots,\lambda_d$, define the [Brauer character](../../../representation-theory.md#brauer-character) by

$$
\chi_V(g)=\sum_{i=1}^{d}\widehat\lambda_i,
$$

where hats denote the chosen complex lifts. This defines a [class function](../../../representation-theory.md#class-function) on the [p-regular elements](../../../representation-theory.md#p-regular-element), not on arbitrary elements of $G$.

A [short exact sequence](../../../module-theory.md#short-exact-sequence) can be represented by block triangular matrices, so the eigenvalue multiset is the union of those on its [submodule](../../../module-theory.md#submodule) and quotient. Thus [Brauer characters](../../../representation-theory.md#brauer-character) are additive on [short exact sequences](../../../module-theory.md#short-exact-sequence). If $S_1,\ldots,S_t$ are the simple $kG$-modules, the [Jordan–Hölder theorem](../../../finite-group-theory.md#jordan-holder-theorem) gives

$$
\chi_V=\sum_{j=1}^{t}[V:S_j]\chi_{S_j}.
$$

We use the standard [Brauer–Nesbitt theorem](../../../representation-theory.md#brauer-nesbitt-theorem) in its character form: over a splitting [field](../../../algebra.md#field) the [Brauer characters](../../../representation-theory.md#brauer-character) of the nonisomorphic [simple modules](../../../module-theory.md#irreducible-module) are linearly independent over $\mathbb C$. Therefore

$$
\boxed{\chi_V=\chi_{V'}\iff[V:S_j]=[V':S_j]\text{ for every }j}.
$$

Both the modular splitting-field criterion and this independence theorem are the representation-theoretic results used here.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Let $g$ be a [p-regular element](../../../representation-theory.md#p-regular-element), with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_i$ on $V$. On both $g^{-1}$ acting on $V$ and $g$ acting on the [dual representation](../../../representation-theory.md#dual-representation) $V^*$, the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\lambda_i^{-1}$. Multiplicative lifts of [roots of unity](../../../algebra.md#root-of-unity) satisfy $\widehat{\lambda_i^{-1}}=\widehat\lambda_i^{-1}=\overline{\widehat\lambda_i}$. Hence

$$
\boxed{\chi_V(g^{-1})=\overline{\chi_V(g)}=\chi_{V^*}(g)}.
$$

All these identities concern the domain of a [Brauer character](../../../representation-theory.md#brauer-character), namely the [p-regular elements](../../../representation-theory.md#p-regular-element). If necessary, extend the [p-modular system](../../../representation-theory.md#p-modular-system) to contain the relevant [roots of unity](../../../algebra.md#root-of-unity) and use one consistent choice of lifts.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For a [p-regular element](../../../representation-theory.md#p-regular-element) $g$, diagonalize its actions on $V$ and $V'$. If their [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\lambda_i$ and $\nu_j$, the [tensor product of group representations](../../../representation-theory.md#tensor-product-of-group-representations) has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_i\nu_j$. The lift of [roots of unity](../../../algebra.md#root-of-unity) is multiplicative, so

$$
\chi_{V\otimes V'}(g)=\sum_{i,j}\widehat\lambda_i\widehat\nu_j=\chi_V(g)\chi_{V'}(g).
$$

Thus $\boxed{\chi_{V\otimes V'}=\chi_V\chi_{V'}}$ as [Brauer characters](../../../representation-theory.md#brauer-character).

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

For a nonzero [group representation](../../../representation-theory.md#group-representation) $V$, there is a $G$-equivariant identification

$$
V\otimes V^*\cong\operatorname{End}_k(V),\qquad v\otimes f\longmapsto(w\mapsto f(w)v),
$$

where $G$ acts on endomorphisms by conjugation. The identity endomorphism is a nonzero fixed vector, so its span is a trivial [submodule](../../../module-theory.md#submodule). It follows that the trivial [simple module](../../../module-theory.md#irreducible-module) is a [Jordan–Hölder factor](../../../finite-group-theory.md#jordan-holder-factor) of $V\otimes V^*$, and character additivity gives $\boxed{1_G\text{ is a constituent of }\chi\overline\chi}$.

Here “constituent” means a composition factor; the trivial [submodule](../../../module-theory.md#submodule) need not be a direct summand. Also the assertion needs $\chi\ne0$: the zero-dimensional module has the zero [Brauer character](../../../representation-theory.md#brauer-character), whose product with its conjugate has no constituent. This is an implicit nonzero-character qualification in the printed statement.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A nonabelian [simple group](../../../finite-group-theory.md#simple-group) is a [perfect group](../../../group-theory.md#perfect-group), so every one-dimensional [group representation](../../../representation-theory.md#group-representation), a homomorphism to the abelian group $k^\times$, is trivial. Thus a nontrivial irreducible [Brauer character](../../../representation-theory.md#brauer-character) cannot have degree $1$.

Suppose instead that its representation has dimension $2$, working over a splitting extension if necessary. Its determinant is a one-dimensional representation and is therefore trivial. Its kernel is a [normal subgroup](../../../group-theory.md#normal-subgroup), and the representation is nontrivial, so simplicity makes it faithful. Consequently $G$ embeds in $\operatorname{SL}_2(k)$.

We use the [Feit–Thompson theorem](../../../finite-group-theory.md#feit-thompson-theorem): every finite group of odd order is solvable. Therefore this nonabelian simple group has even order, and [Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) supplies an [involution](../../../group-theory.md#involution) $t$. In odd [characteristic](../../../algebra.md#characteristic-of-a-field), its representing matrix $A$ satisfies $A^2=I$ and is diagonalizable with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) in $\{1,-1\}$. Since $\det A=1$, it is $I$ or $-I$. Faithfulness excludes $I$, so $t$ acts as the scalar matrix $-I$. It commutes with the whole image; faithfulness then makes $t$ central in $G$, contradicting nonabelian simplicity. Hence $\boxed{\chi(1)>2}$.

The [odd order theorem](../../../finite-group-theory.md#feit-thompson-theorem) is the deep standard group-theoretic input in this proof; its use is explicit rather than hidden in an unsupported assertion that $G$ has an involution.

## 3

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [modular representation ring](../../../representation-theory.md#modular-representation-ring) $R_k(G)$ is the abelian group generated by isomorphism classes $[V]$ of finite-dimensional $kG$-[modules](../../../module-theory.md#module-mathematics), with relations

$$
[V]=[U]+[W]\quad\text{whenever }0\to U\to V\to W\to0\text{ is exact}.
$$

The [Jordan–Hölder theorem](../../../finite-group-theory.md#jordan-holder-theorem) says that it is a free abelian group with basis the classes of the [simple modules](../../../module-theory.md#irreducible-module), and $[V]=\sum_S[V:S][S]$. To see independence, composition multiplicity for each fixed simple $S$ is an additive map to $\mathbb Z$ and reads off its basis coefficient.

Define $[V][W]=[V\otimes_k W]$, using the diagonal action in the [tensor product of group representations](../../../representation-theory.md#tensor-product-of-group-representations). Tensoring over a [field](../../../algebra.md#field) is exact in either argument, so multiplication respects the defining relations. Associativity and the symmetry $v\otimes w\mapsto w\otimes v$ give a [commutative ring](../../../commutative-algebra.md#commutative-ring) with identity $[k]$, the [trivial representation](../../../representation-theory.md#trivial-representation). Thus $\boxed{R_k(G)\text{ is a commutative ring, freely based on simple modules}}$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

There is a missing hypothesis in the original PDF: $k$ must be a [splitting field for finite group representations](../../../representation-theory.md#splitting-field-for-finite-group-representations). For example,

$$
\mathbb F_2C_3\cong\mathbb F_2[X]/(X^3-1)\cong\mathbb F_2\times\mathbb F_4,
$$

because $X^3-1=(X-1)(X^2+X+1)$ and the quadratic factor is irreducible. This algebra has two [simple modules](../../../module-theory.md#irreducible-module), whereas $C_3$ has three conjugacy classes, all $2$-regular. Thus the printed assertion for an arbitrary [field](../../../algebra.md#field) is false.

Under the intended splitting hypothesis, fix compatible lifts defining [Brauer characters](../../../representation-theory.md#brauer-character). Let $\mathcal K_{p'}$ be the set of conjugacy classes of [p-regular elements](../../../representation-theory.md#p-regular-element). Character additivity and the tensor-product formula define the unital algebra homomorphism

$$
\Phi:\mathbb C\otimes_{\mathbb Z}R_k(G)\longrightarrow\prod_{C\in\mathcal K_{p'}}\mathbb C,\qquad z\otimes[V]\longmapsto\bigl(z\chi_V(g_C)\bigr)_C.
$$

We use the [Brauer character basis theorem](../../../representation-theory.md#brauer-character-basis-theorem): over a splitting [field](../../../algebra.md#field) the irreducible [Brauer characters](../../../representation-theory.md#brauer-character) form a complex basis of the [class functions](../../../representation-theory.md#class-function) on the p-regular conjugacy classes. Therefore $\Phi$ maps the basis $1\otimes[S]$ bijectively to a basis and is an algebra isomorphism. Comparing dimensions gives

$$
\boxed{\mathbb C\otimes R_k(G)\cong\mathbb C^{\mathcal K_{p'}},\qquad\#\{\text{simple }kG\text{-modules}\}=|\mathcal K_{p'}|\quad(k\text{ splitting})}.
$$

Isomorphism classes are understood in the count.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

First the product is also split. Write $A_i=kG_i$ and $J_i=\operatorname{rad}A_i$. The ideal

$$
I=J_1\otimes A_2+A_1\otimes J_2\subset A_1\otimes A_2\cong k(G_1\times G_2)
$$

is nilpotent: if $J_1^r=J_2^s=0$, every product of $r+s-1$ of its factors vanishes. The quotient is

$$
(A_1/J_1)\otimes(A_2/J_2),
$$

a product of full [matrix algebras](../../../associative-algebra.md#matrix-algebra) over $k$, because each $A_i$ is split. A [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal) lies in the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical), and a semisimple quotient forces the reverse inclusion, so $I$ is exactly the radical. Thus $k$ is a [splitting field for finite group representations](../../../representation-theory.md#splitting-field-for-finite-group-representations) of the product.

For [simple modules](../../../module-theory.md#irreducible-module) $S_i$, [Schur lemma](../../../representation-theory.md#schur-s-lemma) and splitting give $\operatorname{End}_{A_i}(S_i)=k$. The [Jacobson density theorem](../../../noncommutative-algebra.md#jacobson-density-theorem) therefore makes the image of $A_i$ on $S_i$ the full $\operatorname{End}_k(S_i)$. Tensoring these maps shows that the product algebra acts on $S_1\otimes S_2$ through its full endomorphism algebra. Hence this [tensor product of group representations](../../../representation-theory.md#tensor-product-of-group-representations) is simple.

On restriction to $G_1$, it is a [direct sum](../../../vector-space.md#direct-sum) of $\dim S_2$ copies of $S_1$. If two external tensor products are isomorphic, their restrictions and the [Jordan–Hölder theorem](../../../finite-group-theory.md#jordan-holder-theorem) force $S_1\cong S'_1$; restricting to $G_2$ similarly forces $S_2\cong S'_2$. The converse follows by tensoring the isomorphisms.

Finally, the p-regular conjugacy classes of $G_1\times G_2$ are precisely pairs of such classes in the factors. The corrected result in part (b) counts as many simples for the product as pairs of simples for the two factors. Our pairwise nonisomorphic tensor products already attain that count, so they exhaust all simples. Thus $\boxed{\operatorname{Irr}_k(G_1\times G_2)=\{S_1\otimes S_2\}}$, uniquely indexed by pairs of simple isomorphism classes.

## 4

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

An [integral form of a group representation](../../../representation-theory.md#integral-form-of-a-group-representation) $V$ is a $G$-stable finite free $\mathcal O$-submodule $W\subset V$ with $K\otimes_{\mathcal O}W\cong V$. Such a form exists: take a basis lattice $L$ and replace it by $\sum_{g\in G}gL$, which is finite and torsion-free and therefore free over the [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring) $\mathcal O$.

Choose ordinary [simple modules](../../../module-theory.md#irreducible-module) $V_i$ with forms $W_i$, and modular [simple modules](../../../module-theory.md#irreducible-module) $S_j$ with [projective covers](../../../module-theory.md#projective-cover) $P_j$. With $\pi$ a [uniformizer](../../../commutative-algebra.md#uniformizer), put $\overline W_i=W_i/\pi W_i$. The [decomposition matrix](../../../representation-theory.md#decomposition-matrix-modular-representation-theory) and [Cartan matrix of a group algebra](../../../representation-theory.md#cartan-matrix-of-a-group-algebra) have entries

$$
d_{ij}=[\overline W_i:S_j],\qquad c_{\ell j}=[P_j:S_\ell].
$$

The first numbers do not depend on the integral form: the [Brauer character](../../../representation-theory.md#brauer-character) of its reduction is the ordinary character restricted to [p-regular elements](../../../representation-theory.md#p-regular-element), and part 2(a) determines all composition multiplicities from this restriction.

For the assertion in (i), set $I=\operatorname{Hom}_{\mathcal OG}(W,W')$. It is a [submodule](../../../module-theory.md#submodule) of the [finite free module](../../../module-theory.md#finite-free-module) $\operatorname{Hom}_{\mathcal O}(W,W')$, hence is finite free over $\mathcal O$. There is a natural injective map

$$
K\otimes_{\mathcal O}I\longrightarrow\operatorname{Hom}_{KG}(M,M').
$$

For any homomorphism $f$ in the target, clearing the finitely many denominators of its values on an $\mathcal O$-basis of $W$ gives $\pi^Nf(W)\subset W'$. Thus $\pi^Nf\in I$, and the map is surjective. Therefore $\boxed{I\text{ is an }\mathcal O\text{-form of }\operatorname{Hom}_{KG}(M,M')}$, regarding this Hom space as a vector space. The original PDF supplies part (i), which is missing from the supplied TeX.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write $\mathfrak p=\pi\mathcal O$. Certainly multiplication by $\pi$ sends every $\mathcal OG$-homomorphism $W\to W'$ to one with image in $\pi W'$. Conversely, if $f:W\to\pi W'$ is such a homomorphism, define $h(w)=\pi^{-1}f(w)\in W'$. This is well defined because $W'$ is torsion-free. Cancellation of $\pi$ shows that $h$ is $\mathcal O$-linear and commutes with the $G$-action. Hence $f=\pi h$, and

$$
\boxed{\mathfrak p\operatorname{Hom}_{\mathcal OG}(W,W')=\operatorname{Hom}_{\mathcal OG}(W,\mathfrak pW')}.
$$

This step in [reduction of Hom from a projective group-algebra lattice](../../../representation-theory.md#reduction-of-hom-from-a-projective-group-algebra-lattice) does not itself require projectivity.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Put $I=\operatorname{Hom}_{\mathcal OG}(W,W')$. Since $W$ is a [projective module](../../../module-theory.md#projective-module), its [Hom functor](../../../algebra.md#hom-functor) is exact. Applied to $0\to\pi W'\to W'\to W'/\pi W'\to0$, it gives

$$
0\longrightarrow\operatorname{Hom}_{\mathcal OG}(W,\pi W')\longrightarrow I\longrightarrow\operatorname{Hom}_{\mathcal OG}(W,W'/\pi W')\longrightarrow0.
$$

The kernel is $\pi I$ by (ii). Every map to $W'/\pi W'$ kills $\pi W$ and factors uniquely through $W/\pi W$; this gives the second isomorphism. Therefore

$$
\boxed{I/\pi I\cong\operatorname{Hom}_{\mathcal OG}(W,W'/\pi W')\cong\operatorname{Hom}_{kG}(W/\pi W,W'/\pi W')}.
$$

By (i), $I$ is finite free with rank $\dim_K\operatorname{Hom}_{KG}(M,M')$. Its reduction has dimension equal to that rank. Thus [reduction of Hom from a projective group-algebra lattice](../../../representation-theory.md#reduction-of-hom-from-a-projective-group-algebra-lattice) yields

$$
\boxed{\dim_K\operatorname{Hom}_{KG}(M,M')=\dim_k\operatorname{Hom}_{kG}(k\otimes_{\mathcal O}W,k\otimes_{\mathcal O}W')}.
$$

The original PDF has the group-algebra subscripts used here; the supplied TeX drops or corrupts several of them.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Completeness permits [idempotent lifting](../../../commutative-algebra.md#idempotent-lifting) from $kG$ to $\mathcal OG$. In particular, each [projective cover](../../../module-theory.md#projective-cover) $P_j$ lifts to a finite projective $\mathcal OG$-lattice $\widetilde P_j$; one can lift an idempotent presenting it as a summand of a [finite free module](../../../module-theory.md#finite-free-module). Set $Q_j=K\otimes_{\mathcal O}\widetilde P_j$.

For a simple $S_\ell$, every map $P_j\to S_\ell$ factors through its simple head $S_j$. Splitting and [Schur lemma](../../../representation-theory.md#schur-s-lemma) give $\dim_k\operatorname{Hom}_{kG}(P_j,S_\ell)=\delta_{j\ell}$. Exactness of this Hom functor along a [composition series](../../../finite-group-theory.md#composition-series) therefore gives

$$
\dim_k\operatorname{Hom}_{kG}(P_j,\overline W_i)=d_{ij}.
$$

Part (iii) identifies this with $\dim_K\operatorname{Hom}_{KG}(Q_j,V_i)$. By [Maschke's theorem](../../../representation-theory.md#maschke-s-theorem) and splitting, $KG$ is split semisimple, so

$$
Q_j\cong\bigoplus_i V_i^{\oplus d_{ij}}.
$$

The reductions of any two integral forms of the same ordinary module have identical [Brauer characters](../../../representation-theory.md#brauer-character), hence identical composition multiplicities. We may thus reduce a direct-sum form for the displayed decomposition instead of $\widetilde P_j$. In the [modular representation ring](../../../representation-theory.md#modular-representation-ring) this gives

$$
[P_j]=\sum_i d_{ij}[\overline W_i]=\sum_\ell\left(\sum_i d_{i\ell}d_{ij}\right)[S_\ell].
$$

Comparing the simple basis coefficients proves $c_{\ell j}=\sum_i d_{i\ell}d_{ij}$, or $\boxed{C=D^TD}$.

## 5

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For the preliminary definitions, a block is $Re$ for a primitive central [idempotent](../../../commutative-algebra.md#idempotent) $e$, and a [module](../../../module-theory.md#module-mathematics) belongs to it when $eM=M$. For a [semisimple algebra](../../../associative-algebra.md#semisimple-algebra), the [Artin–Wedderburn theorem](../../../associative-algebra.md#artin-wedderburn-theorem) identifies its blocks with the factors $M_{n_i}(D_i)$ in its product decomposition. Each factor is a [block of a finite-dimensional algebra](../../../associative-algebra.md#block-of-a-finite-dimensional-algebra).

We prove [Ext separation of finite-length modules](../../../algebra.md#ext-separation-of-finite-length-modules). The extension hypothesis is $\operatorname{Ext}^1(S,T)=\operatorname{Ext}^1(T,S)=0$ for simples in opposite sets. First, for a simple $S\in\mathcal C_1$ and a module $N$ of finite [composition length](../../../finite-group-theory.md#composition-length) with factors in $\mathcal C_2$, we have $\operatorname{Ext}^1(S,N)=0$. Induct on the length of $N$: for $0\to N'\to N\to T\to0$ with $T$ simple, the long exact sequence of the [Ext functor](../../../algebra.md#ext-functor) contains

$$
\operatorname{Ext}^1(S,N')\longrightarrow\operatorname{Ext}^1(S,N)\longrightarrow\operatorname{Ext}^1(S,T),
$$

whose outer groups are zero. The same argument works with the two sets interchanged.

Now induct on the length of $M$, with $M=0$ immediate. Take a simple quotient in $0\to N\to M\to S\to0$. By induction, $N=N_1\oplus N_2$ with factors in the respective sets. Suppose $S\in\mathcal C_1$; the other case is symmetric. Quotienting by $N_1$ gives

$$
0\longrightarrow N_2\longrightarrow M/N_1\longrightarrow S\longrightarrow0.
$$

This splits by the preceding Ext vanishing. Let $U_1$ be the inverse image in $M$ of the chosen complementary copy of $S$. Then $U_1\cap N_2=0$, $U_1+N_2=M$, and $0\to N_1\to U_1\to S\to0$. Thus $U_1$ has only factors in $\mathcal C_1$, while $U_2=N_2$ has only factors in $\mathcal C_2$.

If two finite-length modules have factors in disjoint sets, any homomorphism between them is zero: a nonzero image would, by the [Jordan–Hölder theorem](../../../finite-group-theory.md#jordan-holder-theorem), have a simple factor belonging to both sets. For any [submodule](../../../module-theory.md#submodule) $V$ of $M$ with factors in $\mathcal C_1$, projection onto $U_2$ is consequently zero, so $V\subset U_1$. The analogous argument applies to $U_2$. Hence

$$
\boxed{M=U_1\oplus U_2,\quad U_i\text{ is the unique largest submodule with factors in }\mathcal C_i}.
$$

In particular both summands are preserved by every endomorphism of $M$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

We prove $(i)\Rightarrow(iii)$, the main step in [Ext-connected components determine blocks](../../../associative-algebra.md#ext-connected-components-determine-blocks). Suppose a [block of a finite-dimensional algebra](../../../associative-algebra.md#block-of-a-finite-dimensional-algebra) $B=Re$ had more than one component of the graph of nonsplit extensions between its [simple modules](../../../module-theory.md#irreducible-module). Partition its simple types into one component and the union of the others. There are no cross-extensions, so part (a) decomposes the left regular $B$-module as $B=U_1\oplus U_2$. Both summands are nonzero: every simple $B$-module is a quotient of the regular module and therefore occurs among its composition factors.

The maximality in (a) makes these summands canonical. Every right multiplication is a left $B$-module endomorphism, so it preserves them. Thus they are two-sided ideals, and their projection $p:B\to U_1$ commutes with both left and right multiplication. Putting $f=p(e)$ gives

$$
p(x)=xf=fx\quad(x\in B),\qquad f^2=f.
$$

Since both summands are nonzero, $f\ne0,e$. This contradicts the primitivity of the central block idempotent $e$. There is therefore just one Ext component within each block, proving that simples in the same block satisfy $\boxed{S\sim T}$.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

We prove $(ii)\Rightarrow(i)$. The central block [idempotents](../../../commutative-algebra.md#idempotent) split every finite-dimensional [module](../../../module-theory.md#module-mathematics) into its block components. A nonzero [indecomposable representation](../../../representation-theory.md#indecomposable-representation), in particular an indecomposable [projective module](../../../module-theory.md#projective-module), has only one such component; otherwise these give a nontrivial direct-sum decomposition.

Every [Jordan–Hölder factor](../../../finite-group-theory.md#jordan-holder-factor) of a module in a block belongs to that block, since its central idempotent acts as identity on [submodules](../../../module-theory.md#submodule) and quotients. Thus any two simple factors of the same projective indecomposable are in the same block. Applying this along the proposed chain yields $\boxed{S,T\text{ belong to the same block}}$.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

We prove $(iii)\Rightarrow(ii)$. Consider one nonsplit [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
0\longrightarrow U\longrightarrow V\mathrel{\mathop{\longrightarrow}^{q}}W\longrightarrow0
$$

with $U,W$ simple. Lift the canonical surjection $P(W)\to W$ from the [projective cover](../../../module-theory.md#projective-cover) through $q$, obtaining $f:P(W)\to V$. Its image maps onto $W$. The intersection $\operatorname{im}f\cap U$ is either zero or $U$, since $U$ is simple. If it were zero, $q$ would identify $\operatorname{im}f$ with $W$, splitting the extension. Hence $U\subset\operatorname{im}f$, and surjectivity onto $W$ then implies $\operatorname{im}f=V$.

Therefore both $U$ and $W$ occur as [Jordan–Hölder factors](../../../finite-group-theory.md#jordan-holder-factor) of the indecomposable projective $P(W)$. Replacing every edge in an Ext chain by this observation proves (ii). Together with the preceding two implications, this proves

$$
\boxed{(i)\iff(ii)\iff(iii)}.
$$

The repeated word “projective” in the printed version of (ii) has no mathematical effect.

## 6

↑ **Parent:** [Paper 138](paper-138.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Write $A=kG$, $N=N_G(D)$ and $C=C_G(D)$. The [Brauer morphism](../../../representation-theory.md#brauer-morphism) is the coefficient projection

$$
\operatorname{Br}_D^G:A^D\longrightarrow kC,\qquad\sum_{g\in G}a_gg\longmapsto\sum_{g\in C}a_gg,
$$

where the superscript $D$ denotes invariance under conjugation. This is an algebra homomorphism: for $c\in C$, the pairs $(x,y)$ with $xy=c$ are permuted by $D$; their coefficient products are constant on each orbit. Every nonfixed orbit has size divisible by $p$ and contributes zero. The fixed pairs are exactly $x,y\in C$, giving the coefficient of $c$ in the product of the projections. It is surjective since $kC\subset A^D$.

We need two trace facts. The kernel is

$$
\ker\operatorname{Br}_D^G=\sum_{Q<D}\operatorname{Tr}_Q^D(A^Q).
$$

Indeed, a basis of $A^D$ consists of conjugation-orbit sums. Nonfixed orbit sums are traces from their proper stabilizers, while fixed basis elements are exactly the elements of $C$. Traces from proper subgroups have zero coefficient at every fixed element, proving the reverse inclusion. Second, [Brauer morphism and relative trace](../../../representation-theory.md#brauer-morphism-and-relative-trace) gives

$$
\operatorname{Br}_D^G\bigl(\operatorname{Tr}_D^G(a)\bigr)=\operatorname{Tr}_D^N\bigl(\operatorname{Br}_D^G(a)\bigr).
$$

One can see this by letting $D$ act on the cosets $G/D$: fixed cosets are exactly $N/D$, and all other orbit contributions vanish after projection. More generally, $\operatorname{Br}_E^G(\operatorname{Tr}_D^G(A^D))=0$ unless $E$ is conjugate into $D$.

Set $I_D=\operatorname{Tr}_D^G(A^D)$ and $J_D=\operatorname{Tr}_D^N(kC)=(kC)_D^N$. The first is an ideal of the [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra) $Z(A)$; the second is an ideal of $(kC)^N$, which is commutative because $C\subset N$. The displayed trace identity and surjectivity of the Brauer projection give a surjective algebra homomorphism

$$
\operatorname{Br}_D^G:I_D\twoheadrightarrow J_D.
$$

The ideals can lack identities, so we justify the required idempotent argument. A finite-dimensional commutative algebra is a product of [Artinian local rings](../../../algebra.md#artinian-local-ring). Its ideal intersects each local factor either in the whole factor, containing its identity, or in a proper [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal). Under a surjection of such ideals, the proper parts have nilpotent image. Each nonzero image of a local-factor identity has a local corner algebra, a quotient of that factor, and is therefore primitive. If $u$ is the sum of these nonzero images, then $j-uj$ lies in the nilpotent image of the proper-factor ideals for every $j$ in the target; an idempotent has $j-uj=0$. Its components in the local corners are consequently zero or the corner identities. These orthogonal images account for every primitive idempotent in the target, because what remains is nilpotent. Thus [primitive idempotents under a surjection of commutative Artinian ideals](../../../commutative-algebra.md#primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals) apply: the primitive idempotents of $J_D$ correspond exactly to primitive central idempotents $b\in I_D$ with $\operatorname{Br}_D^G(b)\ne0$.

To identify these with the required blocks, we prove the [trace criterion for defect groups](../../../representation-theory.md#trace-criterion-for-defect-groups). Choose a subgroup $D_0$ of smallest order with $b\in I_{D_0}$. Such a subgroup exists: for a Sylow $p$-subgroup $P$, $b=\operatorname{Tr}_P^G(b/[G:P])$. If $\operatorname{Br}_{D_0}^G(b)=0$, write $b=\operatorname{Tr}_{D_0}^G(a)$ and replace $a$ by $ba$. The kernel formula and transitivity of trace would give

$$
b\in\sum_{Q<D_0}I_Q.
$$

Multiplying by $b$ gives the identity of the local algebra $bZ(A)$ in a sum of the ideals $bI_Q$. If all were proper, they would lie in its unique maximal ideal; hence some $bI_Q$ contains $b$, contradicting minimality. Therefore $\operatorname{Br}_{D_0}^G(b)\ne0$.

The general trace-vanishing assertion shows that any $E$ with nonzero Brauer image is conjugate into $D_0$. Conversely, every conjugate of $D_0$ has nonzero image. Hence the maximal such subgroups, each called a [defect group of a block](../../../representation-theory.md#defect-group-of-a-block), are precisely the conjugates of $D_0$. It also follows, using trace transitivity, that $b\in I_D$ if and only if a defect group is conjugate into $D$. Combining this with $\operatorname{Br}_D^G(b)\ne0$ forces equality of the subgroup orders, so the idempotents singled out above are exactly those with defect group $D$.

We have proved the desired bijection

$$
\boxed{b\longmapsto\operatorname{Br}_D^G(b):\{\text{blocks of }kG\text{ with defect }D\}\overset{\sim}{\longrightarrow}\operatorname{Prim}(J_D)}.
$$

Finally, [Brauer first main theorem](../../../representation-theory.md#brauer-first-main-theorem) states that these blocks correspond bijectively to the blocks of $kN_G(D)$ with defect group $D$. Apply the same argument to $N$: its normalizer of $D$ is itself and its centralizer of $D$ is still $C$. The target ideal is therefore the same $J_D$. Matching the two bijections proves the theorem and gives the [Brauer correspondence](../../../representation-theory.md#brauer-correspondence), characterized by equal nonzero Brauer images. Notice that we never assume the entire kernel on $I_D$ is nilpotent; it may kill whole blocks of smaller defect.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Take $D=\langle(12)(34)\rangle$ and

$$
P=\{1,(12)(34),(13)(24),(14)(23)\}.
$$

Every involution in $A_5$ is a double transposition. They form one conjugacy class: an odd $S_5$ conjugator can be made even by multiplying by a transposition centralizing the source double transposition. Thus all order-two subgroups of $A_5$ are conjugate. Since $|A_5|=60$, $P$ is a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup). A permutation normalizing $P$ fixes its unique common fixed letter, $5$, and every even permutation of the other four letters permutes its three double transpositions. Hence $N_{A_5}(P)=A_4$. Any permutation centralizing $(12)(34)$ fixes $5$; within $S_4$ it may exchange the two pairs and interchange letters in either pair, giving eight possibilities, of which exactly the four elements of $P$ are even. Thus $C_{A_5}(D)=P$. Since $P$ is abelian and contains $D$, also $C_{A_5}(P)=P$.

The given single block of $kA_4$ has identity $1$ and defect $P$, since $\operatorname{Br}_P^{A_4}(1)=1$ and $P$ is Sylow. By [Brauer first main theorem](../../../representation-theory.md#brauer-first-main-theorem), $kA_5$ has exactly one block with defect $P$.

Suppose a block idempotent $b$ had defect $D$. Then $\operatorname{Br}_D^{A_5}(b)$ is a nonzero idempotent in $kP$. A [group algebra of a p-group in characteristic p is local](../../../representation-theory.md#group-algebra-of-a-p-group-in-characteristic-p-is-local), so this image is $1$. But both the Brauer projections at $D$ and at $P$ retain exactly the basis elements of the same centralizer $P$. Consequently

$$
\operatorname{Br}_P^{A_5}(b)=\operatorname{Br}_D^{A_5}(b)=1.
$$

Thus $b$ has the full Sylow defect $P$, contradicting maximality of $D$. These are the [2-modular defect groups of A5](../../../representation-theory.md#2-modular-defect-groups-of-a5), and $\boxed{C_2\text{ cannot be a defect group}}$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Put $a=(123)$ and $t=(12)$. Conjugation by $a$ fixes the three given idempotents of $k\langle a\rangle$, while $tat^{-1}=a^{-1}$ fixes $e_1$ and interchanges $e_2,e_3$. Their orbits are therefore $\boxed{\{e_1\},\{e_2,e_3\}}$, with central orbit sums

$$
b_0=e_1=1+a+a^2,\qquad b_1=e_2+e_3=a+a^2,
$$

using $\omega+\omega^2=1$ in characteristic $2$.

To ensure these sums really are primitive central idempotents, examine the two ideals. The first has basis $b_0,b_0t$, with $b_0a=b_0$, so $b_0kG\cong kC_2$, a [local ring](../../../commutative-algebra.md#local-ring). The second has dimension $4$: $b_1k\langle a\rangle=ke_2\oplus ke_3$ has dimension $2$, and the two cosets of $\langle a\rangle$ double it. In the two-dimensional representation

$$
a\longmapsto\begin{pmatrix}\omega&0\\0&\omega^2\end{pmatrix},\qquad t\longmapsto\begin{pmatrix}0&1\\1&0\end{pmatrix},
$$

These matrices satisfy $a^3=t^2=1$ and $tat^{-1}=a^{-1}$, so they define a representation of $S_3$. In it, $b_1$ acts as identity and $b_0$ as zero. The distinct diagonal entries supply the two diagonal matrix units, and multiplying by the swap matrix supplies the off-diagonal units. The induced map $b_1kG\to M_2(k)$ is thus surjective and, by dimension, an isomorphism. Both summands have no nontrivial central idempotents, so $b_0,b_1$ are exactly the [2-modular blocks of S3](../../../representation-theory.md#2-modular-blocks-of-s3).

The [Brauer morphism](../../../representation-theory.md#brauer-morphism) at the trivial subgroup is the identity. For $H=\langle t\rangle$, $C_G(H)=H$, and neither $a$ nor $a^2$ lies in this centralizer. Thus

$$
\boxed{\begin{array}{c|c|c|c}
\text{block}&\operatorname{Br}_1^G&\operatorname{Br}_H^G&\text{defect group}\\\hline
b_0=1+a+a^2&b_0&1&H\\
b_1=a+a^2&b_1&0&1
\end{array}}.
$$

Indeed $H$ is Sylow, and all nontrivial $2$-subgroups are conjugate to it; these images therefore determine maximality in the definition of a [defect group of a block](../../../representation-theory.md#defect-group-of-a-block). The original PDF provides the $S_3,\mathbb F_4,N,H$ setup missing from the TeX transcription.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
