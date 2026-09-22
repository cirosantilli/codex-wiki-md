# Associative algebra

↑ **Parent:** [Algebra over a field](algebra.md#algebra-over-a-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Associative_algebra)

An associative algebra is an [algebra over a field](algebra.md#algebra-over-a-field) whose multiplication satisfies $(ab)c=a(bc)$. Unless stated otherwise, the algebras considered here have a multiplicative identity.

**Table of contents**

- [Primitive ideal](#primitive-ideal)
- [Ore extension](#ore-extension)
- [Algebra involution](#algebra-involution)
- [Unital algebra](#unital-algebra)
- [Star-algebra](#star-algebra)
  - [Hermitian element of a star algebra](#hermitian-element-of-a-star-algebra)
  - [Star-subalgebra](#star-subalgebra)
- [Cocenter of a finite-dimensional algebra](#cocenter-of-a-finite-dimensional-algebra)
  - [Frobenius map on an algebra cocenter](#frobenius-map-on-an-algebra-cocenter)
- [Representation variety of an associative algebra](#representation-variety-of-an-associative-algebra)
- [Units of a finite-dimensional algebra](#units-of-a-finite-dimensional-algebra)
- [Free associative algebra](#free-associative-algebra)
- [Frobenius algebra](#frobenius-algebra)
- [Opposite algebra](#opposite-algebra)
- [Right ideal](#right-ideal)
  - [Maximal right ideal](#maximal-right-ideal)
- [Formal associative deformation](#formal-associative-deformation)
  - [Weyl deformation of a polynomial algebra in two variables](#weyl-deformation-of-a-polynomial-algebra-in-two-variables)
  - [First-order associative deformation](#first-order-associative-deformation)
    - [Second-order obstruction to an associative deformation](#second-order-obstruction-to-an-associative-deformation)
  - [Trivial formal deformation](#trivial-formal-deformation)
    - [Formal rigidity from vanishing second Hochschild cohomology](#formal-rigidity-from-vanishing-second-hochschild-cohomology)
- [Gelfand–Kirillov dimension](#gelfand-kirillov-dimension)
  - [Gelfand–Kirillov dimension of a module](#gelfand-kirillov-dimension-of-a-module)
    - [Bernstein growth dimension of a Weyl algebra module](#bernstein-growth-dimension-of-a-weyl-algebra-module)
      - [Characteristic variety of a Weyl algebra module](#characteristic-variety-of-a-weyl-algebra-module)
        - [Independence of characteristic support from a good module filtration](#independence-of-characteristic-support-from-a-good-module-filtration)
      - [Holonomic Weyl algebra module](#holonomic-weyl-algebra-module)
        - [Multiplicity bounds the length of a holonomic Weyl module](#multiplicity-bounds-the-length-of-a-holonomic-weyl-module)
      - [Bernstein inequality for Weyl algebra modules](#bernstein-inequality-for-weyl-algebra-modules)
        - [Faithful finite-step action of a Weyl algebra](#faithful-finite-step-action-of-a-weyl-algebra)
          - [Scalar extraction by iterated Weyl commutators](#scalar-extraction-by-iterated-weyl-commutators)
- [Block of an Artinian algebra](#block-of-an-artinian-algebra)
- [Maximal commutative subalgebra](#maximal-commutative-subalgebra)
- [Centralizer of a subalgebra](#centralizer-of-a-subalgebra)
  - [Commutant of an operator algebra](#commutant-of-an-operator-algebra)
    - [Von Neumann double commutant theorem](#von-neumann-double-commutant-theorem)
      - [Kaplansky density theorem](#kaplansky-density-theorem)
    - [Double commutant theorem for star-algebras](#double-commutant-theorem-for-star-algebras)
    - [Double-centralizer theorem for semisimple operator algebras](#double-centralizer-theorem-for-semisimple-operator-algebras)
- [Matrix algebra](#matrix-algebra)
- [Block of a finite-dimensional algebra](#block-of-a-finite-dimensional-algebra)
  - [Ext-connected components determine blocks](#ext-connected-components-determine-blocks)
- [Basic algebra](#basic-algebra)
  - [Ext quiver](#ext-quiver)
- [Central simple algebra](#central-simple-algebra)
  - [Quaternion algebra](#quaternion-algebra)
    - [Quaternion norm obstruction at primes congruent to three modulo four](#quaternion-norm-obstruction-at-primes-congruent-to-three-modulo-four)
  - [Reduced norm](#reduced-norm)
  - [Inner automorphisms of a matrix algebra](#inner-automorphisms-of-a-matrix-algebra)
  - [Splitting field of a central simple algebra](#splitting-field-of-a-central-simple-algebra)
  - [Degree of a central simple algebra](#degree-of-a-central-simple-algebra)
  - [Artin–Wedderburn theorem](#artin-wedderburn-theorem)
    - [Burnside matrix-algebra theorem](#burnside-matrix-algebra-theorem)
  - [Tensor product of central simple algebras](#tensor-product-of-central-simple-algebras)
  - [Brauer group](#brauer-group)
    - [Brauer class](#brauer-class)
    - [Albert-Brauer-Hasse-Noether theorem](#albert-brauer-hasse-noether-theorem)
    - [Independent quaternion classes over rational numbers](#independent-quaternion-classes-over-rational-numbers)
    - [Brauer p-divisibility in characteristic p](#brauer-p-divisibility-in-characteristic-p)
    - [Witt residue sequence](#witt-residue-sequence)
      - [Local Brauer invariant](#local-brauer-invariant)
        - [Local fundamental class](#local-fundamental-class)
        - [Restriction and corestriction of local Brauer invariants](#restriction-and-corestriction-of-local-brauer-invariants)
    - [Period of a Brauer class](#period-of-a-brauer-class)
    - [Index of a central simple algebra](#index-of-a-central-simple-algebra)
    - [Crossed-product algebra of a Galois extension](#crossed-product-algebra-of-a-galois-extension)
      - [Cyclic algebra](#cyclic-algebra)
        - [Splitting criterion for a cyclic algebra](#splitting-criterion-for-a-cyclic-algebra)
        - [Norm projection formula for cyclic Brauer pairings](#norm-projection-formula-for-cyclic-brauer-pairings)
      - [Cohomological construction of a Brauer class](#cohomological-construction-of-a-brauer-class)
- [Center of an associative algebra](#center-of-an-associative-algebra)
  - [Central idempotent](#central-idempotent)
    - [Primitive central idempotent](#primitive-central-idempotent)
- [Group algebra](#group-algebra)
  - [Complex group algebra detects p-nilpotency](#complex-group-algebra-detects-p-nilpotency)
  - [Center of the infinite dihedral group algebra](#center-of-the-infinite-dihedral-group-algebra)
  - [Character idempotent](#character-idempotent)
  - [Conjugacy-class sum](#conjugacy-class-sum)
  - [Group norm element](#group-norm-element)
  - [Completed group algebra](#completed-group-algebra)
    - [Weighted group algebra of a uniform pro-p group](#weighted-group-algebra-of-a-uniform-pro-p-group)
    - [Iwasawa algebra](#iwasawa-algebra)
      - [Measure realization of an Iwasawa algebra](#measure-realization-of-an-iwasawa-algebra)
      - [Iwasawa algebra of a Zp-extension](#iwasawa-algebra-of-a-zp-extension)
        - [Pseudo-isomorphism](#pseudo-isomorphism)
        - [Iwasawa-module rank](#iwasawa-module-rank)
      - [Filtration on a group](#filtration-on-a-group)
        - [p-valuation](#p-valuation)
          - [Ordered basis of a complete p-valued group](#ordered-basis-of-a-complete-p-valued-group)
          - [p-saturated group](#p-saturated-group)
        - [Associated graded Lie algebra of a filtered group](#associated-graded-lie-algebra-of-a-filtered-group)
      - [Lazard filtration on a group algebra](#lazard-filtration-on-a-group-algebra)
        - [Lazard enveloping-algebra map](#lazard-enveloping-algebra-map)
      - [Center of an Iwasawa algebra of a complete p-valued group](#center-of-an-iwasawa-algebra-of-a-complete-p-valued-group)
      - [Lazard logarithm of a p-saturated group](#lazard-logarithm-of-a-p-saturated-group)
        - [Primitive elements of a completed rational Iwasawa algebra](#primitive-elements-of-a-completed-rational-iwasawa-algebra)
- [Left ideal](#left-ideal)
  - [Maximal left ideal](#maximal-left-ideal)
    - [Scalar right action on a maximal-left-ideal quotient](#scalar-right-action-on-a-maximal-left-ideal-quotient)
- [Semisimple algebra](#semisimple-algebra)
- [Hochschild chain complex](#hochschild-chain-complex)
  - [Hochschild homology](#hochschild-homology)
- [Hochschild cochain complex](#hochschild-cochain-complex)
  - [Hochschild cup product](#hochschild-cup-product)
  - [Normalized Hochschild cochain complex](#normalized-hochschild-cochain-complex)
  - [Hochschild cocycle](#hochschild-cocycle)
  - [Hochschild cohomology](#hochschild-cohomology)
    - [Ground-ring qualification in Hochschild cohomology](#ground-ring-qualification-in-hochschild-cohomology)
    - [Hochschild cohomology of a polynomial algebra in one variable](#hochschild-cohomology-of-a-polynomial-algebra-in-one-variable)
    - [Second Hochschild cohomology classifies split square-zero extensions](#second-hochschild-cohomology-classifies-split-square-zero-extensions)
    - [Hochschild-Kostant-Rosenberg theorem](#hochschild-kostant-rosenberg-theorem)
    - [Gerstenhaber bracket](#gerstenhaber-bracket)
    - [Hochschild cohomological dimension](#hochschild-cohomological-dimension)
    - [Derivation into a bimodule](#derivation-into-a-bimodule)
      - [Derivation of an algebra](#derivation-of-an-algebra)
        - [Derivations of smooth functions are vector fields](#derivations-of-smooth-functions-are-vector-fields)
      - [Inner derivation](#inner-derivation)
        - [First Hochschild cohomology as outer derivations](#first-hochschild-cohomology-as-outer-derivations)
      - [Universal bimodule derivation](#universal-bimodule-derivation)
        - [Inner derivation through the universal bimodule derivation](#inner-derivation-through-the-universal-bimodule-derivation)
- [Specialization of an algebra](#specialization-of-an-algebra)

## Primitive ideal

↑ **Parent:** [Associative algebra](associative-algebra.md)

A primitive ideal of a unital [associative algebra](associative-algebra.md) is the [annihilator of a module](module-theory.md#annihilator-of-a-module) for a nonzero [simple module](module-theory.md#irreducible-module). Every maximal proper two-sided ideal is primitive: its quotient is a simple ring, and any simple module over that quotient has zero annihilator there. In a unital [Banach algebra](banach-algebra.md), a simple module can be realized as $A/L$ for a [maximal left ideal](#maximal-left-ideal); this ideal is closed, making the representation a bounded algebraically irreducible action on a [Banach space](banach-space.md).

## Ore extension

↑ **Parent:** [Associative algebra](associative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ore_extension)

An Ore extension uses a unital endomorphism $\sigma$ of $A$ and a $\sigma$-derivation $\delta$, satisfying $\delta(ab)=\sigma(a)\delta(b)+\delta(a)b$. Its elements have unique expressions $\sum_i a_it^i$ and multiplication is determined by the displayed relation. Applying the relation to $t(ab)$ shows why the endomorphism and [derivation](#derivation-of-an-algebra) conditions are exactly the compatibility conditions for [associativity](group.md#associative-property). A differential Ore extension has $\sigma=\operatorname{id}$. Adjoining ordinary partial derivatives successively to a [polynomial ring](commutative-algebra.md#polynomial-ring) gives the ordered-monomial construction of a [Weyl algebra](noncommutative-algebra.md#weyl-algebra).

## Algebra involution

↑ **Parent:** [Associative algebra](associative-algebra.md)

An algebra involution on a complex [associative algebra](associative-algebra.md) is a [conjugate-linear map](vector-space.md#antilinear-map) satisfying $(xy)^*=y^*x^*$ and $(x^*)^*=x$. It fixes the identity when one exists. A star algebra is an algebra equipped with such a map. These algebraic identities do not themselves impose [norm](functional-analysis.md#norm) [continuity](calculus.md#continuous-function) or the [C-star identity](banach-algebra.md#c-star-identity).

## Unital algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

An [associative algebra](associative-algebra.md) with a two-sided multiplicative identity. For a [subalgebra](algebra.md#subalgebra) of [bounded operators](topological-vector-space.md#continuous-linear-operator), the term [unital](#unital-algebra) here means that it contains the identity of the represented [Hilbert space](hilbert-space.md).

## Star-algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

A complex [associative algebra](associative-algebra.md) with a conjugate-linear involution satisfying the displayed product-reversal identities. An [operator algebra](functional-analysis.md#operator-algebra) closed under the Hilbert-space adjoint is a [star-algebra](#star-algebra). A [C-star algebra](banach-algebra.md#c-star-algebra) additionally has a complete [norm](functional-analysis.md#norm) with $\|a^*a\|=\|a\|^2$.

### Hermitian element of a star algebra

↑ **Parent:** [Star-algebra](#star-algebra)

A [Hermitian algebra element](#hermitian-element-of-a-star-algebra) of a [star-algebra](#star-algebra) is an element fixed by its [algebra involution](#algebra-involution). The identity and zero are [Hermitian algebra elements](#hermitian-element-of-a-star-algebra). For every $x$, both $xx^*$ and $x^*x$ are [Hermitian algebra elements](#hermitian-element-of-a-star-algebra). A real spectrum for all such elements is an extra condition in a general [Banach algebra](banach-algebra.md), rather than a consequence of the involution identities alone.

### Star-subalgebra

↑ **Parent:** [Star-algebra](#star-algebra)

A linear [subalgebra](algebra.md#subalgebra) closed under the involution. In [bounded operators](topological-vector-space.md#continuous-linear-operator), this means [closure](topology.md#closure-topology) under the [adjoint operator](hilbert-space.md#adjoint-operator); neither [norm](functional-analysis.md#norm) [closure](topology.md#closure-topology) nor operator-topology [closure](topology.md#closure-topology) is part of the definition. These distinctions matter in the [Von Neumann double commutant theorem](#von-neumann-double-commutant-theorem) and the [Kaplansky density theorem](#kaplansky-density-theorem).

## Cocenter of a finite-dimensional algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

The [cocenter of a finite-dimensional algebra](#cocenter-of-a-finite-dimensional-algebra) is the quotient by the vector subspace spanned by additive commutators $ab-ba$; this subspace need not be an [ideal](commutative-algebra.md#ideal). For a [group algebra](#group-algebra), its basis is indexed by [conjugacy classes](group-theory.md#conjugacy-class): every commutator of basis elements is a difference of conjugates, and every difference of conjugates is a commutator. For $M_n(k)$, off-diagonal matrix units and $E_{ii}-E_{jj}$ show that the quotient is one-dimensional, identified by the [trace](linear-algebra.md#matrix-trace).

### Frobenius map on an algebra cocenter

↑ **Parent:** [Cocenter of a finite-dimensional algebra](#cocenter-of-a-finite-dimensional-algebra)

In [characteristic](algebra.md#characteristic-of-a-field) $p>0$, the displayed map on the [cocenter of a finite-dimensional algebra](#cocenter-of-a-finite-dimensional-algebra) is additive and Frobenius-semilinear. Expand a $p$th power into words: nonconstant cyclic-word orbits have length $p$ and cancel modulo commutators. Also $(ab)^p$ and $(ba)^p$ have the same cocenter class, so the map kills additive commutators and is well defined.

Over a perfect [field](algebra.md#field) with split semisimple quotient, the stable image of this map has dimension equal to the number of [simple modules](module-theory.md#irreducible-module) of the [algebra](algebra.md). Indeed, the kernel of $C(A)\to C(A/J(A))$ has representatives in the nilpotent [Jacobson radical](noncommutative-algebra.md#jacobson-radical), so an iterate kills it. On the [semisimple algebra](#semisimple-algebra) quotient, each matrix-block coordinate is a field trace, and $\operatorname{tr}(a^p)=\operatorname{tr}(a)^p$. For a split semisimple quotient, Frobenius is bijective on every coordinate. In a [group algebra](#group-algebra) over an [algebraically closed field](algebra.md#algebraically-closed-field), the stable image has the [p-regular element](representation-theory.md#p-regular-element) conjugacy classes as its basis, proving the simple-module counting theorem.

## Representation variety of an associative algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

For a finitely generated [associative algebra](associative-algebra.md), choose matrices for its generators and impose its polynomial relations. This defines an [affine variety](algebraic-geometry.md#affine-algebraic-set). With prescribed [orthogonal idempotents](commutative-algebra.md#orthogonal-idempotent) $1=\sum_ie_i$, require their images to be the standard projections on $\bigoplus_i k^{n_i}$. The resulting variety is $\operatorname{Rep}_A(\mathbf n)$, acted on by $\prod_i\operatorname{GL}_{n_i}(k)$. Without a chosen idempotent decomposition, the usual variety is $\operatorname{Rep}_A(r)=\operatorname{Hom}_{k\text{-alg}}(A,M_r(k))$. Its orbits are module isomorphism classes, and their stabilizers are automorphism groups.

## Units of a finite-dimensional algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

The unit group $E^\times$ is a nonempty open subset of the affine space $E$, detected by the determinant of left multiplication. It is therefore an irreducible connected [linear algebraic group](lie-theory.md#linear-algebraic-group). Its map to $(E/J(E))^\times$ has kernel $1+J(E)$, a closed unipotent subgroup since the radical is nilpotent.

## Free associative algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

The free associative algebra has a basis of finite words in its generators, including the empty word as identity. Multiplication concatenates words without commutativity relations. It is the [path algebra](algebra.md#path-algebra) of the [quiver with r loops](algebra.md#quiver-with-r-loops). With one generator it is a polynomial algebra.

## Frobenius algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frobenius_algebra)

A finite-dimensional unital [associative algebra](associative-algebra.md) over a [field](algebra.md#field) admitting a [linear functional](linear-algebra.md#linear-functional) $\varepsilon$ whose pairing $(a,b)\mapsto\varepsilon(ab)$ is nondegenerate. The [dual numbers](commutative-algebra.md#dual-number) with functional extracting the nilpotent coefficient are an example; semisimplicity is unnecessary.

## Opposite algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

The same underlying [module](module-theory.md#module-mathematics) as an [associative algebra](associative-algebra.md), with multiplication $a\cdot_{\mathrm{op}}b=ba$. Right multiplications identify $H^{\mathrm{op}}$ with $\operatorname{End}_H(H)$ for the left regular [module](module-theory.md#module-mathematics).

## Right ideal

↑ **Parent:** [Associative algebra](associative-algebra.md)

A right ideal $I$ in a unital [associative algebra](associative-algebra.md) $A$ is a [vector subspace](vector-space.md#vector-subspace) with $IA\subseteq I$, equivalently a [submodule](module-theory.md#submodule) of the right regular [module](module-theory.md#module-mathematics). It need not be a left [ideal](commutative-algebra.md#ideal). Its finite generation refers to right multiplication by elements of $A$.

### Maximal right ideal

↑ **Parent:** [Right ideal](#right-ideal)

A proper [right ideal](#right-ideal) $L$ is maximal if no proper [right ideal](#right-ideal) strictly contains it. Equivalently, $A/L$ is a [simple module](module-theory.md#irreducible-module). The [Jacobson radical](noncommutative-algebra.md#jacobson-radical) is the intersection of all [maximal right ideals](#maximal-right-ideal).

## Formal associative deformation

↑ **Parent:** [Associative algebra](associative-algebra.md)

A formal associative deformation is a unital $k[[t]]$-bilinear product continuous for the [adic topology](commutative-algebra.md#adic-topology) on $A[[t]]$ of the form $a*b=ab+\sum_{r\geq1}t^r\mu_r(a,b)$. Each coefficient $\mu_r$ is a $k$-bilinear map $A\otimes A\to A$, and the whole product satisfies [associativity](group.md#associative-property). For an infinite-dimensional [algebra](algebra.md), $A[[t]]$ is the completed [tensor product](linear-algebra.md#tensor-product) $\varprojlim_nA\otimes k[t]/(t^n)$ and generally differs from the ordinary $A\otimes k[[t]]$.

### Weyl deformation of a polynomial algebra in two variables

↑ **Parent:** [Formal associative deformation](#formal-associative-deformation)

The algebra over $k[t]$ defined by $yx-xy=t$ has ordered [basis](vector-space.md#basis) $x^iy^j$, by its differential Ore-extension construction. Its $t$-adic completion is a formal associative [formal associative deformation](#formal-associative-deformation) of $k[x,y]$. In characteristic zero its first-order multiplication term is $f(a,b)=\partial_y a\,\partial_x b$. The cocycle is not a coboundary: a degree-two coboundary on a commutative algebra is symmetric, whereas $f(y,x)-f(x,y)=1$.

### First-order associative deformation

↑ **Parent:** [Formal associative deformation](#formal-associative-deformation)

The order-$\varepsilon$ part of [associativity](group.md#associative-property) is $af(b,c)-f(ab,c)+f(a,bc)-f(a,b)c=0$, so $f$ is a [Hochschild cocycle](#hochschild-cocycle). A change of coordinates $T=1+\varepsilon g$ changes $f$ to $f+\delta g$. Therefore equivalence classes of first-order associative deformations of a fixed underlying algebra are its second [Hochschild cohomology](#hochschild-cohomology). Unital deformations use normalized cochains.

#### Second-order obstruction to an associative deformation

↑ **Parent:** [First-order associative deformation](#first-order-associative-deformation)

Expanding [associativity](group.md#associative-property) for $a*b=ab+tf(a,b)+t^2\mu_2(a,b)$ modulo $t^3$ gives the displayed equation. If $\delta f=0$, its right side is a degree-three [Hochschild cocycle](#hochschild-cocycle). Its class in $HH^3(R,R)$ must vanish to extend the first-order [formal associative deformation](#formal-associative-deformation) to second order. A nonzero class in $HH^2$ therefore need not integrate to a full [formal associative deformation](#formal-associative-deformation).

### Trivial formal deformation

↑ **Parent:** [Formal associative deformation](#formal-associative-deformation)

A [formal associative deformation](#formal-associative-deformation) is trivial if a $k[[t]]$-linear [automorphism](algebra.md#automorphism) continuous for the [adic topology](commutative-algebra.md#adic-topology) $T=\operatorname{id}\pmod t$ fixing the identity transports the deformed multiplication to the original one. This is equivalence by a formal change of coordinates, stronger than merely an abstract [algebra isomorphism](algebra.md#algebra-isomorphism) between unspecified middle terms.

#### Formal rigidity from vanishing second Hochschild cohomology

↑ **Parent:** [Trivial formal deformation](#trivial-formal-deformation)

If $HH^2(A,A)=0$, every [formal associative deformation](#formal-associative-deformation) on the [adic completion of a module](commutative-algebra.md#adic-completion-of-a-module) $A[[t]]$ is trivial. After killing lower coefficients, [associativity](group.md#associative-property) makes the order-$r$ coefficient a [Hochschild cocycle](#hochschild-cocycle) $\mu_r=\delta g_r$. Transport by $\operatorname{id}+t^rg_r$ subtracts $\delta g_r$ and kills it. The successive transformations stabilize modulo each $t^n$ and converge to an invertible change of coordinates. Completeness, and equivalence congruent to the identity modulo $t$, are essential to this argument.

<h2 id="gelfand-kirillov-dimension">Gelfand–Kirillov dimension</h2>

↑ **Parent:** [Associative algebra](associative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gelfand–Kirillov_dimension)

For a nonzero finitely generated [algebra](algebra.md) over a [field](algebra.md#field), choose a finite-dimensional generating [vector subspace](vector-space.md#vector-subspace) $V$ containing $1$. The dimension is $\operatorname{GKdim}A=\limsup_{n\to\infty}\log(\dim_kV^n)/\log n$. Changing $V$ only rescales the filtration index by bounded factors. A nonzero finite-dimensional [algebra](algebra.md) has dimension zero; a [polynomial ring](commutative-algebra.md#polynomial-ring) in $r$ variables has dimension $r$. The zero [algebra](algebra.md) is often assigned dimension $-\infty$.

<h3 id="gelfand-kirillov-dimension-of-a-module">Gelfand–Kirillov dimension of a module</h3>

↑ **Parent:** [Gelfand–Kirillov dimension](#gelfand-kirillov-dimension)

For a nonzero right [module](module-theory.md#module-mathematics) $M$ that is a [finitely generated module](module-theory.md#finitely-generated-module), choose a finite-dimensional generating [vector subspace](vector-space.md#vector-subspace) $W$ and define $\operatorname{GKdim}_AM=\limsup_{n\to\infty}\log(\dim_kWV^n)/\log n$, where $V$ generates the [algebra](algebra.md) and contains $1$. For a left [module](module-theory.md#module-mathematics) use $V^nW$. It is independent of these choices and measures polynomial-order growth of a generating [filtration of a module](module-theory.md#filtration-of-a-module).

#### Bernstein growth dimension of a Weyl algebra module

↑ **Parent:** [Gelfand–Kirillov dimension of a module](#gelfand-kirillov-dimension-of-a-module)

For a nonzero finitely generated [Weyl algebra](noncommutative-algebra.md#weyl-algebra) [module](module-theory.md#module-mathematics), choose a finite-dimensional generating subspace $M_0$. Under the [Bernstein filtration](noncommutative-algebra.md#bernstein-filtration), $\dim(F_jA_nM_0)$ is eventually polynomial because the graded [module](module-theory.md#module-mathematics) is finite over a polynomial ring. Its degree is independent of the generating subspace, since two generating filtrations bound each other after fixed shifts. It equals the [Gelfand–Kirillov dimension of a module](#gelfand-kirillov-dimension-of-a-module).

##### Characteristic variety of a Weyl algebra module

↑ **Parent:** [Bernstein growth dimension of a Weyl algebra module](#bernstein-growth-dimension-of-a-weyl-algebra-module)

A good [Bernstein filtration](noncommutative-algebra.md#bernstein-filtration) on a finitely generated module produces a finite graded module over $\operatorname{gr}A_n\cong\mathbb C[x_1,\ldots,x_n,\xi_1,\ldots,\xi_n]$. Its support is the characteristic variety for this filtration. Its algebraic dimension is the [Bernstein growth dimension of a Weyl algebra module](#bernstein-growth-dimension-of-a-weyl-algebra-module), which is independent of the choice of good filtration.

###### Independence of characteristic support from a good module filtration

↑ **Parent:** [Characteristic variety of a Weyl algebra module](#characteristic-variety-of-a-weyl-algebra-module)

Fix the [Bernstein filtration](noncommutative-algebra.md#bernstein-filtration) on the [Weyl algebra](noncommutative-algebra.md#weyl-algebra). Two [good filtrations of a module](module-theory.md#good-filtration-of-a-module) are bounded shifts of one another: $F_iM\subseteq G_{i+c}M$ and conversely. If an operator of degree $d$ has symbol annihilating $\operatorname{gr}_FM$, its $r$th power lowers the expected filtration degree by $r$. For $r>2c$, comparison of filtrations forces the same power of its symbol to annihilate $\operatorname{gr}_GM$. Reversing the roles gives equality of the radical [annihilator](module-theory.md#annihilator-ring-theory) ideals and hence equality of [support of a module](module-theory.md#support-of-a-module). The algebra filtration is held fixed; changing between order and Bernstein filtrations need not preserve the same variety.

##### Holonomic Weyl algebra module

↑ **Parent:** [Bernstein growth dimension of a Weyl algebra module](#bernstein-growth-dimension-of-a-weyl-algebra-module)

A nonzero finitely generated [Weyl algebra](noncommutative-algebra.md#weyl-algebra) module over $A_n(\mathbb C)$ is holonomic when it attains the lower bound in the [Bernstein inequality for Weyl algebra modules](#bernstein-inequality-for-weyl-algebra-modules). The zero module is also conventionally called holonomic. Nonzero subquotients of a holonomic module remain holonomic. Additivity and integrality of the leading Hilbert-polynomial multiplicity then bound the number of nonzero factors in any submodule chain, giving finite composition length.

###### Multiplicity bounds the length of a holonomic Weyl module

↑ **Parent:** [Holonomic Weyl algebra module](#holonomic-weyl-algebra-module)

Every nonzero subquotient of a [holonomic Weyl algebra module](#holonomic-weyl-algebra-module) over a characteristic-zero [field](algebra.md#field) has dimension $n$, by [Bernstein inequality for Weyl algebra modules](#bernstein-inequality-for-weyl-algebra-modules) and [dimension and multiplicity in a filtered exact sequence](module-theory.md#dimension-and-multiplicity-in-a-filtered-exact-sequence). Each strict step in a [submodule](module-theory.md#submodule) chain consumes positive [multiplicity of a filtered module](module-theory.md#multiplicity-of-a-filtered-module). With a [standard graded algebra](commutative-algebra.md#standard-graded-algebra) normalization these multiplicities are integral. There are therefore at most $m(M)$ strict steps. The [module](module-theory.md#module-mathematics) is [Artinian](algebra.md#artinian-ring) and [Noetherian](algebra.md#noetherian-ring), and its [module length](module-theory.md#length-of-a-module) is bounded by that multiplicity.

##### Bernstein inequality for Weyl algebra modules

↑ **Parent:** [Bernstein growth dimension of a Weyl algebra module](#bernstein-growth-dimension-of-a-weyl-algebra-module)

For a nonzero finitely generated [module](module-theory.md#module-mathematics) over the complex [Weyl algebra](noncommutative-algebra.md#weyl-algebra) $A_n$, its [Bernstein growth dimension of a Weyl algebra module](#bernstein-growth-dimension-of-a-weyl-algebra-module) is at least $n$. The [faithful finite-step action of a Weyl algebra](#faithful-finite-step-action-of-a-weyl-algebra) gives $\dim F_jA_n\leq(\dim M_j)(\dim M_{2j})$. Comparing degrees $2n$ and $2d(M)$ proves the inequality. The polynomial [module](module-theory.md#module-mathematics) has dimension $n$, so the bound is sharp. This is an algebraic growth inequality, distinct from probabilistic Bernstein inequalities.

###### Faithful finite-step action of a Weyl algebra

↑ **Parent:** [Bernstein inequality for Weyl algebra modules](#bernstein-inequality-for-weyl-algebra-modules)

For $M_j=F_jA_nM_0$ and $M_0\ne0$, the action map in the display is injective. If $a\in F_j$ kills $M_j$, each commutator $[a,z]$ with a generator lies in $F_{j-1}$ and kills $M_{j-1}$. Induction makes all these commutators zero, so $a$ is [scalar](vector-space.md#scalar); since it kills $M_0$, it is zero. This finite-step faithfulness does not require the whole [module](module-theory.md#module-mathematics) to be finite-dimensional.

###### Scalar extraction by iterated Weyl commutators

↑ **Parent:** [Faithful finite-step action of a Weyl algebra](#faithful-finite-step-action-of-a-weyl-algebra)

For a nonzero element of a [Weyl algebra](noncommutative-algebra.md#weyl-algebra) over a characteristic-zero [field](algebra.md#field), choose a monomial $x^\alpha D^\beta$ of maximal total degree with coefficient $c_{\alpha\beta}\ne0$. The displayed iterated [commutators](lie-algebra.md#commutator) kill every lower-degree monomial. Another monomial of the same degree survives only if all its exponents dominate $(\alpha,\beta)$, which forces equality. Hence the result is a nonzero [scalar](vector-space.md#scalar). If the element has filtered degree at most $j$, expansion of these [commutators](lie-algebra.md#commutator) gives a sum of terms $uav$ with both $u$ and $v$ of degree at most $j$. This proves [faithful finite-step action of a Weyl algebra](#faithful-finite-step-action-of-a-weyl-algebra) over any characteristic-zero [field](algebra.md#field).

## Block of an Artinian algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

A block of an [associative algebra](associative-algebra.md) with a finite decomposition of its identity is a two-sided [direct summand](vector-space.md#direct-summand) $Ae$ corresponding to a [primitive central idempotent](#primitive-central-idempotent) $e$. Its identity is $e$, and it cannot be split into two nonzero [algebras](algebra.md) by [central idempotents](#central-idempotent). For a [group algebra](#group-algebra) of a finite [group](group.md), this agrees with a [block of a group algebra](representation-theory.md#block-of-a-group-algebra). Orthogonal [primitive central idempotents](#primitive-central-idempotent) give $A=\bigoplus_iAe_i$.

## Maximal commutative subalgebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

A commutative unital subalgebra $D$ of an [associative algebra](associative-algebra.md) $A$ is maximal commutative if no larger commutative subalgebra contains it. Equivalently $C_A(D)=D$: any element of its [centralizer of a subalgebra](#centralizer-of-a-subalgebra) generates a commutative algebra together with $D$. The full diagonal [matrix algebra](#matrix-algebra) inside $M_n(\mathbb C)$ is an example.

## Centralizer of a subalgebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

For a subalgebra $B$ of an [associative algebra](associative-algebra.md) $A$, its centralizer is

$$
C_A(B)=\{a\in A:ab=ba\text{ for every }b\in B\}.
$$

It is a subalgebra of $A$. When $A$ is a [group algebra](#group-algebra) and $B$ is the group algebra of a [subgroup](group.md#subgroup) $H$, its elements are exactly the linear combinations with coefficients constant on the conjugation orbits of $H$.

### Commutant of an operator algebra

↑ **Parent:** [Centralizer of a subalgebra](#centralizer-of-a-subalgebra)

The commutant of $A\subseteq\operatorname{End}(T)$ is $A\prime=\{b:ba=ab\text{ for all }a\in A\}$. This centralizer is an operator algebra. The [double-centralizer theorem for semisimple operator algebras](#double-centralizer-theorem-for-semisimple-operator-algebras) and [Schur–Weyl duality](lie-theory.md#schur-weyl-duality) use this meaning, which is distinct from the centralizer of a single element of a group.

#### Von Neumann double commutant theorem

↑ **Parent:** [Commutant of an operator algebra](#commutant-of-an-operator-algebra)

For a unital star-subalgebra $A$ of the [bounded operators](topological-vector-space.md#continuous-linear-operator) on a complex [Hilbert space](hilbert-space.md), its [strong operator topology](functional-analysis.md#strong-operator-topology) and [weak operator topology](functional-analysis.md#weak-operator-topology) closures equal its double [commutant of an operator algebra](#commutant-of-an-operator-algebra). To approximate $T\in A''$ on finitely many vectors, take their tuple in $H^m$. The projection onto its diagonal-$A$ cyclic subspace has matrix entries in $A'$, so it commutes with the diagonal action of $T$. Therefore the image tuple under $T$ lies in that cyclic subspace and can be approximated by a single $a\in A$.

##### Kaplansky density theorem

↑ **Parent:** [Von Neumann double commutant theorem](#von-neumann-double-commutant-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kaplansky_density_theorem)

For a [unital](#unital-algebra) [star-subalgebra](#star-subalgebra) $A\subseteq B(H)$, its [unit ball](functional-analysis.md#unit-ball) is dense in the [unit ball](functional-analysis.md#unit-ball) of $A''$ in the [strong operator topology](functional-analysis.md#strong-operator-topology). The same holds for [self-adjoint](linear-operator-theory.md#self-adjoint-operator) unit balls and for positive unit balls, and the full unit balls may be approximated strongly together with their adjoints. Passing first to the [norm](functional-analysis.md#norm) [closure](topology.md#closure-topology) allows [continuous functional calculus](banach-algebra.md#continuous-functional-calculus); [resolvent](functional-analysis.md#resolvent-of-an-operator) identities prove strong [continuity](calculus.md#continuous-function) of continuous functions vanishing at infinity, even for unbounded approximating nets of [self-adjoint operators](linear-operator-theory.md#self-adjoint-operator). A cutoff function supplies the [norm](functional-analysis.md#norm) bound, and a two-by-two [self-adjoint](linear-operator-theory.md#self-adjoint-operator) [matrix](vector-space.md#matrix) removes the [self-adjoint](linear-operator-theory.md#self-adjoint-operator) restriction.

#### Double commutant theorem for star-algebras

↑ **Parent:** [Commutant of an operator algebra](#commutant-of-an-operator-algebra)

A unital [subalgebra](algebra.md#subalgebra) $A\subseteq\operatorname{End}(V)$ closed under the [adjoint operator](hilbert-space.md#adjoint-operator), on a finite-dimensional real or complex [inner product space](linear-algebra.md#inner-product-space), equals its double [commutant of an operator algebra](#commutant-of-an-operator-algebra). Here is a proof that does not require a classification of [algebras](algebra.md). For $N=\dim V$, choose a [basis](vector-space.md#basis) $(v_1,\ldots,v_N)$ and let $W=\{(av_1,\ldots,av_N):a\in A\}\subseteq V^N$. The diagonal action of $A$ preserves $W$ and $W^\perp$, so the [orthogonal projection](hilbert-space.md#orthogonal-projection) onto $W$ commutes with that action. Each matrix entry of this projection belongs to $A'$. Hence the diagonal action of $b\in A''$ commutes with the projection and preserves $W$. Since $1\in A$, the tuple $(v_1,\ldots,v_N)$ belongs to $W$, and therefore $(bv_1,\ldots,bv_N)=(av_1,\ldots,av_N)$ for one $a\in A$. This implies $b=a$. Without the unital hypothesis the conclusion is $A''=A+\mathbb F1$.

#### Double-centralizer theorem for semisimple operator algebras

↑ **Parent:** [Commutant of an operator algebra](#commutant-of-an-operator-algebra)

For a finite-dimensional [semisimple algebra](#semisimple-algebra) acting faithfully on $T$, write $T=\bigoplus_i S_i\otimes M_i$. Then the algebra acts by the full matrix algebra on each simple factor, while its commutant acts by the full matrix algebra on each multiplicity factor. Taking the commutant twice recovers the original image. This is the algebraic basis of [Schur–Weyl duality](lie-theory.md#schur-weyl-duality).

## Matrix algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

For an [associative algebra](associative-algebra.md) $A$, its matrix algebra $M_n(A)$ consists of all $n$ by $n$ [matrices](vector-space.md#matrix) over $A$, with ordinary matrix multiplication. If $A=k$ is a [field](algebra.md#field), this is $\operatorname{End}_k(k^n)$ and is a [central simple algebra](#central-simple-algebra). Full matrix algebras over division rings are the factors in the [Artin–Wedderburn theorem](#artin-wedderburn-theorem).

## Block of a finite-dimensional algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

A block of a finite-dimensional [associative algebra](associative-algebra.md) $R$ is a two-sided ideal $Re$ associated with a [primitive idempotent](commutative-algebra.md#primitive-idempotent) $e$ in the [center of an associative algebra](#center-of-an-associative-algebra). Its identity is $e$, and $R$ is the product of these blocks. An $R$-[module](module-theory.md#module-mathematics) belongs to this block if $eM=M$. For a [semisimple algebra](#semisimple-algebra), the [Artin–Wedderburn theorem](#artin-wedderburn-theorem) says the blocks are its full [matrix algebras](#matrix-algebra) over division rings. For a [group algebra](#group-algebra) this specializes to a [block of a group algebra](representation-theory.md#block-of-a-group-algebra).

### Ext-connected components determine blocks

↑ **Parent:** [Block of a finite-dimensional algebra](#block-of-a-finite-dimensional-algebra)

For a finite-dimensional [associative algebra](associative-algebra.md), form a graph on its [simple modules](module-theory.md#irreducible-module), joining $S,T$ when $\operatorname{Ext}^1(S,T)$ or $\operatorname{Ext}^1(T,S)$ is nonzero. Its connected components are exactly the [simple modules](module-theory.md#irreducible-module) belonging to each [block of a finite-dimensional algebra](#block-of-a-finite-dimensional-algebra). They are also the components generated by sharing a [Jordan–Hölder factor](finite-group-theory.md#jordan-holder-factor) occurrence in an [indecomposable representation](representation-theory.md#indecomposable-representation) that is a [projective module](module-theory.md#projective-module).

Indeed, [Ext separation of finite-length modules](algebra.md#ext-separation-of-finite-length-modules) would split the regular module of a block into canonical summands if that block had two graph components. Right multiplication preserves these summands, so its projection supplies a nontrivial central [idempotent](commutative-algebra.md#idempotent), contradicting the definition of a block. An indecomposable projective belongs to one block. Finally, a nonsplit extension $0\to U\to V\to W\to0$ of [simple modules](module-theory.md#irreducible-module) is a quotient of the [projective cover](module-theory.md#projective-cover) of $W$: a lift onto $W$ must contain $U$, since otherwise the extension splits. Thus its two endpoints share factors in an indecomposable projective.

## Basic algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

A finite-dimensional algebra over an algebraically closed field is basic when its semisimple quotient is a finite product of copies of the field, equivalently when every simple module occurs with multiplicity one in the semisimple quotient of the regular representation.

### Ext quiver

↑ **Parent:** [Basic algebra](#basic-algebra)

For a finite-dimensional [associative algebra](associative-algebra.md) over an [algebraically closed field](algebra.md#algebraically-closed-field), the [Ext quiver](#ext-quiver) has a vertex for each [simple module](module-theory.md#irreducible-module) isomorphism class and $a_{ij}$ arrows $i\to j$. For a [basic algebra](#basic-algebra) with $P_i=Ae_i$, applying $\operatorname{Hom}_A(-,S_j)$ to the projective-cover sequence gives $a_{ij}=\dim e_j(J/J^2)e_i$. Our [path algebra](algebra.md#path-algebra) convention multiplies consecutive arrows $\alpha:i\to j$, $\beta:j\to l$ as $\beta\alpha$, making left modules have arrow maps $V_i\to V_j$. The orientation convention must be stated when comparing other definitions.

## Central simple algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Central_simple_algebra)

A central simple algebra over a [field](algebra.md#field) $k$ is a finite-dimensional associative $k$-algebra that is a [simple ring](commutative-algebra.md#simple-ring) and whose center is exactly $k$.

### Quaternion algebra

↑ **Parent:** [Central simple algebra](#central-simple-algebra)

For a [field](algebra.md#field) of characteristic other than two and nonzero $a,b$, the [quaternion algebra](#quaternion-algebra) has basis $1,i,j,ij$ with the displayed relations. It is a four-dimensional [central simple algebra](#central-simple-algebra). After adjoining a square root of $a$, diagonalizing $i$ and taking $j=\left(\begin{smallmatrix}0&b\\1&0\end{smallmatrix}\right)$ identifies it with $M_2$. Quaternion conjugation fixes scalars and negates $i,j,ij$, giving norm $x_0^2-a x_1^2-b x_2^2+ab x_3^2$. An element is invertible exactly when its norm is nonzero. Thus the [quaternion algebra](#quaternion-algebra) is either a [division algebra](algebra.md#division-algebra) or a split [matrix algebra](#matrix-algebra). The familiar [quaternion](algebra.md#quaternion) algebra is $(-1,-1)_{\mathbb R}$.

#### Quaternion norm obstruction at primes congruent to three modulo four

↑ **Parent:** [Quaternion algebra](#quaternion-algebra)

For $p\equiv3\pmod4$ and $z=x+iy\ne0$ with rational $x,y$, divide $x^2+y^2$ by the square of the common minimum $p$-adic valuation. Its remaining unit cannot vanish modulo $p$, because $-1$ is not a square there. The norm therefore has even valuation. In particular a rational parameter $a$ with odd valuation at such a prime is not a norm, and $(-1,a)_{\mathbb Q}$ is a division [quaternion algebra](#quaternion-algebra): its norm $N(z)-aN(w)$ cannot vanish for a nonzero element $z+w j$.

### Reduced norm

↑ **Parent:** [Central simple algebra](#central-simple-algebra)

The [reduced norm](#reduced-norm) of an element of a [central simple algebra](#central-simple-algebra) of degree $d$ is its [determinant](linear-algebra.md#determinant) after any splitting isomorphism to $M_d$. [Inner automorphisms of a matrix algebra](#inner-automorphisms-of-a-matrix-algebra) preserve that [determinant](linear-algebra.md#determinant), while Galois invariance descends its polynomial coefficients to the center. It is a multiplicative homogeneous degree-$d$ polynomial, vanishing exactly on noninvertible elements. On a [central division algebra](algebra.md#central-division-algebra) it is anisotropic.

### Inner automorphisms of a matrix algebra

↑ **Parent:** [Central simple algebra](#central-simple-algebra)

Every $L$-algebra automorphism of $M_d(L)$ is conjugation by an invertible matrix. For matrix units, the vectors $h(E_{i1})w$ with $0\ne w\in\operatorname{im}h(E_{11})$ form a basis in which $h$ acts in the usual way on all matrix units. Scalar conjugating matrices act trivially, giving $\operatorname{Aut}_L(M_d(L))=\operatorname{PGL}_d(L)$.

### Splitting field of a central simple algebra

↑ **Parent:** [Central simple algebra](#central-simple-algebra)

An extension $E/K$ splits a [central simple algebra](#central-simple-algebra) $A$ of degree $d$ when $A\otimes_KE\cong M_d(E)$. A finite separable splitting field exists. Splitting is preserved by further scalar extension and is equivalent to the vanishing of the restricted [Brauer group](#brauer-group) class.

### Degree of a central simple algebra

↑ **Parent:** [Central simple algebra](#central-simple-algebra)

A [central simple algebra](#central-simple-algebra) $A$ has dimension $d^2$ over its center. Its degree is this integer $d$. Over a splitting field it becomes $M_d$, so degree records the matrix size independently of the chosen splitting.

<h3 id="artin-wedderburn-theorem">Artin–Wedderburn theorem</h3>

↑ **Parent:** [Central simple algebra](#central-simple-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Artin–Wedderburn_theorem)

Every finite-dimensional semisimple algebra is a finite product of matrix algebras over division algebras. In particular, every [central simple algebra](#central-simple-algebra) over $k$ is isomorphic to $M_r(D)$ for a finite-dimensional central division algebra $D$ over $k$. The integer $r$ and the isomorphism class of $D$ are unique.

Indeed, decompose the right regular module of a finite-dimensional semisimple algebra $A$ as

$$
A_A\cong\bigoplus_{i=1}^sS_i^{n_i},
$$

where the $S_i$ are pairwise nonisomorphic [simple modules](module-theory.md#irreducible-module). The [Schur lemma](representation-theory.md#schur-s-lemma) makes $D_i=\operatorname{End}_A(S_i)$ a [division ring](commutative-algebra.md#division-ring) and gives $\operatorname{Hom}_A(S_i,S_j)=0$ for $i\ne j$. Left multiplication identifies

$$
A\cong\operatorname{End}_A(A_A)
\cong\prod_{i=1}^sM_{n_i}(D_i).
$$

Conversely, the column module over $M_n(D)$ is simple and the regular module is a direct sum of $n$ copies of it, so finite products of such matrix rings are semisimple. The simple-module decomposition also proves uniqueness up to permuting the factors.

#### Burnside matrix-algebra theorem

↑ **Parent:** [Artin–Wedderburn theorem](#artin-wedderburn-theorem)

For a nonzero finite-dimensional complex [vector space](vector-space.md) $V$, a unital [matrix algebra](#matrix-algebra) acting irreducibly on $V$ is the full endomorphism algebra. Its [Jacobson radical](noncommutative-algebra.md#jacobson-radical) annihilates $V$: otherwise the radical times $V$ is all of $V$, contradicting nilpotence. Faithfulness kills the radical, and the [Artin–Wedderburn theorem](#artin-wedderburn-theorem) then leaves one simple matrix factor acting on its standard column [module](module-theory.md#module-mathematics). This is a matrix-algebra theorem, distinct from the orbit-counting [Burnside lemma](representation-theory.md#burnside-s-lemma) and the finite-group [Burnside's theorem](group.md#burnside-s-theorem).

### Tensor product of central simple algebras

↑ **Parent:** [Central simple algebra](#central-simple-algebra)

The [tensor product](linear-algebra.md#tensor-product) over $k$ of two central simple $k$-algebras is central simple. After extending scalars to an algebraic closure, both factors and their tensor product become full matrix algebras; faithful flatness then descends simplicity and the center.

### Brauer group

↑ **Parent:** [Central simple algebra](#central-simple-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brauer_group)

The Brauer group of a field $k$ consists of [Morita equivalence](noncommutative-algebra.md#morita-equivalence) classes of central simple $k$-algebras. Multiplication is induced by tensor product, the identity is $[k]$, and the inverse of $[A]$ is the class of the opposite algebra $A^{\mathrm{op}}$.

#### Brauer class

↑ **Parent:** [Brauer group](#brauer-group)

The Brauer class of a [central simple algebra](#central-simple-algebra) is its equivalence class under adjoining matrix-algebra factors. Two algebras have the same class exactly when their central division-algebra representatives are isomorphic. The zero class consists of split matrix algebras; the inverse of $[A]$ is the class of the [opposite algebra](#opposite-algebra). For a [cyclic algebra](#cyclic-algebra) $(L/K,\sigma,a)$, the class is zero exactly when $a$ is a [field norm](algebraic-number-theory.md#field-norm) from $L$.

#### Albert-Brauer-Hasse-Noether theorem

↑ **Parent:** [Brauer group](#brauer-group)

For a [number field](algebraic-number-theory.md#number-field) $K$, localization of the [Brauer group](#brauer-group) is injective. Its image is exactly the finite-support tuples of local classes whose [local Brauer invariants](#local-brauer-invariant) sum to zero. The non-Archimedean summands have invariant [group](group.md) $\mathbb Q/\mathbb Z$, real summands have $\{0,1/2\}$, and complex summands are zero. For a cyclic character $\chi$ and parameter $a$, the invariant of the local [cyclic algebra](#cyclic-algebra) is $\chi(\operatorname{Art}_{K_v}(a))$. Thus the zero-sum condition on principal parameters is the additive form of [Artin reciprocity](algebraic-number-theory.md#artin-reciprocity-law).

#### Independent quaternion classes over rational numbers

↑ **Parent:** [Brauer group](#brauer-group)

Associate to each prime $p\equiv3\pmod4$ the class of $(-1,p)_{\mathbb Q}$. These classes have order two, since quaternion conjugation identifies the algebra with its opposite. The product rule $[(-1,a)][(-1,b)]=[(-1,ab)]$ follows by factoring their [tensor product](linear-algebra.md#tensor-product) into the commuting subalgebras generated by $i_1,j_1j_2$ and by $i_1i_2,j_2$; the second is the split algebra $(1,b)$. Every nonempty finite product of distinct such primes has an odd valuation at one of them. The [quaternion norm obstruction at primes congruent to three modulo four](#quaternion-norm-obstruction-at-primes-congruent-to-three-modulo-four) therefore makes its class nonzero, proving independence. Euclid's construction $4p_1\cdots p_m-1$ proves there are infinitely many such primes.

#### Brauer p-divisibility in characteristic p

↑ **Parent:** [Brauer group](#brauer-group)

In characteristic $p$, the exact sequence $1\to K_s^{\times}\xrightarrow{p}K_s^{\times}\to K_s^{\times}/(K_s^{\times})^p\to1$ has a quotient killed by $p$. The [characteristic p Galois dimension bound](group-theory.md#characteristic-p-galois-dimension-bound) makes its second cohomology zero. Hence multiplication by $p$ on $\operatorname{Br}(K)$ is surjective. The root map is injective, and its failure of surjectivity on a separable closure is encoded by the quotient.

#### Witt residue sequence

↑ **Parent:** [Brauer group](#brauer-group)

For a complete discretely valued field $K$ with perfect [residue field](commutative-algebra.md#residue-field) $k$, there is a split exact sequence $0\to\operatorname{Br}(k)\to\operatorname{Br}(K)\xrightarrow{\partial_K}H^1(k,\mathbb Q/\mathbb Z)\to0$. The residue is canonical. A [uniformizer](commutative-algebra.md#uniformizer) chooses a splitting $\chi\mapsto(\chi,\pi)$; this choice does not make the residue itself noncanonical.

##### Local Brauer invariant

↑ **Parent:** [Witt residue sequence](#witt-residue-sequence)

For a [local field](arithmetic.md#local-field) with finite [residue field](commutative-algebra.md#residue-field), evaluate the Witt residue character on arithmetic Frobenius. This gives $\operatorname{inv}_K:\operatorname{Br}(K)\cong\mathbb Q/\mathbb Z$. For the unramified degree-$m$ [cyclic algebra](#cyclic-algebra) with arithmetic Frobenius generator and parameter $a$, the invariant is $v_K(a)/m$. Its reduced denominator is the index of the division representative.

###### Local fundamental class

↑ **Parent:** [Local Brauer invariant](#local-brauer-invariant)

For a finite [Galois extension](galois-theory.md#finite-galois-extension) $L/K$ of non-Archimedean [local fields](arithmetic.md#local-field), its relative [Brauer group](#brauer-group) is the kernel of restriction $\operatorname{Br}(K)\to\operatorname{Br}(L)$ and identifies with $H^2(\operatorname{Gal}(L/K),L^\times)$. Restriction multiplies the [local Brauer invariant](#local-brauer-invariant) by $[L:K]$. This kernel is therefore cyclic of order $[L:K]$, and the indicated class is its distinguished generator. In an [unramified extension](arithmetic.md#unramified-extension) with [arithmetic Frobenius](arithmetic.md#frobenius-automorphism) generator it is represented by the [cyclic algebra](#cyclic-algebra) with parameter a [uniformizer](commutative-algebra.md#uniformizer).

###### Restriction and corestriction of local Brauer invariants

↑ **Parent:** [Local Brauer invariant](#local-brauer-invariant)

For a finite extension of [local fields](arithmetic.md#local-field) $L/K$, restriction multiplies the [local Brauer invariant](#local-brauer-invariant) by $[L:K]$ and corestriction preserves it. For restriction, the residue-character value multiplies by the [residue degree](arithmetic.md#residue-degree) and the parameter valuation by the [ramification index](arithmetic.md#ramification-index). For corestriction, lift the residue character using divisibility of $\mathbb Q/\mathbb Z$ and use the [norm projection formula for cyclic Brauer pairings](#norm-projection-formula-for-cyclic-brauer-pairings).

#### Period of a Brauer class

↑ **Parent:** [Brauer group](#brauer-group)

The period is the order of a class in the [Brauer group](#brauer-group). It divides its index. Over a [local field](arithmetic.md#local-field) with finite [residue field](commutative-algebra.md#residue-field), the period and index are both the reduced denominator of its [local Brauer invariant](#local-brauer-invariant).

#### Index of a central simple algebra

↑ **Parent:** [Brauer group](#brauer-group)

If $A\cong M_r(D)$ with $D$ a [central division algebra](algebra.md#central-division-algebra), its index is $\deg D$. It depends only on the [Brauer group](#brauer-group) class. The index divides every finite splitting-field degree and equals the degree of a maximal subfield of the division representative.

#### Crossed-product algebra of a Galois extension

↑ **Parent:** [Brauer group](#brauer-group)

For a finite Galois extension $L/k$, Galois group $G$, and normalized two-cocycle $\phi:G\times G\to L^\times$, the crossed-product algebra is

$$
A(L,G,\phi)=\bigoplus_{\sigma\in G}Lu_\sigma,
$$

with $u_\sigma a=\sigma(a)u_\sigma$ and $u_\sigma u_\tau=\phi(\sigma,\tau)u_{\sigma\tau}$. It is a central simple $k$-algebra split by $L$.

##### Cyclic algebra

↑ **Parent:** [Crossed-product algebra of a Galois extension](#crossed-product-algebra-of-a-galois-extension)

For a cyclic extension $E/K$ of degree $m$ with generator $\sigma$ and $a\in K^{\times}$, the [cyclic algebra](#cyclic-algebra) is generated by $E$ and $u$ with $ub=\sigma(b)u$, $u^m=a$. It is a [central simple algebra](#central-simple-algebra) of degree $m$. Its Brauer class can also be written $(\chi,a)$, where $\chi(\sigma)=1/m$.

###### Splitting criterion for a cyclic algebra

↑ **Parent:** [Cyclic algebra](#cyclic-algebra)

If $a=N_{L/K}c$, let $L$ act on itself by multiplication and let the extra generator act by $c\sigma$. Its $n$th power is multiplication by $a$, and these operators give the [cyclic algebra](#cyclic-algebra) as $\operatorname{End}_K(L)$. Conversely, if the algebra is a [matrix algebra](#matrix-algebra) on an $n$-dimensional [vector space](vector-space.md), its embedded degree-$n$ field $L$ makes that space one-dimensional over $L$. The extra generator is then $c\sigma$ in an $L$-basis, so its $n$th power forces $a=Nc$.

###### Norm projection formula for cyclic Brauer pairings

↑ **Parent:** [Cyclic algebra](#cyclic-algebra)

For a finite extension $L/K$, an unramified or general cyclic character $\chi$ over $K$, and $a\in L^{\times}$, transfer satisfies $\operatorname{Cor}_{L/K}(\operatorname{Res}\chi,a)=(\chi,N_{L/K}a)$. It is the cup-product projection formula combined with the [field norm](algebraic-number-theory.md#field-norm) on multiplicative degree-zero coefficients. With the norm definition of Brauer transfer it also covers purely inseparable steps.

##### Cohomological construction of a Brauer class

↑ **Parent:** [Crossed-product algebra of a Galois extension](#crossed-product-algebra-of-a-galois-extension)

Cohomologous normalized two-cocycles define isomorphic crossed-product algebras: replacing $\phi$ by the coboundary associated with a one-cochain rescales the basis elements $u_\sigma$. Consequently the crossed-product construction induces a map

$$
H^2(G,L^\times)\longrightarrow\operatorname{Br}(k).
$$

## Center of an associative algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

The center of an associative algebra $A$ is

$$
Z(A)=\{z\in A:za=az\text{ for every }a\in A\}.
$$

### Central idempotent

↑ **Parent:** [Center of an associative algebra](#center-of-an-associative-algebra)

A central idempotent is an [idempotent](commutative-algebra.md#idempotent) in the [center of an associative algebra](#center-of-an-associative-algebra). It gives a decomposition $A=Ae\oplus A(1-e)$ into two-sided [ideals](commutative-algebra.md#ideal), with products between the summands zero. The identities of these summands are $e$ and $1-e$.

#### Primitive central idempotent

↑ **Parent:** [Central idempotent](#central-idempotent)

A nonzero [central idempotent](#central-idempotent) is primitive central if it is not a sum of two nonzero orthogonal [central idempotents](#central-idempotent). For an [Artinian ring](algebra.md#artinian-ring), it determines a [block of an Artinian algebra](#block-of-an-artinian-algebra). This differs from a [primitive idempotent](commutative-algebra.md#primitive-idempotent) in the whole [ring](commutative-algebra.md#ring): for a [matrix algebra](#matrix-algebra) of size greater than one over a [field](algebra.md#field), $1$ is primitive central but is a sum of diagonal [idempotents](commutative-algebra.md#idempotent).

## Group algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Group_algebra)

The group algebra $k[G]$ is the [vector space](vector-space.md) with basis $G$ and multiplication obtained by extending the group law $k$-bilinearly.

### Complex group algebra detects p-nilpotency

↑ **Parent:** [Group algebra](#group-algebra)

The matrix-block sizes in the [Artin–Wedderburn theorem](#artin-wedderburn-theorem) for $\mathbb C[G]$ recover the [irreducible character degrees](representation-theory.md#irreducible-character-degree) with their multiplicities. They determine the degree-square sum and the number $|G:G'|$ of linear characters. [Isaacs' character-degree criterion for p-nilpotency](group-theory.md#isaacs-character-degree-criterion-for-p-nilpotency) therefore detects each normal p-complement and applying it for every prime also detects [nilpotent groups](group-theory.md#nilpotent-group). The set of distinct degrees without multiplicities does not contain the same information.

### Center of the infinite dihedral group algebra

↑ **Parent:** [Group algebra](#group-algebra)

Write the [group algebra](#group-algebra) as $\mathbb C[X,X^{-1}]\oplus\mathbb C[X,X^{-1}]Y$, with $Y^2=1$ and $YX=X^{-1}Y$. Commuting $f(X)+g(X)Y$ with $X$ forces $g=0$, and commuting with $Y$ forces $f(X)=f(X^{-1})$. Every symmetric Laurent polynomial is a polynomial in $z=X+X^{-1}$, using the recursion $X^{m+1}+X^{-m-1}=z(X^m+X^{-m})-(X^{m-1}+X^{1-m})$. The algebra is free of rank four over this center, with [basis](vector-space.md#basis) $1,X,Y,XY$; the relation $X^2-zX+1=0$ proves spanning, and applying $X\mapsto X^{-1}$ proves independence of $1,X$.

### Character idempotent

↑ **Parent:** [Group algebra](#group-algebra)

If the order of a finite abelian group $\Delta$ is invertible in the coefficient ring and all its character values belong to that ring, its character idempotents are orthogonal and sum to one. They decompose any [module](module-theory.md#module-mathematics) into character components. In a cyclotomic tower with odd $p$, the [Teichmüller character](arithmetic.md#teichmuller-character) provides these components integrally over $\mathbb Z_p$.

### Conjugacy-class sum

↑ **Parent:** [Group algebra](#group-algebra)

For a [conjugacy class](group-theory.md#conjugacy-class) $C$ of a finite [group](group.md), $z_C=\sum_{g\in C}g$ is central in its [group algebra](#group-algebra). In a complex [irreducible representation](representation-theory.md#irreducible-representation) of degree $d$ and [character of a representation](representation-theory.md#character-of-a-representation) $\chi$, it acts by $|C|\chi(g)/d$; its trace gives this formula and [Schur lemma](representation-theory.md#schur-s-lemma) gives scalarity.

### Group norm element

↑ **Parent:** [Group algebra](#group-algebra)

The group norm element in the [group algebra](#group-algebra) $kG$ is $N_G=\sum_{g\in G}g$. It spans the invariant subspace of the left regular [group representation](representation-theory.md#group-representation), and $N_G^2=|G|N_G$. If the [characteristic](algebra.md#characteristic-of-a-field) divides $|G|$, a projection from $kG$ onto $kN_G$ would send $N_G$ to both itself and zero, proving that $kG$ is not a [semisimple algebra](#semisimple-algebra). Its action on indecomposable modules is described by [group norm element detects the trivial projective cover](representation-theory.md#group-norm-element-detects-the-trivial-projective-cover).

### Completed group algebra

↑ **Parent:** [Group algebra](#group-algebra)

For a profinite group $G$ and a finite or profinite coefficient ring $R$, the completed group algebra is

$$
R[[G]]=\varprojlim_{U\trianglelefteq_oG}R[G/U],
$$

where $U$ ranges over the open normal subgroups. It records convergent noncommutative power series in topological generators of $G$.

#### Weighted group algebra of a uniform pro-p group

↑ **Parent:** [Completed group algebra](#completed-group-algebra)

Choose ordered minimal [topological generators](topological-group.md#topological-generator) $a_1,\ldots,a_d$ of a [uniform pro-p group](topological-group.md#uniform-pro-p-group) for odd $p$, put $b_i=a_i-1$, and choose $1/(p-1)<s<1$. Ordered monomials $b^\alpha=b_1^{\alpha_1}\cdots b_d^{\alpha_d}$ give power-series coordinates in the integral [completed group algebra](#completed-group-algebra). The displayed [Non-Archimedean absolute value](arithmetic.md#non-archimedean-absolute-value) filtration gives a complete normed $\mathbb Q_p$-algebra after completion of the rational [group algebra](#group-algebra). The power relation raises valuation by one, and interchanging $b_i,b_j$ adds terms of valuation at least $1+s>2s$, so multiplication does not decrease total valuation. The [p-adic logarithm](arithmetic.md#p-adic-logarithm) and [p-adic exponential](arithmetic.md#p-adic-exponential-function) are inverse on the relevant small balls. In particular $\log G$ is a faithful realization of the [Lie algebra of a uniform pro-p group](lie-algebra.md#lie-algebra-of-a-uniform-pro-p-group), useful for verifying its intrinsic limit operations and the [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula) without assuming the correspondence in advance.

#### Iwasawa algebra

↑ **Parent:** [Completed group algebra](#completed-group-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iwasawa_algebra)

An Iwasawa algebra is a [completed group algebra](#completed-group-algebra) such as $\mathbb Z_p[[G]]$ or $\mathbb F_p[[G]]$ for a compact p-adic analytic group $G$.

##### Measure realization of an Iwasawa algebra

↑ **Parent:** [Iwasawa algebra](#iwasawa-algebra)

A [p-adic measure](measure-theory.md#p-adic-measure) gives the compatible finite-quotient elements $\sum_{gU}\mu(gU)[gU]\in I[G/U]$. The transition maps sum coefficients over fibers. Conversely compatible coefficients define values on cosets, then all clopen sets, and hence integration. Thus the inverse limit [Iwasawa algebra](#iwasawa-algebra) is the ring of measures, with multiplication given by [convolution of p-adic measures](measure-theory.md#convolution-of-p-adic-measures). Completeness of $I$ suffices even when its residue field is infinite.

##### Iwasawa algebra of a Zp-extension

↑ **Parent:** [Iwasawa algebra](#iwasawa-algebra)

Choose a topological generator $\gamma$ of the [Galois group](galois-theory.md#galois-group) of a [Zp-extension](algebraic-number-theory.md#zp-extension) and set $T=\gamma-1$. The [completed group algebra](#completed-group-algebra) becomes the [formal power series ring](commutative-algebra.md#formal-power-series) $\mathbb Z_p[[T]]$, a two-dimensional complete regular local [integral domain](commutative-algebra.md#integral-domain) with maximal ideal $(p,T)$. Its finite-layer quotient is $\Lambda/((1+T)^{p^n}-1)\cong\mathbb Z_p[\Gamma/\Gamma^{p^n}]$.

###### Pseudo-isomorphism

↑ **Parent:** [Iwasawa algebra of a Zp-extension](#iwasawa-algebra-of-a-zp-extension)

A homomorphism between finitely generated one-variable [Iwasawa modules](algebraic-number-theory.md#iwasawa-module) is a pseudo-isomorphism if its kernel and cokernel are finite. Finite errors do not change the [Iwasawa-module rank](#iwasawa-module-rank) or the [characteristic ideal](algebraic-number-theory.md#characteristic-ideal) of a torsion module. They can still change its integral structure, so a [pseudo-isomorphism](#pseudo-isomorphism) is weaker than an [isomorphism](algebra.md#isomorphism).

###### Iwasawa-module rank

↑ **Parent:** [Iwasawa algebra of a Zp-extension](#iwasawa-algebra-of-a-zp-extension)

For a finitely generated [module](module-theory.md#module-mathematics) over the [integral domain](commutative-algebra.md#integral-domain) $\Lambda$, its Iwasawa-module rank counts free summands up to [pseudo-isomorphism](#pseudo-isomorphism). Rank zero is equivalent to being a [torsion module](module-theory.md#torsion-module). A positive rank $r$ forces the $\mathbb Z_p$-ranks of finite-layer [coinvariant modules](module-theory.md#coinvariant-module) to grow like $r p^n+O(1)$.

##### Filtration on a group

↑ **Parent:** [Iwasawa algebra](#iwasawa-algebra)

A filtration on a group $G$ is a function $\omega:G\to\mathbb R\cup\{\infty\}$ satisfying

$$
\omega(xy^{-1})\geq\min\{\omega(x),\omega(y)\},
\qquad
\omega([x,y])\geq\omega(x)+\omega(y).
$$

It is separated when $\omega(x)=\infty$ only for $x=1$.

###### p-valuation

↑ **Parent:** [Filtration on a group](#filtration-on-a-group)

For a [prime number](number-theory.md#prime-number) $p$, a p-valuation is a separated [filtration on a group](#filtration-on-a-group) such that every $x\ne1$ satisfies

$$
\omega(x)>\frac1{p-1},
\qquad
\omega(x^p)=\omega(x)+1.
$$

A group equipped with one is called a p-valued group.

###### Ordered basis of a complete p-valued group

↑ **Parent:** [p-valuation](#p-valuation)

An ordered basis $(g_1,\ldots,g_d)$ of a complete finite-rank p-valued group gives each element a unique convergent expression $g_1^{\lambda_1}\cdots g_d^{\lambda_d}$ with $\lambda_i\in\mathbb Z_p$, and its valuation is the minimum of $\omega(g_i)+v_p(\lambda_i)$ over the nonzero coordinates.

###### p-saturated group

↑ **Parent:** [p-valuation](#p-valuation)

A p-valued group is p-saturated when it is complete and every $x$ with

$$
\omega(x)>\frac{p}{p-1}
$$

has a pth root in the group.

###### Associated graded Lie algebra of a filtered group

↑ **Parent:** [Filtration on a group](#filtration-on-a-group)

For $G_\lambda=\{g:\omega(g)\geq\lambda\}$ and $G_{\lambda+}=\{g:\omega(g)>\lambda\}$, the associated graded group

$$
\operatorname{gr}G=\bigoplus_\lambda G_\lambda/G_{\lambda+}
$$

is a graded [Lie algebra](lie-algebra.md) with bracket induced by the [group commutator](group.md#group-commutator). For a p-valuation, $t\operatorname{gr}_\lambda(g)=\operatorname{gr}_{\lambda+1}(g^p)$ makes it a graded $\mathbb F_p[t]$-Lie algebra.

##### Lazard filtration on a group algebra

↑ **Parent:** [Iwasawa algebra](#iwasawa-algebra)

For a p-valued group $(G,\omega)$, give $p^r(g_1-1)\cdots(g_s-1)$ weight $r+\sum_i\omega(g_i)$. The spans of elements of weight at least $\lambda$ form a multiplicative filtration on $\mathbb Z_p[G]$ and its completions.

###### Lazard enveloping-algebra map

↑ **Parent:** [Lazard filtration on a group algebra](#lazard-filtration-on-a-group-algebra)

The initial form of $g-1$ depends only on the initial form of $g$ in $\operatorname{gr}G$. The resulting Lie map extends to a surjective graded algebra homomorphism

$$
U_{\mathbb F_p[t]}(\operatorname{gr}G)\twoheadrightarrow\operatorname{gr}\mathbb Z_p[G].
$$

For a complete finite-rank p-valued group, ordered-basis expansions show that it is an isomorphism.

##### Center of an Iwasawa algebra of a complete p-valued group

↑ **Parent:** [Iwasawa algebra](#iwasawa-algebra)

If $G$ is a complete finite-rank p-valued group with center $Z(G)$, then

$$
Z\bigl(\mathbb F_p[[G]]\bigr)=\mathbb F_p[[Z(G)]].
$$

The key facts are that the finite-conjugacy center of a p-valued group equals its center and that compatibility through the finite group-algebra quotients eliminates coefficients on infinite conjugacy classes.

##### Lazard logarithm of a p-saturated group

↑ **Parent:** [Iwasawa algebra](#iwasawa-algebra)

Inside the completed rational Iwasawa algebra, the convergent series

$$
\log g=\sum_{n\geq1}\frac{(-1)^{n+1}}n(g-1)^n
$$

sends a finite-rank p-saturated group to a $\mathbb Z_p$-Lie algebra. The [Baker--Campbell--Hausdorff formula](linear-operator-theory.md#baker-campbell-hausdorff-formula) and its commutator expansion prove closure under addition and the [commutator](lie-algebra.md#commutator) bracket.

###### Primitive elements of a completed rational Iwasawa algebra

↑ **Parent:** [Lazard logarithm of a p-saturated group](#lazard-logarithm-of-a-p-saturated-group)

If $(g_1,\ldots,g_d)$ is an ordered basis of a finite-rank p-saturated group, then

$$
P(\widehat{\mathbb Q_pG})
=\bigoplus_{i=1}^d\mathbb Q_p\log(g_i),
$$

where a primitive element $x$ satisfies $\Delta(x)=x\otimes1+1\otimes x$ for the completed [Hopf algebra](algebra.md#hopf-algebra) coproduct.

## Left ideal

↑ **Parent:** [Associative algebra](associative-algebra.md)

A left ideal $L$ of an [associative algebra](associative-algebra.md) $A$ is a [vector subspace](vector-space.md#vector-subspace) satisfying $AL\subseteq L$. Equivalently, it is a submodule of the left regular $A$-module.

### Maximal left ideal

↑ **Parent:** [Left ideal](#left-ideal)

A [maximal left ideal](#maximal-left-ideal) is a proper [left ideal](#left-ideal) contained in no larger proper [left ideal](#left-ideal). In a unital [Banach algebra](banach-algebra.md) it is [norm](functional-analysis.md#norm) [closed](topology.md#closed-set): its closure is a [left ideal](#left-ideal), and if that closure were the entire algebra it would contain elements of $L$ within distance less than one of $1$, hence invertible by the [Neumann series](banach-algebra.md#neumann-series). A proper [left ideal](#left-ideal) contains no invertible element. The quotient $A/L$ is consequently a [quotient Banach space](banach-space.md#quotient-banach-space) and a [simple module](module-theory.md#irreducible-module).

#### Scalar right action on a maximal-left-ideal quotient

↑ **Parent:** [Maximal left ideal](#maximal-left-ideal)

In a complex unital [Banach algebra](banach-algebra.md), right multiplication by $a$ induces a bounded [module endomorphism](module-theory.md#module-endomorphism) $T$ of $A/L$ when $La\subseteq L$. Every nonzero module endomorphism of this [simple module](module-theory.md#irreducible-module) is algebraically bijective, since its [kernel](linear-algebra.md#kernel-of-a-linear-map) and range are [submodules](module-theory.md#submodule). Its inverse is bounded by the [bounded inverse theorem](functional-analysis.md#bounded-inverse-theorem). Choosing $\lambda$ in the nonempty [spectrum of an element](banach-algebra.md#spectrum-of-an-element) of $T$ forces $T-\lambda I=0$. Applying this identity to $1+L$ gives $a-\lambda1\in L$, with uniqueness because $1\notin L$.

## Semisimple algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semisimple_algebra)

A finite-dimensional [associative algebra](associative-algebra.md) is semisimple when its left regular module is a direct sum of simple modules. Equivalently, every [left ideal](#left-ideal) is a direct summand. In particular, a semisimple algebra has no nonzero square-zero left ideal: if $L^2=0$ and a module projection $A\to L$ exists, its value $e$ at $1$ satisfies $e\in L$ and $e^2=e$, forcing $e=0$.

## Hochschild chain complex

↑ **Parent:** [Associative algebra](associative-algebra.md)

For a $k$-algebra $R$ and an $R$-$R$-[bimodule](module-theory.md#bimodule) $M$, the Hochschild chains are

$$
C_n(R,M)=M\otimes_kR^{\otimes_kn}.
$$

Their boundary is

$$
\begin{aligned}
b(m\otimes r_1\otimes\cdots\otimes r_n)
={}&mr_1\otimes r_2\otimes\cdots\otimes r_n\\
&+\sum_{i=1}^{n-1}(-1)^im\otimes r_1\otimes\cdots\otimes r_ir_{i+1}\otimes\cdots\otimes r_n\\
&+(-1)^nr_nm\otimes r_1\otimes\cdots\otimes r_{n-1}.
\end{aligned}
$$

Associativity and the bimodule axioms give $b^2=0$.

### Hochschild homology

↑ **Parent:** [Hochschild chain complex](#hochschild-chain-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hochschild_homology)

The Hochschild homology of a $k$-algebra with coefficients in a bimodule is the homology

$$
HH_n(R,M)=H_n(C_\bullet(R,M),b).
$$

## Hochschild cochain complex

↑ **Parent:** [Associative algebra](associative-algebra.md)

The Hochschild cochains are $C^n(R,M)=\operatorname{Hom}_k(R^{\otimes_kn},M)$, with coboundary

$$
\begin{aligned}
(\delta f)(r_1,\ldots,r_{n+1})
={}&r_1f(r_2,\ldots,r_{n+1})\\
&+\sum_{i=1}^n(-1)^if(r_1,\ldots,r_ir_{i+1},\ldots,r_{n+1})\\
&+(-1)^{n+1}f(r_1,\ldots,r_n)r_{n+1}.
\end{aligned}
$$

### Hochschild cup product

↑ **Parent:** [Hochschild cochain complex](#hochschild-cochain-complex)

For $f\in C^p(A,A)$ and $g\in C^q(A,A)$, set $(f\smile g)(a_1,\ldots,a_{p+q})=f(a_1,\ldots,a_p)g(a_{p+1},\ldots,a_{p+q})$. This associative cochain multiplication descends to [Hochschild cohomology](#hochschild-cohomology), where it gives a [graded commutative algebra](commutative-algebra.md#graded-commutative-algebra). It is one operation in the [Gerstenhaber algebra](commutative-algebra.md#gerstenhaber-algebra) structure.

### Normalized Hochschild cochain complex

↑ **Parent:** [Hochschild cochain complex](#hochschild-cochain-complex)

For a unital [associative algebra](associative-algebra.md), normalized positive-degree cochains vanish whenever an argument is $1$. They form a subcomplex of the [Hochschild cochain complex](#hochschild-cochain-complex) computing the same [Hochschild cohomology](#hochschild-cohomology). The unit-insertion contracting homotopy on degenerate bar terms proves the normalization equivalence. A normalized degree-two [Hochschild cocycle](#hochschild-cocycle) defines a unital [square-zero extension of an algebra](commutative-algebra.md#square-zero-extension-of-an-algebra).

### Hochschild cocycle

↑ **Parent:** [Hochschild cochain complex](#hochschild-cochain-complex)

A Hochschild cocycle is a cochain $f$ with $\delta f=0$ in the [Hochschild cochain complex](#hochschild-cochain-complex). For degree two, this is $a\mu(b,c)-\mu(ab,c)+\mu(a,bc)-\mu(a,b)c=0$. It is the condition for [associativity](group.md#associative-property) of a [square-zero extension of an algebra](commutative-algebra.md#square-zero-extension-of-an-algebra).

### Hochschild cohomology

↑ **Parent:** [Hochschild cochain complex](#hochschild-cochain-complex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hochschild_cohomology)

The Hochschild cohomology groups are

$$
HH^n(R,M)=H^n(C^\bullet(R,M),\delta).
$$

#### Ground-ring qualification in Hochschild cohomology

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

The ordinary [Hochschild cochain complex](#hochschild-cochain-complex) is defined using a chosen commutative ground [ring](commutative-algebra.md#ring) $k$. The bar complex is exact via insertion of $1$, but its terms are projective over the enveloping algebra when $R$ is projective over $k$, in particular when $k$ is a [field](algebra.md#field). Without that hypothesis the ordinary cochain groups compute relative [Hochschild cohomology](#hochschild-cohomology) and cannot automatically be identified with absolute Ext. Likewise, ordinary second cohomology classifies ground-ring-linearly split square-zero extensions, not arbitrary nonsplit [ring](commutative-algebra.md#ring) extensions.

// Destination: module-theory.bigb

#### Hochschild cohomology of a polynomial algebra in one variable

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

Over a [field](algebra.md#field), the [bimodule](module-theory.md#bimodule) resolution $0\to k[x]\otimes k[x]\xrightarrow{x\otimes1-1\otimes x}k[x]\otimes k[x]\to k[x]\to0$ is exact: multiplication identifies the quotient by $x\otimes1-1\otimes x$, and that element is a non-zero-divisor in the two-variable [polynomial ring](commutative-algebra.md#polynomial-ring). Applying the [bimodule](module-theory.md#bimodule) Hom functor gives zero differential, proving the displayed [Hochschild cohomology](#hochschild-cohomology). Degree-one classes are the [derivations](#derivation-of-an-algebra) $f(x)\partial_x$.

#### Second Hochschild cohomology classifies split square-zero extensions

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

Fix an $R$-[bimodule](module-theory.md#bimodule) $M$. A unital ground-ring-linear split extension with square-zero kernel $M$ can be identified with $R\oplus M$, with multiplication $(a,u)(b,v)=(ab,av+ub+f(a,b))$. [Associativity](group.md#associative-property) is exactly $\delta f=0$. Changing a unital linear section by $g:R\to M$ changes $f$ by $\delta g$. Thus equivalence classes of these split extensions are $HH^2(R,M)$. Over a [field](algebra.md#field) every such vector-space extension splits; over a general ground [ring](commutative-algebra.md#ring) a splitting hypothesis is essential for this ordinary cochain classification.

#### Hochschild-Kostant-Rosenberg theorem

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

For the [polynomial ring](commutative-algebra.md#polynomial-ring) $A=k[X_1,\ldots,X_r]$ in [characteristic](algebra.md#characteristic-of-a-field) zero, antisymmetrization identifies $HH^*(A,A)$ with $\bigwedge_A^*\operatorname{Der}_k(A)$. The map on a wedge of $p$ [derivations](#derivation-of-an-algebra) is $\frac1{p!}\sum_{\sigma\in S_p}\operatorname{sgn}(\sigma)\prod_jD_{\sigma(j)}(a_j)$. The [Hochschild cup product](#hochschild-cup-product) becomes the [exterior product](linear-algebra.md#exterior-product), and the left [Gerstenhaber bracket](#gerstenhaber-bracket) becomes the left [Schouten-Nijenhuis bracket](linear-algebra.md#schouten-nijenhuis-bracket). This assertion requires a smoothness hypothesis when generalized beyond [polynomial rings](commutative-algebra.md#polynomial-ring).

#### Gerstenhaber bracket

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

Write $f\circ g=\sum_{i=0}^{p-1}(-1)^{i(q-1)}f\circ_i g$ for insertion of a degree-$q$ cochain into a degree-$p$ one. With the unsigned [Hochschild cup product](#hochschild-cup-product) and the left [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule), take $[f,g]=(-1)^{(p-1)(q-1)}f\circ g-g\circ f$. It descends to [Hochschild cohomology](#hochschild-cohomology) and gives a [Gerstenhaber algebra](commutative-algebra.md#gerstenhaber-algebra). The alternative insertion bracket $f\circ g-(-1)^{(p-1)(q-1)}g\circ f$ differs by the displayed degree sign and obeys the corresponding right rule. Degree-one brackets are [commutators](lie-algebra.md#commutator) of [derivations](#derivation-of-an-algebra) in either convention.

#### Hochschild cohomological dimension

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

The Hochschild cohomological dimension of an [associative algebra](associative-algebra.md) over a [field](algebra.md#field) is $\operatorname{Dim}(A)=\operatorname{pd}_{A\otimes A^{\mathrm{op}}}A$. Equivalently, $HH^n(A,M)$ vanishes above that dimension for every [bimodule](module-theory.md#bimodule) $M$. A bound by one implies $HH^2(A,A)=0$ and hence [formal rigidity from vanishing second Hochschild cohomology](#formal-rigidity-from-vanishing-second-hochschild-cohomology).

#### Derivation into a bimodule

↑ **Parent:** [Hochschild cohomology](#hochschild-cohomology)

A $k$-linear derivation from a $k$-algebra $R$ to an $R$-$R$-[bimodule](module-theory.md#bimodule) $M$ is a map $d:R\to M$ satisfying

$$
d(rs)=r d(s)+d(r)s.
$$

##### Derivation of an algebra

↑ **Parent:** [Derivation into a bimodule](#derivation-into-a-bimodule)

For an [associative algebra](associative-algebra.md) $A$ over a [field](algebra.md#field) $k$, a derivation is a $k$-[linear map](vector-space.md#linear-map) $D:A\to A$ satisfying $D(ab)=D(a)b+aD(b)$. It is the case $M=A$ of a [derivation into a bimodule](#derivation-into-a-bimodule); the order of factors matters when $A$ is noncommutative. Substituting $a=b=1$ gives $D(1)=0$. Such maps form a [Lie algebra](lie-algebra.md) under the [commutator](lie-algebra.md#commutator) $[D,E]=D\circ E-E\circ D$.

More generally, for a [commutative ring](commutative-algebra.md#commutative-ring) $R$, a derivation from a commutative $R$-[algebra](algebra.md) $B$ into a $B$-[module](module-theory.md#module-mathematics) $M$ is an $R$-[linear map](vector-space.md#linear-map) $D:B\to M$ with $D(r)=0$ for $r\in R$ and $D(bb')=bD(b')+b'D(b)$. The second term has this order because the [algebra](algebra.md) is commutative. [Derivations of smooth functions are vector fields](#derivations-of-smooth-functions-are-vector-fields) provide a geometric example.

###### Derivations of smooth functions are vector fields

↑ **Parent:** [Derivation of an algebra](#derivation-of-an-algebra)

Every real-linear [derivation of an algebra](#derivation-of-an-algebra) $D:C^\infty(M)\to C^\infty(M)$ on a [smooth manifold](differential-geometry.md#smooth-manifold) has the form $Dh=Z(h)$ for a unique smooth [vector field](calculus.md#vector-field) $Z$. The product rule makes $D$ local: multiplying a function that vanishes near a point by a [smooth cutoff function](analysis.md#smooth-cutoff-function) supported there gives zero derivative at that point. Locally write $h(x)=h(p)+\sum_i(x^i-x^i(p))h_i(x)$, where $h_i(p)=\partial_i h(p)$. Applying $D$ at $p$ gives $Dh(p)=\sum_i D(x^i)(p)\partial_i h(p)$; the smooth coefficients $D(x^i)$ define the claimed [vector field](calculus.md#vector-field). No continuity hypothesis is needed. In dimension zero all such derivations vanish.

##### Inner derivation

↑ **Parent:** [Derivation into a bimodule](#derivation-into-a-bimodule)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_derivation)

For $m\in M$, the formula $d_m(r)=rm-mr$ defines an inner derivation $R\to M$.

###### First Hochschild cohomology as outer derivations

↑ **Parent:** [Inner derivation](#inner-derivation)

The degree-one Hochschild cocycles are exactly the maps that are a [derivation into a bimodule](#derivation-into-a-bimodule), while degree-one coboundaries are exactly the [inner derivations](#inner-derivation). Therefore

$$
HH^1(R,M)\cong\operatorname{Der}_k(R,M)/\operatorname{Inn}(R,M).
$$

##### Universal bimodule derivation

↑ **Parent:** [Derivation into a bimodule](#derivation-into-a-bimodule)

Let $\mu:R\otimes_kR\to R$ be multiplication and $\Omega_R^{\mathrm{nc}}=\ker\mu$, with the outer $R$-bimodule structure. Then

$$
D(r)=r\otimes1-1\otimes r
$$

is a derivation and composition with $D$ gives a natural isomorphism

$$
\operatorname{Hom}_{R-R}(\Omega_R^{\mathrm{nc}},M)
\cong\operatorname{Der}_k(R,M).
$$

The inverse sends $d$ to

$$
\theta_d\left(\sum_ir_i\otimes s_i\right)=\sum_id(r_i)s_i.
$$

The condition $\sum_ir_is_i=0$ makes this map left as well as right $R$-linear. Every element of $\Omega_R^{\mathrm{nc}}$ is a sum of terms $D(r)s$, which proves uniqueness.

###### Inner derivation through the universal bimodule derivation

↑ **Parent:** [Universal bimodule derivation](#universal-bimodule-derivation)

Under the universal isomorphism, the inner derivation $d_m(r)=rm-mr$ corresponds to

$$
\theta_m\left(\sum_ir_i\otimes s_i\right)=\sum_ir_ims_i.
$$

Thus inner derivations correspond exactly to bimodule maps on $\Omega_R^{\mathrm{nc}}$ that extend across the inclusion $\Omega_R^{\mathrm{nc}}\subseteq R\otimes_kR$.

## Specialization of an algebra

↑ **Parent:** [Associative algebra](associative-algebra.md)

If an algebra is defined over a parameter ring $R$, a ring homomorphism $R\to k$ produces a specialized $k$-algebra by extension of scalars. Defining relations specialize by replacing every parameter by its image in $k$.

## ↑ Ancestors (5)

1. [Algebra over a field](algebra.md#algebra-over-a-field)
2. [Algebra](algebra.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (30)

- [Algebra involution](#algebra-involution)
- [Bar resolution of an associative algebra](algebra.md#bar-resolution-of-an-associative-algebra)
- [Block of a finite-dimensional algebra](#block-of-a-finite-dimensional-algebra)
- [Block of an Artinian algebra](#block-of-an-artinian-algebra)
- [Centralizer of a subalgebra](#centralizer-of-a-subalgebra)
- [Complex matrix representation of quaternions](algebra.md#complex-matrix-representation-of-quaternions)
- [Derivation of an algebra](#derivation-of-an-algebra)
- [Ext-connected components determine blocks](#ext-connected-components-determine-blocks)
- [Ext quiver](#ext-quiver)
- [Faddeev-Zamolodchikov algebra](quantum-field-theory.md#faddeev-zamolodchikov-algebra)
- [Frobenius algebra](#frobenius-algebra)
- [Hochschild cohomological dimension](#hochschild-cohomological-dimension)
- [Left ideal](#left-ideal)
- [Left inverse of an algebra element](banach-algebra.md#left-inverse-of-an-algebra-element)
- [Matrix algebra](#matrix-algebra)
- [Maximal commutative subalgebra](#maximal-commutative-subalgebra)
- [Normalized Hochschild cochain complex](#normalized-hochschild-cochain-complex)
- [Opposite algebra](#opposite-algebra)
- [Opposite ring](commutative-algebra.md#opposite-ring)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-3.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128.md#3/solution)
- [Primitive ideal](#primitive-ideal)
- [Representation variety of an associative algebra](#representation-variety-of-an-associative-algebra)
- [Right ideal](#right-ideal)
- [Semisimple algebra](#semisimple-algebra)
- [Square-zero extension of an algebra](commutative-algebra.md#square-zero-extension-of-an-algebra)
- [Star-algebra](#star-algebra)
- [Unital algebra](#unital-algebra)
