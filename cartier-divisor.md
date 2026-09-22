# Cartier divisor

↑ **Parent:** [Algebraic geometry](algebraic-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartier_divisor)

A Cartier divisor is locally represented by nonzero rational functions whose ratios on overlaps are regular units. It is principal when one global rational function represents all local data.

**Table of contents**

- [Pullback of a Cartier divisor](#pullback-of-a-cartier-divisor)
- [Cartier divisor exact sequence for an integral domain](#cartier-divisor-exact-sequence-for-an-integral-domain)
- [Divisor line bundle](#divisor-line-bundle)
- [Real Cartier divisor](#real-cartier-divisor)
  - [Ample real divisor](#ample-real-divisor)
  - [Real linear equivalence of divisors](#real-linear-equivalence-of-divisors)
- [Positivity of divisors](#positivity-of-divisors)
  - [Semiample divisor](#semiample-divisor)
    - [Semiampleness of a square-zero rational curve](#semiampleness-of-a-square-zero-rational-curve)
    - [Semiample and curve-positive ampleness criterion](#semiample-and-curve-positive-ampleness-criterion)
    - [Restriction ampleness implies semiampleness for an effective divisor](#restriction-ampleness-implies-semiampleness-for-an-effective-divisor)
  - [Big divisor](#big-divisor)
    - [Algebraic Morse inequality for ample divisors](#algebraic-morse-inequality-for-ample-divisors)
    - [Bigness under finite normalization](#bigness-under-finite-normalization)
    - [Big real divisor](#big-real-divisor)
      - [Negative curves of a big real divisor lie in finitely many divisors](#negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors)
        - [Uniform ample subtraction from a big divisor with ample exceptional restrictions](#uniform-ample-subtraction-from-a-big-divisor-with-ample-exceptional-restrictions)
      - [Componentwise bigness on a projective scheme](#componentwise-bigness-on-a-projective-scheme)
      - [Rational approximation of an ample-plus-effective real divisor](#rational-approximation-of-an-ample-plus-effective-real-divisor)
      - [Big cone](#big-cone)
    - [Birational linear system criterion for bigness](#birational-linear-system-criterion-for-bigness)
    - [Kodaira's lemma](#kodaira-s-lemma)
    - [Section subtraction lemma for big divisors](#section-subtraction-lemma-for-big-divisors)
  - [Numerical equivalence of divisors](#numerical-equivalence-of-divisors)
    - [Real numerical divisor classes](#real-numerical-divisor-classes)
      - [Nef cone](#nef-cone)
        - [Ample cone](#ample-cone)
          - [Nef-plus-ample ampleness lemma](#nef-plus-ample-ampleness-lemma)
      - [Closed cone of curves](#closed-cone-of-curves)
  - [Nef line bundle](#nef-line-bundle)
    - [Volume of a nef divisor](#volume-of-a-nef-divisor)
  - [Ample Cartier divisor](#ample-cartier-divisor)
    - [Toric ampleness criterion](#toric-ampleness-criterion)
    - [Vanishing-section ampleness criterion](#vanishing-section-ampleness-criterion)
    - [Euler-characteristic ampleness criterion](#euler-characteristic-ampleness-criterion)
    - [Kleiman's criterion](#kleiman-s-criterion)
    - [Nakai–Moishezon criterion](#nakai-moishezon-criterion)
      - [Real Nakai–Moishezon criterion](#real-nakai-moishezon-criterion)
- [Linear equivalence of Cartier divisors](#linear-equivalence-of-cartier-divisors)
  - [Principal Cartier divisor](#principal-cartier-divisor)
- [Effective Cartier divisor](#effective-cartier-divisor)
  - [Relative effective Cartier divisor on a curve](#relative-effective-cartier-divisor-on-a-curve)
  - [Locally principal subvariety](#locally-principal-subvariety)
  - [Divisor restriction exact sequence](#divisor-restriction-exact-sequence)
- [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)
  - [Iitaka dimension](#iitaka-dimension)
  - [Movable part of a linear system](#movable-part-of-a-linear-system)
  - [Fixed part of a linear system](#fixed-part-of-a-linear-system)
    - [Fixed component](#fixed-component)
  - [Basepoint-free divisor](#basepoint-free-divisor)
    - [Toric basepoint-free criterion](#toric-basepoint-free-criterion)
  - [Very ample divisor](#very-ample-divisor)
    - [High-degree divisor is very ample on a smooth projective curve](#high-degree-divisor-is-very-ample-on-a-smooth-projective-curve)
- [Hyperplane divisor](#hyperplane-divisor)
  - [Hyperplane section](#hyperplane-section)
    - [Bertini's theorem](#bertini-s-theorem)
    - [Hyperplane-section divisor of a projective plane curve](#hyperplane-section-divisor-of-a-projective-plane-curve)
- [Line bundle associated to a divisor](#line-bundle-associated-to-a-divisor)
- [Cartier class group](#cartier-class-group)

## Pullback of a Cartier divisor

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

For a [morphism of varieties](algebraic-geometry.md#morphism-of-algebraic-varieties) $f:X\to Y$, pull back local defining rational functions of a [Cartier divisor](cartier-divisor.md) $D$ whenever they remain nonzero on each component of $X$. Their ratios remain regular units, defining $f^*D$. Equivalently, pull back the associated [line bundle](ringed-space.md#line-bundle) and its rational section. A dominant morphism always permits this construction.

## Cartier divisor exact sequence for an integral domain

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

For an [integral domain](commutative-algebra.md#integral-domain) $A$ with [fraction field](commutative-algebra.md#field-of-fractions) $K$, realize [Cartier divisors](cartier-divisor.md) as [invertible fractional ideals](commutative-algebra.md#invertible-fractional-ideal), with local divisor equation $f$ corresponding to the ideal $fA$. This is the $\mathcal O(-D)$ convention. The maps in the displayed [exact sequence](homology.md#exact-sequence) are unit inclusion, $f\mapsto fA$, and $I\mapsto[I]$. A principal fractional ideal is trivial as a divisor exactly when its generator is a unit. An invertible fractional ideal is trivial in the [Picard group of a ring](ringed-space.md#picard-group-of-a-ring) exactly when it is principal. Every rank-one projective module embeds in $K$ and produces an invertible fractional ideal, proving surjectivity. Local multiplication identifies $I\otimes_AJ$ with $IJ$, so these are group homomorphisms.

## Divisor line bundle

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

On an [integral scheme](ringed-space.md#integral-scheme), for a [Cartier divisor](cartier-divisor.md) locally represented by $a_i\in K^*$, its divisor line bundle is the subsheaf of rational functions locally equal to $a_i^{-1}\mathcal O_X$. Unit ratios glue these free rank-one modules. Given a nonzero [rational section of a line bundle](ringed-space.md#rational-section-of-a-line-bundle) $s=a_ie_i$, the maps $e_i\mapsto a_i^{-1}$ identify that [invertible sheaf](ringed-space.md#line-bundle) with $\mathcal O_X(D)$. Replacing $s$ by a nonzero rational multiple changes $D$ by a [principal Cartier divisor](#principal-cartier-divisor).

## Real Cartier divisor

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

A real Cartier divisor is a finite real linear combination of [Cartier divisors](cartier-divisor.md). A rational Cartier divisor is defined analogously with rational coefficients; after multiplication by a common denominator it is Cartier.

### Ample real divisor

↑ **Parent:** [Real Cartier divisor](#real-cartier-divisor)

A real Cartier divisor is ample if it is a positive real combination of [ample Cartier divisors](#ample-cartier-divisor). Equivalently its [numerical class](#real-numerical-divisor-classes) lies in the [ample cone](#ample-cone). To recover an actual positive combination from the numerical condition, write the divisor in a finite Cartier basis and take nearby rational points in the inverse image of the open ample cone. A small rational simplex around the original coefficient vector expresses it as a positive convex combination of rational ample Cartier combinations; clearing denominators gives ample Cartier divisors.

### Real linear equivalence of divisors

↑ **Parent:** [Real Cartier divisor](#real-cartier-divisor)

Real linear equivalence means that $D-E$ is a finite real combination of [principal Cartier divisors](#principal-cartier-divisor). Rational linear equivalence uses rational coefficients instead. Both imply [numerical equivalence of divisors](#numerical-equivalence-of-divisors).

## Positivity of divisors

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

The positivity of a [Cartier divisor](cartier-divisor.md) can be measured by sections, [intersection numbers](algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve), or its [numerical class](#real-numerical-divisor-classes). [Ample divisors](#ample-cartier-divisor) give projective embeddings after taking a multiple; [nef divisors](#nef-line-bundle) are their numerical limits; [big divisors](#big-divisor) have the maximum possible order of section growth. Nefness and bigness are different conditions.

### Semiample divisor

↑ **Parent:** [Positivity of divisors](#positivity-of-divisors)

A [Cartier divisor](cartier-divisor.md) is [semiample](#semiample-divisor) if some positive multiple is a [basepoint-free divisor](#basepoint-free-divisor), equivalently its [divisor line bundle](#divisor-line-bundle) has a globally generated positive power. Such a power defines a [Kodaira map](ringed-space.md#kodaira-map) $f$ with $\mathcal O(mD)=f^*\mathcal O(1)$. [Semiampleness](#semiample-divisor) implies nefness but need not imply [ampleness](#ample-cartier-divisor): a fibre divisor of a morphism to a curve is a basic example.

#### Semiampleness of a square-zero rational curve

↑ **Parent:** [Semiample divisor](#semiample-divisor)

A [smooth rational curve](projective-space.md#smooth-rational-curve) $C$ with $C^2=0$ on a [smooth projective surface](algebraic-geometry.md#smooth-projective-surface) is [semiample](#semiample-divisor) and has [Iitaka dimension](#iitaka-dimension) one. Its normal bundle is trivial, so the restriction sequences for $mC$ have quotient $\mathcal O_C$ and zero quotient $H^1$. The finite dimensions of $H^1(X,mC)$ decrease and stabilize. Restriction of sections to $C$ is then surjective; a lift of $1$ and the canonical section generate globally. Exactness also gives $h^0(X,mC)-h^0(X,(m-1)C)=1$ eventually.

#### Semiample and curve-positive ampleness criterion

↑ **Parent:** [Semiample divisor](#semiample-divisor)

A [semiample divisor](#semiample-divisor) on an integral [projective variety](projective-space.md#projective-variety) is [ample](ringed-space.md#ample-line-bundle) if it has positive degree on every integral [projective curve](projective-space.md#projective-curve). Its [Kodaira map](ringed-space.md#kodaira-map) cannot contract a positive-dimensional fibre, since such a fibre contains a curve and the pulled-back hyperplane bundle has degree zero there. Thus the morphism is proper and a [quasi-finite morphism](ringed-space.md#quasi-finite-morphism), hence a [finite morphism](algebraic-geometry.md#finite-morphism). The [finite pullback of an ample line bundle](ringed-space.md#finite-pullback-of-an-ample-line-bundle) is [ample](ringed-space.md#ample-line-bundle).

#### Restriction ampleness implies semiampleness for an effective divisor

↑ **Parent:** [Semiample divisor](#semiample-divisor)

If $E$ is an [effective Cartier divisor](#effective-cartier-divisor) on a [projective scheme](ringed-space.md#projective-scheme) and $\mathcal O_E(E)$ is [ample](ringed-space.md#ample-line-bundle), then $E$ is [semiample](#semiample-divisor). The [divisor restriction exact sequence](#divisor-restriction-exact-sequence) and [Serre vanishing](ringed-space.md#serre-vanishing) make $H^1(X,(m-1)E)\to H^1(X,mE)$ surjective for large $m$. Their finite dimensions stabilize, so restriction on [global sections](ringed-space.md#global-section) is eventually surjective. Lift generators on $E$; off $E$, the canonical section of $mE$ generates. Together these generate $\mathcal O_X(mE)$, including on nonreduced $X$.

### Big divisor

↑ **Parent:** [Positivity of divisors](#positivity-of-divisors)

A [Cartier divisor](cartier-divisor.md) $D$ on an integral $n$-dimensional projective variety is big when $h^0(X,mD)\geq c m^n$ for some $c>0$ and infinitely many positive integers $m$. Equivalently, its [Iitaka dimension](#iitaka-dimension) is $n$. [Kodaira's lemma](#kodaira-s-lemma) characterizes bigness by an ample-plus-effective decomposition, and the [birational linear system criterion for bigness](#birational-linear-system-criterion-for-bigness) shows why this growth captures the full variety.

#### Algebraic Morse inequality for ample divisors

↑ **Parent:** [Big divisor](#big-divisor)

For [ample](ringed-space.md#ample-line-bundle) rational Cartier classes $B,C$ on an integral projective $n$-fold with $n\ge1$, $B^n>nB^{n-1}\cdot C$ implies $B-C$ is big. Scale to [very ample](ringed-space.md#very-ample-line-bundle) integral divisors. Choose an effective [Cartier divisor](cartier-divisor.md) $G\in|C|$. Repeated restriction gives $h^0(m(B-C))\ge h^0(mB)-m h^0(G,mB)$: multiply each negatively twisted restriction by a section avoiding its associated points to inject it into $\mathcal O_G(mB)$. [Asymptotic Riemann–Roch](ringed-space.md#asymptotic-riemann-roch) and [Serre vanishing](ringed-space.md#serre-vanishing) give the positive leading lower bound along sufficiently divisible section indices after undoing the scaling. No complex-analytic Morse theory or characteristic-zero vanishing is used.

#### Bigness under finite normalization

↑ **Parent:** [Big divisor](#big-divisor)

Let $\nu:X^\nu\to X$ be the finite normalization of an integral projective variety. The [coherent sheaf](ringed-space.md#coherent-sheaf) $\mathcal Q=\nu_*\mathcal O_{X^\nu}/\mathcal O_X$ is supported in dimension at most $n-1$. For a [Cartier divisor](cartier-divisor.md) $D$, the [projection formula for sheaves](ringed-space.md#projection-formula) and the resulting [long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology) give

$$
0\leq h^0(X^\nu,m\nu^*D)-h^0(X,mD)\leq h^0(X,\mathcal Q\otimes\mathcal O_X(mD))=O(m^{n-1}).
$$

The last step uses the [polynomial bound for sections of a fixed divisor](algebraic-geometry.md#polynomial-bound-for-sections-of-a-fixed-divisor). Therefore the leading order $m^n$ growth, and hence bigness, is preserved in both directions. This handles nonnormal varieties without assuming a resolution of singularities in positive characteristic.

#### Big real divisor

↑ **Parent:** [Big divisor](#big-divisor)

A big real divisor is an actual positive real combination of [big Cartier divisors](#big-divisor). Equivalently it is real linearly equivalent, or numerically equivalent, to an [ample real divisor](#ample-real-divisor) plus an effective real divisor. The [rational approximation of an ample-plus-effective real divisor](#rational-approximation-of-an-ample-plus-effective-real-divisor) and [Kodaira's lemma](#kodaira-s-lemma) connect these formulations. [Fujino's notes on big real divisors](https://www.math.kyoto-u.ac.jp/~fujino/big-r-divisor5.pdf) give the definition also for nonnormal varieties; [bigness under finite normalization](#bigness-under-finite-normalization) relates it to section growth.

##### Negative curves of a big real divisor lie in finitely many divisors

↑ **Parent:** [Big real divisor](#big-real-divisor)

Write a big real [Cartier divisor](cartier-divisor.md) on an integral [projective variety](projective-space.md#projective-variety) as $D\sim_{\mathbb R}B+E$, with $B$ [ample](ringed-space.md#ample-line-bundle) and $E$ effective real Cartier. Every curve outside $\operatorname{Supp}E$ has $D\cdot C=B\cdot C+E\cdot C>0$. Therefore curves negative against $D$ lie in finitely many support components of codimension one. On a [projective scheme](ringed-space.md#projective-scheme) use [componentwise bigness on a projective scheme](#componentwise-bigness-on-a-projective-scheme) and collect the supports on its finitely many integral components; codimension one is taken in the relevant component.

###### Uniform ample subtraction from a big divisor with ample exceptional restrictions

↑ **Parent:** [Negative curves of a big real divisor lie in finitely many divisors](#negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors)

If a big class $D=B+E$ has [ample](ringed-space.md#ample-line-bundle) restriction to every component $E_i$ of the effective support, then for any [ample](ringed-space.md#ample-line-bundle) $A$ a sufficiently small $\epsilon>0$ makes $D-\epsilon A$ [nef](#nef-line-bundle). Use openness of the [ample cone](#ample-cone) to keep $B-\epsilon A$ and all $(D-\epsilon A)|_{E_i}$ [ample](ringed-space.md#ample-line-bundle) with one finite minimum of bounds. Curves inside the support use these restrictions; curves outside use effectivity of $E$. Thus one does not need a uniform choice over infinitely many [subvarieties](algebraic-geometry.md#closed-subvariety).

##### Componentwise bigness on a projective scheme

↑ **Parent:** [Big real divisor](#big-real-divisor)

For a possibly reducible [projective scheme](ringed-space.md#projective-scheme), componentwise bigness means that a real Cartier class restricts to a [big real divisor](#big-real-divisor) on every reduced irreducible component. This specifies the convention needed by positivity arguments that treat all curves. Maximal total section growth alone is weaker: on $\mathbb P^2\amalg\mathbb P^2$, the bundle $(\mathcal O(1),\mathcal O(-1))$ has quadratic total growth but negative degree on every line in the second component. Thus its negative curves cannot be confined to finitely many divisors.

##### Rational approximation of an ample-plus-effective real divisor

↑ **Parent:** [Big real divisor](#big-real-divisor)

Suppose $D\sim_{\mathbb R}tA+E$ on an integral projective variety, where $t>0$, $A$ is ample Cartier and $E$ is effective real Cartier. Then $D$ is an actual positive combination of [big Cartier divisors](#big-divisor).

Here is a finite-dimensional proof. First assume $X$ is normal. Express $D$ and $E$ in finite Cartier bases and write $D-tA-E$ as a finite combination of [principal Cartier divisors](#principal-cartier-divisor). The union of the supports of these finitely many divisors has finitely many prime components. Their integer multiplicities turn the equality into finitely many rational linear equations and effectivity into finitely many rational linear inequalities. The given coefficient tuple lies in a rational polyhedron. Take its smallest face; within that face it lies in the relative interior, and $t>0$ is an open condition. A small simplex with rational vertices in this relative interior contains the tuple. Each vertex gives $D_\nu\sim_{\mathbb Q}t_\nu A+E_\nu$ with $t_\nu>0$ and $E_\nu\geq0$. Clearing denominators and applying [Kodaira's lemma](#kodaira-s-lemma) shows that $D_\nu$ is a positive rational multiple of a big Cartier divisor. Taking the original convex weights proves the required actual equality.

If $X$ is nonnormal, pull the finite Cartier bases and the relation to its finite normalization and impose the same rational equations and effectivity inequalities there. The vertex divisors remain rational Cartier divisors on $X$ because they were constructed in bases from $X$. They are big on the normalization, hence big on $X$ by [bigness under finite normalization](#bigness-under-finite-normalization). This proves the same conclusion. Effectivity is used in the usual effective Cartier sense so that pullback is effective; arbitrary cycles on a nonnormal variety cannot be substituted without defining a compatible divisor theory.

##### Big cone

↑ **Parent:** [Big real divisor](#big-real-divisor)

The big cone in $N^1(X)_{\mathbb R}$ is open and convex: write a big class as ample plus effective, perturb only the ample summand, and use openness of the [ample cone](#ample-cone). For positive-dimensional $X$, intersection with $H^{n-1}$ for any very ample divisor $H$ is strictly positive on every big class. Hence this cone contains no line and does not contain the zero class.

#### Birational linear system criterion for bigness

↑ **Parent:** [Big divisor](#big-divisor)

A [Cartier divisor](cartier-divisor.md) on an integral projective variety is big if and only if some multiple has a [complete linear system of a divisor](#complete-linear-system-of-a-divisor) giving a rational map birational onto its image. [Kodaira's lemma](#kodaira-s-lemma) embeds a very ample subsystem in a suitable multiple. Conversely, $n$ [algebraically independent elements](algebra.md#algebraically-independent-elements) among the section ratios give $\binom{q+n}{n}$ independent degree-$q$ section monomials, where $n=\dim X$. Smoothness is not necessary.

<h4 id="kodaira-s-lemma">Kodaira's lemma</h4>

↑ **Parent:** [Big divisor](#big-divisor)

A [Cartier divisor](cartier-divisor.md) $D$ on an integral projective variety is big exactly when, for every [ample divisor](#ample-cartier-divisor) $A$, some positive integer $j$ satisfies $jD\sim A+E$ with $E$ effective. To prove the forward direction, subtract an effective high multiple of $A$ using the [section subtraction lemma for big divisors](#section-subtraction-lemma-for-big-divisors), then add an effective representative of the remaining multiple. For the reverse direction, multiply sections of $qA$ by the section of $qE$ and use the ample [Hilbert polynomial](algebraic-geometry.md#hilbert-polynomial).

#### Section subtraction lemma for big divisors

↑ **Parent:** [Big divisor](#big-divisor)

If $D$ is a [big divisor](#big-divisor) and $F$ an [effective Cartier divisor](#effective-cartier-divisor), infinitely many $m$ have $H^0(X,mD-F)\ne0$. The [divisor restriction exact sequence](#divisor-restriction-exact-sequence) bounds the dimension lost upon restriction to $F$ by $O(m^{n-1})$, using the [polynomial bound for sections of a fixed divisor](algebraic-geometry.md#polynomial-bound-for-sections-of-a-fixed-divisor); this cannot exhaust the $c m^n$ sections along the infinite growth sequence.

### Numerical equivalence of divisors

↑ **Parent:** [Positivity of divisors](#positivity-of-divisors)

Two [Cartier divisors](cartier-divisor.md) are numerically equivalent when they have equal [intersection numbers](algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) with every integral complete curve. A numerically trivial divisor has zero intersection with every such curve. Unlike [linear equivalence of Cartier divisors](#linear-equivalence-of-cartier-divisors), numerical equivalence does not require the same [line bundle](ringed-space.md#line-bundle).

#### Real numerical divisor classes

↑ **Parent:** [Numerical equivalence of divisors](#numerical-equivalence-of-divisors)

The finite-dimensional [real vector space](vector-space.md#real-vector-space) $N^1(X)_{\mathbb R}$ consists of real combinations of [Cartier divisors](cartier-divisor.md) modulo [numerical equivalence of divisors](#numerical-equivalence-of-divisors). Its elements are numerical divisor classes. The space of curve classes paired with it is $N_1(X)_{\mathbb R}$.

##### Nef cone

↑ **Parent:** [Real numerical divisor classes](#real-numerical-divisor-classes)

The nef cone is the closed [convex cone](mathematical-optimization.md#convex-cone) of [nef divisor](#nef-line-bundle) classes. It is dual to the [closed cone of curves](#closed-cone-of-curves). Its interior is the [ample cone](#ample-cone) on a [projective scheme](ringed-space.md#projective-scheme).

###### Ample cone

↑ **Parent:** [Nef cone](#nef-cone)

The ample cone consists of [real numerical divisor classes](#real-numerical-divisor-classes) represented by [ample real divisors](#ample-real-divisor). It is an open [convex cone](mathematical-optimization.md#convex-cone), and [Kleiman's criterion](#kleiman-s-criterion) identifies it with the interior of the [nef cone](#nef-cone).

###### Nef-plus-ample ampleness lemma

↑ **Parent:** [Ample cone](#ample-cone)

The sum of a [nef](#nef-line-bundle) real Cartier class and an [ample](ringed-space.md#ample-line-bundle) real Cartier class on a [projective scheme](ringed-space.md#projective-scheme) is [ample](ringed-space.md#ample-line-bundle). By [Kleiman's criterion](#kleiman-s-criterion), the [ample cone](#ample-cone) is the interior of the [nef cone](#nef-cone). If a ball about an [ample](ringed-space.md#ample-line-bundle) class lies in that convex cone, translating it by a [nef](#nef-line-bundle) class still lies in the cone. The sum is consequently still an interior point.

##### Closed cone of curves

↑ **Parent:** [Real numerical divisor classes](#real-numerical-divisor-classes)

The closed cone of curves is the closure in $N_1(X)_{\mathbb R}$ of the [convex cone](mathematical-optimization.md#convex-cone) generated by classes of integral curves. A [nef divisor](#nef-line-bundle) pairs nonnegatively with this entire closed cone. Its boundary can contain limiting classes which are not represented by one curve.

### Nef line bundle

↑ **Parent:** [Positivity of divisors](#positivity-of-divisors)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nef_line_bundle)

A [line bundle](ringed-space.md#line-bundle) is nef when its degree on every integral complete curve is nonnegative. Equivalently a [Cartier divisor](cartier-divisor.md) $D$ is nef when $D\cdot C\geq0$ for every such curve. On a projective scheme, adding a positive ample class to a nef class makes it ample; taking limits in the [intersection product](algebraic-geometry.md#intersection-product-of-cartier-divisors) shows that a nef divisor has nonnegative top [self-intersection number](algebraic-geometry.md#self-intersection-number).

#### Volume of a nef divisor

↑ **Parent:** [Nef line bundle](#nef-line-bundle)

For a [nef divisor](#nef-line-bundle) on an integral projective variety of dimension $n$,

$$
h^0(X,mD)=\frac{D^n}{n!}m^n+O(m^{n-1}).
$$

Indeed, combine [asymptotic Riemann–Roch](ringed-space.md#asymptotic-riemann-roch) with [cohomology growth for nef twists](ringed-space.md#cohomology-growth-for-nef-twists). Thus its normalized section-growth [limit](calculus.md#limit-of-a-function) is $D^n/n!$, and it is big exactly when $D^n>0$.

### Ample Cartier divisor

↑ **Parent:** [Positivity of divisors](#positivity-of-divisors)

A [Cartier divisor](cartier-divisor.md) is ample when its associated [line bundle](ringed-space.md#line-bundle) is [ample](ringed-space.md#ample-line-bundle). The [Nakai–Moishezon criterion](#nakai-moishezon-criterion) and [Kleiman's criterion](#kleiman-s-criterion) characterize this condition numerically.

#### Toric ampleness criterion

↑ **Parent:** [Ample Cartier divisor](#ample-cartier-divisor)

In the notation of the [toric basepoint-free criterion](#toric-basepoint-free-criterion), the divisor is ample exactly when $\langle m_\sigma,v_\rho\rangle>-a_\rho$ for each ray outside $\sigma$. Equivalently, the normal fan of its divisor polytope is the original fan.

// Target: geometry-and-topology.bigb

#### Vanishing-section ampleness criterion

↑ **Parent:** [Ample Cartier divisor](#ample-cartier-divisor)

A [Cartier divisor](cartier-divisor.md) is [ample](ringed-space.md#ample-line-bundle) if for every positive-dimensional integral closed [subvariety](algebraic-geometry.md#closed-subvariety) some positive multiple restricts to a bundle with a nonzero section having a nonempty zero locus. Inductively the divisor is [ample](ringed-space.md#ample-line-bundle) on all lower-dimensional subschemes. On an integral component the chosen section cuts out a nonempty [effective Cartier divisor](#effective-cartier-divisor) $E$ whose restriction bundle $\mathcal O_E(E)$ is [ample](ringed-space.md#ample-line-bundle). The [restriction ampleness implies semiampleness for an effective divisor](#restriction-ampleness-implies-semiampleness-for-an-effective-divisor) lemma makes the original divisor [semiample](#semiample-divisor). On a curve the vanishing section forces positive degree, so the [semiample and curve-positive ampleness criterion](#semiample-and-curve-positive-ampleness-criterion) proves [ampleness](#ample-cartier-divisor).

#### Euler-characteristic ampleness criterion

↑ **Parent:** [Ample Cartier divisor](#ample-cartier-divisor)

A [Cartier divisor](cartier-divisor.md) $D$ on a [projective scheme](ringed-space.md#projective-scheme) is [ample](ringed-space.md#ample-line-bundle) exactly when $\chi(V,\mathcal O_V(mD))\to+\infty$ for every positive-dimensional integral closed [subvariety](algebraic-geometry.md#closed-subvariety) $V$, including irreducible components. For the converse induct on dimension: restrictions to hyperplane sections are [ample](ringed-space.md#ample-line-bundle), so [higher cohomology vanishing from an ample hyperplane restriction](ringed-space.md#higher-cohomology-vanishing-from-an-ample-hyperplane-restriction) gives $h^0=\chi+h^1\to\infty$. A nonzero section vanishing at a chosen point then exists. The [vanishing-section ampleness criterion](#vanishing-section-ampleness-criterion) finishes. Divergence alone does not imply a positive top-degree coefficient.

<h4 id="kleiman-s-criterion">Kleiman's criterion</h4>

↑ **Parent:** [Ample Cartier divisor](#ample-cartier-divisor)

For a [projective scheme](ringed-space.md#projective-scheme), a divisor class is in the [ample cone](#ample-cone) exactly when it is strictly positive on every nonzero element of the [closed cone of curves](#closed-cone-of-curves). Equivalently, the ample cone is the interior of the [nef cone](#nef-cone). The projectivity assumption matters: the same characterization is not asserted here for arbitrary proper schemes.

<h4 id="nakai-moishezon-criterion">Nakai–Moishezon criterion</h4>

↑ **Parent:** [Ample Cartier divisor](#ample-cartier-divisor)

An integral [Cartier divisor](cartier-divisor.md) $D$ on a [projective scheme](ringed-space.md#projective-scheme) is [ample](ringed-space.md#ample-line-bundle) if and only if $D^{\dim Y}\cdot Y>0$ for every positive-dimensional integral closed [subvariety](algebraic-geometry.md#closed-subvariety) $Y$. Testing only curves is sufficient in dimension one, but not in higher dimensions.

<h5 id="real-nakai-moishezon-criterion">Real Nakai–Moishezon criterion</h5>

↑ **Parent:** [Nakai–Moishezon criterion](#nakai-moishezon-criterion)

A real Cartier class on a [projective scheme](ringed-space.md#projective-scheme) is [ample](ringed-space.md#ample-line-bundle) if and only if its top self-intersection on every positive-dimensional integral [subvariety](algebraic-geometry.md#closed-subvariety) is positive. For the converse curve tests give nefness. Small [ample](ringed-space.md#ample-line-bundle) perturbations and rational approximation give [ample](ringed-space.md#ample-line-bundle) rational $B,C$ with $D-A=B-C$ satisfying the [algebraic Morse inequality for ample divisors](#algebraic-morse-inequality-for-ample-divisors), hence bigness. Induction gives [ample](ringed-space.md#ample-line-bundle) restrictions on codimension-one [subvarieties](algebraic-geometry.md#closed-subvariety); [uniform ample subtraction from a big divisor with ample exceptional restrictions](#uniform-ample-subtraction-from-a-big-divisor-with-ample-exceptional-restrictions) makes $D-\epsilon A$ [nef](#nef-line-bundle). The [nef-plus-ample ampleness lemma](#nef-plus-ample-ampleness-lemma) concludes. For reducible schemes perform the finite component tests simultaneously.

## Linear equivalence of Cartier divisors

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

Two [Cartier divisors](cartier-divisor.md) are linearly equivalent when their difference is a [principal Cartier divisor](#principal-cartier-divisor). Their associated [line bundles](ringed-space.md#line-bundle) are then isomorphic, so their [global section](ringed-space.md#global-section) spaces have the same dimension. This definition works in every dimension.

### Principal Cartier divisor

↑ **Parent:** [Linear equivalence of Cartier divisors](#linear-equivalence-of-cartier-divisors)

A principal Cartier divisor is represented on every chart by the same nonzero [rational function](isolated-singularity.md#rational-function). It is linearly equivalent to zero and has zero [intersection number](algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) with every complete curve.

## Effective Cartier divisor

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

An effective Cartier divisor is cut out locally by one [non-zero-divisor](mathematics.md#non-zero-divisor); it is a codimension-one closed subscheme. On an integral scheme a nonzero [global section](ringed-space.md#global-section) of a [line bundle](ringed-space.md#line-bundle) defines such a divisor, possibly empty. On a nonreduced scheme a nonzero section need not be regular, so its zero locus need not be a Cartier divisor.

### Relative effective Cartier divisor on a curve

↑ **Parent:** [Effective Cartier divisor](#effective-cartier-divisor)

A relative effective divisor of degree $m$ on a [smooth projective curve](projective-space.md#smooth-projective-curve) is an [effective Cartier divisor](#effective-cartier-divisor) in $C\times T$ that is finite and flat of degree $m$ over $T$. Its associated [line bundle](ringed-space.md#line-bundle) has degree $m$ on every fibre. The [symmetric product of a curve](algebraic-geometry.md#symmetric-product-of-a-curve) $C^{(m)}$ represents these families and carries their universal divisor. Locally on a smooth coordinate chart, the divisor is described by a monic polynomial, whose coefficients are elementary symmetric functions of its points; this description includes collisions and works in positive characteristic.

### Locally principal subvariety

↑ **Parent:** [Effective Cartier divisor](#effective-cartier-divisor)

A proper subvariety locally defined by one non-zero-divisor is an [effective Cartier divisor](#effective-cartier-divisor). On an integral [variety](algebraic-geometry.md#algebraic-variety) a nonzero local equation is automatically a [non-zero-divisor](mathematics.md#non-zero-divisor). Its [conormal sheaf](ringed-space.md#conormal-sheaf) is a [line bundle](ringed-space.md#line-bundle), since $A/(f)\cong(f)/(f^2)$ via multiplication by $f$. Allowing the zero equation would include the whole [variety](algebraic-geometry.md#algebraic-variety) and would not give this conclusion.

### Divisor restriction exact sequence

↑ **Parent:** [Effective Cartier divisor](#effective-cartier-divisor)

For an [effective Cartier divisor](#effective-cartier-divisor) $E$ and any [Cartier divisor](cartier-divisor.md) $D$, multiplication by a defining section of $E$ gives the displayed [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves). Its [long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology) compares sections and cohomology on $X$ with their restrictions to $E$.

## Complete linear system of a divisor

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

This is the full [linear system of divisors](algebraic-geometry.md#linear-system-of-divisors), obtained by using every global section of the associated [line bundle](ringed-space.md#line-bundle). For a [Cartier divisor](cartier-divisor.md) on an integral projective variety, the complete linear system $|D|$ consists of its effective representatives under [linear equivalence of Cartier divisors](#linear-equivalence-of-cartier-divisors). A basis of $H^0(X,\mathcal O_X(D))$ defines a rational map to projective space.

### Iitaka dimension

↑ **Parent:** [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Iitaka_dimension)

The Iitaka dimension of a [Cartier divisor](cartier-divisor.md) $D$ is the maximum dimension of the images of the rational maps given by its nonempty multiples $|mD|$. It is $-\infty$ if all positive multiples have no sections. For an integral $n$-dimensional projective variety it lies between zero and $n$ when nonnegative. The [Kodaira dimension](algebraic-geometry.md#kodaira-dimension) of the variety is the special case $D=K_X$.

### Movable part of a linear system

↑ **Parent:** [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)

The movable part is $|D-F|$, where $F$ is the [fixed part](#fixed-part-of-a-linear-system). It has no [fixed components](#fixed-component). On a [smooth algebraic surface](algebraic-geometry.md#smooth-algebraic-surface) its associated divisor is [nef](#nef-line-bundle): for each curve choose a member avoiding that curve and use nonnegative local [intersection multiplicities](algebraic-geometry.md#intersection-multiplicity).

### Fixed part of a linear system

↑ **Parent:** [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)

For a nonempty [complete linear system of a divisor](#complete-linear-system-of-a-divisor) on a smooth projective variety, the coefficient of a prime divisor in its fixed part is the minimum of its multiplicities in all members. Multiplication by the section of $F$ identifies the sections of $D-F$ with those of $D$.

#### Fixed component

↑ **Parent:** [Fixed part of a linear system](#fixed-part-of-a-linear-system)

A fixed component is a prime divisor appearing in every member of a [complete linear system of a divisor](#complete-linear-system-of-a-divisor). This concerns divisorial components; a linear system can have isolated basepoints even when it has no fixed component.

### Basepoint-free divisor

↑ **Parent:** [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)

A divisor is basepoint-free when its global sections have no common zero. Its complete linear system therefore defines a [Kodaira map](ringed-space.md#kodaira-map) everywhere.

#### Toric basepoint-free criterion

↑ **Parent:** [Basepoint-free divisor](#basepoint-free-divisor)

For an invariant Cartier divisor $D=\sum_\rho a_\rho D_\rho$ on a complete smooth toric variety, let $m_\sigma$ satisfy $\langle m_\sigma,v_\rho\rangle=-a_\rho$ for rays in a maximal cone $\sigma$. The divisor is basepoint-free exactly when every $m_\sigma$ lies in the [lattice polytope of a toric divisor](toric-geometry.md#lattice-polytope-of-a-toric-divisor) $P_D$. Its character section then trivializes the line bundle on the entire chart $U_\sigma$.

// Target: geometry-and-topology.bigb

### Very ample divisor

↑ **Parent:** [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)

A [very ample divisor](#very-ample-divisor) is a divisor whose associated [line bundle](ringed-space.md#line-bundle) is a [very ample line bundle](ringed-space.md#very-ample-line-bundle). A divisor is very ample when its complete linear system defines a closed embedding into projective space.

#### High-degree divisor is very ample on a smooth projective curve

↑ **Parent:** [Very ample divisor](#very-ample-divisor)

On a smooth projective curve of genus $g$, every divisor of degree at least $2g+1$ is very ample. Riemann--Roch shows that its sections separate distinct points and tangent directions by comparing $L(D)$ with $L(D-P-Q)$ and $L(D-2P)$.

## Hyperplane divisor

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

A hyperplane divisor on [projective space](projective-space.md) is the effective [Cartier divisor](cartier-divisor.md) cut out by one nonzero linear homogeneous polynomial. Its class generates $\operatorname{Cl}(\mathbb P_k^n)\cong\mathbb Z$.

### Hyperplane section

↑ **Parent:** [Hyperplane divisor](#hyperplane-divisor)

A hyperplane section of a projective variety $X\subset\mathbb P^n$ is the scheme-theoretic intersection $X\cap H$ with a [projective hyperplane](algebraic-topology.md#projective-hyperplane) $H$. Its associated [line bundle](ringed-space.md#line-bundle) is $\mathcal O_X(1)$.

<h4 id="bertini-s-theorem">Bertini's theorem</h4>

↑ **Parent:** [Hyperplane section](#hyperplane-section)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bertini's_theorem)

For a smooth integral projective variety over $\mathbb C$, a general hyperplane section in a projective embedding is smooth; if its dimension is at least two, the section is also irreducible. More general statements concern linear systems and their base loci. The smoothness statement is developed in [the Stacks Project's Bertini section](https://stacks.math.columbia.edu/tag/0FD4).

#### Hyperplane-section divisor of a projective plane curve

↑ **Parent:** [Hyperplane section](#hyperplane-section)

If a [projective line](finite-group-theory.md#projective-line) $H$ does not contain the [projective plane curve](algebraic-geometry.md#projective-plane-curve) $X$, its hyperplane-section divisor is

$$
[X\cap H]=\sum_{p\in X\cap H}I_p(X,H)p,
$$

where $I_p(X,H)$ is the [intersection multiplicity](algebraic-geometry.md#intersection-multiplicity). The [Bézout theorem](algebraic-geometry.md#bezout-s-theorem) gives $\deg[X\cap H]=(\deg X)(\deg H)=\deg X$.

## Line bundle associated to a divisor

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

For a [Cartier divisor](cartier-divisor.md) $D$, the associated line bundle $\mathcal O(D)$ has local sections given by [meromorphic functions](isolated-singularity.md#meromorphic-function) $f$ satisfying $(f)+D\geq0$. Its canonical meromorphic section has divisor $D$.

## Cartier class group

↑ **Parent:** [Cartier divisor](cartier-divisor.md)

The Cartier class group is the group of Cartier divisors modulo principal Cartier divisors. On an integral scheme it is naturally $H^1(X,\mathcal O_X^*)$.

## ↑ Ancestors (5)

1. [Algebraic geometry](algebraic-geometry.md)
2. [Geometry and topology](geometry-and-topology.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (68)

- [Abel map of an algebraic curve](abelian-variety.md#abel-map-of-an-algebraic-curve)
- [Algebraic Morse inequality for ample divisors](#algebraic-morse-inequality-for-ample-divisors)
- [Ample Cartier divisor](#ample-cartier-divisor)
- [Asymptotic Riemann–Roch](ringed-space.md#asymptotic-riemann-roch)
- [Big divisor](#big-divisor)
- [Bigness under finite normalization](#bigness-under-finite-normalization)
- [Birational linear system criterion for bigness](#birational-linear-system-criterion-for-bigness)
- [Canonical divisor of a smooth variety](ringed-space.md#canonical-divisor-of-a-smooth-variety)
- [Cartier-divisor description of the Picard group](ringed-space.md#cartier-divisor-description-of-the-picard-group)
- [Cartier divisor exact sequence for an integral domain](#cartier-divisor-exact-sequence-for-an-integral-domain)
- [Class-group generator of a well-formed weighted projective space](toric-geometry.md#class-group-generator-of-a-well-formed-weighted-projective-space)
- [Complete linear system of a divisor](#complete-linear-system-of-a-divisor)
- [Determinant description of the theta divisor](abelian-variety.md#determinant-description-of-the-theta-divisor)
- [Divisor line bundle](#divisor-line-bundle)
- [Divisor restriction exact sequence](#divisor-restriction-exact-sequence)
- [Euler-characteristic ampleness criterion](#euler-characteristic-ampleness-criterion)
- [Fractional ideal](commutative-algebra.md#fractional-ideal)
- [Hyperplane divisor](#hyperplane-divisor)
- [Iitaka dimension](#iitaka-dimension)
- [Intersection product of Cartier divisors](algebraic-geometry.md#intersection-product-of-cartier-divisors)
- [Jacobian variety](abelian-variety.md#jacobian-variety)
- [Kodaira's lemma](#kodaira-s-lemma)
- [Line bundle associated to a divisor](#line-bundle-associated-to-a-divisor)
- [Linear equivalence of Cartier divisors](#linear-equivalence-of-cartier-divisors)
- [Linear system of divisors](algebraic-geometry.md#linear-system-of-divisors)
- [Nakai–Moishezon criterion](#nakai-moishezon-criterion)
- [Nef line bundle](#nef-line-bundle)
- [Negative curves of a big real divisor lie in finitely many divisors](#negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors)
- [Normalization of an algebraic variety](algebraic-geometry.md#normalization-of-an-algebraic-variety)
- [Numerical equivalence of divisors](#numerical-equivalence-of-divisors)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-18.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-25.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-3.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-13.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-113.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-134.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-134.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-134.md#3/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-139.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-139.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-139.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-113.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-113.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-113.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-113.md#4/d/solution)
- [Picard-group localization on a smooth variety](ringed-space.md#picard-group-localization-on-a-smooth-variety)
- [Picard scheme of a curve](ringed-space.md#picard-scheme-of-a-curve)
- [Polynomial bound for sections of a fixed divisor](algebraic-geometry.md#polynomial-bound-for-sections-of-a-fixed-divisor)
- [Positivity of divisors](#positivity-of-divisors)
- [Projection formula for algebraic cycles](algebraic-geometry.md#projection-formula-for-algebraic-cycles)
- [Pullback of a Cartier divisor](#pullback-of-a-cartier-divisor)
- [Q-Cartier divisor](algebraic-geometry.md#q-cartier-divisor)
- [Rational section of a line bundle](ringed-space.md#rational-section-of-a-line-bundle)
- [Real Cartier divisor](#real-cartier-divisor)
- [Real numerical divisor classes](#real-numerical-divisor-classes)
- [Riemann–Roch theorem for algebraic surfaces](algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces)
- [Semiample divisor](#semiample-divisor)
- [Smooth algebraic surface](algebraic-geometry.md#smooth-algebraic-surface)
- [Smooth projective surface](algebraic-geometry.md#smooth-projective-surface)
- [Symmetric product of a curve](algebraic-geometry.md#symmetric-product-of-a-curve)
- [Theta divisor](abelian-variety.md#theta-divisor)
- [Torsion trivialization in a determinant quotient](abelian-variety.md#torsion-trivialization-in-a-determinant-quotient)
- [Vanishing-section ampleness criterion](#vanishing-section-ampleness-criterion)
