# Homological algebra

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Homological_algebra)

Homological algebra studies [chain complexes](homology.md#chain-complex), [homology](homology.md), [cohomology](cohomology.md), and the derived constructions that measure failure of exactness.

**Table of contents**

- [Derived category of sheaves](#derived-category-of-sheaves)
  - [Ghost morphism in a derived category](#ghost-morphism-in-a-derived-category)
  - [Verdier duality](#verdier-duality)
  - [Constructible complex of sheaves](#constructible-complex-of-sheaves)
  - [Bounded below derived category of sheaves](#bounded-below-derived-category-of-sheaves)
    - [Exact triangle in a derived category](#exact-triangle-in-a-derived-category)
- [Left derived functor](#left-derived-functor)
  - [Left derived functors on an abelian category](#left-derived-functors-on-an-abelian-category)
- [Injective resolution](#injective-resolution)
- [Right derived functor](#right-derived-functor)
  - [Contravariant right derived functor](#contravariant-right-derived-functor)
- [Spectral sequence](#spectral-sequence)
  - [Künneth spectral sequence](#kunneth-spectral-sequence)
    - [Two-column degeneration of a Künneth spectral sequence](#two-column-degeneration-of-a-kunneth-spectral-sequence)
  - [Convergence of a spectral sequence](#convergence-of-a-spectral-sequence)
    - [Bounded filtered-complex convergence theorem](#bounded-filtered-complex-convergence-theorem)
- [Tor functor](#tor-functor)
  - [Tor for a principal non-zero-divisor quotient](#tor-for-a-principal-non-zero-divisor-quotient)
  - [First Tor of a cyclic quotient](#first-tor-of-a-cyclic-quotient)
- [Cochain complex](#cochain-complex)
  - [Cochain map](#cochain-map)
  - [Shift of a cochain complex](#shift-of-a-cochain-complex)
  - [Cycle module](#cycle-module)
    - [Cocycle](#cocycle)
  - [Boundary module](#boundary-module)
    - [Coboundary](#coboundary)
  - [Filtered cochain complex](#filtered-cochain-complex)
  - [Cochain subcomplex](#cochain-subcomplex)
  - [Short exact sequence of cochain complexes](#short-exact-sequence-of-cochain-complexes)
  - [Coboundary map](#coboundary-map)
- [Hom functor](#hom-functor)
  - [Ext functor](#ext-functor)
    - [Ext from a principal non-zero-divisor quotient](#ext-from-a-principal-non-zero-divisor-quotient)
    - [Nonzero Ext of the rationals with integer coefficients](#nonzero-ext-of-the-rationals-with-integer-coefficients)
    - [Long exact sequence of Ext groups](#long-exact-sequence-of-ext-groups)
    - [Extension group](#extension-group)
      - [Baer sum](#baer-sum)
    - [Localization of Ext over a Noetherian ring](#localization-of-ext-over-a-noetherian-ring)
    - [Ext groups between polynomial-ring residue modules](#ext-groups-between-polynomial-ring-residue-modules)
      - [Koszul self-Ext algebra](#koszul-self-ext-algebra)
    - [Ext separation of finite-length modules](#ext-separation-of-finite-length-modules)
- [Projective resolution](#projective-resolution)
  - [Resolution by finitely generated free modules](#resolution-by-finitely-generated-free-modules)
  - [Horseshoe lemma](#horseshoe-lemma)
  - [Standard projective resolution of a quiver representation](#standard-projective-resolution-of-a-quiver-representation)
    - [Extension complex of quiver representations](#extension-complex-of-quiver-representations)
      - [Kernel-cokernel obstruction to splitting a quiver extension](#kernel-cokernel-obstruction-to-splitting-a-quiver-extension)
  - [Projective presentation](#projective-presentation)
  - [Koszul resolution](#koszul-resolution)
  - [Free resolution](#free-resolution)
    - [Hilbert's syzygy theorem](#hilbert-s-syzygy-theorem)
    - [Minimal graded free resolution](#minimal-graded-free-resolution)
    - [Syzygy module](#syzygy-module)
    - [Bar resolution of an associative algebra](#bar-resolution-of-an-associative-algebra)

## Derived category of sheaves

↑ **Parent:** [Homological algebra](homological-algebra.md)

The derived category of sheaves is formed by localizing cochain complexes of sheaves at quasi-isomorphisms, equivalently localizing their homotopy category. The bounded, bounded below and bounded above variants are denoted $D^b(X)$, $D^+(X)$ and $D^-(X)$. Cohomology sheaves are invariant under quasi-isomorphism and therefore define functors on these categories. Constructible bounded complexes form a natural subcategory on which [Verdier duality](#verdier-duality) reverses arrows and, under the usual finiteness hypotheses, is an involution.

### Ghost morphism in a derived category

↑ **Parent:** [Derived category of sheaves](#derived-category-of-sheaves)

A ghost is a morphism inducing zero on every [cohomology sheaf](sheaf-of-modules.md#cohomology-sheaf), but it need not itself be zero. For the equator $j:S^1\hookrightarrow S^2$ and complement $i:U\hookrightarrow S^2$, the connecting morphism $j_*\mathbb Q_{S^1}\to i_!\mathbb Q_U[1]$ is a ghost. Its source and target have [cohomology sheaves](sheaf-of-modules.md#cohomology-sheaf) in different degrees, but its induced map $H^1(S^1)\to H_c^2(U)$ is nonzero, proving that the derived morphism is nonzero.

### Verdier duality

↑ **Parent:** [Derived category of sheaves](#derived-category-of-sheaves)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Verdier_duality)

On bounded constructible complexes over locally compact stratified spaces, [Verdier duality](#verdier-duality) is $D_XE=R\mathcal Hom(E,\omega_X^\bullet)$, where $\omega_X^\bullet$ is the dualizing complex. For an oriented real $N$-manifold, $D_X\mathbb Q_X\cong\mathbb Q_X[N]$. Proper direct image commutes with this duality, and $i_x^!D_XE\cong D_{\{x\}}i_x^*E$. These properties exchange stalk support conditions with [costalk](sheaf-of-modules.md#costalk) conditions.

### Constructible complex of sheaves

↑ **Parent:** [Derived category of sheaves](#derived-category-of-sheaves)

A bounded complex is constructible for a given stratification when each of its [cohomology sheaves](sheaf-of-modules.md#cohomology-sheaf) restricts to a finite-rank [local system](sheaf-of-modules.md#local-system) on every stratum. Constructibility concerns [cohomology sheaves](sheaf-of-modules.md#cohomology-sheaf), not an arbitrary choice of resolution.

### Bounded below derived category of sheaves

↑ **Parent:** [Derived category of sheaves](#derived-category-of-sheaves)

The category $D^+(X)$ is obtained from bounded below [cochain complexes](#cochain-complex) of [sheaves](algebraic-geometry.md#sheaf-mathematics) by passing to cochain-homotopy classes of maps and then inverting [quasi-isomorphisms](homology.md#quasi-isomorphism). It can equally be modeled by injective resolutions. The cohomology-sheaf functors descend to this localization, and an object is zero exactly when all its [cohomology sheaves](sheaf-of-modules.md#cohomology-sheaf) vanish.

#### Exact triangle in a derived category

↑ **Parent:** [Bounded below derived category of sheaves](#bounded-below-derived-category-of-sheaves)

An exact, or distinguished, triangle is one isomorphic to $E\xrightarrow{f}F\to\operatorname{Cone}(f)\to E[1]$. For a degreewise short exact sequence $0\to E\to F\to G\to0$, the map $\operatorname{Cone}(f)\to G$ taking $(v,e)$ to the image of $v$ is a [quasi-isomorphism](homology.md#quasi-isomorphism): its kernel is the contractible cone of the identity on $E$. Consequently the short exact sequence defines such a triangle.

## Left derived functor

↑ **Parent:** [Homological algebra](homological-algebra.md)

For an additive right-exact [functor](functor.md) on module categories, apply it to a [projective resolution](#projective-resolution) and take [homology](homology.md). Lifts of module maps exist by projectivity; any two lifts are [chain homotopic](homology.md#chain-homotopy), giving independence and functoriality. The zeroth derived functor is naturally $F$, positive degrees vanish on projective modules, and the [horseshoe lemma](#horseshoe-lemma) produces a long exact homology sequence from each short exact sequence. A [Tor functor](#tor-functor) is the left derived functor of a [tensor product of modules](module-theory.md#tensor-product-of-modules) functor.

### Left derived functors on an abelian category

↑ **Parent:** [Left derived functor](#left-derived-functor)

For a [right-exact additive functor](category-theory.md#right-exact-additive-functor) out of an [abelian category with enough projectives](category-theory.md#abelian-category-with-enough-projectives), apply the [functor](functor.md) to a [projective resolution](#projective-resolution) and take [homology objects](category-theory.md#homology-object). The zeroth derived [functor](functor.md) is $F$, positive derived [functors](functor.md) vanish on projective objects, and the degreewise split [horseshoe lemma](#horseshoe-lemma) produces a long exact sequence from every [short exact sequence in an abelian category](category-theory.md#short-exact-sequence-in-an-abelian-category). The target can be any abelian [category](category.md), including an [opposite category](category.md#opposite-category) of one.

## Injective resolution

↑ **Parent:** [Homological algebra](homological-algebra.md)

An exact augmented cochain complex with injective module terms. Module categories have enough injectives: coinduction $J=\operatorname{Hom}_{\mathbb Z}(A,\mathbb Q/\mathbb Z)$ is injective by its character adjunction, and the maps $m\mapsto(a\mapsto\phi(am))$, over all additive characters $\phi$ of $M$, embed $M$ into a product of copies of $J$. Products of injectives are injective by coordinatewise extension. Repeat on cokernels to obtain a resolution.

## Right derived functor

↑ **Parent:** [Homological algebra](homological-algebra.md)

For an additive covariant [left-exact functor](functor.md#finite-limit-preserving-functor) on module categories, choose an [injective resolution](#injective-resolution) $M\to I^\bullet$ and set $R^iF(M)=H^i(F(I^\bullet))$. For a contravariant functor, use a [projective resolution](#projective-resolution) instead, as in [contravariant right derived functor](#contravariant-right-derived-functor). Resolution comparison and homotopies give independence and functoriality; short exact sequences give long exact derived-functor sequences. The zeroth functor is naturally $F$.

### Contravariant right derived functor

↑ **Parent:** [Right derived functor](#right-derived-functor)

For an additive contravariant [left-exact functor](functor.md#finite-limit-preserving-functor), apply it to a [projective resolution](#projective-resolution) of $M$. Reversal of the arrows gives a [cochain complex](#cochain-complex). Comparison maps lift using projectivity, and any two lifts are chain homotopic, so its cohomology is independent of the resolution. The functors are contravariant, vanish on projective modules in positive degrees, and send $0\to M'\to M\to M''\to0$ to $0\to F(M'')\to F(M)\to F(M')\to R^1F(M'')\to\cdots$. Degreewise split resolutions from the [horseshoe lemma](#horseshoe-lemma) yield this sequence.

## Spectral sequence

↑ **Parent:** [Homological algebra](homological-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spectral_sequence)

A succession of bigraded pages with $E_{r+1}=H(E_r,d_r)$. In the cohomological convention, the differential has bidegree $(r,1-r)$. A filtered complex produces such successive approximations to its [cohomology](cohomology.md).

<h3 id="kunneth-spectral-sequence">Künneth spectral sequence</h3>

↑ **Parent:** [Spectral sequence](#spectral-sequence)

For a bounded complex $P$ of projective right modules and a left module $M$ of finite [projective dimension](module-theory.md#projective-dimension), a finite projective resolution of $M$ yields a bounded [double cochain complex](homology.md#double-cochain-complex). Its two [spectral sequences](#spectral-sequence) give the displayed abutment. Over a noncommutative ring, the handedness of the two tensor factors is essential.

<h4 id="two-column-degeneration-of-a-kunneth-spectral-sequence">Two-column degeneration of a Künneth spectral sequence</h4>

↑ **Parent:** [Künneth spectral sequence](#kunneth-spectral-sequence)

If only the columns $p=-1,0$ are nonzero, a cohomological differential of bidegree $(r,1-r)$ has no possible nonzero source-target pair for $r\geq2$. Projective boundaries in a complex of projectives give this condition because every cohomology module has projective dimension at most one.

### Convergence of a spectral sequence

↑ **Parent:** [Spectral sequence](#spectral-sequence)

The stable page identifies the [associated graded module](commutative-algebra.md#associated-graded-module) of a filtration of the abutment. For a finite filtration this is an exhaustive, separated finite extension description. It does not itself determine a canonical splitting. Unbounded filtrations require further convergence hypotheses.

#### Bounded filtered-complex convergence theorem

↑ **Parent:** [Convergence of a spectral sequence](#convergence-of-a-spectral-sequence)

A finite filtration of a [cochain complex](#cochain-complex) produces a convergent [spectral sequence](#spectral-sequence). The induced abutment filtration is the image of $H^n(F^pC)\to H^n(C)$. Finiteness in each degree suffices; a bounded range of cochain degrees is not required.

## Tor functor

↑ **Parent:** [Homological algebra](homological-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tor_functor)

The Tor functor is the [homology](homology.md) of a [tensor product of modules](module-theory.md#tensor-product-of-modules) with a [free resolution](#free-resolution): $\operatorname{Tor}_i^R(M,N)=H_i(F_\bullet\otimes_RN)$ for a [free resolution](#free-resolution) $F_\bullet$ of $M$. It measures the failure of tensoring to preserve [exact sequences](homology.md#exact-sequence). For a [commutative ring](commutative-algebra.md#commutative-ring), one may resolve either argument; the [double complex](homology.md#double-complex) of the two resolutions proves that both computations agree.

### Tor for a principal non-zero-divisor quotient

↑ **Parent:** [Tor functor](#tor-functor)

For a [non-zero-divisor](mathematics.md#non-zero-divisor) $a\in A$, resolve $A/(a)$ by $0\to A\xrightarrow{a}A\to A/(a)\to0$. Tensoring with $M$ gives the kernel and cokernel in the displayed formula; all higher [Tor functors](#tor-functor) vanish. Resolving either argument gives the same homology by the two filtrations of the double complex of the two free resolutions. For $M=A/(a)$, both degrees zero and one equal $A/(a)$.

### First Tor of a cyclic quotient

↑ **Parent:** [Tor functor](#tor-functor)

Start a [free resolution](#free-resolution) of $A/I$ with $P_0=A$ and a free module $P_1$ surjecting onto $I$. The next differential presents the relations in $I$. Right exactness of the [tensor product of modules](module-theory.md#tensor-product-of-modules) identifies $\operatorname{coker}(P_2\otimes_AM\to P_1\otimes_AM)$ with $I\otimes_AM$. Taking degree-one homology then gives the displayed kernel formula. Hence vanishing for every ideal is equivalent to the [flatness criterion using ideals](module-theory.md#flatness-criterion-using-ideals).

## Cochain complex

↑ **Parent:** [Homological algebra](homological-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cochain_complex)

A cochain complex is a sequence of abelian groups or modules and maps $d^n:C^n\to C^{n+1}$ satisfying $d^{n+1}d^n=0$. Its cohomology is $H^n(C)=\ker d^n/\operatorname{im}d^{n-1}$.

### Cochain map

↑ **Parent:** [Cochain complex](#cochain-complex)

A [cochain map](#cochain-map) $f:E\to F$ consists of degreewise maps $f^i:E^i\to F^i$ satisfying $d_F^i f^i=f^{i+1}d_E^i$. This identity sends cocycles to cocycles and coboundaries to coboundaries, hence induces maps on [cohomology](cohomology.md). For complexes of [sheaves](algebraic-geometry.md#sheaf-mathematics) the same identity holds as an identity of [sheaf](algebraic-geometry.md#sheaf-mathematics) morphisms.

### Shift of a cochain complex

↑ **Parent:** [Cochain complex](#cochain-complex)

The shift $E[1]$ has $E[1]^i=E^{i+1}$ and differential $-d_E^{i+1}$. Thus $H^i(E[1])=H^{i+1}(E)$. In general the differential of $E[r]$ is $(-1)^r d_E$.

### Cycle module

↑ **Parent:** [Cochain complex](#cochain-complex)

The submodule of cocycles in degree $q$. A projective [boundary module](#boundary-module) $B^{q+1}$ makes $0\to Z^q\to P^q\to B^{q+1}\to0$ split when $P^q$ is projective, so $Z^q$ is then also projective.

#### Cocycle

↑ **Parent:** [Cycle module](#cycle-module)

An element killed by the next differential of a [cochain complex](#cochain-complex). Its class modulo [coboundaries](#coboundary) is a [cohomology class](cohomology.md#cohomology-class).

### Boundary module

↑ **Parent:** [Cochain complex](#cochain-complex)

The submodule of coboundaries in degree $q$. The [cohomology group](cohomology.md#cohomology-group) is the corresponding [cycle module](#cycle-module) modulo the boundary module.

#### Coboundary

↑ **Parent:** [Boundary module](#boundary-module)

An element in the image of the preceding differential of a [cochain complex](#cochain-complex). Every [coboundary](#coboundary) is a [cocycle](#cocycle), since consecutive differentials compose to zero.

### Filtered cochain complex

↑ **Parent:** [Cochain complex](#cochain-complex)

A [cochain complex](#cochain-complex) with a decreasing filtration by [cochain subcomplexes](#cochain-subcomplex). A filtration finite in each degree is bounded in the degreewise sense; uniform bounds $F^aC=C$ and $F^bC=0$ are sufficient. The associated [spectral sequence](#spectral-sequence) starts with the graded quotient complexes.

### Cochain subcomplex

↑ **Parent:** [Cochain complex](#cochain-complex)

A sequence of submodules preserved by the differential of a [cochain complex](#cochain-complex). Its inclusion is a map of complexes.

### Short exact sequence of cochain complexes

↑ **Parent:** [Cochain complex](#cochain-complex)

A degreewise [short exact sequence](module-theory.md#short-exact-sequence) of [cochain complexes](#cochain-complex) induces a [long exact sequence from a coefficient sequence](homology.md#long-exact-sequence-from-a-coefficient-sequence) in the coefficient case, and a long exact cohomology sequence generally. Its degree-one [connecting homomorphism](homology.md#connecting-homomorphism) lifts a quotient cocycle, takes its coboundary, and identifies that result in the subcomplex.

### Coboundary map

↑ **Parent:** [Cochain complex](#cochain-complex)

A coboundary map is the degree-one differential $d^n:C^n\to C^{n+1}$ of a [cochain complex](#cochain-complex).

## Hom functor

↑ **Parent:** [Homological algebra](homological-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hom_functor)

The Hom functor sends two $R$-modules to the abelian group of $R$-linear maps between them. It is contravariant in its first argument and covariant in its second.

### Ext functor

↑ **Parent:** [Hom functor](#hom-functor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ext_functor)

The Ext functors are the right derived functors of the [Hom functor](#hom-functor). They can be computed by applying $\operatorname{Hom}_R(-,N)$ to a [projective resolution](#projective-resolution) of $M$ and taking [cohomology](cohomology.md).

#### Ext from a principal non-zero-divisor quotient

↑ **Parent:** [Ext functor](#ext-functor)

For a non-zero-divisor $a\in A$, the free resolution $0\to A\xrightarrow{a}A\to A/(a)\to0$ gives degree-zero kernel and degree-one cokernel, and all higher [Ext functors](#ext-functor) vanish. Directly in an [injective resolution](#injective-resolution) of the second variable, multiplication by $a$ is surjective in every term: the map $aA\to I$ taking $ax$ to $xm$ extends to $A\to I$. Thus $0\to\operatorname{Hom}_A(A/(a),I^\bullet)\to I^\bullet\xrightarrow{a}I^\bullet\to0$ is a short exact sequence of complexes and gives the same result. The displayed Hom functor is covariant in $M$; changing it to $\operatorname{Hom}_A(M,A/(a))$ changes the variable that is resolved.

#### Nonzero Ext of the rationals with integer coefficients

↑ **Parent:** [Ext functor](#ext-functor)

A [free resolution](#free-resolution) of $\mathbb Q$ has generators $a_n=1/n!$ and independent relations $a_n-(n+1)a_{n+1}$. Thus the [Ext functor](#ext-functor) gives the cokernel of the map on integer sequence products

$$
(u_n)\longmapsto(u_n-(n+1)u_{n+1}).
$$

The constant sequence one is not in its image. A preimage would require $u_1\equiv\sum_{j=1}^N j!\pmod{(N+1)!}$ for every $N$. For $N\geq3$, the sum is below $2N!$, tends to infinity, and its distance from $(N+1)!$ also tends to infinity. No fixed integer satisfies all these congruences. Hence $\operatorname{Ext}_{\mathbb Z}^1(\mathbb Q,\mathbb Z)\ne0$.

#### Long exact sequence of Ext groups

↑ **Parent:** [Ext functor](#ext-functor)

Applying the contravariant [Hom functor](#hom-functor) $\operatorname{Hom}_R(-,W)$ to $0\to I\to X\to C\to0$ gives

$$
0\to\operatorname{Hom}(C,W)\to\operatorname{Hom}(X,W)\to\operatorname{Hom}(I,W)\to\operatorname{Ext}^1(C,W)\to\operatorname{Ext}^1(X,W)\to\operatorname{Ext}^1(I,W)\to\operatorname{Ext}^2(C,W)\to\cdots.
$$

The connecting map sends $I\to W$ to its [pushout of a module extension](module-theory.md#pushout-of-a-module-extension). Its vanishing means that map extends to $X\to W$. For a [hereditary ring](module-theory.md#hereditary-ring), $\operatorname{Ext}^2(C,W)=0$, making the indicated restriction on first [extension groups](#extension-group) surjective. The covariant variable has its corresponding long exact sequence.

#### Extension group

↑ **Parent:** [Ext functor](#ext-functor)

An [extension group](#extension-group) is a value of an [Ext functor](#ext-functor). In degree one it classifies [short exact sequences](module-theory.md#short-exact-sequence) $0\to N\to E\to M\to0$ up to isomorphisms fixing the endpoints. The zero class is the split extension; its addition is the [Baer sum](#baer-sum). Higher degrees can be represented by longer exact extensions, or computed from a [projective resolution](#projective-resolution).

##### Baer sum

↑ **Parent:** [Extension group](#extension-group)

To add two extensions of $M$ by $N$, take their [direct sum](vector-space.md#direct-sum), form a [pullback in a category](category.md#pullback-category-theory) along the diagonal $M\to M\oplus M$, and form a [pushout in a category](category.md#pushout-in-a-category) along addition $N\oplus N\to N$. This produces another extension of $M$ by $N$ and defines addition in $\operatorname{Ext}^1_R(M,N)$. In a [quiver representation](algebra.md#representation-of-a-quiver), vertexwise splittings express the two extensions by off-diagonal arrow matrices, and the Baer sum adds those matrices modulo the [extension complex of quiver representations](#extension-complex-of-quiver-representations) coboundaries.

#### Localization of Ext over a Noetherian ring

↑ **Parent:** [Ext functor](#ext-functor)

Over a [Noetherian ring](algebra.md#noetherian-ring), a [finitely generated module](module-theory.md#finitely-generated-module) $N$ has a free resolution with every term finitely generated. Hom from a finite [free module](module-theory.md#free-module) commutes with localization, and [exactness of localization](commutative-algebra.md#exactness-of-localization) commutes with cohomology. Thus the displayed isomorphism holds for every $i\geq0$ and arbitrary $M$. The finiteness condition is on the first argument; the second need not be finitely generated.

#### Ext groups between polynomial-ring residue modules

↑ **Parent:** [Ext functor](#ext-functor)

When $X$ acts as zero, resolve the first module with the [Koszul resolution](#koszul-resolution) on $(p,X)$. Writing $N=\mathbb Z/q$, the resulting groups are $\ker(p:N\to N)$ in degree zero, $(N/pN)\oplus\ker p$ in degree one, and $N/pN$ in degree two, with zero higher groups. This works for composite as well as prime moduli.

##### Koszul self-Ext algebra

↑ **Parent:** [Ext groups between polynomial-ring residue modules](#ext-groups-between-polynomial-ring-residue-modules)

For an ideal generated by a finite [regular sequence](commutative-algebra.md#regular-sequence) in a commutative ring, the self-[Ext functor](#ext-functor) algebra is exterior on the degree-one dual generators. Contraction chain maps on the [Koszul resolution](#koszul-resolution) represent those generators, square to zero, and anticommute. The exterior square-zero relations also apply in characteristic two.

#### Ext separation of finite-length modules

↑ **Parent:** [Ext functor](#ext-functor)

Partition the isomorphism classes of [simple modules](module-theory.md#irreducible-module) into two sets $\mathcal C_1,\mathcal C_2$, with $\operatorname{Ext}^1(S,T)=\operatorname{Ext}^1(T,S)=0$ whenever $S,T$ lie in different sets. Every [module](module-theory.md#module-mathematics) $M$ of finite [composition length](finite-group-theory.md#composition-length) then has a unique decomposition $M=U_1\oplus U_2$ into its largest [submodules](module-theory.md#submodule) whose [Jordan–Hölder factors](finite-group-theory.md#jordan-holder-factor) belong to the respective sets.

For a simple $S\in\mathcal C_1$ and a finite-length $N$ with factors in $\mathcal C_2$, induction through the long exact sequence of the [Ext functor](#ext-functor) gives $\operatorname{Ext}^1(S,N)=0$. Induct on the length of $M$: take $0\to N\to M\to S\to0$, split $N=N_1\oplus N_2$, and suppose $S\in\mathcal C_1$. The quotient extension $0\to N_2\to M/N_1\to S\to0$ splits. The inverse image of its $S$-summand complements $N_2$ in $M$ and has only factors in $\mathcal C_1$. Finally, Hom between modules with factors in different sets is zero, since any nonzero image would have a factor in both sets. Projecting any proposed [submodule](module-theory.md#submodule) to the opposite summand therefore proves maximality and uniqueness.

## Projective resolution

↑ **Parent:** [Homological algebra](homological-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Projective_resolution)

A projective resolution of an $R$-module $M$ is an exact sequence

$$
\cdots\longrightarrow P_2\longrightarrow P_1\longrightarrow P_0\longrightarrow M\longrightarrow0
$$

in which every $P_i$ is a [projective module](module-theory.md#projective-module).

### Resolution by finitely generated free modules

↑ **Parent:** [Projective resolution](#projective-resolution)

A [finitely generated module](module-theory.md#finitely-generated-module) over a [Noetherian ring](algebra.md#noetherian-ring) admits a possibly infinite [free resolution](#free-resolution) whose every term is finitely generated. Surject a finite free module onto it; the kernel is finitely generated because a finite free module is [Noetherian](algebra.md#noetherian-ring). Repeat this construction on the successive kernels. If the original module has finite [projective dimension](module-theory.md#projective-dimension) $n$, its $n$th syzygy is projective by dimension shifting of the [Ext functor](#ext-functor), giving a length-$n$ resolution with finite projective terms.

### Horseshoe lemma

↑ **Parent:** [Projective resolution](#projective-resolution)

For a short exact sequence of modules with projective resolutions of its outer terms, there is a projective resolution of the middle term forming a degreewise split short exact sequence of resolutions. Lift the degree-zero projective cover of the quotient into the middle module and add the projective cover of the submodule; this surjects onto the middle module. Its kernel fits into the corresponding short exact sequence of kernels. Repeating this construction proves the claim. Additive contravariant functors preserve the degreewise split exact sequences with their direction reversed.

### Standard projective resolution of a quiver representation

↑ **Parent:** [Projective resolution](#projective-resolution)

Set $A=kQ$, $P_i=Ae_i$, $X_i=e_iX$. There is an exact sequence

$$
0\to\bigoplus_{\rho:i\to j}P_j\otimes_kX_i\xrightarrow{d}\bigoplus_iP_i\otimes_kX_i\to X\to0,
$$

where $d(p\otimes x)=p\rho\otimes x-p\otimes f_\rho(x)$ in the source and target summands, and the augmentation is $p\otimes x\mapsto px$. Each $P_i$ is a summand of $A$, so the two terms are [projective modules](module-theory.md#projective-module). This also works for infinite-dimensional modules.

#### Extension complex of quiver representations

↑ **Parent:** [Standard projective resolution of a quiver representation](#standard-projective-resolution-of-a-quiver-representation)

Put $C^0=\bigoplus_i\operatorname{Hom}(X_i,Y_i)$ and $C^1=\bigoplus_{\rho:i\to j}\operatorname{Hom}(X_i,Y_j)$. The differential has components $g_\rho h_i-h_jf_\rho$. Its kernel is $\operatorname{Hom}_Q(X,Y)$ and its cokernel is $\operatorname{Ext}^1_Q(X,Y)$. In a vertexwise splitting of an extension, the off-diagonal arrow blocks change by these coboundaries when the splitting changes.

##### Kernel-cokernel obstruction to splitting a quiver extension

↑ **Parent:** [Extension complex of quiver representations](#extension-complex-of-quiver-representations)

Restriction at one arrow induces a surjection $\operatorname{Ext}^1_Q(X,Y)\twoheadrightarrow\operatorname{Hom}_k(\ker f_\rho,\operatorname{coker}g_\rho)$. Coboundaries vanish on the kernel after quotienting by the image, while every map between these spaces can be lifted and extended. Nonzero kernel and cokernel therefore force a nonsplit extension. For $X=Y$, rigidity forces every arrow to have maximal rank.

### Projective presentation

↑ **Parent:** [Projective resolution](#projective-resolution)

A [short exact sequence](module-theory.md#short-exact-sequence) presenting a [module](module-theory.md#module-mathematics) as a quotient of a [projective module](module-theory.md#projective-module). The kernel need not be projective. Continuing a projective presentation gives a [projective resolution](#projective-resolution).

### Koszul resolution

↑ **Parent:** [Projective resolution](#projective-resolution)

For a [regular sequence](commutative-algebra.md#regular-sequence) $f_1,\ldots,f_r$ in a commutative [ring](commutative-algebra.md#ring) $R$, its Koszul complex is the finite free [projective resolution](#projective-resolution) of $R/(f_1,\ldots,f_r)$ with terms $\bigwedge^jR^r$ and [boundary map](homology.md#boundary-operator) contracting by $(f_1,\ldots,f_r)$. Exactness follows by induction: append $f_r$ using the [mapping cone](homology.md#mapping-cone-homological-algebra) for multiplication by $f_r$, which is injective on the preceding quotient. For a [polynomial ring](commutative-algebra.md#polynomial-ring) viewed as a [bimodule](module-theory.md#bimodule), use the [regular sequence](commutative-algebra.md#regular-sequence) $X_{i,\ell}-X_{i,r}$ in the enveloping [algebra](algebra.md).

### Free resolution

↑ **Parent:** [Projective resolution](#projective-resolution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Free_resolution)

A free resolution is a [projective resolution](#projective-resolution) in which every resolving module is a [free module](module-theory.md#free-module).

<h4 id="hilbert-s-syzygy-theorem">Hilbert's syzygy theorem</h4>

↑ **Parent:** [Free resolution](#free-resolution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert's_syzygy_theorem)

Every [finitely generated module](module-theory.md#finitely-generated-module) with a grading over the [polynomial ring](commutative-algebra.md#polynomial-ring) $S=k[X_1,\ldots,X_n]$ has a finite graded [free resolution](#free-resolution) of length at most $n$. The [Koszul resolution](#koszul-resolution) of $k$ has length $n$, so $\operatorname{Tor}_i^S(M,k)=0$ for $i>n$. In a [minimal graded free resolution](#minimal-graded-free-resolution), this [Tor functor](#tor-functor) is $F_i/(X_1,\ldots,X_n)F_i$; the [graded Nakayama lemma](mathematics.md#graded-nakayama-lemma) forces $F_i=0$ for $i>n$.

#### Minimal graded free resolution

↑ **Parent:** [Free resolution](#free-resolution)

Over $S=k[X_1,\ldots,X_n]$ with its standard grading and $\mathfrak m=(X_1,\ldots,X_n)$, a graded [free resolution](#free-resolution) is minimal when $d_i(F_i)\subseteq\mathfrak mF_{i-1}$ for every $i\ge1$. It is constructed by choosing minimal homogeneous generators for each successive [syzygy module](#syzygy-module), using the [graded Nakayama lemma](mathematics.md#graded-nakayama-lemma). After tensoring with $k=S/\mathfrak m$, all its differentials vanish, so $F_i/\mathfrak mF_i\cong\operatorname{Tor}_i^S(M,k)$; these dimensions and degrees are intrinsic to $M$.

#### Syzygy module

↑ **Parent:** [Free resolution](#free-resolution)

Given a [free resolution](#free-resolution) $\cdots\to F_1\to F_0\to M\to0$, its first syzygy module is $\ker(F_0\to M)$, the [module](module-theory.md#module-mathematics) of relations among the chosen generators of $M$. Higher syzygy modules are successive [kernels](kernel-of-a-linear-map.md). They depend on the choice of resolution; a [minimal graded free resolution](#minimal-graded-free-resolution) gives canonical ranks and degrees of generators over a standard [graded ring](commutative-algebra.md#graded-ring) structure on a [polynomial ring](commutative-algebra.md#polynomial-ring).

#### Bar resolution of an associative algebra

↑ **Parent:** [Free resolution](#free-resolution)

The bar resolution of an [associative algebra](associative-algebra.md) $A$ over a [field](algebra.md#field) has degree-$n$ term $A^{\otimes(n+2)}$ as an $A^e$-[module](module-theory.md#module-mathematics), with the outer factors carrying the left and right actions. Its boundary multiplies each consecutive pair with alternating signs, and its augmentation is multiplication $A\otimes A\to A$. It is exact: the $k$-linear contracting homotopy inserts $1$ at the left. Applying $\operatorname{Hom}_{A^e}(-,M)$ gives the [Hochschild cochain complex](associative-algebra.md#hochschild-cochain-complex) of the [bimodule](module-theory.md#bimodule) $M$.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-3.md#5/solution)
