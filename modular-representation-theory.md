# Modular representation theory

↑ **Parent:** [Representation theory](representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_representation_theory)

Modular representation theory studies representations of a finite group $G$ over a field whose characteristic divides $|G|$. The [group algebra](associative-algebra.md#group-algebra) is then generally nonsemisimple, and projective modules, radicals, blocks and vertices replace complete reducibility as central tools.

**Table of contents**

- [p-local module](#p-local-module)
- [Splitting p-modular system](#splitting-p-modular-system)
- [Indecomposable modules for a cyclic p-group](#indecomposable-modules-for-a-cyclic-p-group)
- [Modular representation ring](#modular-representation-ring)
- [Indecomposable modules of a cyclic p-group in characteristic p](#indecomposable-modules-of-a-cyclic-p-group-in-characteristic-p)
- [Group algebra of a p-group in characteristic p is local](#group-algebra-of-a-p-group-in-characteristic-p-is-local)
- [p-modular system](#p-modular-system)
  - [Integral form of a group representation](#integral-form-of-a-group-representation)
    - [Reduction of Hom from a projective group-algebra lattice](#reduction-of-hom-from-a-projective-group-algebra-lattice)
- [p-regular element](#p-regular-element)
- [Brauer character](#brauer-character)
  - [Brauer–Nesbitt theorem](#brauer-nesbitt-theorem)
    - [Brauer character basis theorem](#brauer-character-basis-theorem)
  - [Projective character](#projective-character)
  - [Brauer character inner product](#brauer-character-inner-product)
    - [Duality of simple and projective Brauer characters](#duality-of-simple-and-projective-brauer-characters)
      - [Column orthogonality for Brauer characters](#column-orthogonality-for-brauer-characters)
- [Symmetric algebra (Frobenius algebra)](#symmetric-algebra-frobenius-algebra)
  - [Head-socle identity for a symmetric algebra](#head-socle-identity-for-a-symmetric-algebra)
  - [Group algebra is a symmetric algebra](#group-algebra-is-a-symmetric-algebra)
    - [Projective modules over a finite group algebra are injective](#projective-modules-over-a-finite-group-algebra-are-injective)
      - [Head and socle of an indecomposable projective group-algebra module](#head-and-socle-of-an-indecomposable-projective-group-algebra-module)
        - [Dual of a projective cover over a group algebra](#dual-of-a-projective-cover-over-a-group-algebra)
      - [Group norm element detects the trivial projective cover](#group-norm-element-detects-the-trivial-projective-cover)
- [Relative projective module](#relative-projective-module)
  - [Relative trace](#relative-trace)
    - [Transfer ideal of conjugation-fixed elements](#transfer-ideal-of-conjugation-fixed-elements)
    - [D. Higman criterion](#d-higman-criterion)
      - [Projectivity detected on a subgroup of invertible index](#projectivity-detected-on-a-subgroup-of-invertible-index)
  - [Vertex of an indecomposable module](#vertex-of-an-indecomposable-module)
    - [Full-vertex modules for a noncyclic p-group](#full-vertex-modules-for-a-noncyclic-p-group)
    - [Green correspondence](#green-correspondence)
      - [Green correspondence from Mackey multiplicity](#green-correspondence-from-mackey-multiplicity)
      - [Green correspondent of a module](#green-correspondent-of-a-module)
      - [Green correspondence for blocks](#green-correspondence-for-blocks)
    - [Source of an indecomposable module](#source-of-an-indecomposable-module)
      - [Trivial source module](#trivial-source-module)
        - [Inflated quotient projectives have trivial source](#inflated-quotient-projectives-have-trivial-source)
        - [Permutation homomorphisms lift through modular reduction](#permutation-homomorphisms-lift-through-modular-reduction)
- [Finite representation type of a group algebra](#finite-representation-type-of-a-group-algebra)
  - [Parameter family for an elementary abelian p-group](#parameter-family-for-an-elementary-abelian-p-group)
  - [Higman criterion for finite representation type of a group algebra](#higman-criterion-for-finite-representation-type-of-a-group-algebra)
- [Defect-zero representation](#defect-zero-representation)
- [Block of a group algebra](#block-of-a-group-algebra)
  - [Residue-content criterion for symmetric-group blocks](#residue-content-criterion-for-symmetric-group-blocks)
    - [Nakayama block theorem](#nakayama-block-theorem)
  - [Central character of a block](#central-character-of-a-block)
  - [Fong–Reynolds matrix decomposition](#fong-reynolds-matrix-decomposition)
  - [Principal block](#principal-block)
  - [Modular reduction of block idempotents](#modular-reduction-of-block-idempotents)
  - [Blocks and Cartan matrices under central p-quotients](#blocks-and-cartan-matrices-under-central-p-quotients)
  - [Block of S3 in characteristic three](#block-of-s3-in-characteristic-three)
    - [Indecomposable projectives of S3 in characteristic three](#indecomposable-projectives-of-s3-in-characteristic-three)
  - [2-modular blocks of S3](#2-modular-blocks-of-s3)
  - [Defect group of a block](#defect-group-of-a-block)
    - [Regular defect-group bimodule inside a block](#regular-defect-group-bimodule-inside-a-block)
    - [Defect groups are centralizer-conjugate Sylow intersections](#defect-groups-are-centralizer-conjugate-sylow-intersections)
    - [Modules in a block are projective relative to its defect group](#modules-in-a-block-are-projective-relative-to-its-defect-group)
    - [Central defect blocks are matrix algebras](#central-defect-blocks-are-matrix-algebras)
    - [Inertial quotient of a block](#inertial-quotient-of-a-block)
      - [Inertial index of a block](#inertial-index-of-a-block)
    - [Defect of a block](#defect-of-a-block)
    - [Brauer pair](#brauer-pair)
    - [Block with cyclic defect group](#block-with-cyclic-defect-group)
      - [Brauer tree algebra](#brauer-tree-algebra)
        - [Uniserial branch of a Brauer tree algebra](#uniserial-branch-of-a-brauer-tree-algebra)
        - [Brauer tree path presentation](#brauer-tree-path-presentation)
        - [Indecomposable count for a cyclic defect block](#indecomposable-count-for-a-cyclic-defect-block)
    - [2-modular defect groups of A5](#2-modular-defect-groups-of-a5)
    - [Trace criterion for defect groups](#trace-criterion-for-defect-groups)
    - [Brauer morphism](#brauer-morphism)
      - [Block idempotents centralize a normal p-subgroup](#block-idempotents-centralize-a-normal-p-subgroup)
      - [Brauer quotient of a module](#brauer-quotient-of-a-module)
      - [Brauer morphism on a defect transfer ideal](#brauer-morphism-on-a-defect-transfer-ideal)
      - [Brauer morphism and relative trace](#brauer-morphism-and-relative-trace)
    - [Brauer correspondence](#brauer-correspondence)
      - [Brauer correspondent of a block](#brauer-correspondent-of-a-block)
      - [Brauer third main theorem](#brauer-third-main-theorem)
      - [Block induction](#block-induction)
        - [Block induction requires the block's defect centralizer](#block-induction-requires-the-block-s-defect-centralizer)
      - [Nagao module theorem](#nagao-module-theorem)
        - [Juhász induction refinement](#juhasz-induction-refinement)
      - [Brauer first main theorem](#brauer-first-main-theorem)
        - [Brauer extended first main theorem](#brauer-extended-first-main-theorem)
      - [5-modular blocks of A5](#5-modular-blocks-of-a5)
  - [Decomposition matrix (modular representation theory)](#decomposition-matrix-modular-representation-theory)
    - [Dominance triangularity of modular symmetric-group decomposition](#dominance-triangularity-of-modular-symmetric-group-decomposition)
    - [Cartan matrix of a group algebra](#cartan-matrix-of-a-group-algebra)
- [2-modular representation theory of GL3 of F2](#2-modular-representation-theory-of-gl3-of-f2)

## p-local module

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A p-local module here is a finite direct sum of [induced representations](representation-theory.md#induced-representation) from [normalizers](group-action.md#normalizer) $N_G(Q)$ of nontrivial [p-subgroups](finite-group-theory.md#p-subgroup) $Q$. This usage includes induction from $G$ itself when $G$ normalizes such a subgroup. [Green correspondence](#green-correspondence) and induction on vertex order express every finite module, or lattice over a complete valuation ring, as a difference of p-local modules after adjoining [projective modules](module-theory.md#projective-module).

## Splitting p-modular system

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

Here $\mathcal O$ is a complete discrete valuation ring with fraction field $K$ of characteristic zero and residue field $k$ of characteristic $p$. The system is splitting for the finite group and its subgroups when their simple representations over $K$ and $k$ are absolutely irreducible. It permits ordinary and modular representation theory to be compared by reduction of lattices modulo the maximal ideal.

## Indecomposable modules for a cyclic p-group

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

For $P$ cyclic of order $q=p^n$ in characteristic $p$, its [group algebra](associative-algebra.md#group-algebra) is $k[t]/(t^q)$. The nilpotent [Jordan normal form](linear-operator-theory.md#jordan-normal-form) classifies its indecomposable finite-dimensional modules as $V_i$, $1\leq i\leq q$. A module homomorphism $V_i\to V_j$ is determined by an element annihilated by $t^i$, so its dimension is $\min(i,j)$.

## Modular representation ring

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

The modular representation ring is the [Grothendieck group](algebraic-topology.md#grothendieck-group) of finite-dimensional [group representations](representation-theory.md#group-representation), with relations $[V]=[U]+[W]$ for every [short exact sequence](module-theory.md#short-exact-sequence) $0\to U\to V\to W\to0$, and multiplication $[V][W]=[V\otimes_k W]$ using the [tensor product of group representations](representation-theory.md#tensor-product-of-group-representations). The [Jordan–Hölder theorem](finite-group-theory.md#jordan-holder-theorem) makes the classes of [simple modules](module-theory.md#irreducible-module) a free integral basis. Tensoring over a [field](algebra.md#field) is exact, so this multiplication is well defined. When $k$ is a [splitting field for finite group representations](representation-theory.md#splitting-field-for-finite-group-representations), [Brauer characters](#brauer-character) identify $\mathbb C\otimes_{\mathbb Z}R_k(G)$ with the algebra of complex [class functions](representation-theory.md#class-function) on [p-regular elements](#p-regular-element). The splitting hypothesis is essential: $\mathbb F_2C_3\cong\mathbb F_2\times\mathbb F_4$ has two [simple modules](module-theory.md#irreducible-module), although $C_3$ has three $2$-regular conjugacy classes.

## Indecomposable modules of a cyclic p-group in characteristic p

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

Let $C_{p^n}=\langle g\rangle$ and let $k$ have characteristic $p$. With $u=g-1$,

$$
kC_{p^n}\cong k[u]/(u^{p^n}).
$$

Its finite-dimensional indecomposable modules are

$$
M_r=k[u]/(u^r),
\qquad 1\leq r\leq p^n.
$$

Each is a [uniserial module](module-theory.md#uniserial-module), with radical $uM_r$ and one-dimensional socle $u^{r-1}M_r$.

## Group algebra of a p-group in characteristic p is local

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

If $G$ is a finite $p$-group and $k$ has characteristic $p$, then the [augmentation ideal](commutative-algebra.md#augmentation-ideal) is the [Jacobson radical](noncommutative-algebra.md#jacobson-radical) of $kG$ and $kG/J(kG)\cong k$. Thus $kG$ is a [local ring](commutative-algebra.md#local-ring), has only the trivial simple module, and its regular module is indecomposable.

## p-modular system

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A p-modular system consists of a characteristic-zero field $K$, a [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) $\mathcal O\subset K$, and its residue field $k$ of characteristic $p$. It is a splitting system for a finite group when both $K$ and $k$ split the relevant group representations.

### Integral form of a group representation

↑ **Parent:** [P-modular system](#p-modular-system)

For a [p-modular system](#p-modular-system) $(K,\mathcal O,k)$, an integral form of a finite-dimensional $KG$-[module](module-theory.md#module-mathematics) $V$ is a $G$-stable finite free $\mathcal O$-submodule $W\subset V$ with $K\otimes_{\mathcal O}W\cong V$. Starting with a basis lattice $L$, the sum $\sum_{g\in G}gL$ supplies such a form: it is finitely generated and [torsion-free](vector-bundle.md#torsion-free-connection), hence free over the [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) $\mathcal O$. Reduction gives the $kG$-module $W/\pi W$, where $\pi$ is a [uniformizer](commutative-algebra.md#uniformizer).

#### Reduction of Hom from a projective group-algebra lattice

↑ **Parent:** [Integral form of a group representation](#integral-form-of-a-group-representation)

Let $W,W'$ be choices of [integral form of a group representation](#integral-form-of-a-group-representation) over a complete [p-modular system](#p-modular-system). Then $I=\operatorname{Hom}_{\mathcal OG}(W,W')$ is finite free, and $K\otimes_{\mathcal O}I=\operatorname{Hom}_{KG}(K\otimes W,K\otimes W')$: clearing denominators proves the spanning assertion. Also $\operatorname{Hom}_{\mathcal OG}(W,\pi W')=\pi I$. If $W$ is a [projective module](module-theory.md#projective-module), applying the [Hom functor](homological-algebra.md#hom-functor) to $0\to\pi W'\to W'\to W'/\pi W'\to0$ yields

$$
I/\pi I\cong\operatorname{Hom}_{kG}(W/\pi W,W'/\pi W').
$$

Consequently these ordinary and modular Hom spaces have the same [dimension of a vector space](vector-space.md#dimension-vector-space). Projectivity is essential: for $G=C_2$ over $\mathbb Z_2$, the trivial and sign lattices have zero Hom between them, whereas their reductions in characteristic $2$ coincide and have a one-dimensional Hom space.

## p-regular element

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A p-regular element of a finite group is an element whose order is coprime to $p$. It is also called a $p'$-element. The complementary elements are p-singular.

## Brauer character

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brauer_character)

Let $M$ be a representation over a splitting field $k$ of characteristic $p$. For a [p-regular element](#p-regular-element) $g$, the eigenvalues of $g$ on $M$ have order prime to $p$. Lift them to characteristic-zero roots of unity by the [Teichmuller lift](non-archimedean-analysis.md#teichmuller-representative); their sum is the Brauer character value $\chi_M(g)$.

<h3 id="brauer-nesbitt-theorem">Brauer–Nesbitt theorem</h3>

↑ **Parent:** [Brauer character](#brauer-character)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brauer–Nesbitt_theorem)

The Brauer character of a finite-dimensional modular representation determines its semisimplification. More strongly, the irreducible Brauer characters are linearly independent as complex-valued functions on the p-regular conjugacy classes.

#### Brauer character basis theorem

↑ **Parent:** [Brauer–Nesbitt theorem](#brauer-nesbitt-theorem)

Over a [splitting field for finite group representations](representation-theory.md#splitting-field-for-finite-group-representations) of characteristic $p$, the irreducible [Brauer characters](#brauer-character) form a complex basis of the [class functions](representation-theory.md#class-function) on the [p-regular elements](#p-regular-element). Independence is the character form of the [Brauer–Nesbitt theorem](#brauer-nesbitt-theorem). To obtain spanning, extend such a class function by zero on the p-singular classes. Ordinary irreducible characters form a basis of all class functions by [character orthogonality](representation-theory.md#character-orthogonality). Restricting them to p-regular elements yields Brauer characters of reductions of an [integral form of a group representation](#integral-form-of-a-group-representation) in a compatible splitting [p-modular system](#p-modular-system); if needed, first extend scalars, which does not change the simple-module list under the splitting hypothesis. Each restriction is a nonnegative integral sum of simple Brauer characters by exact-sequence additivity and the [Jordan–Hölder theorem](finite-group-theory.md#jordan-holder-theorem). Thus these restrictions span, proving the assertion. Consequently the number of simple modules equals the number of p-regular conjugacy classes, and evaluation identifies the complexified [modular representation ring](#modular-representation-ring) with the product of one copy of $\mathbb C$ for each such class.

### Projective character

↑ **Parent:** [Brauer character](#brauer-character)

The Brauer character of a projective module over a group algebra is called a projective character. It is the restriction to p-regular elements of the ordinary character of a lifted projective lattice; that ordinary character vanishes on p-singular elements.

### Brauer character inner product

↑ **Parent:** [Brauer character](#brauer-character)

For class functions on the p-regular elements of a finite group,

$$
\langle\phi,\psi\rangle_{p'}
=\frac1{|G|}\sum_{g\ p\text{-regular}}\overline{\phi(g)}\psi(g).
$$

Equivalently, summing over p-regular conjugacy-class representatives $x$ gives weights $1/|C_G(x)|$.

#### Duality of simple and projective Brauer characters

↑ **Parent:** [Brauer character inner product](#brauer-character-inner-product)

If $S_i$ are the simple modules of a split group algebra and $P_i$ are their [projective covers](module-theory.md#projective-cover), then

$$
\langle\chi_{P_i},\chi_{S_j}\rangle_{p'}=\delta_{ij}.
$$

##### Column orthogonality for Brauer characters

↑ **Parent:** [Duality of simple and projective Brauer characters](#duality-of-simple-and-projective-brauer-characters)

For p-regular elements $g,h$,

$$
\sum_S\chi_S(g^{-1})\chi_{P_S}(h)
=\begin{cases}|C_G(g)|&g\text{ and }h\text{ are conjugate},\\0&\text{otherwise},\end{cases}
$$

where $S$ ranges over the simple modules and $P_S$ is the projective cover of $S$.

## Symmetric algebra (Frobenius algebra)

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A finite-dimensional algebra $A$ is symmetric when there is a nondegenerate symmetric bilinear form $B:A\times A\to k$ satisfying $B(ab,c)=B(a,bc)$. Equivalently, $A\cong A^*$ as $A$-bimodules.

### Head-socle identity for a symmetric algebra

↑ **Parent:** [Symmetric algebra (Frobenius algebra)](#symmetric-algebra-frobenius-algebra)

For a finite-dimensional [symmetric algebra](#symmetric-algebra-frobenius-algebra) over any [field](algebra.md#field), an indecomposable [projective module](module-theory.md#projective-module) $P=Ae$ has isomorphic simple [head of a module](module-theory.md#head-of-a-module) and [socle](module-theory.md#socle-mathematics). A symmetrizing functional pairs $eA$ with $Ae$ nondegenerately, identifying $Ae$ with the left [dual module](module-theory.md#dual-module) $D(eA)$. Taking its [socle](module-theory.md#socle-mathematics) gives $D(eA/eAJ(A))$. This dual of the right simple top and the left simple top $Ae/J(A)e$ belong to the same matrix block of the [semisimple algebra](associative-algebra.md#semisimple-algebra) $A/J(A)$, so they are isomorphic. The result does not require an algebraically closed ground [field](algebra.md#field).

### Group algebra is a symmetric algebra

↑ **Parent:** [Symmetric algebra (Frobenius algebra)](#symmetric-algebra-frobenius-algebra)

For a finite group $G$, the coefficient of the identity in $xy$ defines a nondegenerate symmetric associative bilinear form on $kG$. Hence $kG\cong(kG)^*$ as bimodules and the [group algebra](associative-algebra.md#group-algebra) is a [symmetric algebra](#symmetric-algebra-frobenius-algebra).

#### Projective modules over a finite group algebra are injective

↑ **Parent:** [Group algebra is a symmetric algebra](#group-algebra-is-a-symmetric-algebra)

For finite-dimensional modules over $kG$, projectivity and injectivity are equivalent. Indeed, $(kG)^*$ is injective because $\operatorname{Hom}_{kG}(-,(kG)^*)\cong\operatorname{Hom}_k(-,k)$ is exact, while symmetry gives $(kG)^*\cong kG$.

##### Head and socle of an indecomposable projective group-algebra module

↑ **Parent:** [Projective modules over a finite group algebra are injective](#projective-modules-over-a-finite-group-algebra-are-injective)

If $P$ is an indecomposable projective $kG$-module, then its head and socle are simple and naturally isomorphic:

$$
P/J(P)\cong\operatorname{Soc}(P).
$$

This is the identity Nakayama permutation of the [symmetric algebra](#symmetric-algebra-frobenius-algebra) $kG$.

###### Dual of a projective cover over a group algebra

↑ **Parent:** [Head and socle of an indecomposable projective group-algebra module](#head-and-socle-of-an-indecomposable-projective-group-algebra-module)

For every simple finite-dimensional $kG$-module $S$,

$$
P_S^*\cong P_{S^*}.
$$

##### Group norm element detects the trivial projective cover

↑ **Parent:** [Projective modules over a finite group algebra are injective](#projective-modules-over-a-finite-group-algebra-are-injective)

Let $M$ be an indecomposable finite-dimensional $kG$-module and let $P_k$ be the projective cover of the trivial module. Then

$$
\dim_k(N_GM)=
\begin{cases}1&M\cong P_k,\\0&\text{otherwise}.
\end{cases}
$$

## Relative projective module

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

For a subgroup $H\leq G$, an $RG$-module $M$ is relatively H-projective when every $RG$-epimorphism onto $M$ that splits after restriction to $H$ already splits over $G$. Equivalently, $M$ is a direct summand of

$$
\operatorname{Ind}_H^G\operatorname{Res}_H^G M.
$$

### Relative trace

↑ **Parent:** [Relative projective module](#relative-projective-module)

For $\alpha\in\operatorname{End}_{RH}(M)$, the relative trace is

$$
\operatorname{Tr}_H^G(\alpha)
=\sum_{g\in[G/H]}g\alpha g^{-1}\in\operatorname{End}_{RG}(M).
$$

#### Transfer ideal of conjugation-fixed elements

↑ **Parent:** [Relative trace](#relative-trace)

Let a finite group $G$ act on an algebra $A$ by conjugation and let $H\leq G$. The transfer ideal from $H$ is

$$
A_H^G=\operatorname{Tr}_H^G(A^H)\subseteq A^G,
\qquad
\operatorname{Tr}_H^G(a)=\sum_{g\in G/H}gag^{-1}.
$$

The notation records both the source subgroup and the ambient fixed-point algebra.

#### D. Higman criterion

↑ **Parent:** [Relative trace](#relative-trace)

D. Higman's criterion says that an $RG$-module $M$ is [relative projective module](#relative-projective-module) for $H$ exactly when there is $\alpha\in\operatorname{End}_{RH}(M)$ satisfying

$$
\operatorname{Tr}_H^G(\alpha)=\operatorname{id}_M.
$$

##### Projectivity detected on a subgroup of invertible index

↑ **Parent:** [D. Higman criterion](#d-higman-criterion)

If $[G:H]$ is invertible in $R$, every $RG$-module is relatively H-projective. An $RG$-module is then projective exactly when its restriction to $RH$ is projective.

### Vertex of an indecomposable module

↑ **Parent:** [Relative projective module](#relative-projective-module)

A vertex of an indecomposable $kG$-module is a subgroup minimal among those for which the module is relatively projective. Vertices exist, form one conjugacy class, and are p-groups when $k$ has characteristic $p$. The vertices of the trivial module are the Sylow p-subgroups.

#### Full-vertex modules for a noncyclic p-group

↑ **Parent:** [Vertex of an indecomposable module](#vertex-of-an-indecomposable-module)

Every noncyclic finite [finite p-group](finite-group-theory.md#finite-p-group) $P$ has a quotient $C_p\times C_p$. Over any [field](algebra.md#field) of characteristic $p$, define a square-zero representation with basis $v_0,\ldots,v_r,w_1,\ldots,w_r$ by $xv_i=w_i$ for $1\le i\le r$, $xv_0=0$, $yv_i=w_{i+1}$ for $0\le i<r$, $yv_r=0$, and $xW=yW=0$. Here $x=g-1$, $y=h-1$, and $W$ is the span of the $w_i$. An endomorphism induces the same scalar on the top and on $W$; the remaining maps from the top to $W$ form a square-zero ideal. Thus the endomorphism ring is local and the module is indecomposable. Inflating to $P$ and choosing $p\nmid 2r+1$ gives infinitely many distinct dimensions with vertex $P$: the trace of a relative-trace identity from any proper subgroup would force dimension zero in the field. This construction works over finite fields too.

#### Green correspondence

↑ **Parent:** [Vertex of an indecomposable module](#vertex-of-an-indecomposable-module)

Let $N_G(D)\leq H\leq G$. Set $\mathcal X=\{D\cap{}^gD:g\notin H\}$ and $\mathcal Y=\{H\cap{}^gD:g\notin H\}$. [Green correspondence](#green-correspondence) pairs indecomposable modules with vertex $D$ for $G$ and $H$: restriction has a unique vertex-$D$ summand, with the other summands relatively projective for $\mathcal Y$; induction has a unique vertex-$D$ summand, with the other summands relatively projective for $\mathcal X$. The two assignments are inverse and preserve sources. Its more general form applies to vertices contained in $D$ but not conjugate into any member of $\mathcal X$.

##### Green correspondence from Mackey multiplicity

↑ **Parent:** [Green correspondence](#green-correspondence)

Let $N_G(D)\leq H\leq G$ and let $U$ be indecomposable with vertex $D$ over $H$. The [Mackey restriction formula](representation-theory.md#mackey-restriction-formula) writes $\operatorname{Res}_H^G\operatorname{Ind}_H^GU=U\oplus T$, where the vertices in $T$ lie in $H\cap{}^gD$ for $g\notin H$. None of these subgroups contains an $H$-conjugate of $D$: equality would put $g$ in $N_G(D)H=H$. Every summand of the induction with a $G$-conjugate of vertex $D$ contributes a vertex-$D$ summand on restriction. [Krull-Schmidt decomposition](module-theory.md#krull-schmidt-decomposition) therefore forces exactly one such summand, with multiplicity one. Choosing sources and using transitivity of induction proves the inverse correspondence and preservation of sources.

##### Green correspondent of a module

↑ **Parent:** [Green correspondence](#green-correspondence)

The Green correspondent is the unique indecomposable summand of restriction or induction having the selected [vertex of an indecomposable module](#vertex-of-an-indecomposable-module), in the setting of [Green correspondence](#green-correspondence). The two correspondence maps are inverse and preserve [sources of an indecomposable module](#source-of-an-indecomposable-module) up to the appropriate normalizer conjugacy.

##### Green correspondence for blocks

↑ **Parent:** [Green correspondence](#green-correspondence)

If $N_G(D)\le H\le G$, [Brauer correspondence](#brauer-correspondence) pairs the [blocks of a group algebra](#block-of-a-group-algebra) of $RG$ and $RH$ having [defect group of a block](#defect-group-of-a-block) $D$. This is [Green correspondence](#green-correspondence) for their [bimodules](module-theory.md#bimodule), with [vertex of an indecomposable module](#vertex-of-an-indecomposable-module) $\Delta D$ in $G\times G$. The normalizer of $\Delta D$ lies in $H\times H$, and the corresponding restriction and induction have unique summands with that vertex.

#### Source of an indecomposable module

↑ **Parent:** [Vertex of an indecomposable module](#vertex-of-an-indecomposable-module)

For an indecomposable [module](module-theory.md#module-mathematics) $M$ with [vertex of an indecomposable module](#vertex-of-an-indecomposable-module) $D$, a source is an indecomposable $RD$-module $S$ which is a [direct summand](vector-space.md#direct-summand) of $\operatorname{Res}_D^G M$ and for which $M$ is a direct summand of $\operatorname{Ind}_D^G S$. It has vertex $D$ as a $D$-module. Sources at a fixed vertex are conjugate by its [normalizer](group-action.md#normalizer).

##### Trivial source module

↑ **Parent:** [Source of an indecomposable module](#source-of-an-indecomposable-module)

Over a modular field or a complete discrete valuation coefficient ring, an indecomposable module has trivial source when a source is the rank-one trivial module of its vertex. These are precisely the indecomposable [direct summands](vector-space.md#direct-summand) of [permutation modules](representation-theory.md#permutation-module). A general trivial source module is a direct sum of these indecomposables.

###### Inflated quotient projectives have trivial source

↑ **Parent:** [Trivial source module](#trivial-source-module)

If $D$ is a normal [p-subgroup](finite-group-theory.md#p-subgroup) of $N$, any indecomposable [projective module](module-theory.md#projective-module) of $k(N/D)$, inflated to $N$, is a summand of $k[N/D]=\operatorname{Ind}_D^Nk$. It has trivial source and vertex $D$. Its [Brauer quotient of a module](#brauer-quotient-of-a-module) at $D$ is the entire module, since $D$ acts trivially and all proper-subgroup [relative traces](#relative-trace) multiply by an index divisible by $p$. This prevents its vertex from being smaller than $D$.

###### Permutation homomorphisms lift through modular reduction

↑ **Parent:** [Trivial source module](#trivial-source-module)

For coset [permutation modules](representation-theory.md#permutation-module), [Mackey restriction formula](representation-theory.md#mackey-restriction-formula) and [Frobenius reciprocity](representation-theory.md#frobenius-reciprocity) identify the homomorphism space with a free module having one orbit-sum basis vector per double coset. The same basis works over the residue field, so reduction of homomorphisms is surjective. Applied to endomorphisms of a permutation module, [idempotent refinement theorem](commutative-algebra.md#idempotent-refinement-theorem) lifts each modular direct summand to a trivial source lattice. Lifting inverse isomorphisms between reductions shows uniqueness among trivial source lattices.

## Finite representation type of a group algebra

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A group algebra $kG$ has finite representation type when it has only finitely many isomorphism classes of finite-dimensional indecomposable modules.

### Parameter family for an elementary abelian p-group

↑ **Parent:** [Finite representation type of a group algebra](#finite-representation-type-of-a-group-algebra)

For $P=C_p\times C_p$, put $x=g-1$, $y=h-1$. On a basis $v,w$, prescribe $xv=w$, $xw=0$, $yv=\lambda w$, $yw=0$. These are valid modules because every product of two radical operators is zero. Each is indecomposable, and an isomorphism preserves the equality $y=\lambda x$, hence preserves $\lambda$. An infinite field therefore gives infinitely many isomorphism classes.

### Higman criterion for finite representation type of a group algebra

↑ **Parent:** [Finite representation type of a group algebra](#finite-representation-type-of-a-group-algebra)

If $k$ has characteristic $p$, then $kG$ has finite representation type exactly when a Sylow p-subgroup of $G$ is cyclic. Restriction and induction reduce the property to the Sylow subgroup; a cyclic p-group has the finitely many indecomposables $k[u]/(u^r)$, while a noncyclic p-group has a quotient $C_p\times C_p$ and hence infinitely many indecomposables.

## Defect-zero representation

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A simple projective module over a split modular group algebra lies in a block of defect zero. It lifts uniquely to an ordinary irreducible character whose degree is divisible by the full p-part of the group order.

## Block of a group algebra

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

A block of a finite group algebra is an indecomposable two-sided ideal $RG e$ determined by a primitive central idempotent $e$. An $RG$-module $M$ lies in this block when $eM=M$.

### Residue-content criterion for symmetric-group blocks

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

For shapes of the same size, equal residue-content multiplicities are equivalent to equal [cores of a partition](representation-theory-of-the-symmetric-group.md#core-of-a-partition) at modulus $p$. Removing a rim $p$-hook subtracts one of each residue. With the number of [beta numbers](representation-theory-of-the-symmetric-group.md#beta-number-of-a-partition) divisible by $p$, the packed-runner charges are $q_r=c_r-c_{r+1}$, so the multiplicities recover the core. [Symmetric polynomials](polynomial.md#symmetric-polynomial) in [Young–Jucys–Murphy elements](representation-theory-of-the-symmetric-group.md#jucys-murphy-element) act by their evaluations on these residues, and generate the modular center. Equality of its [characters](representation-theory.md#character-of-a-representation) is precisely the block-equivalence criterion for [simple modules](module-theory.md#irreducible-module).

#### Nakayama block theorem

↑ **Parent:** [Residue-content criterion for symmetric-group blocks](#residue-content-criterion-for-symmetric-group-blocks)

At fixed degree $n$ in positive [characteristic](algebra.md#characteristic-of-a-field) $p$, two [Specht modules](representation-theory-of-the-symmetric-group.md#specht-module) belong to the same [block of a group algebra](#block-of-a-group-algebra) exactly when their labels have the same [core of a partition](representation-theory-of-the-symmetric-group.md#core-of-a-partition) at modulus $p$. The simple labels in that block are precisely the [regular partitions](representation-theory-of-the-symmetric-group.md#regular-partition) with that core. The theorem follows by combining the [residue-content criterion for symmetric-group blocks](#residue-content-criterion-for-symmetric-group-blocks) with the [Jucys–Murphy description of the center of a symmetric-group algebra](representation-theory-of-the-symmetric-group.md#jucys-murphy-description-of-the-center-of-a-symmetric-group-algebra).

### Central character of a block

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

The center of an indecomposable finite-dimensional [block of a group algebra](#block-of-a-group-algebra) is a commutative [Artinian local ring](algebra.md#artinian-local-ring). Its quotient by its [Jacobson radical](noncommutative-algebra.md#jacobson-radical) is a [field](algebra.md#field), giving the block's central character. Over a [splitting field for finite group representations](representation-theory.md#splitting-field-for-finite-group-representations) the residue field is the coefficient field; without this assumption one retains the residue field rather than pretending every central character is scalar-valued over $k$.

<h3 id="fong-reynolds-matrix-decomposition">Fong–Reynolds matrix decomposition</h3>

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

Let $N\triangleleft G$, let $b$ be a [block of a group algebra](#block-of-a-group-algebra) of $kN$, and let $I$ be its inertia subgroup. A block of $kG$ covering $b$ is a full [matrix algebra](associative-algebra.md#matrix-algebra) of degree $[G:I]$ over its corresponding block of $kI$. When $I=N$, the corner is just $kNb$. Let $e_B$ be the global block idempotent and put $c=e_Bb$. With coset representatives $g_i$, the elements $g_i c g_j^{-1}$ are matrix units in that global block because different conjugates of $b$ are orthogonal. When $I=N$, one has $c=b$.

### Principal block

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

The principal [block of a group algebra](#block-of-a-group-algebra) is the unique [block of a group algebra](#block-of-a-group-algebra) containing the [trivial representation](representation-theory.md#trivial-representation). Its primitive [central idempotent](associative-algebra.md#central-idempotent) is the unique one with augmentation $1$. Its [defect groups of a block](#defect-group-of-a-block) are the [Sylow subgroups](finite-group-theory.md#sylow-subgroup) for the residue characteristic.

### Modular reduction of block idempotents

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

For a complete [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) $\mathcal O$ with residue [field](algebra.md#field) $k$, class sums give bases of $Z(\mathcal OG)$ and $Z(kG)$, so reduction of the [center of an associative algebra](associative-algebra.md#center-of-an-associative-algebra) is surjective. [Idempotent lifting](commutative-algebra.md#idempotent-lifting) in this complete commutative [algebra](algebra.md) gives a bijection of primitive [central idempotents](associative-algebra.md#central-idempotent), hence of [blocks of a group algebra](#block-of-a-group-algebra). Corresponding [blocks of a group algebra](#block-of-a-group-algebra) have the same [defect groups of a block](#defect-group-of-a-block): [relative traces](#relative-trace) reduce, and a lifted trace whose reduction is the block identity is a unit in its complete block center.

### Blocks and Cartan matrices under central p-quotients

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

Let $Z=\langle z\rangle\leq Z(G)$ have order $p$ and set $t=z-1$. The [nilpotent ideal](commutative-algebra.md#nilpotent-ideal) $t kG$ is generated by a central element. If an idempotent lifts a central idempotent of the quotient, its off-diagonal corner satisfies $eA(1-e)\subseteq t eA(1-e)$ and therefore is zero. Thus central block idempotents lift centrally and uniquely. A [principal indecomposable module](module-theory.md#principal-indecomposable-module) is free over $kZ$, and the $p$ factors of its $t$-filtration are all its reduction modulo $t$. Consequently, under the natural indexing of simple modules, $C_G=pC_{G/Z}$.

### Block of S3 in characteristic three

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

Over a [field](algebra.md#field) of [characteristic](algebra.md#characteristic-of-a-field) three, the [group algebra](associative-algebra.md#group-algebra) $A=kS_3$ has a single [block of an Artinian algebra](associative-algebra.md#block-of-an-artinian-algebra). Put $r=(123)$, $s=(12)$ and $a=r-1$. Then $a^3=0$, $sas=-a+a^2$, and $J(A)=aA$: the latter is a [nilpotent ideal](commutative-algebra.md#nilpotent-ideal), with [semisimple ring](commutative-algebra.md#semisimple-ring) quotient $kC_2$. The [center of an associative algebra](associative-algebra.md#center-of-an-associative-algebra) is $k1\oplus ka^2\oplus ka^2s$, whose last two summands form a [square-zero ideal](commutative-algebra.md#square-zero-ideal). A [central idempotent](associative-algebra.md#central-idempotent) $d1+n$ satisfies $d^2=d$ and $(2d-1)n=0$, hence is zero or one. Thus no nontrivial central block decomposition exists.

#### Indecomposable projectives of S3 in characteristic three

↑ **Parent:** [Block of S3 in characteristic three](#block-of-s3-in-characteristic-three)

With $s=(12)$, the [idempotents](commutative-algebra.md#idempotent) $e_\pm=(1\pm s)/2$ split the right regular [module](module-theory.md#module-mathematics) into two three-dimensional [projective modules](module-theory.md#projective-module). Their tops are respectively the [trivial representation](representation-theory.md#trivial-representation) and [sign representation](representation-theory-of-the-symmetric-group.md#sign-representation). The [nilpotent ideal](commutative-algebra.md#nilpotent-ideal) $J(kS_3)$ ensures that any nonzero [direct summand](vector-space.md#direct-summand) has nonzero top, so the one-dimensional tops make these [projective modules](module-theory.md#projective-module) indecomposable. Their successive [radical series of a module](module-theory.md#radical-series-of-a-module) factors are trivial, sign, trivial and sign, trivial, sign. This decomposition concerns right [modules](module-theory.md#module-mathematics); the [block of S3 in characteristic three](#block-of-s3-in-characteristic-three) remains a single [algebra](algebra.md).

### 2-modular blocks of S3

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

Over a [splitting field for finite group representations](representation-theory.md#splitting-field-for-finite-group-representations) of characteristic $2$, put $a=(123)$. The [block of a group algebra](#block-of-a-group-algebra) idempotents of $kS_3$ are $b_0=1+a+a^2$ and $b_1=a+a^2$. Their block algebras are $b_0kS_3\cong kC_2$ and $b_1kS_3\cong M_2(k)$, with a [defect group of a block](#defect-group-of-a-block) given by $C_2$ and $1$, respectively. The first is a [local ring](commutative-algebra.md#local-ring); for the second, the representation $a\mapsto\operatorname{diag}(\omega,\omega^2)$, $(12)\mapsto\left(\begin{smallmatrix}0&1\\1&0\end{smallmatrix}\right)$ generates the full matrix algebra. The [Cartan matrix of a group algebra](#cartan-matrix-of-a-group-algebra) is $\operatorname{diag}(2,1)$, and the ordinary trivial, sign, and two-dimensional characters give [decomposition matrix](#decomposition-matrix-modular-representation-theory) $\left(\begin{smallmatrix}1&0\\1&0\\0&1\end{smallmatrix}\right)$.

### Defect group of a block

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

A defect group of a block idempotent $e$ is a maximal p-subgroup $D$ for which the Brauer image $\operatorname{Br}_D(e)$ is nonzero. Equivalently, the vertices of the block algebra as an $R[G\times G]$-module are the diagonal subgroups $\Delta D$ for the defect groups $D$. All defect groups of a block are conjugate.

#### Regular defect-group bimodule inside a block

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

For a block idempotent $b$ with defect $D$, the [Brauer quotient of a module](#brauer-quotient-of-a-module) of its [modular block](#block-of-a-group-algebra) [bimodule](module-theory.md#bimodule) at $\Delta D$ is nonzero: on the fixed basis $C_G(D)$, the block projection acts by $\operatorname{Br}_D(b)$. Restriction to $D\times D$ splits into transitive [permutation modules](representation-theory.md#permutation-module); their stabilizers have order at most $|D|$. A nonzero quotient at $\Delta D$ therefore forces a summand with stabilizer exactly $\Delta D$, which is the regular $kD$ [bimodule](module-theory.md#bimodule). Tensoring on the right with any $kD$-module $U$ gives $U\mid\operatorname{Res}_D^G(b\operatorname{Ind}_D^G U)$. Consequently [finite representation type](module-theory.md#finite-representation-type) of the [modular block](#block-of-a-group-algebra) forces finite representation type of $kD$.

#### Defect groups are centralizer-conjugate Sylow intersections

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

Let $P$ be any [Sylow subgroup](finite-group-theory.md#sylow-subgroup) containing a [defect group of a block](#defect-group-of-a-block) $D$. Regard the [block of a group algebra](#block-of-a-group-algebra) as a [permutation module](representation-theory.md#permutation-module) summand for $G\times G$, acting by left and right multiplication. Its vertex is $\Delta D$. Restricting to $P\times P$ retains a summand with this vertex. Transitive [permutation modules](representation-theory.md#permutation-module) for a [finite p-group](finite-group-theory.md#finite-p-group) are indecomposable, with their point stabilizers as vertices. Thus some orbit in $G$ has stabilizer $\Delta D$ at a suitably chosen point $c$. This means $c$ centralizes $D$ and $P\cap{}^cP=D$. Choosing $P$ to contain a Sylow subgroup of $N_G(D)$ shows that $D=O_p(N_G(D))$; every normal [p-subgroup](finite-group-theory.md#p-subgroup) of $G$ is contained in both Sylow factors and hence in $D$.

#### Modules in a block are projective relative to its defect group

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

For a [block of a group algebra](#block-of-a-group-algebra) with identity $e$ and [defect group of a block](#defect-group-of-a-block) $D$, the [trace criterion for defect groups](#trace-criterion-for-defect-groups) writes $e=\operatorname{Tr}_D^G(a)$ with $a\in(RG)^D$. On any module in the block, multiplication by $a$ is $D$-linear and its [relative trace](#relative-trace) is the identity. The [D. Higman criterion](#d-higman-criterion) therefore makes the module relatively $D$-projective.

#### Central defect blocks are matrix algebras

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

Let $k$ be an [algebraically closed field](algebra.md#algebraically-closed-field) and let a [block of a group algebra](#block-of-a-group-algebra) $B$ have a central [defect group of a block](#defect-group-of-a-block) $D$. Its quotient by $J(kD)B$ is a defect-zero block, hence a full [matrix algebra](associative-algebra.md#matrix-algebra) over $k$. The [algebra](algebra.md) $B$ is free over the central [local ring](commutative-algebra.md#local-ring) $kD$. Lift a primitive idempotent from this matrix quotient; its corner is free of rank one over $kD$, and is therefore $kD$. Lifting matrix units gives $B\cong\operatorname{Mat}_r(kD)$.

#### Inertial quotient of a block

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

For a maximal [Brauer pair](#brauer-pair) $(D,b_D)$ of a [block of a group algebra](#block-of-a-group-algebra), the inertial quotient is the displayed quotient of its pair stabilizer by $DC_G(D)$. It has order coprime to $p$, and its order is the [inertial index of a block](#inertial-index-of-a-block). For abelian $D$, conjugation embeds it in $\operatorname{Aut}(D)$.

##### Inertial index of a block

↑ **Parent:** [Inertial quotient of a block](#inertial-quotient-of-a-block)

Choose a maximal Brauer pair $(D,b_D)$ for the block. Its inertial quotient is $N_G(D,b_D)/(DC_G(D))$, and its order is the inertial index. For cyclic $D$ of order $q$, this is a prime-to-$p$ divisor of $p-1$. The number of edges of the block's Brauer tree is this index, and the exceptional multiplicity is $(q-1)/e(B)$.

#### Defect of a block

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

The defect of a [block of a group algebra](#block-of-a-group-algebra) is the [integer](integer.md) $d$ for which a [defect group of a block](#defect-group-of-a-block) has order $p^d$. Conjugacy of [defect groups of a block](#defect-group-of-a-block) makes this independent of the choice. A [block of a group algebra](#block-of-a-group-algebra) has defect zero when its [defect group of a block](#defect-group-of-a-block) is trivial.

#### Brauer pair

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

For a block idempotent $e$, an $e$-Brauer pair consists of a $p$-subgroup $P$ and a block idempotent $b_P$ of $kC_G(P)$ for which $b_P\operatorname{Br}_P(e)\ne0$. The subgroup of a maximal pair is a defect group. A maximal pair's stabilizer defines the inertial quotient of the block.

#### Block with cyclic defect group

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

A block has finite representation type exactly when its defect group is cyclic. In the forward implication, the block bimodule restricted to its defect group on both sides contains the regular defect-group bimodule as a summand; tensoring with arbitrary defect-group modules transfers finiteness to the defect group. Conversely, vertices are contained in the defect group and a cyclic $p$-group has only finitely many indecomposable modules, so there are only finitely many possible induced sources and their summands.

##### Brauer tree algebra

↑ **Parent:** [Block with cyclic defect group](#block-with-cyclic-defect-group)

The basic algebra of a split block with cyclic defect is a Brauer tree algebra: its simple modules are indexed by the edges of a tree, with a distinguished vertex carrying the exceptional multiplicity. For a one-edge tree of multiplicity $m$, its basic algebra is $k[t]/(t^{m+1})$. Its ideals form the chain of powers of $t$, so its unique indecomposable projective is uniserial of length $m+1$.

###### Uniserial branch of a Brauer tree algebra

↑ **Parent:** [Brauer tree algebra](#brauer-tree-algebra)

Let $i$ be an edge at $v$. Kill the other radical branch of its indecomposable [projective module](module-theory.md#projective-module). The resulting [uniserial module](module-theory.md#uniserial-module) has length $m_v\operatorname{val}(v)$ and its factors follow the cyclic edge order beginning at $i$. Quotienting its radical powers gives all shorter such modules. The edge succession uniquely fixes the path, and its nonzero arrow maps can be rescaled to one, giving uniqueness up to isomorphism. At an exceptional leaf this reduces to a nilpotent single Jordan chain; the other leaf loop, when present, is a socle path and vanishes in these shorter quotients.

###### Brauer tree path presentation

↑ **Parent:** [Brauer tree algebra](#brauer-tree-algebra)

Use a finite [tree](tree-graph-theory.md) with cyclically ordered incident edges at each vertex, and multiplicities one except possibly at one vertex. Quiver vertices are tree edges; arrows follow each cyclic successor order, including loops at vertices of valency one. For an edge $i$ with endpoints $v,w$, write $C_{i,v}$ for the cycle around $v$. Impose $C_{i,v}^{m_v}=C_{i,w}^{m_w}$, $C_{i,v}^{m_v}\alpha_{i,v}=0$, and zero for any path that switches from one vertex-cycle to the other. The quotient of this [path algebra](algebra.md#path-algebra) is the basic [Brauer tree algebra](#brauer-tree-algebra); redundant valency-one loops can be eliminated. Its indecomposable projective at $i$ has simple top and socle labelled by $i$, with two uniserial radical branches of lengths $m_v\operatorname{val}(v)$ and $m_w\operatorname{val}(w)$ meeting in that socle.

###### Indecomposable count for a cyclic defect block

↑ **Parent:** [Brauer tree algebra](#brauer-tree-algebra)

For a split [block of a group algebra](#block-of-a-group-algebra) with cyclic [defect group of a block](#defect-group-of-a-block) of order $q=p^n$ and [inertial index of a block](#inertial-index-of-a-block) $e$, its [Brauer tree algebra](#brauer-tree-algebra) has $e$ simple modules and exceptional multiplicity $(q-1)/e$. Its [stable Auslander–Reiten quiver](module-theory.md#stable-auslander-reiten-quiver) is $\mathbb ZA_{q-1}/\langle\tau^e\rangle$, giving $e(q-1)$ nonprojective indecomposables. Adding the $e$ indecomposable projectives gives $eq$ indecomposables in total.

#### 2-modular defect groups of A5

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

In characteristic $2$, a [Sylow subgroup](finite-group-theory.md#sylow-subgroup) $P$ of $A_5$ is a [Klein four-group](finite-group-theory.md#klein-four-group), and its [normalizer](group-action.md#normalizer) is $A_4$. Since $kA_4$ has one block, [Brauer first main theorem](#brauer-first-main-theorem) gives a unique block of $kA_5$ with defect $P$. No order-two subgroup $D$ can be a [defect group of a block](#defect-group-of-a-block): both $C_{A_5}(D)$ and $C_{A_5}(P)$ equal $P$, so the [Brauer morphisms](#brauer-morphism) of a central block idempotent at $D$ and at $P$ are equal. A nonzero image is $1$, since a [group algebra of a p-group in characteristic p is local](#group-algebra-of-a-p-group-in-characteristic-p-is-local), and consequently $D$ is not maximal among subgroups with nonzero Brauer image.

#### Trace criterion for defect groups

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

For a $p$-subgroup $D$ of a finite [group](group.md) $G$, set $I_D=\operatorname{Tr}_D^G((kG)^D)$, a [transfer ideal of conjugation-fixed elements](#transfer-ideal-of-conjugation-fixed-elements) in $Z(kG)$. A [block of a group algebra](#block-of-a-group-algebra) idempotent $b$ lies in $I_D$ if and only if a [defect group of a block](#defect-group-of-a-block) of $b$ is conjugate to a subgroup of $D$. In particular, defect groups can equivalently be defined as minimal subgroups $D$ with $b\in I_D$.

Here is a proof using the [Brauer morphism](#brauer-morphism). A subgroup of smallest order with $b\in I_D$ exists, since a [Sylow subgroup](finite-group-theory.md#sylow-subgroup) $P$ gives $b=\operatorname{Tr}_P^G(b/[G:P])$. Write $b=\operatorname{Tr}_D^G(a)$ and replace $a$ by $ba$. If $\operatorname{Br}_D(b)=0$, then $ba$ belongs to the kernel of the Brauer morphism, which is the sum of proper-subgroup relative traces. Hence $b\in\sum_{Q<D}I_Q$. The algebra $bZ(kG)$ is a commutative [Artinian ring](algebra.md#artinian-ring) and a [local ring](commutative-algebra.md#local-ring), so multiplying this equality by $b$ forces some ideal $bI_Q$ to contain its identity $b$. This contradicts minimality. On the other hand, $\operatorname{Br}_E(I_D)=0$ unless $E$ is conjugate into $D$: the $E$-action on $G/D$ has no fixed coset otherwise, and nonfixed orbit sizes vanish in characteristic $p$. Thus these minimal subgroups are precisely the maximal subgroups with nonzero Brauer image. They are all conjugate. Trace transitivity proves the stated criterion for larger $D$.

#### Brauer morphism

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

For a p-subgroup $D\leq G$, let $D$ act on $kG$ by conjugation. The Brauer morphism is the algebra homomorphism

$$
\operatorname{Br}_D:(kG)^D\longrightarrow kC_G(D),
\qquad
\sum_{g\in G}a_gg\longmapsto
\sum_{g\in C_G(D)}a_gg.
$$

##### Block idempotents centralize a normal p-subgroup

↑ **Parent:** [Brauer morphism](#brauer-morphism)

For a normal [p-subgroup](finite-group-theory.md#p-subgroup) $P\triangleleft G$, every [central idempotent](associative-algebra.md#central-idempotent) $e$ of $kG$ satisfies $e=\operatorname{Br}_P(e)\in kC_G(P)$. Indeed a nonfixed conjugation orbit sum maps to zero in $k(G/P)$, so $e-\operatorname{Br}_P(e)$ belongs to the [nilpotent ideal](commutative-algebra.md#nilpotent-ideal) $J(kP)kG$. Normality makes the Brauer image a [central idempotent](associative-algebra.md#central-idempotent) of $kG$, and two central idempotents congruent modulo a nilpotent ideal coincide. Consequently the [blocks of a group algebra](#block-of-a-group-algebra) of $kG$ correspond to $G$-orbits of blocks of $kC_G(P)$.

##### Brauer quotient of a module

↑ **Parent:** [Brauer morphism](#brauer-morphism)

For a $p$-subgroup $P$, the Brauer quotient removes all fixed vectors produced by proper-subgroup [relative traces](#relative-trace). On a [permutation module](representation-theory.md#permutation-module) it has a basis of the permutation-basis elements fixed by $P$: nonsingleton orbit sums are traces and disappear. The construction commutes with direct sums and idempotent projections. For an indecomposable [trivial source module](#trivial-source-module), it is nonzero exactly when a vertex contains a conjugate of $P$.

##### Brauer morphism on a defect transfer ideal

↑ **Parent:** [Brauer morphism](#brauer-morphism)

For $N=N_G(D)$ and $C=C_G(D)$, the [Brauer morphism](#brauer-morphism) restricts to a surjection

$$
\operatorname{Br}_D:I_D=\operatorname{Tr}_D^G((kG)^D)\longrightarrow J_D=\operatorname{Tr}_D^N(kC)=(kC)_D^N.
$$

This follows from [Brauer morphism and relative trace](#brauer-morphism-and-relative-trace) and the fact that $kC$ is contained in $(kG)^D$. The target is an ideal in the commutative algebra $(kC)^N$. Applying [primitive idempotents under a surjection of commutative Artinian ideals](commutative-algebra.md#primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals) and the [trace criterion for defect groups](#trace-criterion-for-defect-groups) identifies block idempotents with defect group $D$ with the primitive idempotents of $J_D$. Applying the same argument to $N$ gives [Brauer first main theorem](#brauer-first-main-theorem). The whole kernel need not be nilpotent, since blocks with smaller defect can be killed.

##### Brauer morphism and relative trace

↑ **Parent:** [Brauer morphism](#brauer-morphism)

Let $D$ be a p-subgroup of $G$, put $N=N_G(D)$, and let $k$ have characteristic $p$. The [Brauer morphism](#brauer-morphism) intertwines the two [relative traces](#relative-trace):

$$
\operatorname{Br}_D\!\left(\operatorname{Tr}_D^G(a)\right)
=\operatorname{Tr}_D^N\!\left(\operatorname{Br}_D(a)\right)
\qquad(a\in(kG)^D).
$$

Indeed, $D$ acts on $G/D$ by left multiplication. A coset $gD$ is fixed exactly when $g\in N$, and every other orbit has size divisible by $p$. After applying $\operatorname{Br}_D$, the summands belonging to one such orbit are equal, so every nonfixed orbit contributes zero in characteristic $p$; the fixed cosets give the trace from $D$ to $N$.

#### Brauer correspondence

↑ **Parent:** [Defect group of a block](#defect-group-of-a-block)

Let $B$ be a block of $kG$ with defect group $D$ and put $N=N_G(D)$. Its Brauer correspondent is the unique block $b$ of $kN$ with defect group $D$ selected by the nonzero Brauer image of the block idempotent of $B$.

##### Brauer correspondent of a block

↑ **Parent:** [Brauer correspondence](#brauer-correspondence)

The Brauer correspondent of a [block of a group algebra](#block-of-a-group-algebra) with [defect group of a block](#defect-group-of-a-block) $D$ in $G$ is the corresponding block of $N_G(D)$ furnished by [Brauer first main theorem](#brauer-first-main-theorem). The more general induced block $b^G$ is defined by [block induction](#block-induction) when the subgroup contains the centralizer of a defect group of $b$.

##### Brauer third main theorem

↑ **Parent:** [Brauer correspondence](#brauer-correspondence)

If a [block of a group algebra](#block-of-a-group-algebra) $b$ of $kH$ has [defect group of a block](#defect-group-of-a-block) $D$ and $DC_G(D)\le H\le G$, then its [block induction](#block-induction) $b^G$ is the [principal block](#principal-block) if and only if $b$ is the [principal block](#principal-block). Equivalently, the [Brauer morphism](#brauer-morphism) of the principal block idempotent at any [p-subgroup](finite-group-theory.md#p-subgroup) $Q$ is the principal block idempotent of $kC_G(Q)$.

##### Block induction

↑ **Parent:** [Brauer correspondence](#brauer-correspondence)

Let $b$ be a [block of a group algebra](#block-of-a-group-algebra) of $kH$ with [defect group of a block](#defect-group-of-a-block) $D$, where $DC_G(D)\le H\le G$. Apply [Brauer first main theorem](#brauer-first-main-theorem) inside $H$ to obtain its correspondent in $N_H(D)$. Composing that correspondent's [central character of a block](#central-character-of-a-block) with the [Brauer morphism](#brauer-morphism) from $Z(kG)$ selects a unique [block of a group algebra](#block-of-a-group-algebra) $b^G$. It is the unique [block of a group algebra](#block-of-a-group-algebra) whose restriction to $H\times H$ contains the block bimodule $b$ as a [direct summand](vector-space.md#direct-summand). Its [defect group of a block](#defect-group-of-a-block) can be larger than $D$ when $H$ does not contain $N_G(D)$.

<h6 id="block-induction-requires-the-block-s-defect-centralizer">Block induction requires the block's defect centralizer</h6>

↑ **Parent:** [Block induction](#block-induction)

The centralizer condition defining [block induction](#block-induction) refers to a [defect group of a block](#defect-group-of-a-block) of the actual source block. Containment of the centralizer of an unrelated [p-subgroup](finite-group-theory.md#p-subgroup) does not suffice. For example, in characteristic $3$ take $G=A_5$, $H=A_4$ and $D=C_3$. Then $DC_G(D)\le H$, but the unique defect-zero block of $kA_4$ occurs on bimodule restriction of both three-dimensional defect-zero blocks of $kA_5$. The two ordinary degree-three characters have identical restriction to $A_4$, namely its degree-three character, and defect-zero reduction gives the same simple projective module. Thus the unique-block characterization fails if $D$ is not the defect group of the source block.

##### Nagao module theorem

↑ **Parent:** [Brauer correspondence](#brauer-correspondence)

For a central idempotent $e$, a module $M=eM$, and $C_G(D)\leq K\leq N_G(D)$, put $b=\operatorname{Br}_D(e)$. Then $M\downarrow_K=bM\oplus(1-b)M$, and every indecomposable summand of the second term has vertex not containing $D$. Indeed $e-b$ is a sum of $K$-orbit sums of group elements not centralizing $D$. Each is a relative trace from a centralizer not containing $D$. Applying these traces to the module and using the local endomorphism ring of an indecomposable summand proves relative projectivity for one such subgroup.

<h6 id="juhasz-induction-refinement">Juhász induction refinement</h6>

↑ **Parent:** [Nagao module theorem](#nagao-module-theorem)

For an indecomposable $kK$-module $V$ with vertex $D$ and $\operatorname{Br}_D(e)V=V$, every indecomposable summand of $(1-e)\operatorname{Ind}_K^G V$ has vertex conjugate into $D\cap{}^gD$ for some $g\notin N_G(D)$. The refinement keeps the intersection subgroups from [Green correspondence](#green-correspondence), rather than asserting only that the remaining vertices are smaller than $D$.

##### Brauer first main theorem

↑ **Parent:** [Brauer correspondence](#brauer-correspondence)

Brauer's first main theorem gives a bijection between the blocks of $kG$ with defect group $D$ and the blocks of $kN_G(D)$ with defect group $D$. Corresponding blocks are related by their images under the [Brauer morphism](#brauer-morphism).

###### Brauer extended first main theorem

↑ **Parent:** [Brauer first main theorem](#brauer-first-main-theorem)

Over a [splitting field for finite group representations](representation-theory.md#splitting-field-for-finite-group-representations), [blocks of a group algebra](#block-of-a-group-algebra) with [defect group of a block](#defect-group-of-a-block) $D$ correspond to $N_G(D)$-orbits of blocks $b_D$ of $k(DC_G(D))$ with defect $D$ whose stabilizer quotient $N_G(D,b_D)/(DC_G(D))$ has order coprime to $p$. Equivalently one uses the defect-zero block of $k(DC_G(D)/D)$. This quotient is the [inertial quotient of a block](#inertial-quotient-of-a-block).

##### 5-modular blocks of A5

↑ **Parent:** [Brauer correspondence](#brauer-correspondence)

Over a splitting field of characteristic five, $A_5$ has a principal block of defect $C_5$ containing the ordinary characters of degrees $1,3,3,4$, and one defect-zero block containing the ordinary character of degree $5$. If $P$ is a Sylow 5-subgroup, then $N_{A_5}(P)\cong D_{10}$ and its unique 5-block is the Brauer correspondent of the principal block of $A_5$.

### Decomposition matrix (modular representation theory)

↑ **Parent:** [Block of a group algebra](#block-of-a-group-algebra)

The decomposition matrix is a specific invariant of [modular representation theory](modular-representation-theory.md).

The decomposition matrix records the multiplicities of simple modular representations in reductions of ordinary representations. If its rows are indexed by ordinary irreducible characters and its columns by irreducible Brauer characters, its entry $d_{\chi\phi}$ is the decomposition number of $\phi$ in the reduction of $\chi$.

#### Dominance triangularity of modular symmetric-group decomposition

↑ **Parent:** [Decomposition matrix (modular representation theory)](#decomposition-matrix-modular-representation-theory)

Rows of the symmetric-group [decomposition matrix](#decomposition-matrix-modular-representation-theory) are all ordinary shapes, columns are [regular partitions](representation-theory-of-the-symmetric-group.md#regular-partition), and $d_{\mu\lambda}=[S^\mu:D^\lambda]$. A nonzero [column antisymmetrizer](representation-theory-of-the-symmetric-group.md#column-antisymmetrizer-of-a-young-tableau) of shape $\lambda$ on $M^\mu$ forces dominance: the first $r$ rows contain at most $\sum_j\min(r,\lambda'_j)$ column entries. For a regular shape its diagonal simple appears once, giving a rectangular triangular matrix and a unitriangular regular-row submatrix.

#### Cartan matrix of a group algebra

↑ **Parent:** [Decomposition matrix (modular representation theory)](#decomposition-matrix-modular-representation-theory)

The Cartan matrix records composition-factor multiplicities in the projective indecomposable modules. For a split modular group algebra, it is

$$
C=D^TD,
$$

where $D$ is the [decomposition matrix](#decomposition-matrix-modular-representation-theory).

## 2-modular representation theory of GL3 of F2

↑ **Parent:** [Modular representation theory](modular-representation-theory.md)

The simple modules have dimensions $1,3,3,8$. The eight-dimensional simple is projective and forms a defect-zero block; the other three simples belong to the principal block. The decomposition and Cartan matrices are computed by restricting the six ordinary irreducible characters to the four odd-order conjugacy classes.

## ↑ Ancestors (5)

1. [Representation theory](representation-theory.md)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Decomposition matrix (modular representation theory)](#decomposition-matrix-modular-representation-theory)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-5.md#1/solution)
- [Representation theory](representation-theory.md)
