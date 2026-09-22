# Paper 151

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_151.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_151.pdf)

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

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $P_\bullet\to\mathbb Z$ be a [projective resolution](../../../algebra.md#projective-resolution) of the trivial $\mathbb ZG$-module. The [projective-resolution definition of group cohomology](../../../group-theory.md#projective-resolution-definition-of-group-cohomology) is

$$
H^n(G,M)=H^n\!\left(\operatorname{Hom}_{\mathbb ZG}(P_\bullet,M)\right).
$$

This is independent, up to a natural [isomorphism](../../../algebra.md#isomorphism), of the chosen [projective resolution](../../../algebra.md#projective-resolution).

The degreewise natural isomorphisms

$$
\operatorname{Hom}_{\mathbb ZG}(P_j,M_1\oplus M_2)
\cong\operatorname{Hom}_{\mathbb ZG}(P_j,M_1)
\oplus\operatorname{Hom}_{\mathbb ZG}(P_j,M_2)
$$

commute with the [coboundary maps](../../../algebra.md#coboundary-map). Taking [cohomology](../../../cohomology.md) proves that [group cohomology commutes with finite direct sums](../../../group-theory.md#group-cohomology-commutes-with-finite-direct-sums):

$$
H^n(G,M_1\oplus M_2)
\cong H^n(G,M_1)\oplus H^n(G,M_2).
$$

Now restrict $P_\bullet$ from $G$ to a subgroup $K$. The [group ring](../../../commutative-algebra.md#group-ring) $\mathbb ZG$ is free as a $\mathbb ZK$-module, so restriction carries [free modules](../../../module-theory.md#free-module) to free modules and [projective modules](../../../module-theory.md#projective-module) to projective modules. Thus the restricted complex is a [projective resolution](../../../algebra.md#projective-resolution) of the trivial $\mathbb ZK$-module. For the [coinduced module](../../../group-theory.md#coinduced-module) $Y=\operatorname{Hom}_{\mathbb ZK}(\mathbb ZG,X)$, the [Hom functor adjunction for a coinduced module](../../../group-theory.md#hom-functor-adjunction-for-a-coinduced-module) gives an isomorphism of [cochain complexes](../../../algebra.md#cochain-complex)

$$
\operatorname{Hom}_{\mathbb ZG}(P_\bullet,Y)
\cong\operatorname{Hom}_{\mathbb ZK}(P_\bullet,X).
$$

Explicitly, a map $F$ is sent to $p\mapsto F(p)(1)$; the inverse sends a $\mathbb ZK$-linear map $a$ to $p\mapsto(r\mapsto a(rp))$. Taking [cohomology](../../../cohomology.md) proves [Shapiro's lemma](../../../group-theory.md#shapiro-s-lemma):

$$
H^n(G,Y)\cong H^n(K,X).
$$

For the [conjugation module of a group ring](../../../group-theory.md#conjugation-module-of-a-group-ring) $N=\mathbb ZG_{\mathrm{conj}}$, the basis $G$ is the disjoint union of its [conjugacy classes](../../../group-theory.md#conjugacy-class). Hence $N$ is the [direct sum](../../../vector-space.md#direct-sum) of the integral permutation modules on those classes. The class of a representative $g_i$ is the transitive $G$-set $G/C_G(g_i)$, where $C_G(g_i)$ is its [centralizer](../../../group-theory.md#centralizer). Since $G$ is finite, this permutation module is both induced and coinduced from the trivial $C_G(g_i)$-module $\mathbb Z$. Applying [group cohomology commutes with finite direct sums](../../../group-theory.md#group-cohomology-commutes-with-finite-direct-sums) and [Shapiro's lemma](../../../group-theory.md#shapiro-s-lemma) yields the [group cohomology of a conjugation module](../../../group-theory.md#group-cohomology-of-a-conjugation-module):

$$
H^n(G,N)\cong\bigoplus_iH^n(C_G(g_i),\mathbb Z).
$$

The [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_3$ has three [conjugacy classes](../../../group-theory.md#conjugacy-class), represented by the identity, a transposition, and a three-cycle. Their [centralizers](../../../group-theory.md#centralizer) are respectively

$$
S_3,\qquad C_2,\qquad C_3.
$$

For any [finite group](../../../group.md#finite-group) $L$ acting trivially on $\mathbb Z$,

$$
H^1(L,\mathbb Z)=\operatorname{Hom}(L,\mathbb Z)=0,
$$

because a [group homomorphism](../../../group-theory.md#group-homomorphism) sends an element of finite order to an element of finite order, while the [additive group](../../../group.md#additive-group) of the integers contains no nonzero [torsion elements](../../../group-theory.md#torsion-element). Therefore

$$
H^1(S_3,N)=0.
$$

The [periodic resolution of a finite cyclic group](../../../group-theory.md#periodic-resolution-of-a-finite-cyclic-group) alternates the maps $t-1$ and $1+t+\cdots+t^{m-1}$. After applying $\operatorname{Hom}_{\mathbb ZC_m}(-,\mathbb Z)$ with the trivial action, these become alternately zero and multiplication by $m$, proving

$$
H^2(C_m,\mathbb Z)\cong\mathbb Z/m\mathbb Z.
$$

Combining this calculation with the supplied $H^2(S_3,\mathbb Z)\cong\mathbb Z/2\mathbb Z$ gives

$$
\boxed{H^2(S_3,N)
\cong\mathbb Z/2\mathbb Z\oplus\mathbb Z/2\mathbb Z\oplus\mathbb Z/3\mathbb Z.}
$$

## 2

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Schur multiplier](../../../group-theory.md#schur-multiplier) of a [group](../../../group.md) $G$ is

$$
M(G)=H_2(G,\mathbb Z),
$$

the second [group homology](../../../group-theory.md#group-homology) group with trivial integral coefficients. If $G\cong F/R$ is a [free presentation](../../../geometric-group-theory.md#free-presentation), [Hopf's formula](../../../group-theory.md#hopf-s-formula) states that

$$
M(G)\cong\frac{R\cap[F,F]}{[F,R]}.
$$

Write $I_F=\ker(\mathbb ZF\to\mathbb Z)$ for the [augmentation ideal](../../../commutative-algebra.md#augmentation-ideal). The [presentation relation sequence](../../../geometric-group-theory.md#presentation-relation-sequence) is

$$
0\longrightarrow R/[R,R]
\longrightarrow\mathbb ZG\otimes_{\mathbb ZF}I_F
\longrightarrow\mathbb ZG
\longrightarrow\mathbb Z\longrightarrow0,
$$

where $r[R,R]\mapsto1\otimes(r-1)$. If $F$ is free on a set $S$, then $I_F$ is free as a left $\mathbb ZF$-module on the elements $s-1$, so the two modules immediately preceding $\mathbb Z$ are free $\mathbb ZG$-modules. Resolving the [relation module](../../../geometric-group-theory.md#relation-module) $R/[R,R]$ by free modules and splicing produces a [free resolution](../../../algebra.md#free-resolution) of $\mathbb Z$.

Apply the right-exact functor $\mathbb Z\otimes_{\mathbb ZG}-$ to this partial resolution. Its degree-two [homology](../../../homology.md) is the kernel of

$$
(R/[R,R])_G\longrightarrow
\left(\mathbb ZG\otimes_{\mathbb ZF}I_F\right)_G.
$$

The [coinvariant module](../../../module-theory.md#coinvariant-module) on the left is $R/[F,R]$. On the right, the map $f-1\mapsto f[F,F]$ identifies the coinvariants with the [abelianization](../../../group-theory.md#abelianization) $F/[F,F]$. The displayed map is induced by the inclusion $R\hookrightarrow F$, so its kernel is

$$
\ker\left(R/[F,R]\longrightarrow F/[F,F]\right)
=\frac{R\cap[F,F]}{[F,R]}.
$$

This proves [Hopf's formula](../../../group-theory.md#hopf-s-formula).

For an [abelian group](../../../group.md#abelian-group) $A$, the [Schur multiplier of an abelian group](../../../group-theory.md#schur-multiplier-of-an-abelian-group) is $M(A)\cong\bigwedge^2A$. One way to see the direct-sum rule is the degree-two [Künneth theorem](../../../cohomology.md#kunneth-theorem):

$$
H_2(A\times B,\mathbb Z)
\cong H_2(A,\mathbb Z)\oplus H_2(B,\mathbb Z)
\oplus\bigl(H_1(A,\mathbb Z)\otimes H_1(B,\mathbb Z)\bigr).
$$

A [cyclic group](../../../group.md#cyclic-group) has zero second integral [group homology](../../../group-theory.md#group-homology), while

$$
C_m\otimes_{\mathbb Z}C_n\cong C_{\gcd(m,n)}.
$$

Consequently

$$
\boxed{M(C_2\times C_4\times C_6)
\cong C_{\gcd(2,4)}\oplus C_{\gcd(2,6)}\oplus C_{\gcd(4,6)}
\cong C_2\oplus C_2\oplus C_2.}
$$

## 3

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $a,b\in I$, the [square-zero ideal](../../../commutative-algebra.md#square-zero-ideal) condition gives

$$
(1+a)(1+b)=1+a+b+ab=1+a+b,
\qquad (1+a)^{-1}=1-a.
$$

Thus the [square-zero unit subgroup](../../../commutative-algebra.md#square-zero-unit-subgroup) $1+I$ is abelian, and

$$
I_{\mathrm{add}}\longrightarrow1+I,
\qquad a\longmapsto1+a
$$

is a [group isomorphism](../../../algebra.md#group-isomorphism) from the [additive group](../../../group.md#additive-group) of $I$.

Use the specified [ring isomorphism](../../../algebra.md#ring-isomorphism) $R/I\cong\mathbb ZG$. For $x\in\mathbb ZG$, choose a lift $r\in R$ and define $x\cdot a=ra$ for $a\in I$. Two lifts differ by an element of $I$, whose product with $a$ vanishes, so this is well defined. Right multiplication is handled identically. The two actions commute by [associativity](../../../group.md#associative-property), making $I$ a [bimodule](../../../module-theory.md#bimodule). If $u\in R$ lifts $g\in G$, then $u$ is a [unit](../../../algebra.md#unit-in-a-ring): a lift $v$ of $g^{-1}$ makes both $uv$ and $vu$ elements of $1+I$, hence units, and a ring element with both a left and a right inverse is invertible. Conjugation therefore defines

$$
g\cdot a=uau^{-1}.
$$

Changing $u$ by an element of $I$ does not change this expression because $I^2=0$. Moreover,

$$
u(1+a)u^{-1}=1+uau^{-1},
$$

so $a\mapsto1+a$ is an isomorphism of $\mathbb ZG$-modules for these [conjugation actions](../../../group-theory.md#conjugation-action).

Let $R^\times\to(R/I)^\times$ be reduction on [unit groups](../../../algebra.md#unit-group), and define $U$ as the inverse image of the distinguished subgroup $G\subseteq(\mathbb ZG)^\times$. Every $g\in G$ has a unit lift by the preceding argument, and the kernel consists exactly of the units congruent to $1$, namely $1+I$. Multiplication in $R$ therefore gives the [group extension](../../../group-theory.md#group-extension)

$$
1\longrightarrow1+I\longrightarrow U\longrightarrow G\longrightarrow1.
$$

Choose a set-theoretic section $s:G\to U$ with $s(1)=1$. Its [extension cocycle](../../../group-theory.md#extension-cocycle)

$$
c(g,h)=s(g)s(h)s(gh)^{-1}\in1+I
$$

satisfies the [two-cocycle](../../../group-theory.md#two-cocycle) identity by [associativity](../../../group.md#associative-property). A different section changes $c$ by a [group coboundary](../../../group-theory.md#group-coboundary), so [second group cohomology classifies group extensions](../../../group-theory.md#second-group-cohomology-classifies-group-extensions) gives a well-defined class

$$
x=[c]\in H^2(G,1+I).
$$

The same construction for $(R_1,I_1)$ gives $U_1$, an extension cocycle $c_1$, and $x_1=[c_1]\in H^2(G,1+I_1)$.

The answer to the final question is no. An abstract [ring isomorphism](../../../algebra.md#ring-isomorphism) $R_1\cong R$ need not carry the distinguished ideal $I_1$ to $I$, need not induce the identity under the two chosen identifications of the [quotient rings](../../../commutative-algebra.md#quotient-ring) with $\mathbb ZG$, and need not induce the prescribed $\mathbb ZG$-module isomorphism $\theta$. Hence it need not give an isomorphism of the two displayed [group extensions](../../../group-theory.md#group-extension), so it imposes no equality $\phi(x_1)=x$. That equality does hold if the ring isomorphism has all three compatibility properties, because it then carries one extension cocycle to the other up to a [group coboundary](../../../group-theory.md#group-coboundary).

## 4

↑ **Parent:** [Paper 151](paper-151.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Put $Q=G/H$ and write $M^H$ for the [invariant submodule](../../../module-theory.md#invariant-submodule). The [five-term exact sequence in group cohomology](../../../group-theory.md#five-term-exact-sequence-in-group-cohomology) associated with the [Lyndon–Hochschild–Serre spectral sequence](../../../group-theory.md#lyndon-hochschild-serre-spectral-sequence) is

$$
0\longrightarrow H^1(Q,M^H)
\xrightarrow{\operatorname{inf}}H^1(G,M)
\xrightarrow{\operatorname{res}}H^1(H,M)^Q
\xrightarrow{d_2}H^2(Q,M^H)
\xrightarrow{\operatorname{inf}}H^2(G,M).
$$

The [inflation map in group cohomology](../../../group-theory.md#inflation-map-in-group-cohomology) composes a cocycle on $Q$ with the quotient homomorphism $G\to Q$. The [restriction map in group cohomology](../../../group-theory.md#restriction-map-in-group-cohomology) restricts a cocycle from $G$ to $H$. The quotient action on the middle term is, for $q=gH$ and a [one-cocycle](../../../group-theory.md#one-cocycle) $f$,

$$
q\cdot[f]=\left[h\longmapsto g\cdot f(g^{-1}hg)\right].
$$

This is independent of the lift and of the representative at the level of [cohomology](../../../cohomology.md). Finally, the [transgression in group cohomology](../../../group-theory.md#transgression-in-group-cohomology) extends a $Q$-invariant class on $H$ to a one-cochain on $G$; its coboundary is $H$-basic and descends to the two-cocycle on $Q$ representing $d_2[f]$. Changing the extension changes that cocycle by a [group coboundary](../../../group-theory.md#group-coboundary).

For the application, choose free generators $x_1,\ldots,x_n$ of $F$ and normal generators $r_1,\ldots,r_n$ of $R$. Since a [finite nonabelian simple group](../../../finite-group-theory.md#finite-nonabelian-simple-group) $K$ is a [perfect group](../../../group-theory.md#perfect-group), its abelianization is zero. The five-term sequence for $1\to R\to F\to K\to1$ with trivial coefficients contains

$$
0\longrightarrow\operatorname{Hom}(K,\mathbb Z)
\longrightarrow\operatorname{Hom}(F,\mathbb Z)
\xrightarrow{\operatorname{res}}\operatorname{Hom}(R,\mathbb Z)^K
\longrightarrow H^2(K,\mathbb Z)
\longrightarrow H^2(F,\mathbb Z).
$$

The first term is zero because $K$ is finite, and the last term is zero because a [free group](../../../geometric-group-theory.md#free-group) has cohomological dimension one. It remains to prove that restriction is surjective.

The [invariant submodule](../../../module-theory.md#invariant-submodule) of homomorphisms $R\to\mathbb Z$ is exactly

$$
\operatorname{Hom}(R/[F,R],\mathbb Z).
$$

The images of the relators $r_1,\ldots,r_n$ generate $R/[F,R]$, so such a homomorphism $\lambda$ is determined by the integer vector $b=(\lambda(r_1),\ldots,\lambda(r_n))^T$. Let $A$ be the [relator exponent-sum matrix](../../../geometric-group-theory.md#relator-exponent-sum-matrix). This square integer matrix presents $K^{\mathrm{ab}}$, which is zero, so $A$ is a [unimodular matrix](../../../linear-algebra.md#unimodular-matrix). There is therefore an integer vector $v$ satisfying $Av=b$. Define $\psi:F\to\mathbb Z$ by assigning to $x_i$ the $i$th entry of $v$. The definition of $A$ gives $\psi(r_j)=\lambda(r_j)$ for every $j$. Since the relator images generate $R/[F,R]$, the restriction of $\psi$ to $R$ equals $\lambda$. Restriction is surjective, exactness now gives

$$
\boxed{H^2(K,\mathbb Z)=0.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
