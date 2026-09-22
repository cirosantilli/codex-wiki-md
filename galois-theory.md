# Galois theory

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Galois_theory)

**Table of contents**

- [Inverse Galois problem](#inverse-galois-problem)
  - [Rigid ramification type](#rigid-ramification-type)
- [Compact Galois module](#compact-galois-module)
- [Solvable field extension](#solvable-field-extension)
- [Radical extension](#radical-extension)
- [Absolute Galois group](#absolute-galois-group)
- [Galois closure of a field extension](#galois-closure-of-a-field-extension)
- [Fundamental theorem of Galois theory](#fundamental-theorem-of-galois-theory)
- [Kummer theory](#kummer-theory)
  - [Finite ramification support for radical extensions](#finite-ramification-support-for-radical-extensions)
  - [Cyclic Galois resolvent](#cyclic-galois-resolvent)
  - [Kummer reflection in Iwasawa theory](#kummer-reflection-in-iwasawa-theory)
  - [Kummer cohomology divisibility criterion](#kummer-cohomology-divisibility-criterion)
  - [Unramified Kummer classes with bounded prime support](#unramified-kummer-classes-with-bounded-prime-support)
  - [Square-class group of a field](#square-class-group-of-a-field)
    - [Square-class group of the 2-adic Gaussian field](#square-class-group-of-the-2-adic-gaussian-field)
    - [Square class](#square-class)
      - [Square-class group of a p-adic field](#square-class-group-of-a-p-adic-field)
  - [Kummer extension](#kummer-extension)
- [Galois cohomology](#galois-cohomology)
  - [Weil–Châtelet group](#weil-chatelet-group)
  - [Galois descent of vector spaces](#galois-descent-of-vector-spaces)
    - [Descent classification of central simple algebras](#descent-classification-of-central-simple-algebras)
    - [Semilinear action](#semilinear-action)
  - [First Galois cohomology unramified outside a finite set](#first-galois-cohomology-unramified-outside-a-finite-set)
  - [Galois module](#galois-module)
    - [Galois module of roots of unity](#galois-module-of-roots-of-unity)
  - [Hilbert's theorem 90](#hilbert-s-theorem-90)
    - [Unit form of Hilbert theorem 90](#unit-form-of-hilbert-theorem-90)
- [Frobenius endomorphism](#frobenius-endomorphism)
- [Formal derivative](#formal-derivative)
  - [Formal derivative in positive characteristic](#formal-derivative-in-positive-characteristic)
    - [Polynomial with zero formal derivative in characteristic p](#polynomial-with-zero-formal-derivative-in-characteristic-p)
- [Separable polynomial](#separable-polynomial)
  - [Separability of roots of unity](#separability-of-roots-of-unity)
  - [Irreducible polynomial in characteristic zero is separable](#irreducible-polynomial-in-characteristic-zero-is-separable)
- [Automorphism-count divisibility theorem](#automorphism-count-divisibility-theorem)
- [Coprime-degree descent for powers](#coprime-degree-descent-for-powers)
- [Algebraic element](#algebraic-element)
  - [Minimal polynomial of an algebraic element](#minimal-polynomial-of-an-algebraic-element)
- [Primitive element of a field extension](#primitive-element-of-a-field-extension)
  - [Primitive elements form a principal Zariski-open set](#primitive-elements-form-a-principal-zariski-open-set)
- [Primitive element theorem](#primitive-element-theorem)
  - [Purely inseparable extension without a primitive element](#purely-inseparable-extension-without-a-primitive-element)
- [Finite separable simple extension implications](#finite-separable-simple-extension-implications)
- [Biquadratic extension](#biquadratic-extension)
  - [Unramified biquadratic extension of a real quadratic field](#unramified-biquadratic-extension-of-a-real-quadratic-field)
- [Transitive subgroups of the symmetric group on four points](#transitive-subgroups-of-the-symmetric-group-on-four-points)
- [Dihedral Galois action on four radical roots](#dihedral-galois-action-on-four-radical-roots)
- [Galois group of an irreducible even quartic](#galois-group-of-an-irreducible-even-quartic)
  - [Klein-four criterion for an irreducible even quartic](#klein-four-criterion-for-an-irreducible-even-quartic)
- [Field homomorphism](#field-homomorphism)
  - [Field isomorphism](#field-isomorphism)
    - [K-isomorphism](#k-isomorphism)
  - [Field embedding](#field-embedding)
    - [Extension theorem for field embeddings](#extension-theorem-for-field-embeddings)
    - [Linear independence of distinct field embeddings](#linear-independence-of-distinct-field-embeddings)
      - [Automorphism-count bound for a finite field extension](#automorphism-count-bound-for-a-finite-field-extension)
      - [Lagrange resolvent eigenvector for a cyclic field automorphism](#lagrange-resolvent-eigenvector-for-a-cyclic-field-automorphism)
    - [Extension count for field embeddings](#extension-count-for-field-embeddings)
- [Tower law for field extensions](#tower-law-for-field-extensions)
- [Splitting field](#splitting-field)
  - [Root-embedding correspondence](#root-embedding-correspondence)
  - [Existence and uniqueness of splitting fields](#existence-and-uniqueness-of-splitting-fields)
  - [Splitting field of x cubed minus two](#splitting-field-of-x-cubed-minus-two)
  - [Finite normal extension as a splitting field](#finite-normal-extension-as-a-splitting-field)
  - [Splitting field of a polynomial obtained by Frobenius substitution](#splitting-field-of-a-polynomial-obtained-by-frobenius-substitution)
  - [Splitting field over a finite field](#splitting-field-over-a-finite-field)
- [Normal extension](#normal-extension)
- [Separable extension](#separable-extension)
  - [Separable algebraic element](#separable-algebraic-element)
- [Purely inseparable extension](#purely-inseparable-extension)
  - [Purely inseparable algebraic element](#purely-inseparable-algebraic-element)
    - [Minimal polynomial of a purely inseparable element](#minimal-polynomial-of-a-purely-inseparable-element)
      - [Purely inseparable polynomial over a rational function field](#purely-inseparable-polynomial-over-a-rational-function-field)
  - [Unique embedding extension through a purely inseparable extension](#unique-embedding-extension-through-a-purely-inseparable-extension)
- [Field automorphism](#field-automorphism)
  - [Field automorphism group](#field-automorphism-group)
- [Finite Galois extension](#finite-galois-extension)
  - [Normal basis theorem](#normal-basis-theorem)
  - [Galois group](#galois-group)
  - [Normal and separable implies Galois](#normal-and-separable-implies-galois)
  - [Abelian extension](#abelian-extension)
- [Roots of unity in a finite field](#roots-of-unity-in-a-finite-field)
- [Kummer extension of rational function fields](#kummer-extension-of-rational-function-fields)
- [Galois group of a polynomial](#galois-group-of-a-polynomial)
  - [Unramified reduction of a polynomial Galois group](#unramified-reduction-of-a-polynomial-galois-group)
  - [Transitivity lifted through unique pth roots](#transitivity-lifted-through-unique-pth-roots)
- [Irreducible factors after Frobenius substitution](#irreducible-factors-after-frobenius-substitution)
  - [Reducibility criterion after Frobenius substitution](#reducibility-criterion-after-frobenius-substitution)
- [Frobenius cycle type](#frobenius-cycle-type)
- [Dedekind factorization cycle test](#dedekind-factorization-cycle-test)
- [Cyclotomic polynomial](#cyclotomic-polynomial)
  - [Cyclotomic reduction at a conductor prime](#cyclotomic-reduction-at-a-conductor-prime)
  - [Cyclotomic factorization](#cyclotomic-factorization)
  - [Irreducibility of cyclotomic polynomials](#irreducibility-of-cyclotomic-polynomials)
  - [Thirtieth cyclotomic polynomial](#thirtieth-cyclotomic-polynomial)
  - [Separability of a cyclotomic polynomial modulo p](#separability-of-a-cyclotomic-polynomial-modulo-p)
  - [Galois embedding for a cyclotomic polynomial](#galois-embedding-for-a-cyclotomic-polynomial)
  - [Cyclotomic field](#cyclotomic-field)
    - [Cyclotomic Artin reciprocity over the rational numbers](#cyclotomic-artin-reciprocity-over-the-rational-numbers)
    - [Cyclotomic unit](#cyclotomic-unit)
      - [Reduction of cyclotomic units at the ramified prime](#reduction-of-cyclotomic-units-at-the-ramified-prime)
      - [Cyclotomic unit index formula](#cyclotomic-unit-index-formula)
      - [Symmetric cyclotomic unit](#symmetric-cyclotomic-unit)
      - [Cyclotomic Euler system](#cyclotomic-euler-system)
        - [Root-of-unity Euler system](#root-of-unity-euler-system)
          - [Cyclotomic Euler norm factor at a new prime](#cyclotomic-euler-norm-factor-at-a-new-prime)
          - [Kolyvagin derivative operator for a cyclic group](#kolyvagin-derivative-operator-for-a-cyclic-group)
          - [Euler-system divisibility for real cyclotomic class modules](#euler-system-divisibility-for-real-cyclotomic-class-modules)
    - [Nonprincipal cyclotomic fields of conductor a prime power](#nonprincipal-cyclotomic-fields-of-conductor-a-prime-power)
    - [Total ramification in a prime-power cyclotomic field](#total-ramification-in-a-prime-power-cyclotomic-field)
    - [Quadratic subfield of a prime cyclotomic field](#quadratic-subfield-of-a-prime-cyclotomic-field)
    - [Prime cyclotomic field degree](#prime-cyclotomic-field-degree)
      - [Discriminant of a prime cyclotomic power basis](#discriminant-of-a-prime-cyclotomic-power-basis)
    - [Maximal real subfield of the fifth cyclotomic field](#maximal-real-subfield-of-the-fifth-cyclotomic-field)
    - [Roots of unity in a rational cyclotomic field](#roots-of-unity-in-a-rational-cyclotomic-field)
    - [Seventh cyclotomic field](#seventh-cyclotomic-field)
      - [Quadratic Gaussian period in the seventh cyclotomic field](#quadratic-gaussian-period-in-the-seventh-cyclotomic-field)
      - [Real cubic subfield of the seventh cyclotomic field](#real-cubic-subfield-of-the-seventh-cyclotomic-field)
    - [Eleventh cyclotomic field](#eleventh-cyclotomic-field)
      - [Quadratic Gaussian period in the eleventh cyclotomic field](#quadratic-gaussian-period-in-the-eleventh-cyclotomic-field)
      - [Maximal real subfield of the eleventh cyclotomic field](#maximal-real-subfield-of-the-eleventh-cyclotomic-field)
    - [Maximal cyclotomic extension](#maximal-cyclotomic-extension)
      - [Maximal cyclotomic extension of the real numbers](#maximal-cyclotomic-extension-of-the-real-numbers)
      - [Maximal cyclotomic extension of the rational numbers](#maximal-cyclotomic-extension-of-the-rational-numbers)
      - [Maximal cyclotomic extension of a finite field](#maximal-cyclotomic-extension-of-a-finite-field)
- [Constructible number](#constructible-number)
  - [Constructible field extension](#constructible-field-extension)
    - [Constructibility of the real seventeenth cyclotomic field](#constructibility-of-the-real-seventeenth-cyclotomic-field)
- [Fixed field](#fixed-field)
  - [Dihedral fixed field in one rational variable](#dihedral-fixed-field-in-one-rational-variable)
  - [Dihedral fixed field of a two-variable rational function field](#dihedral-fixed-field-of-a-two-variable-rational-function-field)
- [Artin fixed-field theorem](#artin-fixed-field-theorem)
  - [Orbit polynomial under a finite automorphism group](#orbit-polynomial-under-a-finite-automorphism-group)
    - [Coefficients of an orbit polynomial for a primitive generator](#coefficients-of-an-orbit-polynomial-for-a-primitive-generator)
    - [Separate orbit polynomials can miss mixed invariants](#separate-orbit-polynomials-can-miss-mixed-invariants)
- [Galois correspondence](#galois-correspondence)
  - [Normal subextension criterion](#normal-subextension-criterion)
  - [Subextensions of an abelian Galois extension](#subextensions-of-an-abelian-galois-extension)
    - [Cyclic Galois extension of the rational numbers of every finite degree](#cyclic-galois-extension-of-the-rational-numbers-of-every-finite-degree)
    - [Finite extensions of the fixed field of a finite-order automorphism of an algebraically closed field](#finite-extensions-of-the-fixed-field-of-a-finite-order-automorphism-of-an-algebraically-closed-field)
  - [Subfields of the splitting field of x to the fourth minus seven](#subfields-of-the-splitting-field-of-x-to-the-fourth-minus-seven)
- [Polynomial discriminant](#polynomial-discriminant)
  - [Squarefree polynomial discriminant does not imply irreducibility](#squarefree-polynomial-discriminant-does-not-imply-irreducibility)
  - [Cubic resolvent of a quartic](#cubic-resolvent-of-a-quartic)
    - [S4 criterion from the cubic resolvent of an irreducible quartic](#s4-criterion-from-the-cubic-resolvent-of-an-irreducible-quartic)
  - [Vandermonde determinant](#vandermonde-determinant)
    - [Weighted Vandermonde determinant](#weighted-vandermonde-determinant)
    - [Vandermonde determinant invariance under monic basis change](#vandermonde-determinant-invariance-under-monic-basis-change)
    - [Vandermonde shift identity](#vandermonde-shift-identity)
    - [Leading coefficient of an exponential alternant](#leading-coefficient-of-an-exponential-alternant)
    - [Vandermonde matrix](#vandermonde-matrix)
      - [Zero power sums force a finite complex multiset to vanish](#zero-power-sums-force-a-finite-complex-multiset-to-vanish)
  - [Discriminant of a depressed cubic](#discriminant-of-a-depressed-cubic)
  - [Discriminant criterion for an alternating Galois group](#discriminant-criterion-for-an-alternating-galois-group)
- [Resolvent (Galois theory)](#resolvent-galois-theory)
  - [Lagrange resolvent for a cubic](#lagrange-resolvent-for-a-cubic)
    - [Cubic resolvent](#cubic-resolvent)
      - [Cardano formula](#cardano-formula)
- [Solvability by radicals](#solvability-by-radicals)
- [Galois group of an irreducible cubic](#galois-group-of-an-irreducible-cubic)
  - [Quadratic resolvent field of a cubic](#quadratic-resolvent-field-of-a-cubic)
  - [Splitting field of x cubed minus x minus one](#splitting-field-of-x-cubed-minus-x-minus-one)
  - [Cubic discriminant criterion](#cubic-discriminant-criterion)
- [Characteristic-two cubic resolvent](#characteristic-two-cubic-resolvent)
- [Artin–Schreier theory](#artin-schreier-theory)
  - [Artin-Schreier embedding problems over a characteristic-p field](#artin-schreier-embedding-problems-over-a-characteristic-p-field)
  - [Artin–Schreier polynomial](#artin-schreier-polynomial)
  - [Artin–Schreier extension](#artin-schreier-extension)

## Inverse Galois problem

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_Galois_problem)

The inverse Galois problem asks which finite groups occur as [Galois groups](#galois-group) over a given [field](algebra.md#field), with the classical problem taking the base [field](algebra.md#field) to be $\mathbb Q$. A regular realization over $K(T)$ and [Galois-preserving Hilbert specialization](algebra.md#galois-preserving-hilbert-specialization) solve an instance over a [Hilbertian field](algebra.md#hilbertian-field). Realization over an algebraically closed constant [field](algebra.md#field)'s [rational function field](algebra.md#rational-function-field) alone does not supply descent to $\mathbb Q$.

### Rigid ramification type

↑ **Parent:** [Inverse Galois problem](#inverse-galois-problem)

Fix ordered branch positions and conjugacy classes $C_i$ in a finite group $G$. The generating product-one tuples $(g_1,\ldots,g_r)\in\prod C_i$ form the inner Nielsen set. The type is rigid when this set is nonempty and a single simultaneous-conjugation orbit. Over $\mathbb C(T)$ this fixes the connected Galois cover up to isomorphism: tuples prescribe the [monodromy](complex-analysis.md#monodromy) epimorphism of the punctured sphere, and conjugate epimorphisms give isomorphic covers; the local completions at punctures are uniquely determined by their cyclic [monodromy](complex-analysis.md#monodromy).

## Compact Galois module

↑ **Parent:** [Galois theory](galois-theory.md)

A compact Galois module is a compact [profinite abelian group](topological-group.md#profinite-abelian-group) equipped with a continuous [Galois group](#galois-group) action. An abelian [pro-p group](topological-group.md#pro-p-group) is naturally a compact $\mathbb Z_p$-[module](module-theory.md#module-mathematics). A continuous action of the [Galois group](#galois-group) of a [Zp-extension](algebraic-number-theory.md#zp-extension) extends to its [Iwasawa algebra of a Zp-extension](associative-algebra.md#iwasawa-algebra-of-a-zp-extension). This compact topology differs from the discrete topology usually used in [Galois cohomology](#galois-cohomology).

## Solvable field extension

↑ **Parent:** [Galois theory](galois-theory.md)

A finite separable extension is solvable when its normal closure has a [solvable group](group-theory.md#solvable-group) as [Galois group](#galois-group). In characteristic zero it is contained in a radical tower after adjoining suitable [roots of unity](algebra.md#root-of-unity); containment need not mean it is itself a tower of radical adjunctions.

## Radical extension

↑ **Parent:** [Galois theory](galois-theory.md)

In the strict tower convention, a radical extension is a field obtained through finitely many adjunctions $a_i^{n_i}\in K_{i-1}$, $K_i=K_{i-1}(a_i)$. Some texts instead use the term for any subfield of such a tower. This distinction matters: [solvability by radicals](#solvability-by-radicals) implies containment in a tower, and need not give a radical tower entirely inside the original field.

## Absolute Galois group

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Absolute_Galois_group)

The absolute Galois group of a field $K$ is $G_K=\operatorname{Gal}(K^{\mathrm{sep}}/K)$. It is a [profinite group](topological-group.md#profinite-group), the inverse limit of the Galois groups of finite Galois extensions. Its continuous actions on discrete modules are the coefficients for [Galois cohomology](#galois-cohomology).

## Galois closure of a field extension

↑ **Parent:** [Galois theory](galois-theory.md)

The Galois closure of a finite separable extension $L/K$ is the smallest [Galois extension](#finite-galois-extension) in a fixed separable closure containing $L$. It is generated by all the conjugates of $L$. If $G=\operatorname{Gal}(M/K)$ and $H=\operatorname{Gal}(M/L)$, their [subgroup core](group-theory.md#core-group-theory) is trivial. This is distinct from the existing group-theoretic [normal closure](group-theory.md#normal-closure).

## Fundamental theorem of Galois theory

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_of_Galois_theory)

For a finite [Galois extension](#finite-galois-extension) $L/K$, intermediate fields correspond inclusion-reversingly to subgroups of $\operatorname{Gal}(L/K)$. Normal subgroups correspond to Galois intermediate extensions.

## Kummer theory

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kummer_theory)

When a field $K$ contains the $n$th roots of unity and its characteristic does not divide $n$, Kummer theory identifies cyclic extensions of degree dividing $n$ with suitable classes in $K^\times/(K^\times)^n$. Cohomologically,

$$
H^1(G_K,\mu_n)\simeq K^\times/(K^\times)^n.
$$

### Finite ramification support for radical extensions

↑ **Parent:** [Kummer theory](#kummer-theory)

For a [number field](algebraic-number-theory.md#number-field) and finite subgroup $\Delta\subset K^*/K^{*n}$, adjoining all the indicated nth roots gives an extension [unramified](arithmetic.md#unramified-extension) outside the displayed finite set. The valuations modulo $n$ are independent of representatives. At a finite place outside $S$, divide each radicand by a local nth power of a [uniformizer](commutative-algebra.md#uniformizer) to obtain a unit. Its polynomial has separable reduction because $n$ is invertible. A finite [unramified extension](arithmetic.md#unramified-extension) containing all residue roots contains all lifted roots by [Hensel's lemma](arithmetic.md#hensel-s-lemma). This proof does not require $\mu_n\subset K$.

### Cyclic Galois resolvent

↑ **Parent:** [Kummer theory](#kummer-theory)

For a cyclic [Galois extension](#finite-galois-extension) $M/K$ of degree $m$, choose a generator $g$ and a primitive $m$th root of unity $\zeta\in K$. Reindexing the displayed sum gives $gR(w)=\zeta R(w)$. [Linear independence of distinct field embeddings](#linear-independence-of-distinct-field-embeddings) ensures this sum is not identically zero as a function of $w$. Choosing $\alpha=R(w)\ne0$ therefore gives $m$ distinct conjugates $\zeta^j\alpha$, while $\alpha^m\in K$. Consequently $M=K(\alpha)$ is the splitting field of $X^m-\alpha^m$. Independence follows by taking a shortest supposed linear relation among distinct automorphisms, evaluating at $uv$ and subtracting a suitable multiple of the relation at $v$ to remove one term but not all terms.

### Kummer reflection in Iwasawa theory

↑ **Parent:** [Kummer theory](#kummer-theory)

For nontrivial even $\chi$ in the full cyclotomic tower of $\mathbb Q$, [Kummer theory](#kummer-theory) relates the [p-ramified Iwasawa module](algebraic-number-theory.md#p-ramified-iwasawa-module) to the reflected odd [unramified Iwasawa module](algebraic-number-theory.md#unramified-iwasawa-module), up to [pseudo-isomorphism](associative-algebra.md#pseudo-isomorphism). Here $\iota(\gamma)=\gamma^{-1}$ and $(1)$ is the [Tate twist](representation-theory.md#tate-twist). The induced substitution on characteristic series is $T\mapsto u(1+T)^{-1}-1$, where $u$ is the cyclotomic value of $\gamma$. Omitting either operation changes the interpolation convention.

### Kummer cohomology divisibility criterion

↑ **Parent:** [Kummer theory](#kummer-theory)

When the characteristic differs from $p$, the Kummer sequence gives $0\to H^n(L,K_s^{\times})/p\to H^{n+1}(L,\mu_p)\to H^{n+1}(L,K_s^{\times})[p]\to0$. For $n\ge1$, the positive-degree multiplicative groups are torsion. Thus the middle group is zero exactly when the first multiplicative group is $p$-divisible and the second has zero $p$-primary torsion.

### Unramified Kummer classes with bounded prime support

↑ **Parent:** [Kummer theory](#kummer-theory)

For a [number field](algebraic-number-theory.md#number-field) $K$, a finite set $S$ and $m\geq2$, let $K(S,m)$ consist of classes $[a]\in K^*/K^{*m}$ whose valuations outside $S$ are divisible by $m$. It fits into $0\to\mathcal O_{K,S}^{\times}/(\mathcal O_{K,S}^{\times})^m\to K(S,m)\to\operatorname{Cl}(\mathcal O_{K,S})[m]\to0$. The [S-unit group](algebra.md#s-unit-group) is finitely generated and the [ideal class group](algebraic-number-theory.md#ideal-class-group) is finite, so $K(S,m)$ is finite. When $S$ contains primes dividing $m$, this controls unramified multiplicative Kummer classes outside $S$.

### Square-class group of a field

↑ **Parent:** [Kummer theory](#kummer-theory)

The square-class group identifies two nonzero elements of a [field](algebra.md#field) when their quotient is a square. Multiplication makes it an [abelian group](group.md#abelian-group) of exponent two, hence a [vector space](vector-space.md) over $\mathbb F_2$. It records quadratic extensions and the images of [Kummer theory](#kummer-theory) for $n=2$.

#### Square-class group of the 2-adic Gaussian field

↑ **Parent:** [Square-class group of a field](#square-class-group-of-a-field)

The [valuation](algebra.md#valuation) contributes one factor $C_2$. The [unit decomposition of the 2-adic Gaussian field](arithmetic.md#unit-decomposition-of-the-2-adic-gaussian-field) contributes $\mu_4/\mu_4^2\cong C_2$ and the additive quotient $\mathbb Z_2[i]/2\mathbb Z_2[i]\cong C_2^2$. Thus there are sixteen [square classes](#square-class) and fifteen [quadratic extensions](algebra.md#quadratic-extension) over this field.

#### Square class

↑ **Parent:** [Square-class group of a field](#square-class-group-of-a-field)

The square class of $a\in K^*$ is its image in the [square-class group of a field](#square-class-group-of-a-field) $K^*/K^{*2}$. Two nonzero elements have the same square class exactly when their quotient is a square. Every element of this quotient has order dividing $2$. Over the [rational numbers](number-theory.md#rational-number), a square class has a unique signed squarefree integer representative.

##### Square-class group of a p-adic field

↑ **Parent:** [Square class](#square-class)

For odd $p$, parity of [valuation](algebra.md#valuation) and the [square class](#square-class) of the unit residue give a [group](group.md) $C_2\times C_2$, represented by $1,u,p,pu$ for a unit $u$ with nonsquare residue. For $p=2$, [valuation](algebra.md#valuation) parity and unit residue modulo eight give $C_2^3$, with generators $-1,5,2$. The unit criteria follow from the [Hensel lemma](arithmetic.md#hensel-s-lemma), using its strong derivative version for $p=2$.

### Kummer extension

↑ **Parent:** [Kummer theory](#kummer-theory)

When a field $K$ contains the relevant roots of unity, adjoining an $n$th root of an element of $K$ gives a Kummer extension. Such extensions describe abelian extensions of exponent dividing $n$.

## Galois cohomology

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Galois_cohomology)

Galois cohomology is the [group cohomology](group-theory.md#group-cohomology) of a Galois group acting on a module. For a discrete $G$-module $M$, the first group is the quotient of crossed homomorphisms $c(\sigma\tau)=c(\sigma)+\sigma c(\tau)$ by maps $c(\sigma)=\sigma m-m$.

<h3 id="weil-chatelet-group">Weil–Châtelet group</h3>

↑ **Parent:** [Galois cohomology](#galois-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weil–Châtelet_group)

For an [abelian variety](abelian-variety.md) $A$ over a field $K$, its Weil–Châtelet group is the [Galois cohomology](#galois-cohomology) group $H^1(K,A(K^{\rm sep}))$, classifying torsors under $A$. Such an [algebraic-group torsor](lie-theory.md#algebraic-group-torsor) becomes $A$ after passing to a separable closure but need not have a $K$-point. A chosen geometric point identifies the torsor with $A$ and its Galois descent with a cocycle; changing that point adds a coboundary. The zero class is precisely the torsor with a rational point. For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), these torsors are genus-one curves with a specified action and Jacobian. Over a number field the kernel of restriction to every completion is the [Tate–Shafarevich group](normalization-of-an-algebraic-curve.md#tate-shafarevich-group).

### Galois descent of vector spaces

↑ **Parent:** [Galois cohomology](#galois-cohomology)

For a [Finite Galois extension](#finite-galois-extension) $L/K$ and a finite-dimensional $L$-space $V$ with a [semilinear action](#semilinear-action) of its [Galois group](#galois-group), the map $L\otimes_KV^G\to V$ is an isomorphism. The vectors $\sum_{\sigma}\sigma(a)\sigma(v)$ are invariant and span $V$ by the [Artin independence theorem](#linear-independence-of-distinct-field-embeddings). Choosing an invariant $L$-basis then identifies the invariant space with its $K$-span. The proof does not divide by the extension degree.

#### Descent classification of central simple algebras

↑ **Parent:** [Galois descent of vector spaces](#galois-descent-of-vector-spaces)

A splitting isomorphism of a [central simple algebra](associative-algebra.md#central-simple-algebra) with $M_n(L)$ transports its Galois action to $T_\sigma=c_\sigma\sigma_0$, giving a [nonabelian first cohomology](group-theory.md#nonabelian-first-cohomology) class. Conversely a cocycle gives a semilinear algebra action whose invariants descend to a [central simple algebra](associative-algebra.md#central-simple-algebra). Equivalent cocycles give isomorphic fixed algebras. This gives a pointed-set bijection $\operatorname{CSA}_n(L/K)\cong H^1(\operatorname{Gal}(L/K),\operatorname{PGL}_n(L))$.

#### Semilinear action

↑ **Parent:** [Galois descent of vector spaces](#galois-descent-of-vector-spaces)

For an extension $L/K$ with [Galois group](#galois-group) $G$, a [semilinear action](#semilinear-action) on an $L$-space is an additive group action satisfying $\sigma(av)=\sigma(a)\sigma(v)$. Scalar coefficients are transformed along with vectors. Invariants form a $K$-space, and [Galois descent of vector spaces](#galois-descent-of-vector-spaces) reconstructs the original space from it.

### First Galois cohomology unramified outside a finite set

↑ **Parent:** [Galois cohomology](#galois-cohomology)

For a finite Galois module $M$ unramified outside a finite set $S$, define $H^1_S(K,M)$ as the classes in [Galois cohomology](#galois-cohomology) whose restriction to inertia is zero at every finite prime outside $S$. This means zero as a cohomology class, rather than zero for every possible representative. Passing to a finite Galois extension on which $M$ is constant reduces the finiteness problem to characters with bounded ramification and a finite restriction kernel.

### Galois module

↑ **Parent:** [Galois cohomology](#galois-cohomology)

A discrete Galois module over $K$ is an abelian group with a continuous action of the [absolute Galois group](#absolute-galois-group) $G_K$. Continuity means that each element has an open stabilizer. Examples are the algebraic points of an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), its finite torsion module $E[m]$, and the group of roots of unity $\mu_m$. [Galois cohomology](#galois-cohomology) takes continuous cocycles with values in such a module.

#### Galois module of roots of unity

↑ **Parent:** [Galois module](#galois-module)

The module $\mu_m$ consists of the $m$th roots of unity in a separable closure. If the field characteristic does not divide $m$, it has $m$ elements and fits into the Kummer sequence $1\to\mu_m\to K_s^{\times}\xrightarrow{m}K_s^{\times}\to1$. Its Galois action is the cyclotomic action; a generator gives a noncanonical identification with $\mathbb Z/m\mathbb Z$.

<h3 id="hilbert-s-theorem-90">Hilbert's theorem 90</h3>

↑ **Parent:** [Galois cohomology](#galois-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hilbert's_theorem_90)

For a finite Galois extension $L/K$, multiplicative Hilbert theorem 90 says $H^1(\operatorname{Gal}(L/K),L^*)=0$. A multiplicative cocycle has the form $c_\sigma=\sigma(b)/b$. One proof forms a nonzero sum $A=\sum_\sigma c_\sigma\sigma(a)$, using linear independence of field automorphisms. Its transformation law is $\tau A=c_\tau^{-1}A$, so $b=A^{-1}$ gives $c_\tau=\tau(b)/b$. Passing to the algebraic closure gives $H^1(K,\overline K^*)=0$, so the multiplicative Kummer sequence identifies $H^1(K,\mu_m)$ with $K^*/K^{*m}$.

#### Unit form of Hilbert theorem 90

↑ **Parent:** [Hilbert's theorem 90](#hilbert-s-theorem-90)

For an [unramified extension](arithmetic.md#unramified-extension) of non-Archimedean [local fields](arithmetic.md#local-field), let $\phi$ generate its cyclic [Galois group](#galois-group). The ordinary [Hilbert theorem 90](#hilbert-s-theorem-90) supplies $b\in L^\times$ with $x=\phi(b)/b$. A common [uniformizer](commutative-algebra.md#uniformizer) $\pi\in K$ gives $y=\pi^{-v_L(b)}b\in\mathcal O_L^\times$, retaining the same quotient because $\phi$ fixes $\pi$. The reverse implication follows by telescoping the [field norm](algebraic-number-theory.md#field-norm).

## Frobenius endomorphism

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frobenius_endomorphism)

In a field of characteristic $p>0$, the Frobenius map $x\mapsto x^p$ is an injective field endomorphism because

$$
(x+y)^p=x^p+y^p.
$$

Consequently every element of an extension field has at most one $p$th root.

## Formal derivative

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Formal_derivative)

The formal derivative of $f(T)=\sum_i a_iT^i$ is $f'(T)=\sum_i ia_iT^{i-1}$.

### Formal derivative in positive characteristic

↑ **Parent:** [Formal derivative](#formal-derivative)

In [characteristic](algebra.md#characteristic-of-a-field) $p$, the coefficient $i$ in a [formal derivative](#formal-derivative) vanishes exactly when $p$ divides $i$.

#### Polynomial with zero formal derivative in characteristic p

↑ **Parent:** [Formal derivative in positive characteristic](#formal-derivative-in-positive-characteristic)

Over a field of characteristic $p>0$,

$$
f'(T)=0
\quad\Longleftrightarrow\quad
f(T)=g(T^p)
$$

for some polynomial $g$. Indeed, zero derivative says every exponent with nonzero coefficient is divisible by $p$.

## Separable polynomial

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separable_polynomial)

A polynomial over a field is separable when it has no repeated root in a splitting field. Equivalently, it is coprime to its [formal derivative](#formal-derivative).

### Separability of roots of unity

↑ **Parent:** [Separable polynomial](#separable-polynomial)

If the [characteristic](algebra.md#characteristic-of-a-field) of a field does not divide the [positive integer](number-theory.md#positive-integer) $m$, then $X^m-1$ is [separable](#separable-polynomial). Its [formal derivative](#formal-derivative) is $mX^{m-1}$, and a common root would have to be both nonzero and zero.

### Irreducible polynomial in characteristic zero is separable

↑ **Parent:** [Separable polynomial](#separable-polynomial)

If $f$ is irreducible over a field of characteristic zero, then $f'\ne0$ and $\deg f'<\deg f$. Thus $f$ cannot divide $f'$, so irreducibility gives $\gcd(f,f')=1$. Consequently $f$ has no repeated root in any extension field.

## Automorphism-count divisibility theorem

↑ **Parent:** [Galois theory](galois-theory.md)

For a finite extension $K/F$, the automorphism group $G=\operatorname{Aut}_F(K)$ has order dividing $[K:F]$. Indeed, Artin's theorem gives $[K:K^G]=|G|$, while $F\subseteq K^G$ and the tower law gives the divisibility.

## Coprime-degree descent for powers

↑ **Parent:** [Galois theory](galois-theory.md)

Let $L/K$ have degree $d$ with $\gcd(d,n)=1$. If $a=x^n\in K$ for some $x\in L$, then

$$
a^d=N_{L/K}(x)^n.
$$

Choosing $r,s\in\mathbb Z$ with $rd+sn=1$ gives

$$
a=\bigl(N_{L/K}(x)^r a^s\bigr)^n,
$$

so $a$ was already an $n$th power in $K$.

## Algebraic element

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algebraic_element)

An element $\alpha$ of a field extension $L/K$ is algebraic over $K$ when some nonzero polynomial in $K[X]$ vanishes at $\alpha$.

### Minimal polynomial of an algebraic element

↑ **Parent:** [Algebraic element](#algebraic-element)

The minimal polynomial of an algebraic element $\alpha$ over $K$ is the unique monic polynomial of least positive degree in $K[X]$ that vanishes at $\alpha$. It is irreducible, and its degree equals $[K(\alpha):K]$.

## Primitive element of a field extension

↑ **Parent:** [Galois theory](galois-theory.md)

A primitive element of a finite extension $L/K$ is an element $\alpha\in L$ such that $L=K(\alpha)$.

The [primitive element theorem](#primitive-element-theorem) proves existence under finite separability; the [primitive element of a field extension](#primitive-element-of-a-field-extension) is the generator whose existence the theorem asserts.

### Primitive elements form a principal Zariski-open set

↑ **Parent:** [Primitive element of a field extension](#primitive-element-of-a-field-extension)

Fix a $K$-basis of a finite extension $L/K$ of degree $n$. The coordinates of $1,\alpha,\ldots,\alpha^{n-1}$ are polynomial functions of the coordinates of $\alpha$, because multiplication in $L$ has fixed structure constants. The determinant $D(\alpha)$ of those coordinate columns is therefore a polynomial, and

$$
K[\alpha]=L\quad\Longleftrightarrow\quad D(\alpha)\ne0.
$$

Thus the primitive-element locus is the distinguished [Zariski-open set](algebraic-geometry.md#zariski-open-set) $D(D)\subseteq\mathbb A_K^n$, possibly empty for a non-simple extension.

## Primitive element theorem

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_element_theorem)

Every finite separable extension $L/K$ is generated by one element: $L=K(\alpha)$ for some $\alpha\in L$.

### Purely inseparable extension without a primitive element

↑ **Parent:** [Primitive element theorem](#primitive-element-theorem)

Let $K=\mathbb F_p(s,t)$ and $L=K(s^{1/p},t^{1/p})$ for algebraically independent $s,t$. The $p^2$ monomials $s^{i/p}t^{j/p}$ with $0\leq i,j<p$ form a basis, whereas every $\alpha\in L$ satisfies $\alpha^p\in K$. Thus $[L:K]=p^2$ but $[K(\alpha):K]\leq p$, so no [primitive element of a field extension](#primitive-element-of-a-field-extension) exists.

## Finite separable simple extension implications

↑ **Parent:** [Galois theory](galois-theory.md)

A finite separable extension is simple by the primitive element theorem. A simple separable extension is finite because its generator is separable and hence algebraic. Finite and simple does not imply separable: in characteristic $p$, $\mathbb F_p(t^{1/p})/\mathbb F_p(t)$ is finite and simple but purely inseparable.

## Biquadratic extension

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Biquadratic_extension)

If $a,b,ab$ are nonsquares in a field $K$ of characteristic other than two, then

$$
K(\sqrt a,\sqrt b)/K
$$

is a degree-four Galois extension with group $C_2\times C_2$. Its three quadratic intermediate fields are $K(\sqrt a)$, $K(\sqrt b)$, and $K(\sqrt{ab})$.

### Unramified biquadratic extension of a real quadratic field

↑ **Parent:** [Biquadratic extension](#biquadratic-extension)

For distinct primes $p,q\equiv1\pmod4$, put $E=\mathbb Q(\sqrt p,\sqrt q)$ and $K=\mathbb Q(\sqrt{pq})$. The [algebraic integers](algebraic-number-theory.md#algebraic-integer) $a=(1+\sqrt p)/2$ and $b=(1+\sqrt q)/2$ generate an order whose basis has [discriminant of elements of a number field](algebraic-number-theory.md#discriminant-of-elements-of-a-number-field) $p^2q^2$: the [trace pairing](algebraic-number-theory.md#trace-pairing) matrix is, up to basis order, the tensor product of the quadratic trace matrices of determinants $p$ and $q$. If its index in $\mathcal O_E$ is $j$, the [discriminant-index formula for an integral lattice](algebraic-number-theory.md#discriminant-index-formula-for-an-integral-lattice) and the [relative discriminant](algebraic-number-theory.md#relative-discriminant) tower formula give

$$
p^2q^2/j^2=d_E=(pq)^2N_{K/\mathbb Q}(\mathfrak d_{E/K}).
$$

Both $j$ and this [ideal norm](algebraic-number-theory.md#ideal-norm) are positive integers, forcing $j=1$ and $\mathfrak d_{E/K}=\mathcal O_K$. Thus $E/K$ is [unramified](arithmetic.md#unramified-extension) at all finite primes. It is also totally real, so no real place ramifies. This quadratic abelian extension is contained in the ordinary [Hilbert class field](algebraic-number-theory.md#hilbert-class-field) of $K$, and [Artin reciprocity](algebraic-number-theory.md#artin-reciprocity-law) gives a quotient of its [ideal class group](algebraic-number-theory.md#ideal-class-group) of order two. The extensions $K(\sqrt p)$ and $K(\sqrt q)$ are equal to $E$, not two different extensions of $K$.

## Transitive subgroups of the symmetric group on four points

↑ **Parent:** [Galois theory](galois-theory.md)

Up to conjugacy, the transitive subgroups of $S_4$ are $C_4$, $V_4$, $D_8$, $A_4$, and $S_4$.

## Dihedral Galois action on four radical roots

↑ **Parent:** [Galois theory](galois-theory.md)

If $r$ cyclically sends $\alpha\mapsto\beta\mapsto-\alpha\mapsto-\beta$ and $s$ fixes $\alpha$ while negating $\beta$, then $r^4=s^2=1$ and $srs=r^{-1}$. These automorphisms realize $D_8$ as the Galois group of the corresponding quartic splitting field.

## Galois group of an irreducible even quartic

↑ **Parent:** [Galois theory](galois-theory.md)

Let $g(X)=X^4+bX^2+c\in\mathbb Q[X]$ be irreducible, let $\alpha$ be a root, and put $\delta=\sqrt c$. Its roots are

$$
\alpha,-\alpha,\frac\delta\alpha,-\frac\delta\alpha,
$$

so its splitting field is $K=\mathbb Q(\alpha,\delta)$. If $\delta\notin\mathbb Q(\alpha)$, then $[K:\mathbb Q]=8$ and the Galois group is $D_8$. If $\delta\in\mathbb Q(\alpha)$, then $[K:\mathbb Q]=4$ and the group is $V_4$ when $\delta\in\mathbb Q$, and $C_4$ otherwise.

### Klein-four criterion for an irreducible even quartic

↑ **Parent:** [Galois group of an irreducible even quartic](#galois-group-of-an-irreducible-even-quartic)

For irreducible $X^4+bX^2+c\in\mathbb Q[X]$, the Galois group is $C_2\times C_2$ exactly when $c$ is a square in $\mathbb Q$. In the transitive Klein-four action on the roots $\alpha,-\alpha,\beta,-\beta$, all three nonidentity double transpositions fix $\alpha\beta=\sqrt c$, forcing it into the fixed field $\mathbb Q$.

## Field homomorphism

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Field_homomorphism)

A field homomorphism preserves addition, multiplication, and the multiplicative identity.

### Field isomorphism

↑ **Parent:** [Field homomorphism](#field-homomorphism)

A field isomorphism is a bijective [field homomorphism](#field-homomorphism); its inverse is also a field homomorphism. For fields extending a specified field $K$, an isomorphism may be required to fix $K$ pointwise, a stronger requirement than an abstract field isomorphism.

#### K-isomorphism

↑ **Parent:** [Field isomorphism](#field-isomorphism)

A K-isomorphism between extensions of $K$ is a [field isomorphism](#field-isomorphism) fixing $K$ pointwise. Simple algebraic extensions $K(\alpha)$ and $K(\beta)$ admit one sending $\alpha$ to $\beta$ exactly when their [minimal polynomials](linear-operator-theory.md#minimal-polynomial) agree: both then identify with the same quotient $K[X]/(m)$.

### Field embedding

↑ **Parent:** [Field homomorphism](#field-homomorphism)

A field embedding $L\to\Omega$ is an injective field homomorphism. A $K$-embedding fixes every element of the base field $K$.

#### Extension theorem for field embeddings

↑ **Parent:** [Field embedding](#field-embedding)

An embedding of a subfield into an algebraically closed field extends over an algebraic extension: for a simple extension, map its generator to a root of the transported [minimal polynomial](linear-operator-theory.md#minimal-polynomial), then iterate or use [Zorn lemma](set-theory.md#zorn-s-lemma). If the larger extension is normal over the fixed base, its image under the extended embedding is itself.

#### Linear independence of distinct field embeddings

↑ **Parent:** [Field embedding](#field-embedding)

Distinct field embeddings $\sigma_1,\ldots,\sigma_n:L\to\Omega$ are linearly independent over $\Omega$ as functions on $L$. Thus a nontrivial linear combination $\sum_i a_i\sigma_i$ cannot vanish on every element of $L$.

For the proof, choose a vanishing relation with the fewest nonzero coefficients and normalize one coefficient to one. If $\sigma_1\ne\sigma_m$, choose $y$ with $\sigma_1(y)\ne\sigma_m(y)$. Evaluating at $xy$ and subtracting $\sigma_m(y)$ times the relation evaluated at $x$ eliminates its $m$th term but leaves a nonzero first coefficient, contradicting minimality.

##### Automorphism-count bound for a finite field extension

↑ **Parent:** [Linear independence of distinct field embeddings](#linear-independence-of-distinct-field-embeddings)

If $K/k$ is finite, then any distinct $k$-automorphisms $\sigma_1,\ldots,\sigma_m$ of $K$ are linearly independent in the $K$-vector space $\operatorname{Hom}_k(K,K)$, whose dimension over $K$ is $[K:k]$. Hence $m\leq[K:k]$. In particular, a finite automorphism group $G$ satisfies $|G|\leq[K:K^G]$.

##### Lagrange resolvent eigenvector for a cyclic field automorphism

↑ **Parent:** [Linear independence of distinct field embeddings](#linear-independence-of-distinct-field-embeddings)

If $\sigma$ has order $n$ and the fixed field contains a primitive $n$th root $\zeta$, then

$$
T_\zeta(\beta)=\sum_{j=0}^{n-1}\zeta^{-j}\sigma^j(\beta)
$$

satisfies $\sigma(T_\zeta(\beta))=\zeta T_\zeta(\beta)$. Independence of the powers of $\sigma$ ensures that $T_\zeta(\beta)$ is nonzero for some $\beta$.

#### Extension count for field embeddings

↑ **Parent:** [Field embedding](#field-embedding)

An embedding of $K(\alpha_1,\ldots,\alpha_i)$ extends across $\alpha_{i+1}$ by sending it to a root of its transformed minimal polynomial. There are between one and the relative degree many choices, with equality for a separable extension.

## Tower law for field extensions

↑ **Parent:** [Galois theory](galois-theory.md)

For finite extensions $K\subseteq E\subseteq L$, the degrees multiply:

$$
[L:K]=[L:E][E:K].
$$

If $(u_i)$ is a $K$-basis of $E$ and $(v_j)$ is an $E$-basis of $L$, then the products $(u_iv_j)$ form a $K$-basis of $L$: spanning follows by expanding first over $E$ and then over $K$, while $K$-linear independence follows by grouping coefficients of each $v_j$ and using both basis properties.

## Splitting field

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Splitting_field)

The splitting field of a polynomial over $K$ is the smallest field extension of $K$ in which the polynomial is a product of linear factors.

### Root-embedding correspondence

↑ **Parent:** [Splitting field](#splitting-field)

A root of an irreducible [polynomial](polynomial.md) in an extension field defines a base-field embedding of the [polynomial](polynomial.md) quotient by evaluation. Conversely the image of the residue class of the variable determines the embedding and is a root. This counts embeddings through separable minimal [polynomials](polynomial.md).

### Existence and uniqueness of splitting fields

↑ **Parent:** [Splitting field](#splitting-field)

Every nonconstant polynomial $f\in K[X]$ has a splitting field of finite degree over $K$. It is constructed by adjoining a root of an irreducible factor and repeating over the enlarged field. Any two splitting fields of $f$ over $K$ are isomorphic by an isomorphism that fixes $K$. Inside one fixed algebraic closure, the field generated by all roots is unique as a subfield.

### Splitting field of x cubed minus two

↑ **Parent:** [Splitting field](#splitting-field)

If $\alpha=\sqrt[3]{2}$ is the positive real root and $\zeta_3=e^{2\pi i/3}$, then the roots of $X^3-2$ are

$$
\alpha,\qquad \zeta_3\alpha,\qquad \zeta_3^2\alpha.
$$

Their splitting field over $\mathbb Q$ is $\mathbb Q(\alpha,\zeta_3)$.

### Finite normal extension as a splitting field

↑ **Parent:** [Splitting field](#splitting-field)

A finite extension $L/K$ is [normal](#normal-extension) exactly when it is the splitting field over $K$ of some polynomial. For the forward direction, multiply the minimal polynomials of finitely many generators of $L$; normality puts all their roots in $L$. The reverse direction follows because a $K$-embedding permutes the roots of a polynomial and hence preserves its splitting field.

### Splitting field of a polynomial obtained by Frobenius substitution

↑ **Parent:** [Splitting field](#splitting-field)

Let $g\in K[T]$ in characteristic $p$, let $f(T)=g(T^p)$, let $L$ split $g$ over $K$, and let $M$ split $f$ over $L$. If $y_i$ are the roots of $g$ and $x_i^p=y_i$, then the [Frobenius endomorphism](#frobenius-endomorphism) makes each $x_i$ unique and

$$
M=L(x_i:i)=K(x_i:i),
$$

because $y_i=x_i^p$. Thus $M$ is already the splitting field of $f$ over $K$, and every root of $f$ is purely inseparable over $L$.

### Splitting field over a finite field

↑ **Parent:** [Splitting field](#splitting-field)

Let $f\in\mathbb F_q[X]$ have irreducible factors of degrees $d_1,\ldots,d_r$. A root of a degree-$d_i$ factor lies in $\mathbb F_{q^n}$ exactly when $d_i$ divides $n$. Consequently the splitting field of $f$ is

$$
\mathbb F_{q^m},
\qquad m=\operatorname{lcm}(d_1,\ldots,d_r).
$$

## Normal extension

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_extension)

An algebraic extension $L/K$ is normal when every irreducible polynomial over $K$ with a root in $L$ splits in $L$. For finite extensions, equivalently every $K$-embedding into an algebraic closure has image $L$.

## Separable extension

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separable_extension)

An algebraic extension is separable when every element has a minimal polynomial with distinct roots.

### Separable algebraic element

↑ **Parent:** [Separable extension](#separable-extension)

An algebraic element $x$ over $K$ is separable when its [minimal polynomial](linear-operator-theory.md#minimal-polynomial) over $K$ has no repeated root in a splitting field. For an irreducible polynomial $m_x$, this is equivalent to $m_x'\ne0$, because then $\gcd(m_x,m_x')=1$.

## Purely inseparable extension

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Purely_inseparable_extension)

An algebraic extension in characteristic $p>0$ is purely inseparable when every one of its elements is purely inseparable over the base field.

### Purely inseparable algebraic element

↑ **Parent:** [Purely inseparable extension](#purely-inseparable-extension)

An algebraic element $x$ is purely inseparable over $K$ when $x^{p^n}\in K$ for some $n\geq0$.

#### Minimal polynomial of a purely inseparable element

↑ **Parent:** [Purely inseparable algebraic element](#purely-inseparable-algebraic-element)

An element is purely inseparable over $K$ exactly when its minimal polynomial has the form

$$
T^{p^n}-a,
\qquad a\in K.
$$

To prove the nontrivial direction, repeatedly factor a zero formal derivative through $T\mapsto T^p$ until the remaining irreducible polynomial has nonzero derivative. Since $T^{p^r}-x^{p^r}$ has only the root $x$, that remaining separable polynomial must be linear.

##### Purely inseparable polynomial over a rational function field

↑ **Parent:** [Minimal polynomial of a purely inseparable element](#minimal-polynomial-of-a-purely-inseparable-element)

Over $K=\mathbb F_p(t)$, the polynomial $X^p-t$ is irreducible by the [Eisenstein criterion](commutative-algebra.md#eisenstein-criterion) in $\mathbb F_p[t][X]$. In any extension containing a root $\alpha$, characteristic $p$ gives

$$
X^p-t=X^p-\alpha^p=(X-\alpha)^p.
$$

It therefore has exactly one distinct root, of multiplicity $p$.

### Unique embedding extension through a purely inseparable extension

↑ **Parent:** [Purely inseparable extension](#purely-inseparable-extension)

If $M/L$ is purely inseparable, an embedding of $L$ into an algebraic closure has at most one extension to $M$: if $x^{p^n}\in L$, the image of $x$ must be the unique $p^n$th root of the image of $x^{p^n}$. Existence in a normal overfield therefore implies uniqueness.

## Field automorphism

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Field_automorphism)

A field automorphism is a bijective [ring homomorphism](commutative-algebra.md#ring-homomorphism) from a [field](algebra.md#field) to itself. The automorphisms fixing a specified subfield form a [Galois group](#galois-group) when the extension is Galois.

### Field automorphism group

↑ **Parent:** [Field automorphism](#field-automorphism)

The field automorphism group fixing $K$ consists of all [field automorphisms](#field-automorphism) of $L$ fixing $K$ pointwise, with composition. It is defined without assuming that $L/K$ is Galois. For $L=K(\alpha)$ with algebraic degree $d$, the action on the roots of the [minimal polynomial](linear-operator-theory.md#minimal-polynomial) inside $L$ is faithful, so this group embeds in $S_d$ and is finite.

## Finite Galois extension

↑ **Parent:** [Galois theory](galois-theory.md)

A finite extension $L/K$ is Galois when it has $[L:K]$ automorphisms fixing $K$.

### Normal basis theorem

↑ **Parent:** [Finite Galois extension](#finite-galois-extension)

For a finite [Galois extension](#finite-galois-extension) $L/K$ with group $G$, there is $\theta\in L$ such that the elements $g(\theta)$ form a $K$-basis. Equivalently the additive $K[G]$-module $L$ is a regular representation. Over [p-adic fields](arithmetic.md#p-adic-field), its [p-adic lattices](arithmetic.md#integral-lattice-in-a-p-adic-vector-space) are thus commensurable with regular lattices; this is useful in [Herbrand quotient](group-theory.md#herbrand-quotient) calculations after applying a [p-adic logarithm](arithmetic.md#p-adic-logarithm) to deep [principal units](arithmetic.md#principal-unit).

### Galois group

↑ **Parent:** [Finite Galois extension](#finite-galois-extension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Galois_group)

The Galois group $\operatorname{Gal}(L/K)$ consists of the field automorphisms of $L$ that fix $K$ pointwise. For a finite Galois extension, its order is $[L:K]$.

### Normal and separable implies Galois

↑ **Parent:** [Finite Galois extension](#finite-galois-extension)

A separable extension has $[L:K]$ embeddings in an algebraic closure, and normality makes every one an automorphism of $L$. Hence a finite normal separable extension is Galois.

### Abelian extension

↑ **Parent:** [Finite Galois extension](#finite-galois-extension)

An abelian extension is a [Galois extension](#finite-galois-extension) whose [Galois group](#galois-group) is an [abelian group](group.md#abelian-group).

## Roots of unity in a finite field

↑ **Parent:** [Galois theory](galois-theory.md)

The multiplicative group $\mathbb F_q^\times$ is cyclic of order $q-1$, so it contains all $m$th roots of unity when $m$ divides $q-1$ and the characteristic does not divide $m$.

## Kummer extension of rational function fields

↑ **Parent:** [Galois theory](galois-theory.md)

If a field $k$ has characteristic prime to $m$ and contains all $m$th roots of unity, then $k(X)/k(X^m)$ is a cyclic Galois extension of degree $m$, with automorphisms $X\mapsto\zeta X$.

## Galois group of a polynomial

↑ **Parent:** [Galois theory](galois-theory.md)

The Galois group of a separable polynomial acts faithfully on its roots; this action is transitive exactly when the polynomial is irreducible.

### Unramified reduction of a polynomial Galois group

↑ **Parent:** [Galois group of a polynomial](#galois-group-of-a-polynomial)

Let $R$ be an integrally closed domain and $f\in R[X]$ monic, with [discriminant](polynomial.md#discriminant) outside a [prime ideal](commutative-algebra.md#prime-ideal) $P$. The roots stay distinct after reduction. In the splitting algebra choose a prime above $P$. Its [decomposition group](arithmetic.md#decomposition-group) maps onto the [Galois group](#galois-group) of the residue [splitting field](#splitting-field); its [inertia group](arithmetic.md#inertia-group) fixes every reduced root and is trivial because reduction bijects the distinct root sets. Thus the residue [Galois group](#galois-group) embeds in the generic group as a [permutation](combinatorics.md#permutation) group. For finite residue [fields](algebra.md#field), irreducible factor degrees give the [Frobenius cycle type](#frobenius-cycle-type).

### Transitivity lifted through unique pth roots

↑ **Parent:** [Galois group of a polynomial](#galois-group-of-a-polynomial)

Suppose a group of field automorphisms acts transitively on elements $y_i$, and each $y_i$ has a unique $p$th root $x_i$ in a stable extension. If every automorphism extends, it sends $x_i$ to the unique root above its image of $y_i$, so the extended group acts transitively on the $x_i$.

## Irreducible factors after Frobenius substitution

↑ **Parent:** [Galois theory](galois-theory.md)

Let $g\in K[T]$ be irreducible and separable in characteristic $p$, and put $f(T)=g(T^p)$. Every monic irreducible factor $h$ of $f$ is either $f$ itself or separable. Indeed, if $h$ were inseparable, then $h(T)=q(T^p)$; divisibility of $q(T^p)$ into $g(T^p)$ forces $q\mid g$, hence $q=g$ and $h=f$.

### Reducibility criterion after Frobenius substitution

↑ **Parent:** [Irreducible factors after Frobenius substitution](#irreducible-factors-after-frobenius-substitution)

Under the same hypotheses, $g(T^p)$ is reducible exactly when every coefficient of $g$ is a $p$th power in $K$. If $g=\sum a_i^pT^i$, then

$$
g(T^p)=\left(\sum a_iT^i\right)^p.
$$

Conversely, if $g(T^p)$ is reducible, all its irreducible factors are separable. Its zero derivative forces every factor multiplicity to be divisible by $p$, so it is a $p$th power in $K[T]$ and all its coefficients are $p$th powers.

## Frobenius cycle type

↑ **Parent:** [Galois theory](galois-theory.md)

Over $\mathbb F_q$, Frobenius acts on roots of an irreducible degree-$n$ polynomial as an $n$-cycle. Factor degrees therefore give its cycle type.

## Dedekind factorization cycle test

↑ **Parent:** [Galois theory](galois-theory.md)

At an unramified prime, the degrees of the irreducible factors of a polynomial modulo that prime give the cycle type of an element of the Galois group.

## Cyclotomic polynomial

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclotomic_polynomial)

$\Phi_n$ is the monic polynomial whose roots are the primitive $n$th roots of unity. It belongs to $\mathbb Z[X]$ and is irreducible over $\mathbb Q$.

### Cyclotomic reduction at a conductor prime

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)

For $a\ge1$ and $p\nmid m$, the identity $\Phi_{p^a m}(X)=\Phi_m(X^{p^a})/\Phi_m(X^{p^{a-1}})$ gives the displayed reduction, since taking a $p$th power equals substitution $X\mapsto X^p$ in characteristic $p$. The reduction of $\Phi_m$ is squarefree because it divides the [separable polynomial](#separable-polynomial) $X^m-1$. The [Kummer-Dedekind theorem](algebraic-number-theory.md#kummer-dedekind-theorem) therefore gives [ramification index of a prime ideal](algebraic-number-theory.md#ramification-index-of-a-prime-ideal) $\varphi(p^a)$ in the [cyclotomic field](#cyclotomic-field). In particular, a conductor factor $2$ occurring only to the first power has index one and creates no ramification by itself.

### Cyclotomic factorization

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)

Partitioning the roots of $X^n-1$ by their exact orders gives

$$
X^n-1=\prod_{d\mid n}\Phi_d(X).
$$

Inductively, the product over proper divisors is a [monic polynomial](polynomial.md#monic-polynomial) in $\mathbb Z[X]$. Division of $X^n-1$ by this monic polynomial stays in $\mathbb Z[X]$ and has zero remainder, proving that $\Phi_n\in\mathbb Z[X]$.

### Irreducibility of cyclotomic polynomials

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)

Every [cyclotomic polynomial](#cyclotomic-polynomial) $\Phi_n$ is an [irreducible polynomial](polynomial.md#irreducible-polynomial) over $\mathbb Q$. If a monic irreducible factor $f\in\mathbb Z[X]$ contains a primitive root $\zeta$, then it also contains $\zeta^p$ for every [prime number](number-theory.md#prime-number) $p\nmid n$: otherwise, writing $\Phi_n=fg$, reduction modulo $p$ and the [Frobenius endomorphism](#frobenius-endomorphism) give $\bar f\mid \bar g(X)^p$. Some irreducible factor would then divide both $\bar f$ and $\bar g$, giving a repeated factor of $X^n-1$, contrary to [separability of roots of unity](#separability-of-roots-of-unity). Iterating over the prime factors of every integer coprime to $n$ shows that $f$ contains all primitive $n$th roots, so $f=\Phi_n$.

### Thirtieth cyclotomic polynomial

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)

The thirtieth cyclotomic polynomial is

$$
\Phi_{30}(X)=X^8+X^7-X^5-X^4-X^3+X+1.
$$

Indeed,

$$
X^{10}-X^5+1=\Phi_6(X)\Phi_{30}(X),
\qquad \Phi_6(X)=X^2-X+1.
$$

### Separability of a cyclotomic polynomial modulo p

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)

If the prime $p$ does not divide $n$, then $X^n-1$ is square-free over $\mathbb F_p$ because its derivative $nX^{n-1}$ is coprime to it. Its factor $\Phi_n$ is therefore separable modulo $p$.

### Galois embedding for a cyclotomic polynomial

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)

If $L$ is the splitting field of $\Phi_n$ over a characteristic-zero field $K$, choosing a primitive root $\zeta_n$ gives an injection

$$
\operatorname{Gal}(L/K)\hookrightarrow(\mathbb Z/n\mathbb Z)^\times,
\qquad
\sigma(\zeta_n)=\zeta_n^{a_\sigma}.
$$

It is surjective exactly when $\Phi_n$ is irreducible over $K$.

### Cyclotomic field

↑ **Parent:** [Cyclotomic polynomial](#cyclotomic-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclotomic_field)

A cyclotomic field is generated by a root of unity. If $K\subseteq\mathbb C$ and $\zeta_n$ is primitive, every $K$-conjugate of $\zeta_n$ is a power $\zeta_n^a$ and already lies in $K(\zeta_n)$. Thus $K(\zeta_n)/K$ is Galois, and its Galois group embeds in $(\mathbb Z/n\mathbb Z)^\times$, so it is abelian.

#### Cyclotomic Artin reciprocity over the rational numbers

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

For the [cyclotomic field](#cyclotomic-field) $\mathbb Q(\zeta_n)$, arithmetic [Frobenius automorphisms](arithmetic.md#frobenius-automorphism) at primes $\ell\nmid n$ send $\zeta_n$ to $\zeta_n^\ell$: reduction distinguishes the nth [roots of unity](algebra.md#root-of-unity), and [Frobenius](arithmetic.md#frobenius-automorphism) raises residues to their $\ell$th powers. Multiplicativity therefore sends a [fractional ideal](commutative-algebra.md#fractional-ideal) with positive rational generator $a$, prime to $n$, to the exponent $a\bmod n$. Its [kernel](linear-algebra.md#kernel-of-a-linear-map) consists exactly of positive generators congruent to one modulo $n$. This proves [Artin reciprocity](algebraic-number-theory.md#artin-reciprocity-law) for the [ray class group](algebraic-number-theory.md#ray-class-group) of modulus $n\infty$ without assuming the general reciprocity theorem.

#### Cyclotomic unit

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

Cyclotomic units include roots of unity and suitable ratios $(1-\zeta^a)/(1-\zeta)$ in [cyclotomic fields](#cyclotomic-field). Compatible roots $\zeta$ make these ratios norm-compatible along cyclotomic towers. Their closed norm-limit module is a concrete submodule of global units, and its local images generate the power series in the [Iwasawa main conjecture](algebraic-number-theory.md#main-conjecture-of-iwasawa-theory).

##### Reduction of cyclotomic units at the ramified prime

↑ **Parent:** [Cyclotomic unit](#cyclotomic-unit)

For $1\le k<p$, choose $l$ with $kl\equiv1\pmod p$. The geometric sum $1+\zeta_p^k+\cdots+\zeta_p^{k(l-1)}$ is the inverse of $u_k$. Hence these are units, and their residues cover $\mathbb F_p^\times$. In the [cyclotomic Milnor square](algebra.md#cyclotomic-milnor-square), this makes the $K_1$ map onto the common [field](algebra.md#field) surjective and eliminates its connecting obstruction to $K_0$.

##### Cyclotomic unit index formula

↑ **Parent:** [Cyclotomic unit](#cyclotomic-unit)

For a real cyclotomic field of odd prime-power conductor, the index of its cyclotomic-unit group has the same p-part as its ideal class number. The [analytic class number formula](algebraic-number-theory.md#analytic-class-number-formula) compares the regulator of all units with the explicit cyclotomic-unit regulator. The equality here is stated at the p-part level, so harmless prime-to-p normalization factors do not affect it.

##### Symmetric cyclotomic unit

↑ **Parent:** [Cyclotomic unit](#cyclotomic-unit)

Half exponents mean the inverse of two in the odd-order root-of-unity group. For $p\nmid ab$, the ratio is a real global unit and is compatible under the norms in the p-power tower. Its [Coleman power series](algebraic-number-theory.md#coleman-power-series) is $(1+T)^{(b-a)/2}(1-(1+T)^a)/(1-(1+T)^b)$, with constant term $a/b$. Its [higher logarithmic derivatives](algebraic-number-theory.md#cyclotomic-higher-logarithmic-derivative) vanish at odd indices and equal $(a^k-b^k)B_k/k$ at even indices, using $B_1=-1/2$.

##### Cyclotomic Euler system

↑ **Parent:** [Cyclotomic unit](#cyclotomic-unit)

A cyclotomic Euler system consists of units in auxiliary cyclotomic extensions satisfying compatible norm relations. Reducing at carefully chosen auxiliary primes and descending these relations bounds class-group modules. Combined with global unit-index formulas, this supplies an alternative route to the [Iwasawa main conjecture](algebraic-number-theory.md#main-conjecture-of-iwasawa-theory).

###### Root-of-unity Euler system

↑ **Parent:** [Cyclotomic Euler system](#cyclotomic-euler-system)

Fix a finite excluded set $S$ containing two, and let $W_S$ contain the [roots of unity](algebra.md#root-of-unity) of orders coprime to every prime in $S$. A root-of-unity Euler system is a nonzero algebraic-valued function $\Phi$ on $W_S$ that is even and Galois equivariant, satisfies $\prod_{\rho^q=1}\Phi(\rho\zeta)=\Phi(\zeta^q)$ for $q\notin S$, and satisfies $\Phi(\rho\zeta)\equiv\Phi(\zeta)\pmod{\mathfrak q}$ when the order of $\zeta$ is prime to $q$, for every prime $\mathfrak q$ over $q$. Values are required to be locally integral units where the congruence is used. These distribution and congruence properties provide auxiliary cyclotomic extensions, beyond a single norm-compatible p-power sequence.

###### Cyclotomic Euler norm factor at a new prime

↑ **Parent:** [Root-of-unity Euler system](#root-of-unity-euler-system)

Let $q\nmid m$ be outside the excluded primes, let $\zeta$ have order $m$, and let $\rho$ be a primitive qth [root of unity](algebra.md#root-of-unity). Galois equivariance identifies the conjugates with $\Phi(\rho^i\zeta)$ for $1\leq i\leq q-1$. The distribution axiom includes the missing $i=0$ factor, so the [field norm](algebraic-number-theory.md#field-norm) is $\Phi(\zeta^q)/\Phi(\zeta)$. Arithmetic [Frobenius](arithmetic.md#frobenius-automorphism) sends $\zeta$ to $\zeta^q$, giving the displayed factor. At higher powers of an already ramified prime all q translates occur instead. These are different norm relations; norm compatibility in just a p-power tower does not supply the auxiliary-prime relation by itself.

###### Kolyvagin derivative operator for a cyclic group

↑ **Parent:** [Root-of-unity Euler system](#root-of-unity-euler-system)

For a cyclic [group](group.md) of order $m$ with generator $\sigma$, let $N=\sum_{i=0}^{m-1}\sigma^i$. Subtracting adjacent coefficients and using $\sigma^m=1$ proves the displayed group-ring identity. If $p^r\mid m$, then $(\sigma-1)D\equiv-N\pmod{p^r}$. Together with the norm relations of a [root-of-unity Euler system](#root-of-unity-euler-system), this makes derivative classes invariant modulo p-power powers and permits Kummer descent, with roots-of-unity corrections where necessary. The congruence axiom controls the associated residue and valuation maps.

###### Euler-system divisibility for real cyclotomic class modules

↑ **Parent:** [Root-of-unity Euler system](#root-of-unity-euler-system)

The divisibility is between generators of characteristic ideals. Auxiliary-prime derivative operators applied to a [root-of-unity Euler system](#root-of-unity-euler-system) produce Kummer classes with controlled valuations. The congruence axiom identifies the valuation at a new auxiliary prime with a residue symbol of the preceding class. The [Chebotarev density theorem](algebraic-number-theory.md#chebotarev-density-theorem) chooses prime representatives of desired ideal classes, and iterating bounds their elementary divisors by the index of the cyclotomic unit. Passing to the norm tower gives the displayed divisibility, with finite errors removed at height-one primes. The reverse divisibility requires the global index and norm-defect comparison.

#### Nonprincipal cyclotomic fields of conductor a prime power

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

Every field $\mathbb Q(\zeta_{59^r})$ contains $\mathbb Q(\sqrt{-59})$ and is totally ramified over it at the prime above $59$. The [class number divisibility under total ramification](algebraic-number-theory.md#class-number-divisibility-under-total-ramification) therefore shows that its [class number](algebraic-number-theory.md#class-number) is divisible by three. Its ring of integers is not a [principal ideal domain](commutative-algebra.md#principal-ideal-domain). The degrees $58\cdot59^{r-1}$ strictly increase, giving infinitely many distinct examples.

#### Total ramification in a prime-power cyclotomic field

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

The prime $\ell$ is totally ramified in $\mathbb Q(\zeta_{\ell^r})$, whose degree is $\varphi(\ell^r)$. The displayed equality is an equality of ideals in its [ring of integers of a number field](algebraic-number-theory.md#ring-of-integers), and the residue field is $\mathbb F_\ell$.

#### Quadratic subfield of a prime cyclotomic field

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

For an odd prime $\ell$, the unique quadratic subfield of $\mathbb Q(\zeta_\ell)$ is the displayed field. A quadratic Gauss sum squares to $(-1)^{(\ell-1)/2}\ell$, and the cyclic [Galois group](#galois-group) has a unique subgroup of index two.

#### Prime cyclotomic field degree

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

For a prime $p$, the [cyclotomic polynomial](#cyclotomic-polynomial) of a primitive $p$th root of unity is

$$
\Phi_p(X)=1+X+\cdots+X^{p-1}.
$$

It is irreducible over $\mathbb Q$, so adjoining one root gives a field of degree $p-1$.

##### Discriminant of a prime cyclotomic power basis

↑ **Parent:** [Prime cyclotomic field degree](#prime-cyclotomic-field-degree)

For an odd prime $p$ and a primitive $p$th root $\zeta_p$,

$$
\operatorname{disc}(1,\zeta_p,\ldots,\zeta_p^{p-2})
=(-1)^{(p-1)/2}p^{p-2}.
$$

#### Maximal real subfield of the fifth cyclotomic field

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

For a primitive fifth root $\zeta_5$, the element $s=\zeta_5+\zeta_5^{-1}$ satisfies $s^2+s-1=0$. Thus the fixed field of complex conjugation is

$$
\mathbb Q(s)=\mathbb Q(\sqrt5).
$$

#### Roots of unity in a rational cyclotomic field

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

The roots of unity in $\mathbb Q(\zeta_n)$ form a cyclic group of order

$$
\operatorname{lcm}(2,n)=
\begin{cases}
n,&n\text{ even},\\
2n,&n\text{ odd}.
\end{cases}
$$

#### Seventh cyclotomic field

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

For a primitive seventh root of unity $\zeta_7$,

$$
\operatorname{Gal}(\mathbb Q(\zeta_7)/\mathbb Q)
\cong(\mathbb Z/7\mathbb Z)^\times\cong C_6,
$$

where $\sigma_a(\zeta_7)=\zeta_7^a$. Its four intermediate fields correspond to the four subgroups of the cyclic group $C_6$.

##### Quadratic Gaussian period in the seventh cyclotomic field

↑ **Parent:** [Seventh cyclotomic field](#seventh-cyclotomic-field)

The unique quadratic subfield of $\mathbb Q(\zeta_7)$ is

$$
\mathbb Q(\eta)=\mathbb Q(\sqrt{-7}),
\qquad
\eta=\frac{-1+\sqrt{-7}}2.
$$

The conjugate period is $-1-\eta$, and

$$
m_{\eta,\mathbb Q}(X)=X^2+X+2.
$$

##### Real cubic subfield of the seventh cyclotomic field

↑ **Parent:** [Seventh cyclotomic field](#seventh-cyclotomic-field)

The unique cubic subfield is the maximal real subfield

$$
\mathbb Q(\theta),
\qquad
\theta=\zeta_7+\zeta_7^{-1},
$$

and

$$
m_{\theta,\mathbb Q}(X)=X^3+X^2-2X-1.
$$

It is the fixed field of complex conjugation.

#### Eleventh cyclotomic field

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

The Galois group of $\mathbb Q(\zeta_{11})/\mathbb Q$ is

$$
(\mathbb Z/11\mathbb Z)^\times\cong C_{10}.
$$

Its only subfield degrees over $\mathbb Q$ are $1,2,5,10$, and every subfield is Galois because this group is abelian.

##### Quadratic Gaussian period in the eleventh cyclotomic field

↑ **Parent:** [Eleventh cyclotomic field](#eleventh-cyclotomic-field)

The unique quadratic subfield of $\mathbb Q(\zeta_{11})$ is

$$
\mathbb Q(\eta)=\mathbb Q(\sqrt{-11}),
\qquad
\eta=\frac{-1+\sqrt{-11}}2.
$$

##### Maximal real subfield of the eleventh cyclotomic field

↑ **Parent:** [Eleventh cyclotomic field](#eleventh-cyclotomic-field)

The fixed field of complex conjugation in $\mathbb Q(\zeta_{11})$ is the degree-five field $\mathbb Q(\zeta_{11}+\zeta_{11}^{-1})$.

#### Maximal cyclotomic extension

↑ **Parent:** [Cyclotomic field](#cyclotomic-field)

For a field $K$ inside a fixed algebraic closure, the maximal cyclotomic extension is the union of the fields $K(\zeta_n)$ generated by roots of unity.

##### Maximal cyclotomic extension of the real numbers

↑ **Parent:** [Maximal cyclotomic extension](#maximal-cyclotomic-extension)

The maximal cyclotomic extension of $\mathbb R$ is $\mathbb C$, since adjoining a primitive fourth root of unity adjoins $i$.

##### Maximal cyclotomic extension of the rational numbers

↑ **Parent:** [Maximal cyclotomic extension](#maximal-cyclotomic-extension)

The maximal cyclotomic extension of $\mathbb Q$ is a proper subfield of $\overline{\mathbb Q}$. Every finite subextension inside a cyclotomic field is Galois and abelian, whereas $\mathbb Q(\sqrt[3]{2})/\mathbb Q$ is not normal.

##### Maximal cyclotomic extension of a finite field

↑ **Parent:** [Maximal cyclotomic extension](#maximal-cyclotomic-extension)

The maximal cyclotomic extension of $\mathbb F_p$ is $\overline{\mathbb F}_p$. A primitive $(p^m-1)$th root of unity generates $\mathbb F_{p^m}$ over $\mathbb F_p$, and these finite fields exhaust the algebraic closure.

## Constructible number

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Constructible_number)

A constructible number is the coordinate of a point obtainable from rational starting data by straightedge-and-compass constructions.

### Constructible field extension

↑ **Parent:** [Constructible number](#constructible-number)

A finite real extension $K/\mathbb Q$ is constructible when it is contained in a tower

$$
\mathbb Q=K_0\subset K_1\subset\cdots\subset K_r,
\qquad [K_i:K_{i-1}]=2.
$$

Equivalently, every element of $K$ can be obtained from rational numbers by field operations and successive square roots.

#### Constructibility of the real seventeenth cyclotomic field

↑ **Parent:** [Constructible field extension](#constructible-field-extension)

The real cyclotomic field

$$
\mathbb Q(\zeta_{17}+\zeta_{17}^{-1})
$$

is Galois of degree eight with cyclic Galois group $(\mathbb Z/17\mathbb Z)^\times/\{\mathord\pm1\}$. A subgroup chain of successive index two gives a tower of three quadratic extensions, proving that $\cos(2\pi/17)$ is constructible.

## Fixed field

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fixed_field)

For a group $G$ of automorphisms of a field $L$, the fixed field is

$$
L^G=\{x\in L:g(x)=x\text{ for every }g\in G\}.
$$

For one automorphism $\sigma$, it is also written $L^\sigma$.

### Dihedral fixed field in one rational variable

↑ **Parent:** [Fixed field](#fixed-field)

Automorphisms $\sigma(z)=\zeta_nz$ and $\tau(z)=1/z$ generate a [dihedral group](finite-group-theory.md#dihedral-group) of order $2n$. The invariant $w=z^n+z^{-n}$ has rational map degree $2n$, so $[\mathbb C(z):\mathbb C(w)]=2n$. The fixed-field theorem for a finite automorphism group gives the same degree over its [fixed field](#fixed-field), proving equality. For odd prime $n$, the nontrivial proper subgroups are the rotation group and the $n$ reflection groups. Their fixed fields are $\mathbb C(z^n)$ and $\mathbb C(z+\zeta_n^{-j}/z)$ for reflections $\sigma^j\tau$, respectively.

### Dihedral fixed field of a two-variable rational function field

↑ **Parent:** [Fixed field](#fixed-field)

On $K=\mathbb Q(x,y)$, let $\sigma(x,y)=(y,-x)$ and $\tau(x,y)=(x,-y)$. They generate a [dihedral group](finite-group-theory.md#dihedral-group) of order eight, and

$$
K^{\langle\sigma,\tau\rangle}
=\mathbb Q(x^2+y^2,x^2y^2).
$$

The inclusion from right to left is immediate. In the other direction, $x^2,y^2$ solve a quadratic over the displayed field and adjoining their square roots has degree at most four; the resulting total degree is at most eight, while the [automorphism-count bound for a finite field extension](#automorphism-count-bound-for-a-finite-field-extension) gives the reverse bound.

## Artin fixed-field theorem

↑ **Parent:** [Galois theory](galois-theory.md)

If a finite group $G$ acts faithfully by automorphisms on a field $L$, then $L/L^G$ is Galois, has degree $|G|$, and has Galois group $G$.

This theorem constructs a [Galois extension](#finite-galois-extension) from a finite group of field automorphisms; it is not an alternative name for the extension itself.

### Orbit polynomial under a finite automorphism group

↑ **Parent:** [Artin fixed-field theorem](#artin-fixed-field-theorem)

For $\alpha\in L$ and a finite automorphism group $G$, the polynomial

$$
f(t,\alpha)=\prod_{g\in G}(t-g(\alpha))
$$

has coefficients in the [fixed field](#fixed-field) $L^G$, because every element of $G$ permutes its factors.

#### Coefficients of an orbit polynomial for a primitive generator

↑ **Parent:** [Orbit polynomial under a finite automorphism group](#orbit-polynomial-under-a-finite-automorphism-group)

If $K\subseteq L^G$ and $L=K(\alpha)$, then the coefficients of $f(t,\alpha)$ generate $L^G$ over $K$. Indeed, for the field $E$ generated by those coefficients, $L=E(\alpha)$ and $[L:E]\leq|G|$, while the [Artin fixed-field theorem](#artin-fixed-field-theorem) gives $[L:L^G]=|G|$.

#### Separate orbit polynomials can miss mixed invariants

↑ **Parent:** [Orbit polynomial under a finite automorphism group](#orbit-polynomial-under-a-finite-automorphism-group)

Let $L=K(\sqrt{a_1},\sqrt{a_2})$ with independent square classes and characteristic different from two, and let $G$ be generated by the automorphism negating both square roots. The two orbit polynomials are $t^2-a_1$ and $t^2-a_2$, so their coefficients generate only $K$, whereas

$$
L^G=K(\sqrt{a_1a_2}).
$$

## Galois correspondence

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Galois_correspondence)

For a finite Galois extension, subgroups correspond in reverse order to intermediate fields by taking fixed fields and field-fixing subgroups.

### Normal subextension criterion

↑ **Parent:** [Galois correspondence](#galois-correspondence)

For a finite Galois extension $L/K$ with group $G$, an intermediate extension $E/K$ is normal exactly when its corresponding subgroup $\operatorname{Gal}(L/E)$ is a [normal subgroup](group-theory.md#normal-subgroup) of $G$.

### Subextensions of an abelian Galois extension

↑ **Parent:** [Galois correspondence](#galois-correspondence)

Every subgroup of an abelian group is normal. Hence every intermediate field of a finite abelian Galois extension is itself Galois over the base field.

#### Cyclic Galois extension of the rational numbers of every finite degree

↑ **Parent:** [Subextensions of an abelian Galois extension](#subextensions-of-an-abelian-galois-extension)

For $r>1$, choose a prime $\ell\equiv1\pmod r$ by Dirichlet's theorem. The cyclic group

$$
\operatorname{Gal}(\mathbb Q(\zeta_\ell)/\mathbb Q)
\cong C_{\ell-1}
$$

has a subgroup of index $r$, whose fixed field is cyclic Galois of degree $r$ over $\mathbb Q$.

#### Finite extensions of the fixed field of a finite-order automorphism of an algebraically closed field

↑ **Parent:** [Subextensions of an abelian Galois extension](#subextensions-of-an-abelian-galois-extension)

Let an automorphism $\sigma$ of an algebraically closed field $L$ have finite order and fixed field $K$. Artin's fixed-field theorem makes $L/K$ finite cyclic Galois. Every finite extension $M/K$ embeds in $L$: in characteristic zero, choose a primitive generator and send it to a root in $L$. Its image is an intermediate field of a cyclic extension and is therefore Galois and cyclic over $K$.

### Subfields of the splitting field of x to the fourth minus seven

↑ **Parent:** [Galois correspondence](#galois-correspondence)

Put $\alpha=\sqrt[4]{7}$ and $L=\mathbb Q(\alpha,i)$. The [dihedral group](finite-group-theory.md#dihedral-group) $D_8=\langle r,s:r^4=s^2=1,\ srs=r^{-1}\rangle$ acts by

$$
r(\alpha)=i\alpha,\quad r(i)=i,\qquad
s(\alpha)=\alpha,\quad s(i)=-i.
$$

The ten subgroups and their fixed fields are

$$
\begin{array}{c|c}
D_8&\mathbb Q\\
\langle r\rangle&\mathbb Q(i)\\
\langle r^2,s\rangle&\mathbb Q(\sqrt7)\\
\langle r^2,rs\rangle&\mathbb Q(\sqrt{-7})\\
\langle r^2\rangle&\mathbb Q(\sqrt7,i)\\
\langle s\rangle&\mathbb Q(\alpha)\\
\langle r^2s\rangle&\mathbb Q(i\alpha)\\
\langle rs\rangle&\mathbb Q((1+i)\alpha)\\
\langle r^3s\rangle&\mathbb Q((1-i)\alpha)\\
\{1\}&L.
\end{array}
$$

The normal subgroups are $D_8$, $\langle r\rangle$, the two displayed Klein four-groups, $\langle r^2\rangle$, and $\{1\}$.

## Polynomial discriminant

↑ **Parent:** [Galois theory](galois-theory.md)

For a monic polynomial with roots $r_i$, its [discriminant](polynomial.md#discriminant) is $\prod_{i<j}(r_i-r_j)^2$ and vanishes exactly for a repeated root.

### Squarefree polynomial discriminant does not imply irreducibility

↑ **Parent:** [Polynomial discriminant](#polynomial-discriminant)

A squarefree [polynomial discriminant](#polynomial-discriminant) does not ensure that the polynomial defines a field of its stated degree. For example, $x^3-2x-1=(x+1)(x^2-x-1)$ has [discriminant](polynomial.md#discriminant) five. Its roots have degrees one or two, so no root generates a cubic [number field](algebraic-number-theory.md#number-field). In particular $1,\alpha,\alpha^2$ cannot be a field [basis](vector-space.md#basis) for any of its roots. The [squarefree discriminant certifies an integral basis](algebraic-number-theory.md#squarefree-discriminant-certifies-an-integral-basis) argument assumes that the polynomial is the minimal polynomial: then the [discriminant](polynomial.md#discriminant) of its power [basis](vector-space.md#basis) is the [field discriminant](algebraic-number-theory.md#field-discriminant) times the square of the order index. For a reducible squarefree polynomial the analogous rank belongs instead to its quotient algebra, which is a product of fields, not to one root field.

### Cubic resolvent of a quartic

↑ **Parent:** [Polynomial discriminant](#polynomial-discriminant)

For a depressed quartic $x^4+px^2+qx+r$ with roots $\alpha_1,\ldots,\alpha_4$, the three pair-partition quantities $\alpha_1\alpha_2+\alpha_3\alpha_4$ and its two analogues are the roots of

$$
y^3-py^2-4ry+(4pr-q^2).
$$

The Galois action on these roots is the quotient of its action on the four quartic roots by the [Klein four-group](finite-group-theory.md#klein-four-group).

#### S4 criterion from the cubic resolvent of an irreducible quartic

↑ **Parent:** [Cubic resolvent of a quartic](#cubic-resolvent-of-a-quartic)

If an irreducible quartic over a field of characteristic zero has a [cubic resolvent of a quartic](#cubic-resolvent-of-a-quartic) whose [Galois group of a polynomial](#galois-group-of-a-polynomial) is $S_3$, then the quartic has Galois group $S_4$. Irreducibility places the quartic group among the [transitive subgroups of the symmetric group on four points](#transitive-subgroups-of-the-symmetric-group-on-four-points), while the action on its three root pairings is surjective onto $S_3$. Of the possibilities $C_4,V_4,D_8,A_4,S_4$, only $S_4$ has this image.

### Vandermonde determinant

↑ **Parent:** [Polynomial discriminant](#polynomial-discriminant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vandermonde_determinant)

The Vandermonde product $\prod_{i<j}(r_i-r_j)$ is alternating, and its square is the discriminant of the monic polynomial with roots $r_i$.

#### Weighted Vandermonde determinant

↑ **Parent:** [Vandermonde determinant](#vandermonde-determinant)

For a nonnegative weight $w$ and [monic polynomials](polynomial.md#monic-polynomial) $p_j$ of degree $j$, this [determinant](linear-algebra.md#determinant) is $\prod_i\sqrt{w(x_i)}\prod_{i<j}(x_j-x_i)$. Its square is the product of the weights times the squared [Vandermonde determinant](#vandermonde-determinant). For normalized weighted [polynomials](polynomial.md) it differs by the product of their norm factors.

#### Vandermonde determinant invariance under monic basis change

↑ **Parent:** [Vandermonde determinant](#vandermonde-determinant)

Evaluating arbitrary [monic polynomials](polynomial.md#monic-polynomial) of successive degrees $0,\ldots,m-1$ gives the same [determinant](linear-algebra.md#determinant) as evaluating the monomials of those degrees. The basis-change [matrix](vector-space.md#matrix) is triangular with diagonal entries one, so its [determinant](linear-algebra.md#determinant) is one. This permits an [orthogonal polynomial](numerical-analysis.md#orthogonal-polynomial) basis to replace the monomials in [eigenvalue](linear-operator-theory.md#eigenvalue) densities.

#### Vandermonde shift identity

↑ **Parent:** [Vandermonde determinant](#vandermonde-determinant)

The left side is an [alternating polynomial](polynomial.md#alternating-polynomial) of total degree one more than $\Delta(x)$. Dividing by the [Vandermonde determinant](#vandermonde-determinant) gives a symmetric homogeneous [polynomial](polynomial.md) of degree one, necessarily $a\sum_i x_i+bt$. At $t=0$, $a=1$; differentiation in $t$ and the [Euler theorem for homogeneous functions](real-analysis.md#euler-theorem-for-homogeneous-functions) give $b=\binom m2$. Thus the identity holds as a [polynomial](polynomial.md) identity, even at repeated coordinates. At shifted partition coordinates with $t=-1$, it proves the removable-corner recurrence in the [hook-length formula](representation-theory-of-the-symmetric-group.md#hook-length-formula).

#### Leading coefficient of an exponential alternant

↑ **Parent:** [Vandermonde determinant](#vandermonde-determinant)

For distinct $\ell_i$ and $c_j$, expand the exponential entries in powers of $t$. Nonzero [determinant](linear-algebra.md#determinant) terms first occur at the distinct powers $0,1,\ldots,m-1$. The coefficient is the product of their two [Vandermonde determinants](#vandermonde-determinant) divided by the factorial product. Ratios of such alternants yield the [Weyl dimension formula](semisimple-lie-algebra.md#weyl-dimension-formula) by taking a torus [character](representation-theory.md#character-of-a-representation) to the identity.

#### Vandermonde matrix

↑ **Parent:** [Vandermonde determinant](#vandermonde-determinant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vandermonde_matrix)

A Vandermonde matrix has entries $V_{ij}=\lambda_i^{j-1}$. Distinct nodes give determinant $\prod_{i<j}(\lambda_j-\lambda_i)\ne0$, explaining independence of polynomial evaluations and distinct-eigenvalue [Krylov subspaces](numerical-analysis.md#krylov-subspace).

##### Zero power sums force a finite complex multiset to vanish

↑ **Parent:** [Vandermonde matrix](#vandermonde-matrix)

Collect the distinct nonzero values among the $\lambda_j$ as $\mu_1,\ldots,\mu_r$ with positive multiplicities $m_j$. The first $r$ power sums imply $\sum_jm_j\mu_j^k=0$ for $1\le k\le r$. The coefficient matrix is an invertible weighted [Vandermonde matrix](#vandermonde-matrix), so all $m_j$ vanish, a contradiction unless $r=0$. Its invertibility also follows because a [polynomial](polynomial.md) $\sum_{k=1}^r a_kz^k$ vanishing at zero and all the $\mu_j$ has $r+1$ distinct roots and degree at most $r$.

### Discriminant of a depressed cubic

↑ **Parent:** [Polynomial discriminant](#polynomial-discriminant)

The depressed cubic $x^3+ax+b$ has discriminant $-4a^3-27b^2$.

### Discriminant criterion for an alternating Galois group

↑ **Parent:** [Polynomial discriminant](#polynomial-discriminant)

For a monic separable polynomial over a field of characteristic other than two, its Galois group is contained in the alternating group exactly when its discriminant is a square in the base field. The Galois action multiplies the Vandermonde product by the sign of the induced root permutation.

## Resolvent (Galois theory)

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Resolvent_(Galois_theory))

A [resolvent](#resolvent-galois-theory) is an auxiliary polynomial built from expressions in the roots of a polynomial. The action of its [Galois group](#galois-group) on those expressions gives information about solvability and intermediate field extensions. A [Lagrange resolvent for a cubic](#lagrange-resolvent-for-a-cubic) uses Fourier combinations of the three roots.

### Lagrange resolvent for a cubic

↑ **Parent:** [Resolvent (Galois theory)](#resolvent-galois-theory)

For cubic roots $\alpha_i$ and a cube root of unity $\omega$, the Fourier combinations $u=\alpha_1+\omega\alpha_2+\omega^2\alpha_3$ and $v$ have cubes satisfying a quadratic resolvent.

#### Cubic resolvent

↑ **Parent:** [Lagrange resolvent for a cubic](#lagrange-resolvent-for-a-cubic)

For $x^3+ax+b$, the Lagrange-resolvent cubes are roots of $X^2+27bX-27a^3$.

##### Cardano formula

↑ **Parent:** [Cubic resolvent](#cubic-resolvent)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cardano_formula)

Cardano's formula solves a depressed cubic by taking square roots in its quadratic resolvent and then compatible cube roots.

## Solvability by radicals

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solvability_by_radicals)

A polynomial is solvable by radicals when its roots lie in a tower obtained by adjoining successive roots; equivalently, its Galois group is solvable.

## Galois group of an irreducible cubic

↑ **Parent:** [Galois theory](galois-theory.md)

An irreducible cubic over a field of characteristic other than two has Galois group $A_3$ when its discriminant is a square and $S_3$ otherwise.

### Quadratic resolvent field of a cubic

↑ **Parent:** [Galois group of an irreducible cubic](#galois-group-of-an-irreducible-cubic)

If a separable cubic has [polynomial discriminant](#polynomial-discriminant) $\Delta$, then adjoining $\sqrt\Delta$ gives the subfield fixed by the alternating part of its Galois group. When the cubic Galois group is $S_3$, this is its unique quadratic subfield.

### Splitting field of x cubed minus x minus one

↑ **Parent:** [Galois group of an irreducible cubic](#galois-group-of-an-irreducible-cubic)

The polynomial $X^3-X-1$ is irreducible over $\mathbb Q$ and has discriminant $-23$, so its splitting field has Galois group $S_3$. Its unique quadratic subfield is the fixed field of $A_3$, namely $\mathbb Q(\sqrt{-23})$.

### Cubic discriminant criterion

↑ **Parent:** [Galois group of an irreducible cubic](#galois-group-of-an-irreducible-cubic)

The discriminant square class detects whether the transitive cubic Galois group lies in the alternating group.

## Characteristic-two cubic resolvent

↑ **Parent:** [Galois theory](galois-theory.md)

Let $x_1,x_2,x_3$ be the roots of the separable polynomial $T^3+aT+b$ in characteristic two. The cyclic sums

$$
r=x_1^2x_2+x_2^2x_3+x_3^2x_1,
\qquad
s=x_2^2x_1+x_3^2x_2+x_1^2x_3
$$

are the distinct roots of

$$
T^2+bT+a^3+b^2.
$$

Even root permutations fix $r,s$, while odd permutations interchange them. The cubic Galois group is therefore contained in $A_3$ exactly when this quadratic splits over the base field.

<h2 id="artin-schreier-theory">Artin–Schreier theory</h2>

↑ **Parent:** [Galois theory](galois-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Artin–Schreier_theory)

[Artin–Schreier theory](#artin-schreier-theory) describes cyclic extensions of prime degree $p$ in [characteristic](algebra.md#characteristic-of-a-field) $p$ using equations $x^p-x=a$.

### Artin-Schreier embedding problems over a characteristic-p field

↑ **Parent:** [Artin–Schreier theory](#artin-schreier-theory)

For a [field](algebra.md#field) $F$ of characteristic $p$, the [exact sequence](homology.md#exact-sequence) $0\to\mathbb F_p\to F^{\mathrm{sep}}\xrightarrow{z\mapsto z^p-z}F^{\mathrm{sep}}\to0$, together with additive normal-basis acyclicity, gives $H^2(\operatorname{Gal}(F^{\mathrm{sep}}/F),\mathbb F_p)=0$. Consequently every central finite embedding problem with [group homomorphism kernel](group-theory.md#kernel-of-a-group-homomorphism) $C_p$ has a continuous weak solution: its pulled-back [two-cocycle](group-theory.md#two-cocycle) is a [coboundary](algebra.md#coboundary), whose correcting one-cochain supplies the lift. Over $\mathbb F_p((t))$, independent Artin–Schreier classes $t^{-m}$, with $m>0$ prime to $p$, allow the lift to be twisted by characters so that inertia maps onto the [group homomorphism kernel](group-theory.md#kernel-of-a-group-homomorphism) as well as onto the original quotient. Induction through central order-$p$ quotients therefore realizes every [finite p-group](finite-group-theory.md#finite-p-group) as the [Galois group](#galois-group) of a [totally ramified extension](arithmetic.md#totally-ramified-extension) with [residue field](commutative-algebra.md#residue-field) $\mathbb F_p$.

<h3 id="artin-schreier-polynomial">Artin–Schreier polynomial</h3>

↑ **Parent:** [Artin–Schreier theory](#artin-schreier-theory)

An Artin–Schreier polynomial over a field of characteristic $p$ has the form

$$
X^p-X-a.
$$

If it has one root $\alpha$, all its roots are $\alpha+c$ for $c\in\mathbb F_p$. It either has a root in the base field and splits completely, or is an [irreducible polynomial](polynomial.md#irreducible-polynomial) of degree $p$.

<h3 id="artin-schreier-extension">Artin–Schreier extension</h3>

↑ **Parent:** [Artin–Schreier theory](#artin-schreier-theory)

An Artin–Schreier extension is a field extension generated by a root $\alpha$ of an irreducible [Artin–Schreier polynomial](#artin-schreier-polynomial). It is a cyclic [Galois extension](#finite-galois-extension) of degree $p$, with automorphisms $\alpha\mapsto\alpha+c$ for $c\in\mathbb F_p$.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-3.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-2.md#1/solution)
