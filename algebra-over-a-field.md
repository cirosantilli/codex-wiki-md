# Algebra over a field

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebra_over_a_field)

An algebra over a [field](algebra.md#field) $k$ is a [vector space](vector-space.md) $A$ over $k$ equipped with a bilinear multiplication $A\times A\to A$.

**Table of contents**

- [Poisson algebra](#poisson-algebra)
  - [Poisson bracket from a central deformation parameter](#poisson-bracket-from-a-central-deformation-parameter)
- [Algebra isomorphism](#algebra-isomorphism)
- [Division algebra](#division-algebra)
  - [Finite-dimensional real division-algebra classification](#finite-dimensional-real-division-algebra-classification)
  - [Central division algebra](#central-division-algebra)
  - [Finite-dimensional division algebra over an algebraically closed field](#finite-dimensional-division-algebra-over-an-algebraically-closed-field)
  - [Quaternion](#quaternion)
    - [Complex matrix representation of quaternions](#complex-matrix-representation-of-quaternions)
    - [Unit quaternion](#unit-quaternion)
- [Subalgebra](#subalgebra)
- [Algebra homomorphism over a field](#algebra-homomorphism-over-a-field)
  - [Points of a noncommutative algebra](#points-of-a-noncommutative-algebra)
    - [Spectral decomposition of a quantum-plane point](#spectral-decomposition-of-a-quantum-plane-point)
- [Structure constant](#structure-constant)
- [Finitely generated algebra](#finitely-generated-algebra)
  - [Infinite cotangent space obstructs finite algebra generation](#infinite-cotangent-space-obstructs-finite-algebra-generation)
  - [Finite presentation of an algebra](#finite-presentation-of-an-algebra)
  - [Finite generation from finitely many principal localizations](#finite-generation-from-finitely-many-principal-localizations)
  - [Artin--Tate lemma](#artin-tate-lemma)
  - [Finite generation descends along a field extension](#finite-generation-descends-along-a-field-extension)
- [Clifford algebra](#clifford-algebra)
  - [Complex Clifford spinor dimension](#complex-clifford-spinor-dimension)
  - [Spinor](#spinor)
  - [Clifford algebra bundle](#clifford-algebra-bundle)
  - [Clifford multiplication](#clifford-multiplication)
  - [Dimension bound from paired Clifford involutions](#dimension-bound-from-paired-clifford-involutions)
  - [Real independence of Clifford-generated vectors](#real-independence-of-clifford-generated-vectors)
  - [Gamma matrices](#gamma-matrices)
    - [Gamma-matrix vector sandwich](#gamma-matrix-vector-sandwich)
    - [Feynman slash notation](#feynman-slash-notation)
    - [Chiral gamma-matrix representation](#chiral-gamma-matrix-representation)
    - [Hermitizing matrix](#hermitizing-matrix)
    - [Gamma matrix adjoint and transpose identities](#gamma-matrix-adjoint-and-transpose-identities)
    - [Gamma matrix trace identities](#gamma-matrix-trace-identities)
    - [Chirality matrix](#chirality-matrix)
    - [Dirac representation of the gamma matrices](#dirac-representation-of-the-gamma-matrices)
      - [Dirac-to-Weyl gamma-matrix similarity transform](#dirac-to-weyl-gamma-matrix-similarity-transform)
- [Hopf algebra](#hopf-algebra)
  - [Primitive element of a Hopf algebra](#primitive-element-of-a-hopf-algebra)
  - [Module algebra](#module-algebra)
  - [Quantum enveloping algebra of sl2](#quantum-enveloping-algebra-of-sl2)
    - [Highest-weight string for quantum sl2](#highest-weight-string-for-quantum-sl2)
    - [Quantum integer](#quantum-integer)
  - [RTT construction](#rtt-construction)
    - [FRT bialgebra](#frt-bialgebra)
    - [Quantum determinant](#quantum-determinant)
    - [Coordinate Hopf algebra of quantum SL2](#coordinate-hopf-algebra-of-quantum-sl2)
  - [Cocommutative Hopf algebra](#cocommutative-hopf-algebra)
  - [Commutative Hopf algebra](#commutative-hopf-algebra)
    - [Function Hopf algebra of a finite group](#function-hopf-algebra-of-a-finite-group)
  - [Invariant vector of a module over a Hopf algebra](#invariant-vector-of-a-module-over-a-hopf-algebra)
  - [Internal hom for modules over a Hopf algebra](#internal-hom-for-modules-over-a-hopf-algebra)
  - [Antipode](#antipode)
- [Associative algebra](associative-algebra.md)
  - [Primitive ideal](associative-algebra.md#primitive-ideal)
  - [Ore extension](associative-algebra.md#ore-extension)
  - [Algebra involution](associative-algebra.md#algebra-involution)
  - [Unital algebra](associative-algebra.md#unital-algebra)
  - [Star-algebra](associative-algebra.md#star-algebra)
    - [Hermitian element of a star algebra](associative-algebra.md#hermitian-element-of-a-star-algebra)
    - [Star-subalgebra](associative-algebra.md#star-subalgebra)
  - [Cocenter of a finite-dimensional algebra](associative-algebra.md#cocenter-of-a-finite-dimensional-algebra)
    - [Frobenius map on an algebra cocenter](associative-algebra.md#frobenius-map-on-an-algebra-cocenter)
  - [Representation variety of an associative algebra](associative-algebra.md#representation-variety-of-an-associative-algebra)
  - [Units of a finite-dimensional algebra](associative-algebra.md#units-of-a-finite-dimensional-algebra)
  - [Free associative algebra](associative-algebra.md#free-associative-algebra)
  - [Frobenius algebra](associative-algebra.md#frobenius-algebra)
  - [Opposite algebra](associative-algebra.md#opposite-algebra)
  - [Right ideal](associative-algebra.md#right-ideal)
    - [Maximal right ideal](associative-algebra.md#maximal-right-ideal)
  - [Formal associative deformation](associative-algebra.md#formal-associative-deformation)
    - [Weyl deformation of a polynomial algebra in two variables](associative-algebra.md#weyl-deformation-of-a-polynomial-algebra-in-two-variables)
    - [First-order associative deformation](associative-algebra.md#first-order-associative-deformation)
      - [Second-order obstruction to an associative deformation](associative-algebra.md#second-order-obstruction-to-an-associative-deformation)
    - [Trivial formal deformation](associative-algebra.md#trivial-formal-deformation)
      - [Formal rigidity from vanishing second Hochschild cohomology](associative-algebra.md#formal-rigidity-from-vanishing-second-hochschild-cohomology)
  - [Gelfand–Kirillov dimension](associative-algebra.md#gelfand-kirillov-dimension)
    - [Gelfand–Kirillov dimension of a module](associative-algebra.md#gelfand-kirillov-dimension-of-a-module)
      - [Bernstein growth dimension of a Weyl algebra module](associative-algebra.md#bernstein-growth-dimension-of-a-weyl-algebra-module)
        - [Characteristic variety of a Weyl algebra module](associative-algebra.md#characteristic-variety-of-a-weyl-algebra-module)
          - [Independence of characteristic support from a good module filtration](associative-algebra.md#independence-of-characteristic-support-from-a-good-module-filtration)
        - [Holonomic Weyl algebra module](associative-algebra.md#holonomic-weyl-algebra-module)
          - [Multiplicity bounds the length of a holonomic Weyl module](associative-algebra.md#multiplicity-bounds-the-length-of-a-holonomic-weyl-module)
        - [Bernstein inequality for Weyl algebra modules](associative-algebra.md#bernstein-inequality-for-weyl-algebra-modules)
          - [Faithful finite-step action of a Weyl algebra](associative-algebra.md#faithful-finite-step-action-of-a-weyl-algebra)
            - [Scalar extraction by iterated Weyl commutators](associative-algebra.md#scalar-extraction-by-iterated-weyl-commutators)
  - [Block of an Artinian algebra](associative-algebra.md#block-of-an-artinian-algebra)
  - [Maximal commutative subalgebra](associative-algebra.md#maximal-commutative-subalgebra)
  - [Centralizer of a subalgebra](associative-algebra.md#centralizer-of-a-subalgebra)
    - [Commutant of an operator algebra](associative-algebra.md#commutant-of-an-operator-algebra)
      - [Von Neumann double commutant theorem](associative-algebra.md#von-neumann-double-commutant-theorem)
        - [Kaplansky density theorem](associative-algebra.md#kaplansky-density-theorem)
      - [Double commutant theorem for star-algebras](associative-algebra.md#double-commutant-theorem-for-star-algebras)
      - [Double-centralizer theorem for semisimple operator algebras](associative-algebra.md#double-centralizer-theorem-for-semisimple-operator-algebras)
  - [Matrix algebra](associative-algebra.md#matrix-algebra)
  - [Block of a finite-dimensional algebra](associative-algebra.md#block-of-a-finite-dimensional-algebra)
    - [Ext-connected components determine blocks](associative-algebra.md#ext-connected-components-determine-blocks)
  - [Basic algebra](associative-algebra.md#basic-algebra)
    - [Ext quiver](associative-algebra.md#ext-quiver)
  - [Central simple algebra](associative-algebra.md#central-simple-algebra)
    - [Quaternion algebra](associative-algebra.md#quaternion-algebra)
      - [Quaternion norm obstruction at primes congruent to three modulo four](associative-algebra.md#quaternion-norm-obstruction-at-primes-congruent-to-three-modulo-four)
    - [Reduced norm](associative-algebra.md#reduced-norm)
    - [Inner automorphisms of a matrix algebra](associative-algebra.md#inner-automorphisms-of-a-matrix-algebra)
    - [Splitting field of a central simple algebra](associative-algebra.md#splitting-field-of-a-central-simple-algebra)
    - [Degree of a central simple algebra](associative-algebra.md#degree-of-a-central-simple-algebra)
    - [Artin–Wedderburn theorem](associative-algebra.md#artin-wedderburn-theorem)
      - [Burnside matrix-algebra theorem](associative-algebra.md#burnside-matrix-algebra-theorem)
    - [Tensor product of central simple algebras](associative-algebra.md#tensor-product-of-central-simple-algebras)
    - [Brauer group](associative-algebra.md#brauer-group)
      - [Brauer class](associative-algebra.md#brauer-class)
      - [Albert-Brauer-Hasse-Noether theorem](associative-algebra.md#albert-brauer-hasse-noether-theorem)
      - [Independent quaternion classes over rational numbers](associative-algebra.md#independent-quaternion-classes-over-rational-numbers)
      - [Brauer p-divisibility in characteristic p](associative-algebra.md#brauer-p-divisibility-in-characteristic-p)
      - [Witt residue sequence](associative-algebra.md#witt-residue-sequence)
        - [Local Brauer invariant](associative-algebra.md#local-brauer-invariant)
          - [Local fundamental class](associative-algebra.md#local-fundamental-class)
          - [Restriction and corestriction of local Brauer invariants](associative-algebra.md#restriction-and-corestriction-of-local-brauer-invariants)
      - [Period of a Brauer class](associative-algebra.md#period-of-a-brauer-class)
      - [Index of a central simple algebra](associative-algebra.md#index-of-a-central-simple-algebra)
      - [Crossed-product algebra of a Galois extension](associative-algebra.md#crossed-product-algebra-of-a-galois-extension)
        - [Cyclic algebra](associative-algebra.md#cyclic-algebra)
          - [Splitting criterion for a cyclic algebra](associative-algebra.md#splitting-criterion-for-a-cyclic-algebra)
          - [Norm projection formula for cyclic Brauer pairings](associative-algebra.md#norm-projection-formula-for-cyclic-brauer-pairings)
        - [Cohomological construction of a Brauer class](associative-algebra.md#cohomological-construction-of-a-brauer-class)
  - [Center of an associative algebra](associative-algebra.md#center-of-an-associative-algebra)
    - [Central idempotent](associative-algebra.md#central-idempotent)
      - [Primitive central idempotent](associative-algebra.md#primitive-central-idempotent)
  - [Group algebra](associative-algebra.md#group-algebra)
    - [Complex group algebra detects p-nilpotency](associative-algebra.md#complex-group-algebra-detects-p-nilpotency)
    - [Center of the infinite dihedral group algebra](associative-algebra.md#center-of-the-infinite-dihedral-group-algebra)
    - [Character idempotent](associative-algebra.md#character-idempotent)
    - [Conjugacy-class sum](associative-algebra.md#conjugacy-class-sum)
    - [Group norm element](associative-algebra.md#group-norm-element)
    - [Completed group algebra](associative-algebra.md#completed-group-algebra)
      - [Weighted group algebra of a uniform pro-p group](associative-algebra.md#weighted-group-algebra-of-a-uniform-pro-p-group)
      - [Iwasawa algebra](associative-algebra.md#iwasawa-algebra)
        - [Measure realization of an Iwasawa algebra](associative-algebra.md#measure-realization-of-an-iwasawa-algebra)
        - [Iwasawa algebra of a Zp-extension](associative-algebra.md#iwasawa-algebra-of-a-zp-extension)
          - [Pseudo-isomorphism](associative-algebra.md#pseudo-isomorphism)
          - [Iwasawa-module rank](associative-algebra.md#iwasawa-module-rank)
        - [Filtration on a group](associative-algebra.md#filtration-on-a-group)
          - [p-valuation](associative-algebra.md#p-valuation)
            - [Ordered basis of a complete p-valued group](associative-algebra.md#ordered-basis-of-a-complete-p-valued-group)
            - [p-saturated group](associative-algebra.md#p-saturated-group)
          - [Associated graded Lie algebra of a filtered group](associative-algebra.md#associated-graded-lie-algebra-of-a-filtered-group)
        - [Lazard filtration on a group algebra](associative-algebra.md#lazard-filtration-on-a-group-algebra)
          - [Lazard enveloping-algebra map](associative-algebra.md#lazard-enveloping-algebra-map)
        - [Center of an Iwasawa algebra of a complete p-valued group](associative-algebra.md#center-of-an-iwasawa-algebra-of-a-complete-p-valued-group)
        - [Lazard logarithm of a p-saturated group](associative-algebra.md#lazard-logarithm-of-a-p-saturated-group)
          - [Primitive elements of a completed rational Iwasawa algebra](associative-algebra.md#primitive-elements-of-a-completed-rational-iwasawa-algebra)
  - [Left ideal](associative-algebra.md#left-ideal)
    - [Maximal left ideal](associative-algebra.md#maximal-left-ideal)
      - [Scalar right action on a maximal-left-ideal quotient](associative-algebra.md#scalar-right-action-on-a-maximal-left-ideal-quotient)
  - [Semisimple algebra](associative-algebra.md#semisimple-algebra)
  - [Hochschild chain complex](associative-algebra.md#hochschild-chain-complex)
    - [Hochschild homology](associative-algebra.md#hochschild-homology)
  - [Hochschild cochain complex](associative-algebra.md#hochschild-cochain-complex)
    - [Hochschild cup product](associative-algebra.md#hochschild-cup-product)
    - [Normalized Hochschild cochain complex](associative-algebra.md#normalized-hochschild-cochain-complex)
    - [Hochschild cocycle](associative-algebra.md#hochschild-cocycle)
    - [Hochschild cohomology](associative-algebra.md#hochschild-cohomology)
      - [Ground-ring qualification in Hochschild cohomology](associative-algebra.md#ground-ring-qualification-in-hochschild-cohomology)
      - [Hochschild cohomology of a polynomial algebra in one variable](associative-algebra.md#hochschild-cohomology-of-a-polynomial-algebra-in-one-variable)
      - [Second Hochschild cohomology classifies split square-zero extensions](associative-algebra.md#second-hochschild-cohomology-classifies-split-square-zero-extensions)
      - [Hochschild-Kostant-Rosenberg theorem](associative-algebra.md#hochschild-kostant-rosenberg-theorem)
      - [Gerstenhaber bracket](associative-algebra.md#gerstenhaber-bracket)
      - [Hochschild cohomological dimension](associative-algebra.md#hochschild-cohomological-dimension)
      - [Derivation into a bimodule](associative-algebra.md#derivation-into-a-bimodule)
        - [Derivation of an algebra](associative-algebra.md#derivation-of-an-algebra)
          - [Derivations of smooth functions are vector fields](associative-algebra.md#derivations-of-smooth-functions-are-vector-fields)
        - [Inner derivation](associative-algebra.md#inner-derivation)
          - [First Hochschild cohomology as outer derivations](associative-algebra.md#first-hochschild-cohomology-as-outer-derivations)
        - [Universal bimodule derivation](associative-algebra.md#universal-bimodule-derivation)
          - [Inner derivation through the universal bimodule derivation](associative-algebra.md#inner-derivation-through-the-universal-bimodule-derivation)
  - [Specialization of an algebra](associative-algebra.md#specialization-of-an-algebra)

## Poisson algebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_algebra)

A [Poisson algebra](#poisson-algebra) is a commutative associative algebra with a [Lie bracket](lie-algebra.md#lie-bracket) that is a derivation in each argument. Smooth functions on a [symplectic manifold](symplectic-geometry.md#symplectic-manifold) are its standard example. The linear span of moment-map components may form a finite-dimensional Lie subalgebra, while closing those components under multiplication normally produces a much larger [Poisson algebra](#poisson-algebra).

### Poisson bracket from a central deformation parameter

↑ **Parent:** [Poisson algebra](#poisson-algebra)

Let $h$ be central and a non-zero-divisor in an associative algebra, with commutative quotient modulo $h$. Dividing commutators by $h$ and reducing modulo $h$ is independent of the lifts, since changing a lift by $hc$ changes the quotient by a commutator, zero modulo $h$. Antisymmetry, the Leibniz rule and the Jacobi identity descend from the corresponding commutator identities. For the [order filtration of a Weyl algebra](noncommutative-algebra.md#order-filtration-of-a-weyl-algebra), the convention is $\{\xi_i,x_j\}=\delta_{ij}$, with the opposite sign for $\{x_i,\xi_j\}$.

## Algebra isomorphism

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)

An algebra isomorphism is a bijective [linear map](vector-space.md#linear-map) preserving multiplication and identity between two [algebras](algebra.md) over the same [field](algebra.md#field). In classification of a [square-zero extension of an algebra](commutative-algebra.md#square-zero-extension-of-an-algebra), an equivalence must additionally induce the identity on the prescribed quotient and kernel.

## Division algebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)

A division algebra over a [field](algebra.md#field) $k$ is a [division ring](commutative-algebra.md#division-ring) equipped with a unital [algebra](algebra.md) structure over $k$, with $k$ mapping into its [center of an associative algebra](associative-algebra.md#center-of-an-associative-algebra). Every nonzero element is invertible; it need not be finite-dimensional over $k$.

### Finite-dimensional real division-algebra classification

↑ **Parent:** [Division algebra](#division-algebra)

A finite-dimensional associative [division algebra](#division-algebra) over $\mathbb R$ is one of the three displayed algebras. A nonreal element has an irreducible quadratic [minimal polynomial](linear-operator-theory.md#minimal-polynomial) and yields $i^2=-1$. Its centralizer is a [division algebra](#division-algebra) over central $\mathbb C$, hence is $\mathbb C$ by splitting [minimal polynomials](linear-operator-theory.md#minimal-polynomial). Decompose the whole algebra into the plus and minus eigenspaces of conjugation by $i$. If the minus space is zero, the algebra is $\mathbb C$; otherwise it is $\mathbb Cj$, since multiplying by $j^{-1}$ takes that space into the centralizer. One has $jz=\overline z j$ and $j^2\in\mathbb R$. Division forces $j^2<0$, which can be rescaled to $-1$, yielding $\mathbb H$. Of these, only $\mathbb R,\mathbb H$ have center $\mathbb R$.

### Central division algebra

↑ **Parent:** [Division algebra](#division-algebra)

A [central division algebra](#central-division-algebra) over $K$ is a finite-dimensional [division algebra](#division-algebra) whose center is exactly $K$. It is a [central simple algebra](associative-algebra.md#central-simple-algebra). Every [Brauer group](associative-algebra.md#brauer-group) class has a unique [central division algebra](#central-division-algebra) representative up to isomorphism.

### Finite-dimensional division algebra over an algebraically closed field

↑ **Parent:** [Division algebra](#division-algebra)

Let $D$ be a finite-dimensional [division algebra](#division-algebra) over an [algebraically closed field](algebra.md#algebraically-closed-field) $k$. Left multiplication by $a\in D$ has an [eigenvalue](linear-operator-theory.md#eigenvalue) $\lambda\in k$ and a nonzero eigenvector $v$. Thus $(a-\lambda)v=0$; multiplying by $v^{-1}$ gives $a=\lambda$. Every element is scalar, so $D=k$.

### Quaternion

↑ **Parent:** [Division algebra](#division-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quaternion)

A quaternion is $a+bi+cj+dk$ with real coefficients, where $i^2=j^2=k^2=ijk=-1$. They form a noncommutative real [division algebra](#division-algebra). The norm squared is $a^2+b^2+c^2+d^2$, and every nonzero quaternion has inverse its conjugate divided by that squared norm. The unit quaternions form the [Lie group](lie-theory.md#lie-group) $S^3$.

#### Complex matrix representation of quaternions

↑ **Parent:** [Quaternion](#quaternion)

The displayed complex [matrices](vector-space.md#matrix), with real coefficients, form a four-dimensional real [associative algebra](associative-algebra.md). Their three imaginary [basis](vector-space.md#basis) [matrices](vector-space.md#matrix) square to minus the identity and satisfy $JK=L$, $KL=J$, $LJ=K$, with the reversed products negative. For $\alpha=aI+bJ+cK+dL$, quaternionic conjugation gives $\alpha\overline\alpha=(a^2+b^2+c^2+d^2)I$. Every nonzero [matrix](vector-space.md#matrix) therefore has inverse $\overline\alpha/(a^2+b^2+c^2+d^2)$ inside this algebra. This realizes the real [division algebra](#division-algebra) of [quaternions](#quaternion) within $M_2(\mathbb C)$; it is not a complex [vector](vector-space.md#vector) subspace.

#### Unit quaternion

↑ **Parent:** [Quaternion](#quaternion)

A [quaternion](#quaternion) of norm $1$ is a unit quaternion. They form the [topological group](topological-group.md) $\operatorname{Sp}(1)$ and identify with the sphere $S^3\subset\mathbb R^4$. Multiplication and inversion preserve the norm. The [Hurewicz theorem](homotopy.md#hurewicz-theorem) identifies $\pi_3(S^3)$ with $H_3(S^3;\mathbb Z)$; hence [homotopy-group addition in a topological group](topological-group.md#homotopy-group-addition-in-a-topological-group) shows that $q\mapsto q^m$ has [mapping degree](homology.md#degree-of-a-continuous-mapping) $m$, rather than $m^2$.

## Subalgebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)

A [linear subspace](vector-space.md#vector-subspace) of an [algebra over a field](algebra-over-a-field.md) closed under multiplication is a subalgebra. If a unital subalgebra is intended, it must also contain the ambient identity. A closed subalgebra of a normed algebra is closed in the [norm topology](normed-vector-space.md#norm-topology).

## Algebra homomorphism over a field

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)

For a [field](algebra.md#field) $k$, a homomorphism of $k$-algebras is a unital [ring homomorphism](commutative-algebra.md#ring-homomorphism) preserving scalar multiplication by every element of $k$. For unital algebras it is equivalently a [ring](commutative-algebra.md#ring) homomorphism commuting with their structural maps from $k$. Pullback by a [morphism of algebraic varieties](algebraic-variety.md#morphism-of-algebraic-varieties) gives such a homomorphism between their [coordinate rings](algebraic-variety.md#coordinate-ring).

### Points of a noncommutative algebra

↑ **Parent:** [Algebra homomorphism over a field](#algebra-homomorphism-over-a-field)

An $R$-point of a unital [algebra over a field](algebra-over-a-field.md) $A$ is a unital [algebra homomorphism over a field](#algebra-homomorphism-over-a-field) $A\to R$. For the [quantum plane](noncommutative-algebra.md#quantum-plane) over the [complex numbers](complex-analysis.md#complex-number), scalar points lie on the two coordinate axes when $q\ne1$, while matrix-valued points are pairs $X,Y$ with $YX=qXY$.

#### Spectral decomposition of a quantum-plane point

↑ **Parent:** [Points of a noncommutative algebra](#points-of-a-noncommutative-algebra)

For finite matrices satisfying $YX=qXY$, with $q$ not a [root of unity](algebra.md#root-of-unity), $Y$ sends the [generalized eigenspace](linear-operator-theory.md#generalized-eigenspace) of $X$ at $\lambda$ into the one at $q^{-1}\lambda$. Finiteness of the [spectrum](linear-operator-theory.md#spectrum-functional-analysis) makes $Y$ nilpotent on the sum of the nonzero $X$ [generalized eigenspaces](linear-operator-theory.md#generalized-eigenspace). Exchanging $X,Y$ gives the corresponding statement for $X$. Splitting the zero [generalized eigenspace](linear-operator-theory.md#generalized-eigenspace) of $X$ by that of $Y$ gives the displayed invariant direct sum; both operators are nilpotent on $U$.

## Structure constant

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Structure_constant)

For a basis $(e_i)$ of a finite-dimensional algebra, its structure constants are the scalars defined by

$$
e_ie_j=\sum_kc_{ij}^{\,k}e_k.
$$

They express multiplication as polynomial coordinate functions.

## Finitely generated algebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finitely_generated_algebra)

A $k$-algebra is finitely generated when finitely many elements generate it under addition, multiplication, and scalar multiplication. Equivalently, it is a quotient of a polynomial ring $k[x_1,\ldots,x_n]$.

### Infinite cotangent space obstructs finite algebra generation

↑ **Parent:** [Finitely generated algebra](#finitely-generated-algebra)

Let $A$ be a commutative algebra over a [field](algebra.md#field) $k$, with a homomorphism $A\to k$ restricting to the identity on $k$, and let $I$ be its kernel. If $A$ is generated by finitely many elements, subtracting their images in $k$ gives finitely many generators in $I$. Every polynomial in those generators, modulo $I^2$, is a linear combination of their classes. Thus $I/I^2$, the [algebraic cotangent space](algebraic-geometry.md#algebraic-cotangent-space) at this point, is finite-dimensional. For $A=k+xk[x,y]$ and $I=xk[x,y]$, the classes $xy^j$, $j\ge0$, form an infinite basis modulo $I^2=x^2k[x,y]$. This is a subalgebra of a [polynomial ring](commutative-algebra.md#polynomial-ring) which is not a [finitely generated algebra](#finitely-generated-algebra).

### Finite presentation of an algebra

↑ **Parent:** [Finitely generated algebra](#finitely-generated-algebra)

A presentation of an [algebra over a field](algebra-over-a-field.md) with finitely many generators and relations. The [Hilbert basis theorem](algebra.md#hilbert-basis-theorem) ensures that every [finitely generated algebra](#finitely-generated-algebra) over a field admits such a presentation. Its [module of Kähler differentials](locally-ringed-space.md#kahler-differential) is presented by the [Jacobian matrix](multivariable-calculus.md#jacobian-matrix) of the relations.

### Finite generation from finitely many principal localizations

↑ **Parent:** [Finitely generated algebra](#finitely-generated-algebra)

Suppose a $k$-algebra $A$ has elements $f_i,g_i$ with $\sum_i g_if_i=1$, and each $A_{f_i}$ is a [finitely generated algebra](#finitely-generated-algebra). Let $B\subseteq A$ contain the $f_i,g_i$ and numerators of finite generating sets of all $A_{f_i}$. Then $B$ is finitely generated and $B_{f_i}=A_{f_i}$. For $a\in A$, clear denominators so that all $f_i^Na$ belong to $B$. A [unit-ideal identity for powers](commutative-algebra.md#unit-ideal-identity-for-powers) gives $1=\sum_i c_if_i^N$ in $B$, hence $a=\sum_i c_i f_i^Na\in B$. Thus $A=B$.

<h3 id="artin-tate-lemma">Artin--Tate lemma</h3>

↑ **Parent:** [Finitely generated algebra](#finitely-generated-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Artin--Tate_lemma)

Let $A\subseteq B\subseteq C$ be rings. If $A$ is Noetherian, $C$ is a finitely generated $A$-algebra, and $C$ is a finite $B$-module, then $B$ is a finitely generated $A$-algebra.

### Finite generation descends along a field extension

↑ **Parent:** [Finitely generated algebra](#finitely-generated-algebra)

Let $L/k$ be a [field extension](algebra.md#field-extension). If $A\otimes_kL$ is a [finitely generated algebra](#finitely-generated-algebra) over $L$, then $A$ is finitely generated over $k$. Choose finitely many generators of $A\otimes_kL$ and collect the finitely many coefficients from $A$ occurring in them. The $k$-subalgebra $A_0$ generated by those coefficients satisfies $(A/A_0)\otimes_kL=0$, and [faithful flatness](module-theory.md#faithfully-flat-module) of $L/k$ gives $A=A_0$.

## Clifford algebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clifford_algebra)

For a vector space with quadratic form $Q$, its Clifford algebra is generated by vectors subject to $v^2=Q(v)1$. In a basis this is equivalently $\gamma^\mu\gamma^\nu+\gamma^\nu\gamma^\mu=2\eta^{\mu\nu}1$.

### Complex Clifford spinor dimension

↑ **Parent:** [Clifford algebra](#clifford-algebra)

After complexifying a nondegenerate metric in $D=2k$ dimensions, pair [gamma matrices](#gamma-matrices) into $k$ fermionic creation and annihilation operators. Their binary occupation states span $2^k$ dimensions, and the [gamma matrices](#gamma-matrices) generate all endomorphisms of this space. The Dirac module is therefore irreducible as a Clifford module. The even algebra preserves the chirality grading, splitting its Lorentz-spinor representation into two irreducible Weyl modules of dimension $2^{k-1}$. In $D=2k+1$, adjoining the old [chirality matrix](#chirality-matrix) as the extra gamma gives an irreducible $2^k$-dimensional [Spin group](semisimple-lie-algebra.md#spin-group) representation with no Weyl splitting. The two possible signs of that extra gamma distinguish Clifford modules but give equivalent [Spin group](semisimple-lie-algebra.md#spin-group) modules.

### Spinor

↑ **Parent:** [Clifford algebra](#clifford-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spinor)

### Clifford algebra bundle

↑ **Parent:** [Clifford algebra](#clifford-algebra)

A [vector bundle](vector-bundle.md) $E$ with a fibrewise [quadratic form](quadratic-form.md) $Q$ defines a bundle whose fibre over $x$ is the [Clifford algebra](#clifford-algebra) $\operatorname{Cl}(E_x,Q_x)$. When the polar form is a [nondegenerate bilinear form](bilinear-form.md#nondegenerate-bilinear-form), local orthonormal frames identify its fibres with a fixed [Clifford algebra](#clifford-algebra), and orthogonal transition maps induce the algebra transition maps. A [Clifford module bundle](vector-bundle.md#clifford-module-bundle) is a bundle of modules over these algebras, rather than the algebra bundle itself. For a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), use its [cotangent bundle](symplectic-geometry.md#cotangent-bundle) and the metric [quadratic form](quadratic-form.md), with the sign convention specified.

### Clifford multiplication

↑ **Parent:** [Clifford algebra](#clifford-algebra)

Clifford multiplication is the action of a [Clifford algebra](#clifford-algebra) on a [module](module-theory.md#module-mathematics). The displayed relation uses the negative [Riemannian metric](riemannian-metric.md) convention; in a compatible [Hermitian inner product](linear-algebra.md#hermitian-inner-product), $c(v)^*=-c(v)$ for real $v$. Another convention writes $C(v)=ic(v)$, giving self-adjoint generators with positive anticommutator. Switching between these conventions switches a geometric [Dirac operator](riemannian-geometry.md#dirac-operator) between self-adjoint and skew-adjoint realizations.

### Dimension bound from paired Clifford involutions

↑ **Parent:** [Clifford algebra](#clifford-algebra)

For $2n$ hermitian Euclidean Clifford generators, the commuting hermitian involutions $J_j=i\gamma^{2j-1}\gamma^{2j}$ admit a common eigenvector. Each odd-indexed generator flips one joint eigenvalue. The $2^n$ resulting vectors are nonzero and mutually orthogonal. Thus any nonzero invariant complex representation has dimension at least $2^n$.

### Real independence of Clifford-generated vectors

↑ **Parent:** [Clifford algebra](#clifford-algebra)

For hermitian generators satisfying $\{\gamma^I,\gamma^J\}_+=2\delta^{IJ}$ and any nonzero vector $v$, the vectors $\gamma^Iv$ are linearly independent over the real numbers. Indeed, $A=\sum_Ia_I\gamma^I$ with real $a_I$ obeys $A^2=(\sum_Ia_I^2)\mathbf1$, so $\|Av\|^2=(\sum_Ia_I^2)\|v\|^2$. Complex coefficients need a different argument.

### Gamma matrices

↑ **Parent:** [Clifford algebra](#clifford-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gamma_matrices)

Gamma matrices give a matrix representation of the [Clifford algebra](#clifford-algebra) of spacetime.

#### Gamma-matrix vector sandwich

↑ **Parent:** [Gamma matrices](#gamma-matrices)

For [gamma matrices](#gamma-matrices) with $\{\gamma^a,\gamma^b\}=2\eta^{ab}$ and $\gamma^{ab}=[\gamma^a,\gamma^b]/2$, contracted [Clifford algebra](#clifford-algebra) gives $\gamma_a\gamma^m\gamma^a=(2-D)\gamma^m$. Expanding the two antisymmetrized factors gives $\gamma_a\gamma_b\gamma^m\gamma^a\gamma^b-D\gamma^m$. The five-gamma product equals $[2D-(D-2)^2]\gamma^m$, by moving the middle contracted gamma through and using the three-gamma contraction twice. Subtraction yields the displayed identity. A convention without the factor one-half in each bivector multiplies the result by four.

#### Feynman slash notation

↑ **Parent:** [Gamma matrices](#gamma-matrices)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Feynman_slash_notation)

Feynman slash notation contracts a [four-vector](special-relativity.md#four-vector) with the [gamma matrices](#gamma-matrices). With mostly-minus signature, the [Clifford algebra](#clifford-algebra) gives $\not p^2=p^2I$, so $(\not p-m)^{-1}=(\not p+m)/(p^2-m^2)$ away from the [mass shell](special-relativity.md#mass-shell).

#### Chiral gamma-matrix representation

↑ **Parent:** [Gamma matrices](#gamma-matrices)

For signature $+---$, use $\gamma^0=\left(\begin{smallmatrix}0&I_2\\I_2&0\end{smallmatrix}\right)$ and $\gamma^i=\left(\begin{smallmatrix}0&\sigma^i\\-\sigma^i&0\end{smallmatrix}\right)$, where $\sigma^i$ are [Pauli matrices](algebra.md#pauli-matrices). Their [Clifford algebra](#clifford-algebra) follows directly from the Pauli [anticommutator](vector-space.md#anticommutator). The [chirality matrix](#chirality-matrix) is $\gamma^5=\operatorname{diag}(-I_2,I_2)$, separating the two chiral components of a [Dirac spinor](relativistic-quantum-field.md#dirac-spinor).

#### Hermitizing matrix

↑ **Parent:** [Gamma matrices](#gamma-matrices)

A [Hermitizing matrix](#hermitizing-matrix) for a set of [gamma matrices](#gamma-matrices) is an invertible [Hermitian matrix](hilbert-space.md#hermitian-operator) $H$ satisfying $\gamma^{a\dagger}=H\gamma^aH^{-1}$. Equivalently, each $H\gamma^a$ is Hermitian. It defines a covariant adjoint $\bar\psi=\psi^\dagger H$. If $\gamma'^a=M\gamma^aM^{-1}$, then $H'=M^{-\dagger}HM^{-1}$ has the same property. In a standard Lorentzian [Dirac basis](#dirac-representation-of-the-gamma-matrices), $H=\gamma^0$ is a conventional choice.

#### Gamma matrix adjoint and transpose identities

↑ **Parent:** [Gamma matrices](#gamma-matrices)

In the standard [Dirac representation of the gamma matrices](#dirac-representation-of-the-gamma-matrices), $(\gamma^0)^\dagger=\gamma^0$ and $(\gamma^i)^\dagger=-\gamma^i$, so $\gamma^{a\dagger}=\gamma^0\gamma^a\gamma^0$. The transpose signs in that representation are positive for $a=0,2$ and negative for $a=1,3$. The [charge-conjugation matrix](quantum-field-theory.md#charge-conjugation-matrix) expresses the basis-independent intertwining relation $C^{-1}\gamma^aC=-(\gamma^a)^T$. Under an arbitrary nonunitary [similarity transformation](linear-algebra.md#similarity-transformation), the [Hermitizing matrix](#hermitizing-matrix) changes by inverse Hermitian congruence; it need not equal the transformed temporal [gamma matrix](#gamma-matrices).

#### Gamma matrix trace identities

↑ **Parent:** [Gamma matrices](#gamma-matrices)

With metric $(+---)$, $\gamma^5=i\gamma^0\gamma^1\gamma^2\gamma^3$ and $\epsilon^{0123}=+1$, odd ordinary [gamma matrix](#gamma-matrices) traces vanish, $\operatorname{Tr}(\gamma^\mu\gamma^\nu)=4g^{\mu\nu}$, and

$$
\operatorname{Tr}(\gamma^\mu\gamma^\nu\gamma^\rho\gamma^\sigma)=4(g^{\mu\nu}g^{\rho\sigma}-g^{\mu\rho}g^{\nu\sigma}+g^{\mu\sigma}g^{\nu\rho}),\qquad \operatorname{Tr}(\gamma^5\gamma^\mu\gamma^\nu\gamma^\rho\gamma^\sigma)=-4i\epsilon^{\mu\nu\rho\sigma}.
$$

The first follows by repeated [Clifford algebra](#clifford-algebra) anticommutation and cyclicity of the [trace](linear-algebra.md#matrix-trace). The second is an antisymmetric tensor, whose normalization is fixed by the $0123$ component.

#### Chirality matrix

↑ **Parent:** [Gamma matrices](#gamma-matrices)

With metric $(+---)$, the chirality matrix has $(\gamma^5)^2=1$ and anticommutes with each [gamma matrix](#gamma-matrices). Its eigenspaces define [chirality](relativistic-quantum-field.md#chirality-physics); $P_L=(1-\gamma^5)/2$ and $P_R=(1+\gamma^5)/2$ are the corresponding projectors. These identities follow directly by moving a [gamma matrix](#gamma-matrices) through the ordered product and using the [Clifford algebra](#clifford-algebra).

#### Dirac representation of the gamma matrices

↑ **Parent:** [Gamma matrices](#gamma-matrices)

With signature $(+,-,-,-)$, one standard representation is $\widetilde\gamma^0=\operatorname{diag}(I_2,-I_2)$ and $\widetilde\gamma^i=\left(\begin{smallmatrix}0&\sigma^i\\-\sigma^i&0\end{smallmatrix}\right)$. Block multiplication and the [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) give time-time [anticommutator](vector-space.md#anticommutator) $2I_4$, mixed [anticommutators](vector-space.md#anticommutator) zero, and spatial [anticommutators](vector-space.md#anticommutator) $-2\delta^{ij}I_4$. Thus these [gamma matrices](#gamma-matrices) represent the spacetime [Clifford algebra](#clifford-algebra).

##### Dirac-to-Weyl gamma-matrix similarity transform

↑ **Parent:** [Dirac representation of the gamma matrices](#dirac-representation-of-the-gamma-matrices)

For the [Dirac representation of the gamma matrices](#dirac-representation-of-the-gamma-matrices), the [unitary matrix](linear-operator-theory.md#unitary-matrix)

$$
U=\frac1{\sqrt2}\begin{pmatrix}I_2&-I_2\\I_2&I_2\end{pmatrix}
$$

sends $\widetilde\gamma^0$ to $\left(\begin{smallmatrix}0&I_2\\I_2&0\end{smallmatrix}\right)$ while commuting with every spatial [gamma matrix](#gamma-matrices). This is the standard [Weyl representation of the gamma matrices](relativistic-quantum-field.md#weyl-representation-of-the-gamma-matrices) with spatial blocks $(0,\sigma^i;-\sigma^i,0)$. The [similarity transformation](linear-algebra.md#similarity-transformation) preserves the [Clifford algebra](#clifford-algebra) relations. Changing block-order or chirality conventions can change the displayed transformation, so its direction must be specified.

## Hopf algebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopf_algebra)

A Hopf algebra is a compatible algebra and coalgebra equipped with a counit and antipode. Coordinate rings of [affine algebraic groups](lie-theory.md#linear-algebraic-group) are commutative Hopf algebras.

### Primitive element of a Hopf algebra

↑ **Parent:** [Hopf algebra](#hopf-algebra)

An element $x$ of positive degree is primitive when $\Delta x=x\otimes1+1\otimes x$. Graded [commutators](lie-algebra.md#commutator) of primitives are primitive, so they form a [graded Lie algebra](lie-algebra.md#graded-lie-algebra). In a [universal enveloping algebra](lie-algebra.md#universal-enveloping-algebra) over $\mathbb Q$, the [primitive elements of a Hopf algebra](#primitive-element-of-a-hopf-algebra) are exactly its given [Lie algebra](lie-algebra.md): the associated graded algebra of the word-length filtration is symmetric, where no nonzero homogeneous polynomial of length greater than one is additive under the diagonal.

### Module algebra

↑ **Parent:** [Hopf algebra](#hopf-algebra)

An [algebra over a field](algebra-over-a-field.md) acted on by a [bialgebra](commutative-algebra.md#bialgebra) is a module algebra when multiplication and unit are [module](module-theory.md#module-mathematics) maps: the displayed product identity holds and $h1=\varepsilon(h)1$. This expresses the product rule determined by [comultiplication](category-theory.md#comultiplication).

### Quantum enveloping algebra of sl2

↑ **Parent:** [Hopf algebra](#hopf-algebra)

Over a [field](algebra.md#field) with $q\ne0$ and $q^2\ne1$, this [Hopf algebra](#hopf-algebra) has generators $E,F,K,K^{-1}$ and relations $KE=q^2EK$, $KF=q^{-2}FK$ and $EF-FE=(K-K^{-1})/(q-q^{-1})$. One [comultiplication](category-theory.md#comultiplication) convention is $\Delta E=E\otimes K+1\otimes E$, $\Delta F=F\otimes1+K^{-1}\otimes F$ and $\Delta K=K\otimes K$. Its [counit](category-theory.md#counit) takes $E,F$ to zero and $K$ to one. The [antipode](#antipode) takes $E$ to $-EK^{-1}$, $F$ to $-KF$ and $K$ to $K^{-1}$.

#### Highest-weight string for quantum sl2

↑ **Parent:** [Quantum enveloping algebra of sl2](#quantum-enveloping-algebra-of-sl2)

If $Ev=0$ and $Kv=\lambda v$, induction using the defining commutator gives the displayed identity. When $q$ is not a [root of unity](algebra.md#root-of-unity), a finite string of length $n+1$ in a [simple module](module-theory.md#irreducible-module) has $\lambda=\epsilon q^n$, $\epsilon=\pm1$. Its distinct $K$ [eigenvalues](linear-operator-theory.md#eigenvalue) make the string vectors independent, and the nonzero raising coefficients prove simplicity.

#### Quantum integer

↑ **Parent:** [Quantum enveloping algebra of sl2](#quantum-enveloping-algebra-of-sl2)

The symmetric quantum integer is the displayed [Laurent polynomial](polynomial.md#laurent-polynomial), with $[0]_q=0$. It obeys $[n+1]_q=q^{-1}[n]_q+q^n$ and $[r]_q[s+1]_q-[s]_q[r+1]_q=[r-s]_q$. At a primitive odd $\ell$th [root of unity](algebra.md#root-of-unity), $[n]_q=0$ exactly when $\ell$ divides $n$.

### RTT construction

↑ **Parent:** [Hopf algebra](#hopf-algebra)

Given a [Yang-Baxter R-matrix](quantum-field-theory.md#yang-baxter-r-matrix), take generators $t_{ij}$ subject to the displayed matrix relation, with $T_1=T\otimes I$, $T_2=I\otimes T$. The coproduct $\Delta t_{ij}=\sum_k t_{ik}\otimes t_{kj}$ and counit $\varepsilon(t_{ij})=\delta_{ij}$ give a [bialgebra](commutative-algebra.md#bialgebra). An antipode requires additional inverses or an appropriate determinant quotient; an arbitrary RTT bialgebra is not automatically a Hopf algebra.

#### FRT bialgebra

↑ **Parent:** [RTT construction](#rtt-construction)

Given an invertible [braiding](category-theory.md#braiding) $C$ on $V\otimes V$, the universal [bialgebra](commutative-algebra.md#bialgebra) coacting on $V$ for which $C$ is a [comodule](multilinear-algebra.md#comodule) map is generated by the matrix coefficients $t_{ij}$. Its [comultiplication](category-theory.md#comultiplication) is $\Delta t_{ij}=\sum_k t_{ik}\otimes t_{kj}$. Colinearity gives quadratic relations. Writing $R=\tau C$ turns the relation into the familiar [RTT construction](#rtt-construction) with the appropriate ordered tensor factors. A [Yang-Baxter R-matrix](quantum-field-theory.md#yang-baxter-r-matrix) supplies a scalar [coquasitriangular structure](category-theory.md#coquasitriangular-structure).

#### Quantum determinant

↑ **Parent:** [RTT construction](#rtt-construction)

For the two-by-two [RTT construction](#rtt-construction) with the standard [Yang-Baxter R-matrix](quantum-field-theory.md#yang-baxter-r-matrix), the displayed determinant commutes with the matrix generators and satisfies $\Delta D_q=D_q\otimes D_q$ and $\varepsilon(D_q)=1$. Imposing $D_q=1$ gives the [coordinate Hopf algebra of quantum SL2](#coordinate-hopf-algebra-of-quantum-sl2); adjoining its inverse instead gives the quantum general-linear coordinate algebra.

#### Coordinate Hopf algebra of quantum SL2

↑ **Parent:** [RTT construction](#rtt-construction)

The generators $a,b,c,d$ obey $ab=qba$, $ac=qca$, $bd=qdb$, $cd=qdc$, $bc=cb$, $ad-da=(q-q^{-1})bc$ and $ad-qbc=1$. Matrix multiplication gives the coproduct, and the antipode matrix is $\left(\begin{smallmatrix}d&-q^{-1}b\\-qc&a\end{smallmatrix}\right)$. For $q\ne0,\pm1$, its quotient with $c=0$, $a=u$, $d=u^{-1}$ and $b=v$ is the quantum Laurent-plane algebra $uv=qvu$, proving noncommutativity. The same quotient distinguishes $\Delta b$ from its flipped coproduct.

### Cocommutative Hopf algebra

↑ **Parent:** [Hopf algebra](#hopf-algebra)

A [Hopf algebra](#hopf-algebra) is cocommutative when flipping the two tensor factors leaves its coproduct unchanged. A [group algebra](associative-algebra.md#group-algebra) has coproduct $g\mapsto g\otimes g$, so it is cocommutative even for a nonabelian group, whose group algebra is not commutative.

### Commutative Hopf algebra

↑ **Parent:** [Hopf algebra](#hopf-algebra)

A [Hopf algebra](#hopf-algebra) is commutative when its multiplication is commutative. This is independent of whether its coproduct is cocommutative; function algebras of finite nonabelian groups give commutative but noncocommutative examples.

#### Function Hopf algebra of a finite group

↑ **Parent:** [Commutative Hopf algebra](#commutative-hopf-algebra)

Functions on a finite group form a [Hopf algebra](#hopf-algebra) under pointwise multiplication, with $(\Delta f)(g,h)=f(gh)$, $\varepsilon(f)=f(1)$ and $(Sf)(g)=f(g^{-1})$. The coproduct is cocommutative exactly when the group is abelian, since delta functions distinguish distinct products $gh,hg$.

### Invariant vector of a module over a Hopf algebra

↑ **Parent:** [Hopf algebra](#hopf-algebra)

For a left [module](module-theory.md#module-mathematics) over a [Hopf algebra](#hopf-algebra), a vector $v$ is invariant when $hv=\varepsilon(h)v$. In the [internal hom for modules over a Hopf algebra](#internal-hom-for-modules-over-a-hopf-algebra), invariant maps are exactly the [R-module homomorphisms](module-theory.md#module-homomorphism) for the acting algebra.

### Internal hom for modules over a Hopf algebra

↑ **Parent:** [Hopf algebra](#hopf-algebra)

The full $\operatorname{Hom}_k(M,N)$ carries the action $(hf)(u)=\sum h_{(1)}f(S(h_{(2)})u)$, making it the internal hom right adjoint to $-\otimes M$. No finite-dimensionality or inverse [antipode](#antipode) is needed.

### Antipode

↑ **Parent:** [Hopf algebra](#hopf-algebra)

The convolution inverse $S$ of the identity on a [bialgebra](commutative-algebra.md#bialgebra): $m(S\otimes1)\Delta=j\varepsilon=m(1\otimes S)\Delta$. Existence makes the [bialgebra](commutative-algebra.md#bialgebra) a [Hopf algebra](#hopf-algebra); $S$ reverses multiplication.

## Associative algebra

↑ **Parent:** [Algebra over a field](algebra-over-a-field.md)

[This section is present in another page, follow this link to view it.](associative-algebra.md)

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (13)

- [Associative algebra](associative-algebra.md)
- [Derivation (differential algebra)](algebra.md#derivation-differential-algebra)
- [Exponential isomorphism between the additive and multiplicative formal groups](normalization-of-an-algebraic-curve.md#exponential-isomorphism-between-the-additive-and-multiplicative-formal-groups)
- [Finite presentation of an algebra](#finite-presentation-of-an-algebra)
- [Module algebra](#module-algebra)
- [Normed algebra](algebra.md#normed-algebra)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-2.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-2.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-2.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#21h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-136.md#5/b/solution)
- [Points of a noncommutative algebra](#points-of-a-noncommutative-algebra)
- [Subalgebra](#subalgebra)
