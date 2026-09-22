# Finite group theory

↑ **Parent:** [Group theory](group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_group_theory)

Finite group theory studies groups with finitely many elements.

**Table of contents**

- [Fitting subgroup](#fitting-subgroup)
  - [Fitting subgroup is self-centralizing in soluble groups](#fitting-subgroup-is-self-centralizing-in-soluble-groups)
  - [Fitting subgroup centralizes the socle](#fitting-subgroup-centralizes-the-socle)
  - [Nilpotent normal subgroup](#nilpotent-normal-subgroup)
  - [p-core](#p-core)
- [Classification of groups of order ten](#classification-of-groups-of-order-ten)
- [Almost simple group](#almost-simple-group)
- [Heisenberg group over a prime field](#heisenberg-group-over-a-prime-field)
- [Tetrahedral symmetry](#tetrahedral-symmetry)
- [Group of order eight](#group-of-order-eight)
- [Feit–Thompson theorem](#feit-thompson-theorem)
- [Alternating group](#alternating-group)
  - [Maximal subgroups of A5](#maximal-subgroups-of-a5)
  - [Automorphisms of alternating groups from triple supports](#automorphisms-of-alternating-groups-from-triple-supports)
  - [Connected triple supports generate an alternating group](#connected-triple-supports-generate-an-alternating-group)
  - [Conjugacy classes of the alternating group on six letters](#conjugacy-classes-of-the-alternating-group-on-six-letters)
- [P-group](#p-group)
- [Symmetric group](#symmetric-group)
  - [Automorphisms of the symmetric group](#automorphisms-of-the-symmetric-group)
    - [Symmetric-group involution class-size collision](#symmetric-group-involution-class-size-collision)
  - [Permutation group](#permutation-group)
    - [Oligomorphic permutation group](#oligomorphic-permutation-group)
  - [A cycle and a transposition generate the symmetric group exactly at coprime separation](#a-cycle-and-a-transposition-generate-the-symmetric-group-exactly-at-coprime-separation)
  - [Transpositions on a connected graph generate the symmetric group](#transpositions-on-a-connected-graph-generate-the-symmetric-group)
  - [Parity of a permutation](#parity-of-a-permutation)
    - [Sign homomorphism](#sign-homomorphism)
  - [Permutation cycle](#permutation-cycle)
    - [Cycle type](#cycle-type)
      - [Permutation order and sign do not determine conjugacy](#permutation-order-and-sign-do-not-determine-conjugacy)
      - [Permutation conjugate to its square](#permutation-conjugate-to-its-square)
      - [Transposition changes the cycle count by one](#transposition-changes-the-cycle-count-by-one)
    - [Three-cycle](#three-cycle)
    - [Disjoint permutation cycles](#disjoint-permutation-cycles)
  - [Support of a permutation](#support-of-a-permutation)
  - [Sign of a permutation](#sign-of-a-permutation)
    - [Odd permutation](#odd-permutation)
    - [Even permutation](#even-permutation)
- [Quaternion group](#quaternion-group)
  - [Minimal faithful permutation degree of the quaternion group](#minimal-faithful-permutation-degree-of-the-quaternion-group)
- [Dicyclic group](#dicyclic-group)
  - [Order-twelve dicyclic character table](#order-twelve-dicyclic-character-table)
  - [Dicyclic character table](#dicyclic-character-table)
- [Finite p-group](#finite-p-group)
  - [p-subgroup](#p-subgroup)
    - [p-radical subgroup](#p-radical-subgroup)
  - [Lower p-series](#lower-p-series)
  - [Powerful p-group](#powerful-p-group)
    - [Minimal cyclic factorization criterion for powerful p-groups](#minimal-cyclic-factorization-criterion-for-powerful-p-groups)
    - [Subgroup generator bound for a powerful finite p-group](#subgroup-generator-bound-for-a-powerful-finite-p-group)
    - [Power lifting in a powerful p-group](#power-lifting-in-a-powerful-p-group)
    - [Powerfully embedded subgroup](#powerfully-embedded-subgroup)
  - [Classification of groups of order p squared](#classification-of-groups-of-order-p-squared)
  - [Normalizer condition for finite p-groups](#normalizer-condition-for-finite-p-groups)
  - [Central intersection property of normal subgroups of finite p-groups](#central-intersection-property-of-normal-subgroups-of-finite-p-groups)
  - [Nontrivial center of a finite p-group](#nontrivial-center-of-a-finite-p-group)
  - [Frattini subgroup](#frattini-subgroup)
    - [Frattini lifting of nilpotence](#frattini-lifting-of-nilpotence)
    - [Non-generator of a finite group](#non-generator-of-a-finite-group)
    - [Frattini quotient](#frattini-quotient)
      - [Burnside basis theorem](#burnside-basis-theorem)
- [Simple group](#simple-group)
  - [Finite simple group](#finite-simple-group)
  - [Simple groups with order a power of two times fifteen](#simple-groups-with-order-a-power-of-two-times-fifteen)
  - [Iwasawa simplicity lemma](#iwasawa-simplicity-lemma)
  - [Simplicity of the alternating group on six letters](#simplicity-of-the-alternating-group-on-six-letters)
  - [Simplicity of alternating groups](#simplicity-of-alternating-groups)
  - [Finite nonabelian simple group](#finite-nonabelian-simple-group)
    - [Least-prime divisibility constraint for a finite simple group](#least-prime-divisibility-constraint-for-a-finite-simple-group)
    - [Mathieu group](#mathieu-group)
    - [Ree group of type G2](#ree-group-of-type-g2)
    - [Suzuki group of Lie type](#suzuki-group-of-lie-type)
  - [Simplicity of the alternating group A5](#simplicity-of-the-alternating-group-a5)
  - [Smallest nonabelian simple group](#smallest-nonabelian-simple-group)
- [General linear group over a finite field](#general-linear-group-over-a-finite-field)
  - [Conjugacy-class generating function for finite general linear groups](#conjugacy-class-generating-function-for-finite-general-linear-groups)
  - [Unitary group over a finite field](#unitary-group-over-a-finite-field)
  - [Projective special unitary group over a finite field](#projective-special-unitary-group-over-a-finite-field)
  - [Parabolic stabilizer of a subspace](#parabolic-stabilizer-of-a-subspace)
  - [Symplectic group over a finite field](#symplectic-group-over-a-finite-field)
    - [Symplectic quotient of the binary subset module](#symplectic-quotient-of-the-binary-subset-module)
    - [Perfectness of finite symplectic groups](#perfectness-of-finite-symplectic-groups)
    - [Symplectic transvection](#symplectic-transvection)
    - [Projective symplectic group over a finite field](#projective-symplectic-group-over-a-finite-field)
  - [Inverse-transpose automorphism](#inverse-transpose-automorphism)
  - [Maximal subgroups of GL3 over F2](#maximal-subgroups-of-gl3-over-f2)
    - [Elementary abelian subgroups in GL3 over F2](#elementary-abelian-subgroups-in-gl3-over-f2)
  - [Singer cycle](#singer-cycle)
  - [Order-p matrices in GL2 over the prime field](#order-p-matrices-in-gl2-over-the-prime-field)
  - [Faithful four-point action of GL2 over F2](#faithful-four-point-action-of-gl2-over-f2)
  - [Order of a general linear group over a finite field](#order-of-a-general-linear-group-over-a-finite-field)
  - [Upper unitriangular group](#upper-unitriangular-group)
    - [Center of an upper unitriangular group](#center-of-an-upper-unitriangular-group)
    - [Unitriangular matrix power formula](#unitriangular-matrix-power-formula)
    - [Unitriangular group of degree three over F3](#unitriangular-group-of-degree-three-over-f3)
  - [Projective general linear group action on the projective line](#projective-general-linear-group-action-on-the-projective-line)
    - [Sharply three-transitive on a projective line](#sharply-three-transitive-on-a-projective-line)
    - [Projective line](#projective-line)
    - [Sylow 2-subgroup of PGL2 over F4](#sylow-2-subgroup-of-pgl2-over-f4)
  - [Special linear group over a finite field](#special-linear-group-over-a-finite-field)
    - [Unique involution in SL2 over an odd field](#unique-involution-in-sl2-over-an-odd-field)
    - [SL2 over F2 as a permutation group](#sl2-over-f2-as-a-permutation-group)
    - [Projective special linear group over a finite field](#projective-special-linear-group-over-a-finite-field)
      - [Exterior-square realization of PSL4 over F2](#exterior-square-realization-of-psl4-over-f2)
      - [Projective special linear group over the field with five elements](#projective-special-linear-group-over-the-field-with-five-elements)
        - [Quaternion construction of an index-five subgroup of PSL2 over F5](#quaternion-construction-of-an-index-five-subgroup-of-psl2-over-f5)
    - [Unipotent conjugacy in SL2 over a finite field](#unipotent-conjugacy-in-sl2-over-a-finite-field)
    - [SL2 action on a finite projective line](#sl2-action-on-a-finite-projective-line)
- [Dihedral group](#dihedral-group)
  - [Dihedral splitting when the half-rotation order is odd](#dihedral-splitting-when-the-half-rotation-order-is-odd)
  - [Classification of subgroups of a dihedral group](#classification-of-subgroups-of-a-dihedral-group)
  - [Dihedral subgroups of every divisor order](#dihedral-subgroups-of-every-divisor-order)
  - [Involutions in an even dihedral group](#involutions-in-an-even-dihedral-group)
- [Sylow theorems](#sylow-theorems)
  - [Sylow basis](#sylow-basis)
    - [Counting Sylow bases in a coprime elementary abelian extension](#counting-sylow-bases-in-a-coprime-elementary-abelian-extension)
  - [Sylow existence by subset action](#sylow-existence-by-subset-action)
  - [A group of order 56 has a normal Sylow subgroup](#a-group-of-order-56-has-a-normal-sylow-subgroup)
  - [Frattini argument](#frattini-argument)
  - [Groups of order p squared q are not simple](#groups-of-order-p-squared-q-are-not-simple)
  - [Sylow subgroup](#sylow-subgroup)
  - [Nonabelian group of order pq](#nonabelian-group-of-order-pq)
    - [Nonabelian group of order 21](#nonabelian-group-of-order-21)
  - [Conjugation action on Sylow subgroups](#conjugation-action-on-sylow-subgroups)
    - [Strengthened Sylow congruence from intersections](#strengthened-sylow-congruence-from-intersections)
    - [Simple group embedding from Sylow conjugation](#simple-group-embedding-from-sylow-conjugation)
  - [Sylow subgroups of S3, S4 and A5](#sylow-subgroups-of-s3-s4-and-a5)
  - [Sylow containment from a coset fixed point](#sylow-containment-from-a-coset-fixed-point)
  - [Sylow counts in a faithful degree-seven action with S4 point stabilizers](#sylow-counts-in-a-faithful-degree-seven-action-with-s4-point-stabilizers)
  - [Even-involution coset fixed-point lemma](#even-involution-coset-fixed-point-lemma)
- [Cauchy theorem for groups](#cauchy-theorem-for-groups)
  - [Cyclic-tuple proof of Cauchy theorem](#cyclic-tuple-proof-of-cauchy-theorem)
- [Power-map criterion for a finite group](#power-map-criterion-for-a-finite-group)
- [Composition series](#composition-series)
  - [Composition chains in products with S5](#composition-chains-in-products-with-s5)
  - [Composition length](#composition-length)
  - [Jordan–Hölder factor](#jordan-holder-factor)
    - [Jordan–Hölder theorem](#jordan-holder-theorem)
- [Klein four-group](#klein-four-group)

## Fitting subgroup

↑ **Parent:** [Finite group theory](finite-group-theory.md)

The largest [nilpotent normal subgroup](#nilpotent-normal-subgroup) of a [finite group](group.md#finite-group) $G$. If $O_p(G)$ denotes its [p-core](#p-core), distinct [p-cores](#p-core) commute, and $F(G)=\prod_pO_p(G)$. Every normal [nilpotent group](group-theory.md#nilpotent-group) has [Sylow subgroups](#sylow-subgroup) which are [characteristic subgroups](algebra.md#characteristic-subgroup), so it is contained in this product.

### Fitting subgroup is self-centralizing in soluble groups

↑ **Parent:** [Fitting subgroup](#fitting-subgroup)

In a finite [soluble group](group-theory.md#solvable-group), $C_G(F(G))\le F(G)$. Put $C=C_G(F)$ and $D=C\cap F=Z(F)$. If $C>D$, choose an elementary abelian [minimal normal subgroup](group-theory.md#minimal-normal-subgroup) of $G/D$ inside $C/D$, and let $K$ be its preimage. Then $K'\le D\le Z(K)$, so $K$ is a [nilpotent normal subgroup](#nilpotent-normal-subgroup), contradicting $K\not\le F$.

### Fitting subgroup centralizes the socle

↑ **Parent:** [Fitting subgroup](#fitting-subgroup)

For a [finite group](group.md#finite-group), $F(G)$ centralizes its [group socle](group-theory.md#socle-of-a-finite-group). A nonabelian [minimal normal subgroup](group-theory.md#minimal-normal-subgroup) meets $F(G)$ trivially: otherwise it is nilpotent, and its nontrivial characteristic center makes it abelian. Their [group commutators](group.md#group-commutator) therefore vanish. An abelian [minimal normal subgroup](group-theory.md#minimal-normal-subgroup) $M$ is an [elementary abelian p-group](group.md#elementary-abelian-group); $M\le O_p(G)$ and $M\cap Z(O_p(G))\ne1$ by the fixed-point counting of a [finite p-group](#finite-p-group) on $M$. Minimal normality makes $M\le Z(O_p(G))$, and other [p-cores](#p-core) commute with $M$.

### Nilpotent normal subgroup

↑ **Parent:** [Fitting subgroup](#fitting-subgroup)

A [normal subgroup](group-theory.md#normal-subgroup) which is a [nilpotent group](group-theory.md#nilpotent-group). In a [finite group](group.md#finite-group) its unique [Sylow subgroups](#sylow-subgroup) are [characteristic subgroups](algebra.md#characteristic-subgroup) and hence normal in the ambient group. Products of [nilpotent normal subgroups](#nilpotent-normal-subgroup) are [nilpotent groups](group-theory.md#nilpotent-group): their normal Sylow subgroups of different prime characteristics commute.

### p-core

↑ **Parent:** [Fitting subgroup](#fitting-subgroup)

The largest normal [p-subgroup](#p-subgroup) of a [finite group](group.md#finite-group). Products of normal [p-subgroups](#p-subgroup) are again normal [p-subgroups](#p-subgroup), since $|AB|=|A||B|/|A\cap B|$. Thus the subgroup generated by all such subgroups is itself a [p-subgroup](#p-subgroup). It is a [characteristic subgroup](algebra.md#characteristic-subgroup).

## Classification of groups of order ten

↑ **Parent:** [Finite group theory](finite-group-theory.md)

A [group](group.md) of order ten is either a [cyclic group](group.md#cyclic-group) or the [dihedral group](#dihedral-group) of the pentagon. [Lagrange's theorem](group-theory.md#lagrange-s-theorem) and the fact that a group of exponent two has power-of-two order force an element of order five or ten. In the latter case the group is cyclic. In the former case its order-five [cyclic subgroup](group.md#cyclic-subgroup) is normal by index two; an outside involution acts on it either trivially or by inversion. The trivial action gives $C_5\times C_2\cong C_{10}$, and inversion gives $D_{10}$.

## Almost simple group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Almost_simple_group)

A group between a nonabelian simple group and its automorphism group. Finite two-transitive groups are either of this type or [affine two-transitive groups](group-theory.md#affine-two-transitive-group), a structural theorem rather than an order-divisibility test.

## Heisenberg group over a prime field

↑ **Parent:** [Finite group theory](finite-group-theory.md)

Upper-unitriangular three-by-three matrices over the prime [finite field](algebra.md#finite-field) form the finite analogue of the real [Heisenberg group](lie-algebra.md#heisenberg-group). In coordinates their multiplication is $(a,b,c)(a',b',c')=(a+a',b+b',c+c'+ab')$. The order is $p^3$, and $(a,b,c)^k=(ka,kb,kc+\binom{k}{2}ab)$. For odd $p$, every nonidentity element has order $p$, but the group is nonabelian. For $p=2$ the exponent statement changes, so odd characteristic is essential for the [nonisomorphic Gassmann equivalent regular subgroups](representation-theory.md#nonisomorphic-gassmann-equivalent-regular-subgroups) construction.

## Tetrahedral symmetry

↑ **Parent:** [Finite group theory](finite-group-theory.md)

A regular tetrahedron has a proper rotational symmetry group $T$ of order 12, isomorphic to the [alternating group](#alternating-group) $A_4$ acting on its four vertices. Its full spatial symmetry group $T_d$ has order 24 and is isomorphic to the [symmetric group](#symmetric-group) $S_4$; the additional operations reverse orientation. Three-fold vertex/face-axis rotations and half-turns about opposite-edge midpoints generate the proper group. The distinction matters when a field symmetry uses only proper rotations, but a scalar density also admits reflections.

## Group of order eight

↑ **Parent:** [Finite group theory](finite-group-theory.md)

Up to [group isomorphism](algebra.md#group-isomorphism), the [groups of order eight](#group-of-order-eight) are $C_8$, $C_4\times C_2$, $C_2^3$, $D_8$ and $Q_8$, with $D_8$ here denoting the eight-element [dihedral group](#dihedral-group). An element of order eight gives the first case. If every nonidentity element has order two the [group](group.md) is an [elementary abelian group](group.md#elementary-abelian-group). Otherwise, after excluding elements of order eight, a [cyclic subgroup](group.md#cyclic-subgroup) of order four has index two; an element outside it either commutes with its generator or inverts it. In the latter case its square is either the identity or the central [involution](group-theory.md#involution), giving the [dihedral group](#dihedral-group) or [quaternion group](#quaternion-group).

<h2 id="feit-thompson-theorem">Feit–Thompson theorem</h2>

↑ **Parent:** [Finite group theory](finite-group-theory.md)

Every finite [group](group.md) of odd order is a [solvable group](group-theory.md#solvable-group). In particular, a nonabelian [simple group](#simple-group) has even order and therefore has an [involution](group-theory.md#involution) by [Cauchy's theorem for finite groups](#cauchy-theorem-for-groups). This is a deep theorem, not an elementary consequence of the [Sylow theorems](#sylow-theorems).

## Alternating group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Alternating_group)

### Maximal subgroups of A5

↑ **Parent:** [Alternating group](#alternating-group)

Every maximal proper subgroup normalizes one of its [minimal normal subgroups](group-theory.md#minimal-normal-subgroup). As $A_5$ has no proper nonabelian simple subgroup, that subgroup is elementary abelian. Its possible types are $C_2,C_2^2,C_3,C_5$. Their normalizers have orders $4,12,6,10$ respectively. The order-four normalizer lies in an order-twelve point stabilizer; the other three types are maximal and each forms a single conjugacy class. There are five, six and ten maximal subgroups of orders twelve, ten and six, respectively.

### Automorphisms of alternating groups from triple supports

↑ **Parent:** [Alternating group](#alternating-group)

Except in degree six, the $3$-cycles are characterized among order-three elements by the largest [centralizer](group-theory.md#centralizer). Their cyclic subgroups correspond to three-element supports. Two different such subgroups commute exactly for disjoint supports; with one common point their generator products have order five, and with two common points those products have order two or three. Thus an automorphism induces an automorphism of $J(n,3)$. The [maximal cliques of a Johnson graph](graph-theory.md#maximal-cliques-of-a-johnson-graph) reconstruct a permutation of the points. After undoing that permutation, an automorphism fixes every cyclic $3$-subgroup. Product orders force its choices of generator inversion to be consistent on the connected graph, and inversion of every $3$-cycle would reverse a noncommuting product. Hence it fixes all $3$-cycles, which generate $A_n$.

### Connected triple supports generate an alternating group

↑ **Parent:** [Alternating group](#alternating-group)

A connected finite hypergraph of three-element supports, with a [three-cycle](#three-cycle) on each support, generates the full alternating group. To merge a new triple meeting an old alternating support in two letters, conjugate over unordered pairs of old letters. For one-letter overlap compare $(a\,b\,c)$ and $(a'\,b\,c)$: their quotient is $(a\,b\,a')$, reducing to two two-letter-overlap steps.

### Conjugacy classes of the alternating group on six letters

↑ **Parent:** [Alternating group](#alternating-group)

The [alternating conjugacy class splitting criterion](group-theory.md#alternating-conjugacy-class-splitting-criterion) gives seven [conjugacy classes](group-theory.md#conjugacy-class) in $A_6$. Their cycle types and sizes are $1^6:1$, $2^2 1^2:45$, $3 1^3:40$, $3^2:40$, $4\,2:90$, and two $5\,1$ classes of size 72. Representatives of the split classes are a 5-cycle and its square. Their sizes sum to 360. A [normal subgroup](group-theory.md#normal-subgroup) must be a union of these classes containing the identity, so these explicit sizes can prove simplicity using [Lagrange's theorem](group-theory.md#lagrange-s-theorem).

## P-group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P-group)

## Symmetric group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_group)

### Automorphisms of the symmetric group

↑ **Parent:** [Symmetric group](#symmetric-group)

An automorphism preserving the transposition class is inner: commuting relations recover the vertex stars of the complete graph, with a small-case adjustment in degrees three and four. An involution class has the same size as the transposition class only in degree six, when triple transpositions also have size fifteen. Hence [outer automorphism groups](group-theory.md#outer-automorphism-group) of symmetric groups are trivial outside degree six and have size at most two in degree six.

// Target: combinatorics.bigb

#### Symmetric-group involution class-size collision

↑ **Parent:** [Automorphisms of the symmetric group](#automorphisms-of-the-symmetric-group)

A [permutation](combinatorics.md#permutation) of order two is a product of $k$ disjoint [transpositions](combinatorics.md#transposition-permutation). Its [conjugacy class](group-theory.md#conjugacy-class) has the displayed size. For $k\geq2$, equality with the [transposition](combinatorics.md#transposition-permutation) class requires $(n-2)!/(n-2k)!=2^{k-1}k!$. The left side grows strictly with $n$. At $n=2k$, its ratio to the right side is one only for $k=3$; at $k=2$ it jumps from below to above one between $n=4$ and $n=5$, and for $k\geq4$ it is already greater than one. Thus degree six is the only possible exceptional degree for an [group automorphism](algebra.md#group-automorphism) not preserving [transpositions](combinatorics.md#transposition-permutation).

### Permutation group

↑ **Parent:** [Symmetric group](#symmetric-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Permutation_group)

A subgroup of the [symmetric group](#symmetric-group) of a set, acting faithfully by [permutations](combinatorics.md#permutation). A finite permutation group specified by generators can be enumerated by repeatedly multiplying the elements already found by those generators until no new element appears. Its orbits and conjugacy classes can then be computed directly.

#### Oligomorphic permutation group

↑ **Parent:** [Permutation group](#permutation-group)

A permutation group on a set is oligomorphic when its diagonal action on ordered $n$-tuples has finitely many orbits for every positive integer $n$. For a countable model of a complete theory, an oligomorphic automorphism group makes every finite-arity [type space](foundations-of-mathematics.md#type-space) finite: realized types are dense, and only finitely many are possible because types are constant on orbits.

### A cycle and a transposition generate the symmetric group exactly at coprime separation

↑ **Parent:** [Symmetric group](#symmetric-group)

For $n\geq2$ and $1\leq k<n$, an $n$-cycle $c=(1\,2\,\ldots\,n)$ and $t=(1\,1+k)$ generate $S_n$ exactly when $\gcd(n,k)=1$. Their conjugate [transpositions](combinatorics.md#transposition-permutation) connect labels differing by $k$ modulo $n$. This [graph](graph.md) is connected exactly at [coprime](number-theory.md#coprime-integers) separation, so [transpositions on a connected graph generate the symmetric group](#transpositions-on-a-connected-graph-generate-the-symmetric-group). Otherwise residue classes modulo $\gcd(n,k)$ form a nontrivial [block system](group-theory.md#block-system) preserved by both generators.

### Transpositions on a connected graph generate the symmetric group

↑ **Parent:** [Symmetric group](#symmetric-group)

Associate a [transposition](combinatorics.md#transposition-permutation) to each edge of a finite [connected graph](graph.md#connected-graph). For a simple path $v_0,\ldots,v_\ell$, let $t_j=(v_{j-1}\ v_j)$. Then $t_1\cdots t_{\ell-1}t_\ell t_{\ell-1}\cdots t_1=(v_0\ v_\ell)$, using rightmost-first composition. Thus edge [transpositions](combinatorics.md#transposition-permutation) generate every [transposition](combinatorics.md#transposition-permutation), and hence the full [symmetric group](#symmetric-group).

### Parity of a permutation

↑ **Parent:** [Symmetric group](#symmetric-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parity_of_a_permutation)

The parity of a permutation records whether it is a product of an even or odd number of transpositions. It is well-defined and equals the sign of the corresponding permutation matrix.

#### Sign homomorphism

↑ **Parent:** [Parity of a permutation](#parity-of-a-permutation)

The sign homomorphism sends an even permutation to $1$ and an odd permutation to $-1$; its kernel is the [alternating group](#alternating-group).

A symmetric group is the [group](group.md) of all [bijections](function.md#bijection) from a set to itself, with [function composition](algebra.md#function-composition) as its operation.

### Permutation cycle

↑ **Parent:** [Symmetric group](#symmetric-group)

A permutation cycle $(a_1\,a_2\,\ldots\,a_k)$ sends $a_i$ to $a_{i+1}$, sends $a_k$ to $a_1$, and fixes every other element. Its [order](group-theory.md#order-of-a-group-element) is $k$.

#### Cycle type

↑ **Parent:** [Permutation cycle](#permutation-cycle)

The cycle type of a [permutation](combinatorics.md#permutation) is the multiset of lengths in its decomposition into [disjoint permutation cycles](#disjoint-permutation-cycles), including one-cycles for fixed points. Two permutations in the same [symmetric group](#symmetric-group) are conjugate exactly when they have the same cycle type.

##### Permutation order and sign do not determine conjugacy

↑ **Parent:** [Cycle type](#cycle-type)

[Conjugation](group-theory.md#conjugation) preserves [order of a group element](group-theory.md#order-of-a-group-element), because $(gxg^{-1})^k=gx^kg^{-1}$, and preserves the [sign of a permutation](#sign-of-a-permutation), because sign is a [group homomorphism](group-theory.md#group-homomorphism) into $\{1,-1\}$. These invariants do not determine [cycle type](#cycle-type). In $S_6$, $(123)$ and $(123)(456)$ both have order three and positive sign, but have three and zero fixed points respectively. Conjugation relabels cycles, so these [permutations](combinatorics.md#permutation) are not conjugate.

##### Permutation conjugate to its square

↑ **Parent:** [Cycle type](#cycle-type)

Squaring an odd-length [permutation cycle](#permutation-cycle) retains its length, whereas an even-length cycle splits into two cycles of half its length. Thus if any even cycle is present, the number of cycles strictly increases, so the [cycle type](#cycle-type) changes. Since [conjugate permutations](group-theory.md#conjugate-permutation) in a [symmetric group](#symmetric-group) have the same cycle type, a permutation is conjugate to its square precisely when all its cycle lengths are odd, equivalently when its [order of a group element](group-theory.md#order-of-a-group-element) is odd.

##### Transposition changes the cycle count by one

↑ **Parent:** [Cycle type](#cycle-type)

Left multiplication of a [permutation](combinatorics.md#permutation) by a [transposition](combinatorics.md#transposition-permutation) $(a\ b)$ swaps the two target labels $a,b$. If they occur in different cycles, $(a\ x_1\ldots x_p)(b\ y_1\ldots y_q)$ becomes the single cycle $(a\ x_1\ldots x_p\ b\ y_1\ldots y_q)$. If they occur in the same cycle, that formula reverses and splits the cycle in two. All other cycles are unchanged, so the total number of cycles, including fixed points, decreases or increases by exactly one. Empty intermediate lists yield one-cycles and require no exceptional case.

#### Three-cycle

↑ **Parent:** [Permutation cycle](#permutation-cycle)

A three-cycle is a [permutation cycle](#permutation-cycle) of length three. On any chosen set of three letters, the two possible three-cycles are inverses of one another.

#### Disjoint permutation cycles

↑ **Parent:** [Permutation cycle](#permutation-cycle)

Permutation cycles with disjoint supports commute. The order of their product is the [least common multiple](number-theory.md#least-common-multiple) of their lengths.

### Support of a permutation

↑ **Parent:** [Symmetric group](#symmetric-group)

The support of a permutation is the set of elements it does not fix. A permutation has finite support when this set is finite.

### Sign of a permutation

↑ **Parent:** [Symmetric group](#symmetric-group)

The sign homomorphism $\operatorname{sgn}:S_n\to\{\pm1\}$ is the determinant of the corresponding permutation matrix. A transposition has sign $-1$, so this also proves that the parity of any transposition decomposition is well-defined.

#### Odd permutation

↑ **Parent:** [Sign of a permutation](#sign-of-a-permutation)

An odd permutation has sign $-1$, equivalently it is a product of an odd number of transpositions.

#### Even permutation

↑ **Parent:** [Sign of a permutation](#sign-of-a-permutation)

An even permutation has sign $+1$, equivalently it is a product of an even number of transpositions.

## Quaternion group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quaternion_group)

The quaternion group $Q_8=\{\pm1,\pm i,\pm j,\pm k\}$ is a nonabelian Dedekind group.

### Minimal faithful permutation degree of the quaternion group

↑ **Parent:** [Quaternion group](#quaternion-group)

The least size of a finite set on which the [quaternion group](#quaternion-group) acts faithfully is eight. Every nontrivial [subgroup](group.md#subgroup) of $Q_8$ contains its central involution $-1$. In an action on fewer than eight points, the [orbit-stabilizer theorem](group-theory.md#orbit-stabilizer-theorem) makes every [stabilizer subgroup](group-theory.md#stabilizer-subgroup) nontrivial, so $-1$ fixes every point. This rules out a [faithful group action](group-theory.md#faithful-group-action), even with several [group orbits](group-theory.md#orbit-of-a-group-action). The regular action on eight points is faithful by [Cayley theorem](group-theory.md#cayley-s-theorem).

## Dicyclic group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dicyclic_group)

The dicyclic group of order $4n$ has generators

$$
a^{2n}=1,\qquad b^2=a^n,\qquad bab^{-1}=a^{-1}.
$$

Every element has a unique form $a^k$ or $a^kb$, with $0\leq k<2n$.

### Order-twelve dicyclic character table

↑ **Parent:** [Dicyclic group](#dicyclic-group)

This [dicyclic group](#dicyclic-group) has classes $1$, $a^3$, $\{a,a^5\}$, $\{a^2,a^4\}$ and the two parity classes of $ba^j$, of sizes $1,1,2,2,3,3$. Its quotient by $\langle a^2\rangle$ is cyclic of order four, supplying four linear characters with $a\mapsto(-1)^j$, $b\mapsto i^j$. Its two remaining irreducible representations have $a\mapsto\operatorname{diag}(\zeta^k,\zeta^{-k})$ and $b\mapsto\left(\begin{smallmatrix}0&(-1)^k\\1&0\end{smallmatrix}\right)$ for $k=1,2$, where $\zeta=e^{i\pi/3}$. The traces are $2\cos(km\pi/3)$ on $a^m$ and zero on $ba^m$. Distinct diagonal eigenlines are exchanged by $b$, proving irreducibility; the degree-square sum $4+4+4=12$ proves completeness.

### Dicyclic character table

↑ **Parent:** [Dicyclic group](#dicyclic-group)

Four one-dimensional characters and $n-1$ two-dimensional characters exhaust a dicyclic group of order $4n$. In the two-dimensional rows, the values at $a^r$ are $2\cos(\pi jr/n)$ and those on the two noncyclic cosets are zero. The one-dimensional rows depend on whether $n$ is odd or even.

## Finite p-group

↑ **Parent:** [Finite group theory](finite-group-theory.md)

A finite p-group is a [finite group](group.md#finite-group) whose order is a power of one [prime number](number-theory.md#prime-number) $p$.

### p-subgroup

↑ **Parent:** [Finite p-group](#finite-p-group)

A p-subgroup is a [subgroup](group.md#subgroup) which is a [finite p-group](#finite-p-group), for a specified prime $p$. Every p-subgroup lies in a [Sylow subgroup](#sylow-subgroup).

#### p-radical subgroup

↑ **Parent:** [P-subgroup](#p-subgroup)

A [p-subgroup](#p-subgroup) is p-radical if it equals the [p-core](#p-core) of its [normalizer](group-theory.md#normalizer). Every [defect group of a block](representation-theory.md#defect-group-of-a-block) is p-radical by [defect groups are centralizer-conjugate Sylow intersections](representation-theory.md#defect-groups-are-centralizer-conjugate-sylow-intersections). Being an intersection of arbitrary Sylow subgroups alone is weaker than the [centralizer](group-theory.md#centralizer)-conjugate statement used in that argument.

### Lower p-series

↑ **Parent:** [Finite p-group](#finite-p-group)

The displayed descending [filtration](stochastic-process.md#filtration-probability-theory) combines powers and [group commutators](group.md#group-commutator). In a [pro-p group](topological-group.md#pro-p-group), take the [closure](topology.md#closure-topology) of the generated product at each step. For a [powerful p-group](#powerful-p-group) these layers are $P_i(G)=G^{p^{i-1}}$, with iterated closed power [subgroups](group.md#subgroup) in the infinite case. The successive quotients are [elementary abelian p-groups](group.md#elementary-abelian-group).

### Powerful p-group

↑ **Parent:** [Finite p-group](#finite-p-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Powerful_p-group)

A [finite p-group](#finite-p-group) is powerful if $[G,G]\leq G^p$ for odd $p$, or $[G,G]\leq G^4$ for $p=2$. Here powers denote generated [subgroups](group.md#subgroup). The same definition applies to [pro-p groups](topological-group.md#pro-p-group) using closed power and [commutator subgroups](group-theory.md#commutator-subgroup). Its [Frattini subgroup](#frattini-subgroup) is $G^p$. For odd $p$, successive power layers admit linear correction of roots, which makes every element of $G^p$ an actual $p$th power.

#### Minimal cyclic factorization criterion for powerful p-groups

↑ **Parent:** [Powerful p-group](#powerful-p-group)

For an odd [prime number](number-theory.md#prime-number) $p$, a finite [p-group](#p-group) that is a product of $d(G)$ [cyclic subgroups](group.md#cyclic-subgroup) is a [powerful p-group](#powerful-p-group). Indeed, $H=G/G^p$ has [exponent of a finite group](group-theory.md#exponent-of-a-finite-group) $p$ and the same minimal generator number $d$. Its cyclic factorization gives $|H|\leq p^d$, while its [Frattini quotient](#frattini-quotient) has order $p^d$. Thus $\Phi(H)=1$, $H$ is an [elementary abelian group](group.md#elementary-abelian-group), and $[G,G]\subseteq G^p$. The condition on the number of factors is essential: the nonabelian [Heisenberg group](lie-algebra.md#heisenberg-group) over $\mathbb F_p$ has exponent $p$ and is a product of three cyclic subgroups, although its minimal generator number is two.

#### Subgroup generator bound for a powerful finite p-group

↑ **Parent:** [Powerful p-group](#powerful-p-group)

For odd $p$, a [subgroup](group.md#subgroup) $H$ of a finite [powerful p-group](#powerful-p-group) $G$ satisfies $d(H)\le d(G)$. Here $d$ is the [dimension](vector-space.md#dimension-vector-space) of the [Frattini quotient](#frattini-quotient). Set $K=H\cap G^p$, $V=G/G^p$, $W=G^p/G^{p^2}$, and $A=HG^p/G^p$. The onto power map $\theta:V\to W$ sends $A$ into the image of $H^p$ in $K/\Phi(K)$. Since $\Phi(K)\le G^{p^2}$, this image has [dimension](vector-space.md#dimension-vector-space) at least $\dim\theta(A)$. Also $\Phi(K)\le\Phi(H)\le K$. Induction on $|G|$, applied to the powerful [subgroup](group.md#subgroup) $G^p$, gives $d(K)\le\dim W$. Consequently

$$
d(H)\le\dim A+\dim W-\dim\theta(A)\le\dim W+\dim\ker\theta=\dim V=d(G).
$$

The last inequality is [rank-nullity theorem](linear-algebra.md#rank-nullity-theorem).

#### Power lifting in a powerful p-group

↑ **Parent:** [Powerful p-group](#powerful-p-group)

For odd $p$, set $P_0=G$ and $P_{i+1}=P_i^p$. Powerful embedding gives $[P_i,G]\leq P_{i+1}$. Modulo $P_{i+2}$, commutators with $P_i$ are central and have exponent dividing $p$, so $(xy)^p\equiv x^py^p$ when $y\in P_i$. Also the power map $P_i/P_{i+1}\to P_{i+1}/P_{i+2}$ is a surjective [homomorphism](algebra.md#homomorphism). First find a root modulo $P_2$, then multiply it by successive corrections in $P_i$. The process terminates for a [finite p-group](#finite-p-group), and converges for a [pro-p group](topological-group.md#pro-p-group) with separated power filtration. This proves that the generated power [subgroup](group.md#subgroup) consists of actual powers.

#### Powerfully embedded subgroup

↑ **Parent:** [Powerful p-group](#powerful-p-group)

A [normal subgroup](group-theory.md#normal-subgroup) $N$ is powerfully embedded in a [finite p-group](#finite-p-group) or [pro-p group](topological-group.md#pro-p-group) $G$ if $[N,G]\leq N^p$ for odd $p$, or $[N,G]\leq N^4$ for $p=2$; use closed generated [subgroups](group.md#subgroup) in the [pro-p group](topological-group.md#pro-p-group) case. The condition implies that $N$ is a [powerful p-group](#powerful-p-group). For odd $p$, both $[N,G]$ and $N^p$ remain powerfully embedded.

### Classification of groups of order p squared

↑ **Parent:** [Finite p-group](#finite-p-group)

The [nontrivial center of a finite p-group](#nontrivial-center-of-a-finite-p-group) theorem implies that the [center of a group](group-theory.md#center-of-a-group) of order $p^2$ has order $p$ or $p^2$. If it has order $p$, the quotient by the center has prime order and is cyclic; a [cyclic quotient by the center](group-theory.md#cyclic-quotient-by-the-center) forces the whole [group](group.md) to be abelian, contradicting the assumed size of its center. Thus the [group](group.md) is abelian. An element of order $p^2$ makes it cyclic. Otherwise choose $a\ne1$ and $b\notin\langle a\rangle$; their order-$p$ [cyclic subgroups](group.md#cyclic-subgroup) intersect trivially and generate the [direct product of groups](group-theory.md#direct-product-of-groups) $C_p\times C_p$. The two possibilities are nonisomorphic because only the cyclic one has an element of order $p^2$.

### Normalizer condition for finite p-groups

↑ **Parent:** [Finite p-group](#finite-p-group)

Every proper [subgroup](group.md#subgroup) $H$ of a [finite p-group](#finite-p-group) is properly contained in its [normalizer](group-theory.md#normalizer). Let $H$ act on the left [cosets](group-theory.md#coset) $G/H$ by left multiplication. The fixed cosets are those represented by elements of $N_G(H)$, so there are $[N_G(H):H]$ of them. All other [orbits of a group action](group-theory.md#orbit-of-a-group-action) have sizes divisible by $p$. Since $[G:H]$ is divisible by $p$ and at least one coset is fixed, the fixed-coset count is a positive multiple of $p$. This also proves $[N_G(H):H]\geq p$.

### Central intersection property of normal subgroups of finite p-groups

↑ **Parent:** [Finite p-group](#finite-p-group)

A nontrivial [normal subgroup](group-theory.md#normal-subgroup) $N$ of a [finite p-group](#finite-p-group) meets the [center of a group](group-theory.md#center-of-a-group) nontrivially. The [conjugation action](group-theory.md#conjugation-action) of $G$ on $N$ has singleton orbits exactly at $N\cap Z(G)$. The [orbit-stabilizer theorem](group-theory.md#orbit-stabilizer-theorem) makes every other orbit size divisible by $p$, so $|N\cap Z(G)|\equiv|N|\equiv0\pmod p$. Since the intersection contains the identity, its size is at least $p$.

### Nontrivial center of a finite p-group

↑ **Parent:** [Finite p-group](#finite-p-group)

Every nontrivial [finite p-group](#finite-p-group) has a nontrivial [center](group-theory.md#center-of-a-group). The conjugation action partitions the group into conjugacy classes whose noncentral sizes are positive powers of $p$; the class equation then implies $|Z(G)|\equiv|G|\equiv0\pmod p$.

### Frattini subgroup

↑ **Parent:** [Finite p-group](#finite-p-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frattini_subgroup)

The Frattini subgroup of a finite p-group is the intersection of its maximal subgroups. It equals $G^p[G,G]$.

#### Frattini lifting of nilpotence

↑ **Parent:** [Frattini subgroup](#frattini-subgroup)

Let $\Phi=\Phi(G)$ in a [finite group](group.md#finite-group). If $H\trianglelefteq G$ contains $\Phi$ and $H/\Phi$ is a [nilpotent group](group-theory.md#nilpotent-group), every [Sylow subgroup](#sylow-subgroup) $P$ of $H$ has $P\Phi\trianglelefteq G$. The [Frattini argument](#frattini-argument) gives $G=(P\Phi)N_G(P)=\Phi N_G(P)$, and the defining non-generator property of $\Phi$ forces $N_G(P)=G$. Hence $H$ is a [nilpotent group](group-theory.md#nilpotent-group).

#### Non-generator of a finite group

↑ **Parent:** [Frattini subgroup](#frattini-subgroup)

An element that can always be omitted from a generating family. These are exactly the elements of the [Frattini subgroup](#frattini-subgroup): a proper generated subgroup is contained in a maximal subgroup, while an element outside a maximal subgroup generates the group together with it.

#### Frattini quotient

↑ **Parent:** [Frattini subgroup](#frattini-subgroup)

The Frattini quotient of a finite p-group is an elementary abelian p-group. Its dimension over $\mathbb F_p$ is the minimum number of generators of $G$; in particular, it has dimension at least two when $G$ is noncyclic.

##### Burnside basis theorem

↑ **Parent:** [Frattini quotient](#frattini-quotient)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burnside_basis_theorem)

A subset generates a finite p-group precisely when its images span the [Frattini quotient](#frattini-quotient). Indeed $\langle S\rangle\Phi(G)=G$ implies $\langle S\rangle=G$, since otherwise a maximal subgroup contains both factors. Minimal generating sets correspond to vector-space bases in the quotient.

## Simple group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_group)

A nontrivial simple group has no normal subgroups other than the identity subgroup and itself.

### Finite simple group

↑ **Parent:** [Simple group](#simple-group)

A nontrivial [finite group](group.md#finite-group) whose only [normal subgroups](group-theory.md#normal-subgroup) are the [trivial group](group.md#trivial-group) and the whole group. A [cyclic group](group.md#cyclic-group) of [prime number](number-theory.md#prime-number) order gives an abelian example; $A_5$ gives a nonabelian [alternating group](#alternating-group) example. Finite versions of [classical groups](group-theory.md#classical-group) can produce further examples after taking suitable subgroups and quotients; small parameters require separate checks.

### Simple groups with order a power of two times fifteen

↑ **Parent:** [Simple group](#simple-group)

For a finite [simple group](#simple-group) of this order, $e=0$ gives a normal Sylow $5$-subgroup, and $e=1$ gives a nontrivial sign homomorphism from the regular action, because an involution swaps fifteen pairs. Thus $e\ge2$. The Sylow $2$-count divides $15$; it cannot be one or three. If it is five, a Sylow subgroup's [normalizer](group-theory.md#normalizer) has index five. If it is fifteen, the [strengthened Sylow congruence from intersections](#strengthened-sylow-congruence-from-intersections) produces two Sylow subgroups meeting in index two. Their common subgroup is normal in both, so its normalizer contains both and has index three or five. Simplicity excludes index three. The resulting faithful degree-five action embeds $G$ in $A_5$ and forces order $60$, proving the conclusion.

### Iwasawa simplicity lemma

↑ **Parent:** [Simple group](#simple-group)

For a faithful primitive group action, suppose a point stabilizer has an abelian normal subgroup whose conjugates generate the whole group. Every nontrivial normal subgroup then contains the derived subgroup. Indeed the normal subgroup is transitive, and all those conjugates have the same image in the quotient, making the quotient abelian. If the whole group is nontrivial and perfect, it is simple.

### Simplicity of the alternating group on six letters

↑ **Parent:** [Simple group](#simple-group)

A [normal subgroup](group-theory.md#normal-subgroup) of $A_6$ has order dividing 360 and consists of the identity plus whole [conjugacy classes of the alternating group on six letters](#conjugacy-classes-of-the-alternating-group-on-six-letters). If it omits the odd-sized class of size 45, its order is an odd divisor and no nontrivial class sum fits. If it includes that class, the possible class sums not exceeding 180 are $46,86,118,126,136,158,176$, none dividing 360. Every proper subgroup has order at most 180; therefore $A_6$ is a [simple group](#simple-group).

### Simplicity of alternating groups

↑ **Parent:** [Simple group](#simple-group)

The alternating group $A_n$ is simple for every $n\geq5$. In particular it has no proper subgroup of index two, since every index-two subgroup is normal.

### Finite nonabelian simple group

↑ **Parent:** [Simple group](#simple-group)

A finite nonabelian simple group is a [finite group](group.md#finite-group) that is a [nonabelian group](group.md#non-abelian-group) and a [simple group](#simple-group). Every such group is a [perfect group](group-theory.md#perfect-group) because its [commutator subgroup](group-theory.md#commutator-subgroup) is a nontrivial normal subgroup.

#### Least-prime divisibility constraint for a finite simple group

↑ **Parent:** [Finite nonabelian simple group](#finite-nonabelian-simple-group)

Let $p$ be the smallest prime divisor of the order of a [finite nonabelian simple group](#finite-nonabelian-simple-group). A cyclic [Sylow subgroup](#sylow-subgroup) would give a [normal p-complement](group-theory.md#normal-p-complement), so if $p^3$ does not divide the order, the [Sylow subgroup](#sylow-subgroup) must be $C_p^2$. [Conjugation](group-theory.md#conjugation) embeds its [normalizer](group-theory.md#normalizer) modulo [centralizer](group-theory.md#centralizer) into $GL_2(p)$, and this quotient has order prime to $p$. For odd $p$, every other prime divisor of $|GL_2(p)|=p(p-1)^2(p+1)$ is smaller than $p$, again forcing trivial [conjugation](group-theory.md#conjugation) and a contradiction to the [Burnside transfer theorem](group-theory.md#burnside-transfer-theorem). For $p=2$, nontrivial [conjugation](group-theory.md#conjugation) must have order three, giving $12\mid |G|$. The [groups](group.md) $PSL_2(5^{2m+1})$ give infinitely many examples with exactly two factors of two in their orders.

#### Mathieu group

↑ **Parent:** [Finite nonabelian simple group](#finite-nonabelian-simple-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mathieu_group)

The natural actions of these five sporadic simple groups have degrees 11, 12, 22, 23 and 24, and respective transitivity degrees 4, 5, 3, 4 and 5. They arise from exceptional finite designs and codes.

#### Ree group of type G2

↑ **Parent:** [Finite nonabelian simple group](#finite-nonabelian-simple-group)

These simple groups have order $q^3(q^3+1)(q-1)$ and a two-transitive action on $q^3+1$ points. The restriction excludes the smallest nonsimple parameter; this family differs from the Ree groups of type $F_4$.

#### Suzuki group of Lie type

↑ **Parent:** [Finite nonabelian simple group](#finite-nonabelian-simple-group)

These simple groups have order $q^2(q^2+1)(q-1)$ and a two-transitive action on a Suzuki ovoid of $q^2+1$ points. The point-stabilizer root group is regular on the remaining points.

### Simplicity of the alternating group A5

↑ **Parent:** [Simple group](#simple-group)

The conjugacy classes of $A_5$ have sizes

$$
1,\quad15,\quad20,\quad12,\quad12.
$$

A normal subgroup is a union of these classes containing the identity. No proper nontrivial such union has size dividing $60$, so Lagrange's theorem proves that $A_5$ is simple.

### Smallest nonabelian simple group

↑ **Parent:** [Simple group](#simple-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smallest_nonabelian_simple_group)

Every finite nonabelian simple group has order at least 60; the alternating group A5 attains this bound.

## General linear group over a finite field

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/General_linear_group_over_a_finite_field)

The group $GL_n(\mathbb F_q)$ consists of invertible $n$ by $n$ matrices over the finite field $\mathbb F_q$.

### Conjugacy-class generating function for finite general linear groups

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

If $k_n(q)$ counts [conjugacy classes](group-theory.md#conjugacy-class) in $GL_n(q)$, then $\sum_{n\ge0}k_n(q)t^n=\prod_{i\ge1}(1-t^i)/(1-qt^i)$. Associate a partition to each irreducible polynomial other than t. The Euler product over those polynomials counts monic polynomials with nonzero constant term and is $(1-u)/(1-qu)$.

### Unitary group over a finite field

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

The [group](group.md) of invertible linear maps preserving a nondegenerate [Hermitian form over a quadratic finite field](linear-algebra.md#hermitian-form-over-a-quadratic-finite-field) is, in an [orthonormal basis](linear-algebra.md#orthonormal-basis), the displayed [matrix group](group-theory.md#matrix-group). Here $q^2$ denotes the size of the field on which the matrices act; some authors denote this same group by $U_n(q)$. Imposing [determinant](linear-algebra.md#determinant) one gives the special unitary subgroup, and subsequently quotienting its scalar center gives the [projective special unitary group over a finite field](#projective-special-unitary-group-over-a-finite-field).

### Projective special unitary group over a finite field

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

The projective quotient of determinant-one matrices preserving a nondegenerate Hermitian form over $\mathbb F_{q^2}$, with conjugation $x\mapsto x^q$. In dimension three its natural two-transitive action has $q^3+1$ isotropic points. For $q\ge3$ its order is $q^3(q^3+1)(q^2-1)/\gcd(3,q+1)$.

### Parabolic stabilizer of a subspace

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

For column vectors with the preserved space first, $A,D$ are invertible and $B$ arbitrary. Thus $P_k\cong\mathbb F_q^{k(n-k)}\rtimes(GL_k(q)\times GL_{n-k}(q))$. Its orbits on $k$-spaces are classified by intersection dimension with the preserved space.

### Symplectic group over a finite field

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

This group preserves a nondegenerate [alternating bilinear form](linear-algebra.md#alternating-bilinear-form) on $\mathbb F_q^{2m}$. Choosing a nonzero vector and a partner of pairing one, then recursing on their orthogonal complement, gives $|Sp_{2m}(q)|=q^{m^2}\prod_{i=1}^m(q^{2i}-1)$. Its center consists of scalars with $\lambda^2=1$.

#### Symplectic quotient of the binary subset module

↑ **Parent:** [Symplectic group over a finite field](#symplectic-group-over-a-finite-field)

For even n, the even-weight subspace of $F_2^n$ has radical $\langle\mathbf1\rangle$ for the dot product. Its quotient is a nondegenerate [alternating bilinear form](linear-algebra.md#alternating-bilinear-form) space of dimension n−2. The [symmetric group](#symmetric-group) acts by coordinate permutations. At n=6 this action is faithful and gives $S_6\cong Sp_4(2)$.

#### Perfectness of finite symplectic groups

↑ **Parent:** [Symplectic group over a finite field](#symplectic-group-over-a-finite-field)

For $q>3$, embedded perfect $SL_2(q)$ groups contain every [symplectic transvection](#symplectic-transvection). For $q=3,m\ge2$, four coefficient-one transvections on the lines of an isotropic plane multiply to the identity; their abelianized class is annihilated by 3 and 4. For $q=2,m\ge3$, seven transvections on an isotropic three-space multiply to the identity; their class is annihilated by 2 and 7. Thus all nonexceptional cases are perfect.

#### Symplectic transvection

↑ **Parent:** [Symplectic group over a finite field](#symplectic-group-over-a-finite-field)

This map preserves the alternating form and has inverse $T_{v,-c}$. Transvections along a fixed line form an abelian normal subgroup of its stabilizer. They generate the symplectic group by aligning successive symplectic basis pairs.

#### Projective symplectic group over a finite field

↑ **Parent:** [Symplectic group over a finite field](#symplectic-group-over-a-finite-field)

The scalar center has order $\gcd(2,q-1)$. The quotient is simple except at $(m,q)=(1,2),(1,3),(2,2)$. The last exception is $Sp_4(2)\cong S_6$.

### Inverse-transpose automorphism

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

Inverse transpose is an automorphism of order at most two. On projective geometry it implements point-hyperplane duality. For $GL_3(2)$ it swaps distinct point- and plane-stabilizer classes, so it is outer.

### Maximal subgroups of GL3 over F2

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

The maximal subgroups are point stabilizers and plane stabilizers of order 24, and [Singer cycle](#singer-cycle) normalizers of order 21. A proper subgroup containing a 7-element has a unique Sylow 7-subgroup, since the other count gives an impossible index-three subgroup of the simple group. A subgroup of order dividing 24 has a fixed point or a three-point orbit on the seven nonzero vectors. A collinear orbit gives an invariant plane; an independent triple gives its fixed vector sum.

#### Elementary abelian subgroups in GL3 over F2

↑ **Parent:** [Maximal subgroups of GL3 over F2](#maximal-subgroups-of-gl3-over-f2)

Every involution of $GL_3(2)$ is a [transvection](vector-space.md#transvection) $I+vf$, because its nilpotent part has square zero and rank one. Two distinct commuting transvections either have common image line or common fixed plane. This gives two types of elementary abelian groups of order four, displayed above. No larger elementary abelian $2$-subgroup is possible: a transvection commuting with all three elements of a common-image group must have that same image, and the dual argument applies to a common-fixed-plane group. Their [normalizers](group-theory.md#normalizer) are respectively point and plane stabilizers of order $24$. The common fixed-space dimensions one and two distinguish their conjugacy classes.

### Singer cycle

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

Multiplication by a generator of $\mathbb F_{q^n}^{\times}$ on the $\mathbb F_q$-space $\mathbb F_{q^n}$ gives a cyclic subgroup regular on nonzero vectors. Its normalizer contains the field Frobenius automorphism. In degree three over $\mathbb F_2$ the full normalizer has order 21.

### Order-p matrices in GL2 over the prime field

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

For prime $p$, every order-$p$ element of $GL_2(\mathbb F_p)$ is conjugate to the displayed nonidentity unipotent matrix. Its cyclic subgroup has vector [group orbits](group-theory.md#orbit-of-a-group-action) of sizes one or $p$; counting all $p^2$ vectors implies at least $p$ fixed vectors. Choose a nonzero fixed [vector](vector-space.md#vector) as first [basis](vector-space.md#basis) vector. The matrix becomes triangular with first diagonal entry one; its other diagonal entry satisfies $d^p=1$ and hence $d=1$ in the prime [finite field](algebra.md#finite-field). The off-diagonal entry is nonzero and can be rescaled to one. All matrices involved have invertible changes of basis.

### Faithful four-point action of GL2 over F2

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

The [general linear group over a finite field](#general-linear-group-over-a-finite-field) $GL_2(\mathbb F_2)$ acts faithfully on the four [vectors](vector-space.md#vector) of $\mathbb F_2^2$, since a matrix fixing all vectors fixes the standard basis. The zero vector is fixed by every element; the induced action on the three nonzero vectors identifies this six-element group with $S_3$. Swapping the two coordinates fixes $(0,0)$ and $(1,1)$ and exchanges the other two vectors, so its four-point [permutation](combinatorics.md#permutation) is odd. This action therefore embeds the group into $S_4$ with nontrivial composite [sign homomorphism](#sign-homomorphism).

### Order of a general linear group over a finite field

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

Choosing linearly independent columns successively gives

$$
|GL_n(\mathbb F_q)|
=(q^n-1)(q^n-q)\cdots(q^n-q^{n-1})
=q^{n(n-1)/2}\prod_{k=1}^n(q^k-1).
$$

### Upper unitriangular group

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

The upper unitriangular group consists of upper triangular matrices with every diagonal entry equal to one. Over $\mathbb F_p$ it has order $p^{n(n-1)/2}$ and is a [Sylow subgroup](#sylow-subgroup) of $GL_n(\mathbb F_p)$.

Its elements form the upper triangular, diagonal-one subset of [triangular matrices](linear-algebra.md#triangular-matrix).

#### Center of an upper unitriangular group

↑ **Parent:** [Upper unitriangular group](#upper-unitriangular-group)

The [upper unitriangular group](#upper-unitriangular-group) is generated by adjacent [elementary transvection matrices](vector-space.md#elementary-transvection-matrix) $I+sE_{i,i+1}$. Commuting a [matrix](vector-space.md#matrix) $X$ with each such generator forces every entry above the diagonal to vanish except possibly its $(1,n)$ entry: comparing $XE_{i,i+1}$ with $E_{i,i+1}X$ kills the entries above position $(i,i)$ in column $i$ and to the right of position $(i+1,i+1)$ in row $i+1$. The surviving [matrices](vector-space.md#matrix) $I+tE_{1n}$ do commute with the entire [group](group.md). In particular the [group center](group-theory.md#center-of-a-group) has order $q$; it distinguishes $U_4(2)$ from $U_3(4)$ despite their common order $64$.

#### Unitriangular matrix power formula

↑ **Parent:** [Upper unitriangular group](#upper-unitriangular-group)

For a three-dimensional strictly upper triangular [matrix](vector-space.md#matrix) $A$, the [binomial theorem](combinatorics.md#binomial-theorem) stops after $A^2$. Over a [finite field](algebra.md#finite-field) of odd prime characteristic $p$, both coefficients $p$ and $\binom p2$ vanish, so every nonidentity [matrix](vector-space.md#matrix) in $UT_3(\mathbb F_p)$ has order $p$. In characteristic two, a [matrix](vector-space.md#matrix) with nonzero $A^2$ instead has order four.

#### Unitriangular group of degree three over F3

↑ **Parent:** [Upper unitriangular group](#upper-unitriangular-group)

The [upper unitriangular group](#upper-unitriangular-group) $UT_3(\mathbb F_3)$ consists of $M(a,b,c)=\begin{pmatrix}1&a&c\\0&1&b\\0&0&1\end{pmatrix}$ for $a,b,c\in\mathbb F_3$. Its multiplication is $M(a,b,c)M(a',b',c')=M(a+a',b+b',c+c'+ab')$. The elements $M(1,0,0)$ and $M(0,1,0)$ do not commute. Yet every element is $I+N$ with $N^3=0$, so characteristic three gives $(I+N)^3=I$. It is a nonabelian [finite group](group.md#finite-group) of order $27$ whose nonidentity elements all have order three.

### Projective general linear group action on the projective line

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)

The group $PGL_2(F)=GL_2(F)/Z$ acts faithfully on

$$
\mathbb P^1(F)=F\cup\{\infty\}
$$

by [Möbius transformations](group-theory.md#mobius-transformation). For $|F|=q$, this embeds $PGL_2(F)$ into the [symmetric group](#symmetric-group) $S_{q+1}$.

#### Sharply three-transitive on a projective line

↑ **Parent:** [Projective general linear group action on the projective line](#projective-general-linear-group-action-on-the-projective-line)

For any field $F$, a [projective linear group](group-theory.md#projective-linear-group) element is uniquely determined by its images of three distinct points of the [projective line](#projective-line), and any ordered distinct target triple is attainable. Given representatives $v_z,v_x$ forming a [basis](vector-space.md#basis) and $v_y=A v_z+B v_x$, the [matrix](vector-space.md#matrix) with columns $A v_z,B v_x$ sends $(0,1,\infty)$ to $(x,y,z)$. Distinctness forces $A,B\ne0$. The [matrices](vector-space.md#matrix) realizing one projective map differ by a nonzero scalar; over $\mathbb F_p$ there are $p-1$ such [matrices](vector-space.md#matrix).

#### Projective line

↑ **Parent:** [Projective general linear group action on the projective line](#projective-general-linear-group-action-on-the-projective-line)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_line)

The projective line over a field $F$ is the set of one-dimensional subspaces of $F^2$ and may be identified with $F\cup\{\infty\}$.

#### Sylow 2-subgroup of PGL2 over F4

↑ **Parent:** [Projective general linear group action on the projective line](#projective-general-linear-group-action-on-the-projective-line)

The translations $x\mapsto x+b$ for $b\in\mathbb F_4$ form a Sylow $2$-subgroup of $PGL_2(\mathbb F_4)$. Every nonidentity translation fixes infinity and exchanges the four finite points in two transpositions, so its action lies in $A_5$.

### Special linear group over a finite field

↑ **Parent:** [General linear group over a finite field](#general-linear-group-over-a-finite-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Special_linear_group_over_a_finite_field)

The determinant-one matrices form the normal subgroup $SL_n(\mathbb F_q)=\ker(\det)$.

#### Unique involution in SL2 over an odd field

↑ **Parent:** [Special linear group over a finite field](#special-linear-group-over-a-finite-field)

Over a field of odd characteristic, an involutory matrix has minimal polynomial dividing $(X-1)(X+1)$, so it is diagonalizable with eigenvalues in $\{1,-1\}$. In dimension two, determinant one requires either both eigenvalues one or both minus one. Hence the only element of order two in $SL_2$ is $-I$; the identity has order one.

#### SL2 over F2 as a permutation group

↑ **Parent:** [Special linear group over a finite field](#special-linear-group-over-a-finite-field)

A determinant-one matrix over $\mathbb F_2$ permutes the three nonzero vectors of $\mathbb F_2^2$. This [group action](group-theory.md#group-action) is faithful because fixing two basis vectors forces the matrix to be the identity. There are $(4-1)(4-2)=6$ invertible matrices, all of determinant one since the only nonzero field element is one, so the action identifies the group with the [symmetric group](#symmetric-group) $S_3$. Reduction of integer determinant-one matrices modulo two is onto: $\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ and $\begin{pmatrix}1&1\\0&1\end{pmatrix}$ induce two distinct transpositions, which generate $S_3$. Its kernel consists of matrices congruent to the identity modulo two, the level-two [principal congruence subgroup](group-theory.md#principal-congruence-subgroup).

#### Projective special linear group over a finite field

↑ **Parent:** [Special linear group over a finite field](#special-linear-group-over-a-finite-field)

The scalar center has order $\gcd(n,q-1)$. For $n>1$ the quotient is simple except at $(n,q)=(2,2),(2,3)$. Its faithful primitive projective-point action, abelian fixed-center transvections, elementary-matrix generation and perfectness give the [Iwasawa simplicity lemma](#iwasawa-simplicity-lemma) proof.

##### Exterior-square realization of PSL4 over F2

↑ **Parent:** [Projective special linear group over a finite field](#projective-special-linear-group-over-a-finite-field)

On the six-dimensional [exterior square](linear-algebra.md#exterior-square) of $\mathbb F_2^4$, the [Pfaffian](linear-algebra.md#pfaffian) $Q=x_{12}x_{34}+x_{13}x_{24}+x_{14}x_{23}$ is a nonsingular plus-type [quadratic form](linear-algebra.md#quadratic-form). The action of $GL_4(2)$ preserves it and is faithful: fixing every decomposable exterior line fixes every two-space and then every one-space. The even-weight binary subset module on eight letters, modulo the all-one vector, gives another six-dimensional plus-type space with $Q=\operatorname{wt}(x)/2\bmod2$. Coordinate permutations embed $S_8$ faithfully into its orthogonal group. That orthogonal group has order $40320$, while $GL_4(2)$ has order $20160$, identifying its index-two image with the [alternating group](#alternating-group) $A_8$.

##### Projective special linear group over the field with five elements

↑ **Parent:** [Projective special linear group over a finite field](#projective-special-linear-group-over-a-finite-field)

The [special linear group](group-theory.md#special-linear-group) $SL_2(5)$ has $24$ nonzero first columns and five second columns giving determinant one, hence order $120$; its centre is $\{I,-I\}$. In the quotient by this centre, the nonidentity [conjugacy classes](group-theory.md#conjugacy-class) have sizes $15,20,12,12$, corresponding to projective element orders $2,3,5,5$. These arise from trace zero, paired traces $\pm1$, and paired unipotent traces $\pm2$. No proper union of these classes with the identity has size dividing $60$, so the quotient is simple. The [simple groups with order a power of two times fifteen](#simple-groups-with-order-a-power-of-two-times-fifteen) result identifies it with $A_5$.

###### Quaternion construction of an index-five subgroup of PSL2 over F5

↑ **Parent:** [Projective special linear group over the field with five elements](#projective-special-linear-group-over-the-field-with-five-elements)

Over $\mathbb F_5$, put

$$
i=\begin{pmatrix}0&1\\4&0\end{pmatrix},\quad
j=\begin{pmatrix}2&0\\0&3\end{pmatrix},\quad
r=\begin{pmatrix}3&2\\1&1\end{pmatrix}.
$$

These determinant-one [matrices](vector-space.md#matrix) satisfy $i^2=j^2=-I$, $ij=-ji$, and $r^3=I$. [Conjugation](group-theory.md#conjugation) by $r$ cycles $i,ij,j$. Thus $\langle i,j\rangle$ is a [quaternion group](#quaternion-group) of order eight, normalized by an element of order three. Their generated [subgroup](group.md#subgroup) has order $24$ in $SL_2(5)$, hence order $12$ after quotienting by $\{\pm I\}$. Its index-five [coset](group-theory.md#coset) action, together with simplicity and perfectness, identifies $PSL_2(5)$ with the [alternating group](#alternating-group) $A_5$.

#### Unipotent conjugacy in SL2 over a finite field

↑ **Parent:** [Special linear group over a finite field](#special-linear-group-over-a-finite-field)

For a [finite field](algebra.md#finite-field) of odd characteristic and nonzero $a,b$, let $U_a=\begin{pmatrix}1&a\\0&1\end{pmatrix}$. An arbitrary determinant-one matrix $P=\begin{pmatrix}r&s\\t&u\end{pmatrix}$ satisfies $PU_a=U_bP$ only if $t=0$ and $ar=bu$. The determinant condition $ru=1$ then gives $b/a=r^2$. Conversely $\operatorname{diag}(r,r^{-1})U_a\operatorname{diag}(r,r^{-1})^{-1}=U_{ar^2}$. Thus nonzero upper [unipotent matrices](lie-theory.md#unipotent-matrix) fall into two [conjugacy classes](group-theory.md#conjugacy-class) under this square-class criterion. For example, $U_1$ and $U_3$ are conjugate over $\mathbb F_{11}$ because $5^2=3$, but not over $\mathbb F_5$. The criterion compares these particular upper unipotent representatives; it does not classify all determinant-one matrices.

#### SL2 action on a finite projective line

↑ **Parent:** [Special linear group over a finite field](#special-linear-group-over-a-finite-field)

A matrix $\begin{pmatrix}a&b\\c&d\end{pmatrix}$ acts on the [projective line](#projective-line) by the [Möbius transformation](group-theory.md#mobius-transformation) $x\mapsto(ax+b)/(cx+d)$, with the pole sent to infinity and infinity sent to $a/c$ when $c\ne0$. The action is transitive because $\begin{pmatrix}t&-1\\1&0\end{pmatrix}$ sends infinity to any finite $t$. The [stabilizer subgroup](group-theory.md#stabilizer-subgroup) of infinity consists of $\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}$ with $a\ne0$. The [orbit-stabilizer theorem](group-theory.md#orbit-stabilizer-theorem) gives $|\mathrm{SL}_2(\mathbb F_q)|=q(q^2-1)$. Its kernel is the scalar matrices of determinant one: a transformation fixing infinity has $c=0$, fixing zero then forces $b=0$, and fixing one gives $a=d$. Thus the kernel is $\{I,-I\}$, with these matrices coinciding in characteristic two.

## Dihedral group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dihedral_group)

The dihedral group $D_{2n}$ is generated by a rotation $r$ of order $n$ and a reflection $s$ with $srs=r^{-1}$; it has order $2n$.

### Dihedral splitting when the half-rotation order is odd

↑ **Parent:** [Dihedral group](#dihedral-group)

Let $r$ have order $2m$ with $m$ odd, and let $s^2=1$, $srs=r^{-1}$. The [subgroup](group.md#subgroup) $H=\langle r^2,s\rangle$ is a dihedral group of order $2m$, while $K=\langle r^m\rangle$ is a central [cyclic group](group.md#cyclic-group) of order two. Since $m$ is odd, $H\cap K=\{1\}$ and $r$ lies in $HK$ by [Bézout's identity](algebra.md#bezout-identity). Thus the original group of order $4m$ is the [direct product of groups](group-theory.md#direct-product-of-groups) $H\times K$. This statement specifies group orders and avoids the two competing conventions for dihedral notation.

### Classification of subgroups of a dihedral group

↑ **Parent:** [Dihedral group](#dihedral-group)

Write $D_{2n}=\langle r,s:r^n=s^2=1,\ srs=r^{-1}\rangle$. A subgroup contained in the rotations is a [cyclic subgroup](group.md#cyclic-subgroup) $\langle r^d\rangle$, with $d\mid n$. If it contains a reflection, every other reflection differs from a chosen $r^js$ by a member of the rotational intersection, so it is $\langle r^d,r^js\rangle$, with $j$ specified modulo $d$. These subgroups have orders $n/d$ and $2n/d$ respectively. This gives a complete list, including the trivial and whole subgroups; see [Peter Cameron's group-theory exercise solutions, question1](https://maths.qmul.ac.uk/~pjc/MTH714U/so3.pdf).

### Dihedral subgroups of every divisor order

↑ **Parent:** [Dihedral group](#dihedral-group)

Write the [dihedral group](#dihedral-group) as $D_{2n}=\langle r,s:r^n=s^2=e,\ srs=r^{-1}\rangle$. If $k\mid n$, the [cyclic subgroup](group.md#cyclic-subgroup) $\langle r^{n/k}\rangle$ has order $k$. For an even divisor $k=2m$ of $2n$, $m\mid n$ and $\langle r^{n/m},s\rangle$ has $m$ rotations and $m$ reflections, hence order $k$. An odd divisor of $2n$ always divides $n$. This proves that the necessary divisibility condition from [Lagrange's theorem](group-theory.md#lagrange-s-theorem) is also sufficient in a [dihedral group](#dihedral-group), although it is not sufficient in arbitrary [finite groups](group.md#finite-group).

### Involutions in an even dihedral group

↑ **Parent:** [Dihedral group](#dihedral-group)

For the [dihedral group](#dihedral-group) of a regular $2n$-gon, $n\ge2$, use $r^{2n}=s^2=1$ and $srs=r^{-1}$. Its [involutions](group-theory.md#involution) are the central half-turn $r^n$ and all reflections $sr^j$. The half-turn has singleton [conjugacy class](group-theory.md#conjugacy-class) and [normal closure](group-theory.md#normal-closure) $\{1,r^n\}$. Conjugating a reflection changes its exponent by an even integer or negates it, so its [conjugacy class](group-theory.md#conjugacy-class) is $\{sr^{j+2k}:0\le k<n\}$. Products of consecutive reflections generate $r^2$, giving [normal closure](group-theory.md#normal-closure) $\langle r^2,sr^j\rangle$, of order $2n$ and index two. The two reflection classes are distinguished by exponent parity.

## Sylow theorems

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylow_theorems)

If $|G|=p^am$ with $p\nmid m$, then $G$ has subgroups of order $p^a$, every $p$-subgroup lies in one, and all such Sylow subgroups are conjugate. Their number satisfies $n_p\equiv1\pmod p$ and $n_p\mid m$.

### Sylow basis

↑ **Parent:** [Sylow theorems](#sylow-theorems)

A Sylow basis consists of one Sylow subgroup for each prime dividing the group order, with any two of them permutable as subgroups. Permutable means $P_pP_q=P_qP_p$, not elementwise commutation. Their product over any subset of primes is a Hall subgroup. Every finite soluble group has such a basis, and all bases are simultaneously conjugate. Induction over an elementary abelian minimal normal subgroup proves these facts using [coprime splitting over an elementary abelian normal subgroup](group-theory.md#coprime-splitting-over-an-elementary-abelian-normal-subgroup): lift the other-prime quotient basis into a complement, and lift the characteristic-prime Sylow subgroup by taking its full preimage.

#### Counting Sylow bases in a coprime elementary abelian extension

↑ **Parent:** [Sylow basis](#sylow-basis)

Let $V$ be an elementary abelian $r$-group and let $r\nmid|H|$, with $H$ soluble. In each Sylow basis of $V\rtimes H$, $V$ is the unique Sylow $r$-subgroup and the product of the remaining Sylow subgroups is a complement to $V$. All complements are $V$-conjugate, and the stabilizer of $H$ under this conjugation is its fixed-vector space $C_V(H)$. Each complement has $b(H)$ Sylow bases, proving the formula. For the permutation module $V=\mathbb F_5^4$ of $S_4$, the fixed-vector space is the one-dimensional constant-coordinate subspace, so the number is $5^3\cdot12=1500$.

### Sylow existence by subset action

↑ **Parent:** [Sylow theorems](#sylow-theorems)

Let $|G|=p^nr$ with $p\nmid r$. The coefficient of $X^{p^n}$ in $(1+X)^{p^nr}$ is $r$ modulo $p$, because $(1+X)^{p^nr}=(1+X^{p^n})^r$ over the field of $p$ elements. Thus the number of subsets of size $p^n$ is not divisible by $p$. Left translation of $G$ on those subsets has an orbit of index prime to $p$. Its stabilizer acts freely on its subset, so its order divides $p^n$, while its prime-to-$p$ index forces its order to be $p^n$. This proves existence of a [Sylow subgroup](#sylow-subgroup) without an induction using Cauchy's theorem.

### A group of order 56 has a normal Sylow subgroup

↑ **Parent:** [Sylow theorems](#sylow-theorems)

The [Sylow theorems](#sylow-theorems) give either one or eight [Sylow subgroups](#sylow-subgroup) of order seven. In the first case that [subgroup](group.md#subgroup) is normal. In the second, their six nonidentity elements are pairwise disjoint, accounting for 48 elements. Only eight elements remain, including the identity, and every [Sylow subgroup](#sylow-subgroup) of order eight lies entirely among them. Thus there is exactly one, and it is a [normal subgroup](group-theory.md#normal-subgroup).

### Frattini argument

↑ **Parent:** [Sylow theorems](#sylow-theorems)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frattini_argument)

If $H$ is a [normal subgroup](group-theory.md#normal-subgroup) of a finite group $G$ and $P$ a [Sylow subgroup](#sylow-subgroup) of $H$, then

$$
G=N_G(P)H.
$$

Normality puts every $g^{-1}Pg$ inside $H$, and Sylow conjugacy there gives $g^{-1}Pg=h^{-1}Ph$. Hence $gh^{-1}$ normalizes $P$, giving the factorization. This reduces questions about $G$ to a [normaliser](group-theory.md#normalizer) and its normal subgroup.

### Groups of order p squared q are not simple

↑ **Parent:** [Sylow theorems](#sylow-theorems)

For distinct primes $p,q$, the [Sylow theorems](#sylow-theorems) force a proper nontrivial [normal subgroup](group-theory.md#normal-subgroup) in any group of order $p^2q$. If $p>q$, the Sylow $p$-subgroup is unique. If $p<q$ and both Sylow counts were nontrivial, the count congruences force $(p,q)=(2,3)$. In order twelve, four Sylow $3$-subgroups exhaust eight nonidentity elements; only three remain for a Sylow $2$-subgroup, making that subgroup unique. Thus the group is not a [simple group](#simple-group).

### Sylow subgroup

↑ **Parent:** [Sylow theorems](#sylow-theorems)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sylow_subgroup)

A Sylow $p$-subgroup of a finite [group](group.md) has the largest power of $p$ dividing the group order.

### Nonabelian group of order pq

↑ **Parent:** [Sylow theorems](#sylow-theorems)

Let $p>q$ be [prime numbers](number-theory.md#prime-number). A nonabelian group of order $pq$ has a unique Sylow $p$-subgroup and exactly $p$ Sylow $q$-subgroups. Hence the Sylow count satisfies $p\equiv1\pmod q$, so $q\mid p-1$.

#### Nonabelian group of order 21

↑ **Parent:** [Nonabelian group of order pq](#nonabelian-group-of-order-pq)

Up to isomorphism, the unique nonabelian group of order $21$ is

$$
C_7\rtimes C_3
=\langle r,s\mid r^7=s^3=1,\ srs^{-1}=r^2\rangle.
$$

Its nonidentity elements of $C_7$ form two conjugacy classes of size three, and the other two $C_7$ cosets form conjugacy classes of size seven.

### Conjugation action on Sylow subgroups

↑ **Parent:** [Sylow theorems](#sylow-theorems)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugation_action_on_Sylow_subgroups)

A group, or one of its Sylow subgroups, acts on the set of Sylow subgroups by conjugation.

#### Strengthened Sylow congruence from intersections

↑ **Parent:** [Conjugation action on Sylow subgroups](#conjugation-action-on-sylow-subgroups)

For a finite [group](group.md) and a [Sylow subgroup](#sylow-subgroup) $P$, conjugation by $P$ on all Sylow subgroups has stabilizer $P\cap Q$ at $Q$: the normal Sylow subgroup $Q$ of $N_G(Q)$ contains every $p$-subgroup of that normalizer. Thus the orbit length is $[P:P\cap Q]$. If every $Q\ne P$ has this index at least $p^a$, each such orbit length is divisible by $p^a$, whereas $P$ is a singleton orbit. Summing orbit lengths proves the displayed stronger [integer congruence](number-theory.md#integer-congruence).

#### Simple group embedding from Sylow conjugation

↑ **Parent:** [Conjugation action on Sylow subgroups](#conjugation-action-on-sylow-subgroups)

A [finite nonabelian simple group](#finite-nonabelian-simple-group) embeds in $A_{n_p}$, where $n_p$ is its number of [Sylow subgroups](#sylow-subgroup) for a prime dividing its order. It is not a [p-group](#p-group) by the nontrivial-centre property. Thus its Sylow subgroups are proper and cannot be normal, so $n_p>1$. The conjugation action is nontrivial, and its normal [kernel of a group homomorphism](group-theory.md#kernel-of-a-group-homomorphism) must therefore be trivial. The sign of this faithful permutation action must be trivial, since a nontrivial sign homomorphism would inject the group into a group of order two. [Lagrange's theorem](group-theory.md#lagrange-s-theorem) consequently gives $|G|\mid n_p!/2$.

### Sylow subgroups of S3, S4 and A5

↑ **Parent:** [Sylow theorems](#sylow-theorems)

The Sylow $2$-subgroups of $S_3$ are its three transposition subgroups, while its unique Sylow $3$-subgroup is $A_3$. The three Sylow $2$-subgroups of $S_4$ are dihedral groups of order eight and are the normalizers of the three cyclic subgroups generated by inverse pairs of $4$-cycles. The five Sylow $2$-subgroups of $A_5$ are Klein four-groups, one fixing each letter.

### Sylow containment from a coset fixed point

↑ **Parent:** [Sylow theorems](#sylow-theorems)

If $P$ is a Sylow $p$-subgroup of $G$ and $Q$ is any $p$-subgroup, let $Q$ act on $G/P$. Since $p$ does not divide $|G/P|$, some coset $gP$ is fixed. Hence $g^{-1}Qg\leq P$, or equivalently $Q\leq gPg^{-1}$.

### Sylow counts in a faithful degree-seven action with S4 point stabilizers

↑ **Parent:** [Sylow theorems](#sylow-theorems)

Suppose a group acts faithfully and transitively on seven points, every point stabilizer is $S_4$, and every two-point stabilizer is a Klein four-group. Then the group has order $168$ and

$$
n_2=21,
\qquad n_3=28,
\qquad n_7=8.
$$

Count pairs consisting of a point and a Sylow subgroup fixing it for $p=2,3$; the two-point stabilizer ensures uniqueness. For $p=7$, a normal Sylow subgroup would force the group into its order-$42$ normalizer in $S_7$.

### Even-involution coset fixed-point lemma

↑ **Parent:** [Sylow theorems](#sylow-theorems)

Suppose a finite group $G$ has no index-two subgroup, $P$ is a Sylow $2$-subgroup, $H$ has index two in $P$, and $x\in G$ has order two. The sign of the action on $G/H$ defines a homomorphism $G\to\{\pm1\}$ and is therefore trivial. Since $[G:H]\equiv2\pmod4$, a fixed-point-free involution would be an odd number of transpositions. Thus $x$ fixes a coset $gH$, equivalently $g^{-1}xg\in H$.

## Cauchy theorem for groups

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy_theorem_for_groups)

If a prime divides the order of a finite group, the group contains an element of that prime order.

One proof lets a cyclic group of order $p$ rotate the tuples

$$
(x_1,\ldots,x_p)\quad\hbox{with}\quad x_1\cdots x_p=1.
$$

The tuple set has size $|G|^{p-1}$, and its fixed tuples are precisely $(x,\ldots,x)$ with $x^p=1$. Counting nonfixed orbits modulo $p$ forces a nonidentity fixed tuple.

### Cyclic-tuple proof of Cauchy theorem

↑ **Parent:** [Cauchy theorem for groups](#cauchy-theorem-for-groups)

For a prime divisor $p$ of the order of a [finite group](group.md#finite-group), rotate the tuples $(g_1,\ldots,g_p)$ whose product is the identity. Rotation preserves that constraint even for a nonabelian [group](group.md), by conjugating the product. Every nonfixed orbit has $p$ elements, while the fixed tuples correspond to $g^p=1$. There are $|G|^{p-1}$ tuples, so the number of fixed tuples is divisible by $p$. Since the identity is one, another solution exists and has order exactly $p$. This supplies an elementary proof of [Cauchy theorem for groups](#cauchy-theorem-for-groups).

## Power-map criterion for a finite group

↑ **Parent:** [Finite group theory](finite-group-theory.md)

For a finite group $G$, the map $x\mapsto x^m$ is bijective exactly when $m$ is coprime to $|G|$. If the two numbers are coprime, an inverse exponent modulo $|G|$ gives an inverse map. If a prime $p$ divides both, the [Cauchy theorem for groups](#cauchy-theorem-for-groups) supplies a nonidentity element sent to the identity.

## Composition series

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Composition_series)

A composition series is a finite subnormal chain whose successive quotients are simple.

### Composition chains in products with S5

↑ **Parent:** [Composition series](#composition-series)

The sign quotient of $S_5$ controls its cyclic composition factors, while its unique nontrivial proper normal subgroup $A_5$ supplies the nonabelian factor. There are four composition chains in $C_2\times S_5$: the three maximal normal subgroups are the kernels of the nonzero maps to $C_2$, and only $C_2\times A_5$ has two choices for its next term. In $S_5\times S_5$ there are eight chains: six pass through $A_5\times A_5$ and one of its two simple direct factors; two instead pass through a single $S_5$ direct factor. The equal-sign subgroup gives two of the six chains. It has no quotient $A_5$, since its odd diagonal element acts by an outer automorphism on either alternating factor.

### Composition length

↑ **Parent:** [Composition series](#composition-series)

The composition length of a finite-length module or group is the number of simple factors in a [composition series](#composition-series). The [Jordan–Hölder theorem](#jordan-holder-theorem) makes this independent of the chosen composition series.

<h3 id="jordan-holder-factor">Jordan–Hölder factor</h3>

↑ **Parent:** [Composition series](#composition-series)

A Jordan–Hölder factor is a simple quotient in a [composition series](#composition-series). The [Jordan–Hölder theorem](#jordan-holder-theorem) says that the multiset of such factors is independent of the chosen composition series.

<h4 id="jordan-holder-theorem">Jordan–Hölder theorem</h4>

↑ **Parent:** [Jordan–Hölder factor](#jordan-holder-factor)

Any two composition series of a finite group or finite-length module have the same length and the same simple factors up to permutation and isomorphism.

## Klein four-group

↑ **Parent:** [Finite group theory](finite-group-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Klein_four-group)

The Klein four-group is the abelian group with three nonidentity elements, all of order two.

## ↑ Ancestors (5)

1. [Group theory](group-theory.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
