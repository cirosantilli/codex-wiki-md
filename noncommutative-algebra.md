# Noncommutative algebra

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noncommutative_algebra)

Noncommutative algebra studies rings whose multiplication need not commute and their one-sided ideals and modules.

**Table of contents**

- [Semiprime ring](#semiprime-ring)
- [Goldie ring](#goldie-ring)
  - [Right Goldie ring](#right-goldie-ring)
    - [Goldie's theorem](#goldie-s-theorem)
      - [Prime classical quotient of a prime right Goldie ring](#prime-classical-quotient-of-a-prime-right-goldie-ring)
      - [Semisimplicity of a classical quotient from regular elements in essential ideals](#semisimplicity-of-a-classical-quotient-from-regular-elements-in-essential-ideals)
- [Regular element of a ring](#regular-element-of-a-ring)
- [Semi-local ring](#semi-local-ring)
  - [Surjectivity from injectivity modulo the Jacobson radical](#surjectivity-from-injectivity-modulo-the-jacobson-radical)
- [Generalized Weyl algebra](#generalized-weyl-algebra)
  - [Krull dimension criterion for rank-one generalized Weyl algebras](#krull-dimension-criterion-for-rank-one-generalized-weyl-algebras)
- [Noncommutative Krull dimension](#noncommutative-krull-dimension)
- [Noncommutative domain](#noncommutative-domain)
- [Quantum plane](#quantum-plane)
  - [Quantum enveloping algebra action on the quantum plane](#quantum-enveloping-algebra-action-on-the-quantum-plane)
    - [Cubic-root quantum-plane socle](#cubic-root-quantum-plane-socle)
  - [Quantum Laurent plane](#quantum-laurent-plane)
  - [Quantum torus](#quantum-torus)
- [Right Artinian ring](#right-artinian-ring)
  - [Right Artinian triangular ring that is not left Noetherian](#right-artinian-triangular-ring-that-is-not-left-noetherian)
  - [Semisimplicity of a right Artinian ring with zero radical](#semisimplicity-of-a-right-artinian-ring-with-zero-radical)
  - [Hopkins-Levitzki theorem](#hopkins-levitzki-theorem)
    - [Minimal-right-ideal proof of radical nilpotence](#minimal-right-ideal-proof-of-radical-nilpotence)
- [Left Noetherian ring](#left-noetherian-ring)
- [Right Noetherian ring](#right-noetherian-ring)
  - [Finite-module extension preserves Noetherianity](#finite-module-extension-preserves-noetherianity)
  - [Right Noetherian domain](#right-noetherian-domain)
  - [Noncommutative Hilbert basis theorem](#noncommutative-hilbert-basis-theorem)
    - [Leading-coefficient proof for a central polynomial extension](#leading-coefficient-proof-for-a-central-polynomial-extension)
    - [Skew Hilbert basis theorem](#skew-hilbert-basis-theorem)
- [Weyl algebra](#weyl-algebra)
  - [Order filtration of a Weyl algebra](#order-filtration-of-a-weyl-algebra)
  - [Simplicity of a Weyl algebra in characteristic zero](#simplicity-of-a-weyl-algebra-in-characteristic-zero)
  - [Ordered monomial basis of a Weyl algebra](#ordered-monomial-basis-of-a-weyl-algebra)
  - [Weyl algebra in positive characteristic](#weyl-algebra-in-positive-characteristic)
  - [Weyl algebra has no nonzero finite-dimensional modules](#weyl-algebra-has-no-nonzero-finite-dimensional-modules)
  - [Bernstein filtration](#bernstein-filtration)
- [Primitive ring](#primitive-ring)
  - [Jacobson density theorem](#jacobson-density-theorem)
- [Morita equivalence](#morita-equivalence)
- [Jacobson radical](#jacobson-radical)
  - [Jacobson radical as greatest quasinilpotent ideal](#jacobson-radical-as-greatest-quasinilpotent-ideal)
  - [Jacobson radical is independent of handedness](#jacobson-radical-is-independent-of-handedness)
  - [Unit criterion for the Jacobson radical](#unit-criterion-for-the-jacobson-radical)
  - [Nilpotent ideal with semisimple quotient radical criterion](#nilpotent-ideal-with-semisimple-quotient-radical-criterion)
  - [Jacobson radical under an integral extension](#jacobson-radical-under-an-integral-extension)
  - [Jacobson ring](#jacobson-ring)
    - [Radical equality for finitely generated integer algebras](#radical-equality-for-finitely-generated-integer-algebras)
    - [Integral extension of a Jacobson ring](#integral-extension-of-a-jacobson-ring)
- [Injective module](#injective-module)
  - [Injective cogenerator of abelian groups](#injective-cogenerator-of-abelian-groups)
  - [Local criterion for injectivity over a Noetherian ring](#local-criterion-for-injectivity-over-a-noetherian-ring)
  - [Baer criterion](#baer-criterion)
  - [Bass-Papp theorem](#bass-papp-theorem)
  - [Divisible module](#divisible-module)
  - [Injective hull](#injective-hull)
    - [Injective hull of an Ore domain](#injective-hull-of-an-ore-domain)
    - [Local endomorphism ring of a uniform injective module](#local-endomorphism-ring-of-a-uniform-injective-module)
- [Ore condition](#ore-condition)
  - [Ore theorem](#ore-theorem)
    - [Right Noetherian domains satisfy the Ore condition](#right-noetherian-domains-satisfy-the-ore-condition)
    - [Left Ore fraction construction](#left-ore-fraction-construction)
  - [Right Ore condition](#right-ore-condition)
    - [Right denominator set](#right-denominator-set)
    - [Classical right ring of quotients](#classical-right-ring-of-quotients)
    - [Right Ore set](#right-ore-set)
  - [Ore localization](#ore-localization)
    - [Classical left ring of quotients](#classical-left-ring-of-quotients)
      - [Matrix and triangular localization over an Ore domain](#matrix-and-triangular-localization-over-an-ore-domain)
  - [Left Ore set](#left-ore-set)
- [Prime ideal of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring)
  - [Prime ring](#prime-ring)
  - [Prime radical of a noncommutative ring](#prime-radical-of-a-noncommutative-ring)
    - [Finite minimal primes and nilpotent prime radical](#finite-minimal-primes-and-nilpotent-prime-radical)

## Semiprime ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semiprime_ring)

A [ring](commutative-algebra.md#ring) is semiprime when it has no nonzero [nilpotent ideals](commutative-algebra.md#nilpotent-ideal). Equivalently, a two-sided [ideal](commutative-algebra.md#ideal) with square zero must be zero. This is weaker than having no nonzero nilpotent elements: a matrix ring over a [field](algebra.md#field) is semiprime and can have nilpotent matrices.

## Goldie ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A [ring](commutative-algebra.md#ring) is right Goldie if it has finite right [uniform dimension](module-theory.md#uniform-dimension) and satisfies the [ascending chain condition](algebra.md#ascending-chain-condition) on [right annihilators](module-theory.md#right-annihilator). The left-sided definition reverses the multiplication. These two definitions need not be equivalent.

### Right Goldie ring

↑ **Parent:** [Goldie ring](#goldie-ring)

A right Goldie ring satisfies the right-sided conditions in the definition of a [Goldie ring](#goldie-ring). Every [right Noetherian ring](#right-noetherian-ring) does: its [right annihilators](module-theory.md#right-annihilator) are [right ideals](associative-algebra.md#right-ideal), and its right regular [module](module-theory.md#module-mathematics) has finite [uniform dimension](module-theory.md#uniform-dimension).

<h4 id="goldie-s-theorem">Goldie's theorem</h4>

↑ **Parent:** [Right Goldie ring](#right-goldie-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Goldie's_theorem)

A [semiprime ring](#semiprime-ring) has a [classical right ring of quotients](#classical-right-ring-of-quotients) that is a [semisimple ring](commutative-algebra.md#semisimple-ring) and [Artinian](algebra.md#artinian-ring) exactly when it is a [right Goldie ring](#right-goldie-ring). In particular, the theorem applies to a [semiprime ring](#semiprime-ring) that is a [right Noetherian ring](#right-noetherian-ring). It extends the fraction-field construction from commutative domains to rings whose quotient can be a finite product of matrix rings over division rings.

##### Prime classical quotient of a prime right Goldie ring

↑ **Parent:** [Goldie's theorem](#goldie-s-theorem)

A nonzero two-sided ideal of the [classical right ring of quotients](#classical-right-ring-of-quotients) contains a nonzero element of the original ring: multiply a nonzero fraction by its regular right denominator. If the original ring is prime, the contractions of any two such ideals have nonzero product, so the quotient ring is prime too. The [Goldie theorem](#goldie-s-theorem) makes it semisimple Artinian, and the [Artin–Wedderburn theorem](associative-algebra.md#artin-wedderburn-theorem) expresses it as a finite product of matrix rings over division rings. Primeness excludes more than one factor.

##### Semisimplicity of a classical quotient from regular elements in essential ideals

↑ **Parent:** [Goldie's theorem](#goldie-s-theorem)

Suppose $R$ is a [right Noetherian ring](#right-noetherian-ring) and every [essential right ideal](module-theory.md#essential-right-ideal) contains a [regular element of a ring](#regular-element-of-a-ring). Preimages of essential regular principal right ideals under left multiplication are essential, so they contain regular elements and prove the [right Ore condition](#right-ore-condition). In the [classical right ring of quotients](#classical-right-ring-of-quotients) $Q$, every [right ideal](associative-algebra.md#right-ideal) is generated by its contraction to $R$, making $Q$ right [Noetherian](algebra.md#noetherian-ring). An [essential right ideal](module-theory.md#essential-right-ideal) of $Q$ contracts to an essential right ideal of $R$, hence contains a regular element and is all of $Q$. A maximal disjoint complement to any [right ideal](associative-algebra.md#right-ideal) has essential sum with it, so every [right ideal](associative-algebra.md#right-ideal) is complemented. The right regular [module](module-theory.md#module-mathematics) is therefore a finite [direct sum](vector-space.md#direct-sum) of [simple modules](module-theory.md#irreducible-module), making $Q$ semisimple Artinian.

## Regular element of a ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A regular element of a [ring](commutative-algebra.md#ring) is a two-sided [non-zero-divisor](mathematics.md#non-zero-divisor). The two cancellation conditions must both hold in a [noncommutative ring](commutative-algebra.md#noncommutative-ring). Products of regular elements remain regular.

## Semi-local ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semi-local_ring)

A [ring](commutative-algebra.md#ring) is semilocal when its quotient by the [Jacobson radical](#jacobson-radical) is a [semisimple ring](commutative-algebra.md#semisimple-ring) that is [Artinian](algebra.md#artinian-ring). Equivalently, that quotient is a [right Artinian ring](#right-artinian-ring): it has zero [Jacobson radical](#jacobson-radical), and the Artinian structure theorem makes it semisimple. A commutative [ring](commutative-algebra.md#ring) is semilocal exactly when it has finitely many [maximal ideals](commutative-algebra.md#maximal-ideal).

### Surjectivity from injectivity modulo the Jacobson radical

↑ **Parent:** [Semi-local ring](#semi-local-ring)

For a [finitely generated module](module-theory.md#finitely-generated-module) $V$ on the right over a [semilocal ring](#semi-local-ring), the displayed condition makes the induced [module endomorphism](module-theory.md#module-endomorphism) on $V/VJ$ [injective](algebra.md#injective-function). This quotient is an [Artinian module](module-theory.md#artinian-module), so [Artinian modules are co-Hopfian](module-theory.md#artinian-modules-are-co-hopfian) makes that map [surjective](algebra.md#surjective-function). The remaining [quotient module](module-theory.md#quotient-module) $V/\alpha(V)$ equals its product with $J$, and [Nakayama lemma](mathematics.md#nakayama-lemma) makes it zero.

## Generalized Weyl algebra

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

For a ring $D$, an automorphism $\sigma$ and central $t$, adjoin $X,Y$ with $Xd=\sigma(d)X$, $Yd=\sigma^{-1}(d)Y$, $YX=t$ and $XY=\sigma(t)$. This construction includes [Weyl algebras](#weyl-algebra) and rank-one [universal enveloping algebras](lie-algebra.md#universal-enveloping-algebra).

### Krull dimension criterion for rank-one generalized Weyl algebras

↑ **Parent:** [Generalized Weyl algebra](#generalized-weyl-algebra)

For a commutative Noetherian base $D$ of finite dimension $d$, the [noncommutative Krull dimension](#noncommutative-krull-dimension) of $D(\sigma,t)$ equals $d$ unless a height-$d$ maximal ideal is periodic under $\sigma$ or contains infinitely many translates $\sigma^n(t)$. This is the commutative-base specialization of Theorem 5.3 in [Krull dimension of Generalized Weyl Algebras with non-commutative coefficients](https://webhomes.maths.ed.ac.uk/~tom/KdimGWA.pdf).

## Noncommutative Krull dimension

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

Set the dimension of the zero module to $-1$. A nonzero module has dimension zero exactly when it is an [Artinian module](module-theory.md#artinian-module). Inductively, dimension at most $d$ means that in every descending chain the successive quotients eventually have dimension less than $d$. The least such ordinal is the Krull dimension; the ordinal definition also covers dimensions beyond finite integers. The left dimension of a ring is that of its left regular [module](module-theory.md#module-mathematics). In noncommutative rings this is not defined simply as the length of a chain of two-sided prime ideals.

## Noncommutative domain

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A noncommutative domain is a nonzero unital [ring](commutative-algebra.md#ring) without zero divisors; commutativity is not required, but commutative [integral domains](commutative-algebra.md#integral-domain) are included in this usage. Left and right cancellation hold for nonzero elements. A [right Noetherian domain](#right-noetherian-domain) embeds in a [division ring](commutative-algebra.md#division-ring) by the [right Ore condition](#right-ore-condition).

## Quantum plane

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

For a [field](algebra.md#field) $k$ and $q\in k^\times$, the quantum plane is $k_q[X,Y]=k\langle X,Y\rangle/(YX-qXY)$. Its ordered [monomials](polynomial.md#monomial) $X^iY^j$, $i,j\geq0$, are a [basis](vector-space.md#basis), and their multiplication is $X^iY^jX^uY^v=q^{ju}X^{i+u}Y^{j+v}$. Leading [monomials](polynomial.md#monomial) show it is a [noncommutative domain](#noncommutative-domain). Some sources interchange $q$ with $q^{-1}$ in the defining relation.

### Quantum enveloping algebra action on the quantum plane

↑ **Parent:** [Quantum plane](#quantum-plane)

For $yx=qxy$, the [quantum enveloping algebra of sl2](algebra.md#quantum-enveloping-algebra-of-sl2) acts by $K(x^ry^s)=q^{r-s}x^ry^s$, $E(x^ry^s)=[s]_qx^{r+1}y^{s-1}$ and $F(x^ry^s)=[r]_qx^{r-1}y^{s+1}$. Negative exponents here have zero coefficients and are omitted. The [quantum integer](algebra.md#quantum-integer) identity $[r][s+1]-[s][r+1]=[r-s]$ verifies the commutator. These operations preserve total degree and make the [quantum plane](#quantum-plane) a [module algebra](algebra.md#module-algebra).

#### Cubic-root quantum-plane socle

↑ **Parent:** [Quantum enveloping algebra action on the quantum plane](#quantum-enveloping-algebra-action-on-the-quantum-plane)

At a primitive cube [root of unity](algebra.md#root-of-unity), the cubic homogeneous [module](module-theory.md#module-mathematics) has [basis](vector-space.md#basis) $x^3,x^2y,xy^2,y^3$. Its only [simple modules](module-theory.md#irreducible-module) occurring as [submodules](module-theory.md#submodule) are the one-dimensional subspaces of $\langle x^3,y^3\rangle$, on which $K=1$ and $E=F=0$. Its quotient by this two-dimensional [submodule](module-theory.md#submodule) is simple, but it has no simple complement: any lift of the highest $K$ [weight space](semisimple-lie-algebra.md#weight-space) contains $x^2y$, whose $E$ image is $x^3\ne0$. Thus the cubic [module](module-theory.md#module-mathematics) is not a [semisimple module](module-theory.md#semisimple-module).

### Quantum Laurent plane

↑ **Parent:** [Quantum plane](#quantum-plane)

For $q\ne0$, define a vector space with basis $u^iv^j$, $i\in\mathbb Z$, $j\ge0$, and product $(u^iv^j)(u^kv^\ell)=q^{-jk}u^{i+k}v^{j+\ell}$. Bilinearity of the exponent verifies associativity. This constructs the algebra and proves the basis independently of its presentation. It localizes the [quantum plane](#quantum-plane) at powers of $u$ and gives a quotient witness for noncommutativity and noncocommutativity of the [coordinate Hopf algebra of quantum SL2](algebra.md#coordinate-hopf-algebra-of-quantum-sl2).

### Quantum torus

↑ **Parent:** [Quantum plane](#quantum-plane)

The two-dimensional quantum torus is the [algebra](algebra.md) with invertible generators $X,Y$ and relation $YX=qXY$, for $q\in k^\times$. Its [basis](vector-space.md#basis) consists of $X^iY^j$ with $i,j\in\mathbb Z$, with the same multiplication rule as the [quantum plane](#quantum-plane). It is a [right Noetherian ring](#right-noetherian-ring): successive adjunction of $X^{-1}$, $Y$, and $Y^{-1}$ satisfies the hypotheses of the [noncommutative Hilbert basis theorem](#noncommutative-hilbert-basis-theorem).

## Right Artinian ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A [ring](commutative-algebra.md#ring) is right Artinian if its [right ideals](associative-algebra.md#right-ideal) satisfy the [descending chain condition](algebra.md#descending-chain-condition), equivalently its right regular [module](module-theory.md#module-mathematics) is an [Artinian module](module-theory.md#artinian-module). Left and right chain conditions should be distinguished for a general [ring](commutative-algebra.md#ring).

### Right Artinian triangular ring that is not left Noetherian

↑ **Parent:** [Right Artinian ring](#right-artinian-ring)

Let $K/k$ be an infinite-dimensional field extension. For the triangular ring in the display, the right regular module has length three: $e_1T$ has its off-diagonal simple submodule and simple quotient, and $e_2T$ is simple. Thus $T$ is right Artinian. Its off-diagonal ideal is, on the left, the infinite-dimensional $k$-vector space $K$. Every $k$-subspace determines a left ideal, so an ascending sequence of finite-dimensional subspaces violates left Noetherianity. For example take $K=k(z)$ and the spans of $1,z,\ldots,z^m$.

### Semisimplicity of a right Artinian ring with zero radical

↑ **Parent:** [Right Artinian ring](#right-artinian-ring)

The finite intersections of [maximal right ideals](associative-algebra.md#maximal-right-ideal) of a [right Artinian ring](#right-artinian-ring) have a minimal member by the [descending chain condition](algebra.md#descending-chain-condition). Intersecting it with any other maximal right ideal changes nothing, so it equals the [Jacobson radical](#jacobson-radical). If that radical is zero, the diagonal map from the regular [module](module-theory.md#module-mathematics) into a finite direct sum of its simple quotients is injective. A submodule of a finite direct sum of simple modules is semisimple and has finite length. This proves semisimplicity of the regular module without assuming Noetherianity first.

### Hopkins-Levitzki theorem

↑ **Parent:** [Right Artinian ring](#right-artinian-ring)

A [right Artinian ring](#right-artinian-ring) is a [right Noetherian ring](#right-noetherian-ring). Its right regular [module](module-theory.md#module-mathematics) therefore has finite [composition length](finite-group-theory.md#composition-length). Its [Jacobson radical](#jacobson-radical) is a [nilpotent ideal](commutative-algebra.md#nilpotent-ideal), and its quotient by that [Jacobson radical](#jacobson-radical) is a [semisimple ring](commutative-algebra.md#semisimple-ring). In particular every finitely generated right [module](module-theory.md#module-mathematics) over such a [ring](commutative-algebra.md#ring) has finite [composition length](finite-group-theory.md#composition-length).

#### Minimal-right-ideal proof of radical nilpotence

↑ **Parent:** [Hopkins-Levitzki theorem](#hopkins-levitzki-theorem)

In a [right Artinian ring](#right-artinian-ring), the powers of its [Jacobson radical](#jacobson-radical) stabilize at an ideal $I$ satisfying $I^2=I$. If $I\ne0$, choose a minimal [right ideal](associative-algebra.md#right-ideal) $K$ with $KI\ne0$. Since $(KI)I=KI$, minimality gives $KI=K$. Choosing $k\in K$ with $kI\ne0$ gives $K=kR$ by the same minimality. Consequently $k=kj$ for some $j\in J(R)$. The [unit criterion for the Jacobson radical](#unit-criterion-for-the-jacobson-radical) makes $1-j$ invertible, forcing $k=0$, a contradiction. This proof avoids incorrectly applying the finitely generated form of [Nakayama lemma](mathematics.md#nakayama-lemma) to an arbitrary Artinian module.

## Left Noetherian ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A ring is left Noetherian when every ascending chain of left ideals stabilizes, equivalently when every left ideal is finitely generated.

## Right Noetherian ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A ring is right Noetherian when every ascending chain of right ideals stabilizes.

### Finite-module extension preserves Noetherianity

↑ **Parent:** [Right Noetherian ring](#right-noetherian-ring)

Suppose $A\subseteq B$ are unital [rings](commutative-algebra.md#ring) and $B$ is a [finitely generated module](module-theory.md#finitely-generated-module) over $A$ on the right. If $A$ is a [right Noetherian ring](#right-noetherian-ring), then $B_A$ is a [Noetherian module](algebra.md#noetherian-module). Every [right ideal](associative-algebra.md#right-ideal) of $B$ is an $A$-[submodule](module-theory.md#submodule), hence has finitely many generators over $A$; these also generate it over $B$. Thus $B$ is a [right Noetherian ring](#right-noetherian-ring). The same argument works on the left under the corresponding hypotheses. Finite-index [group ring](commutative-algebra.md#group-ring) extensions give an important example, using coset representatives as a finite module basis.

### Right Noetherian domain

↑ **Parent:** [Right Noetherian ring](#right-noetherian-ring)

A [noncommutative domain](#noncommutative-domain) whose [right ideals](associative-algebra.md#right-ideal) satisfy the [ascending chain condition](algebra.md#ascending-chain-condition) is a right Noetherian domain. Its right regular [module](module-theory.md#module-mathematics) is a [uniform module](module-theory.md#uniform-module), so any two nonzero principal [right ideals](associative-algebra.md#right-ideal) intersect. Thus its nonzero elements satisfy the [right Ore condition](#right-ore-condition) and it embeds in a [division ring](commutative-algebra.md#division-ring) by [Ore localization](#ore-localization).

### Noncommutative Hilbert basis theorem

↑ **Parent:** [Right Noetherian ring](#right-noetherian-ring)

If an [algebra](algebra.md) $B$ is generated by a subalgebra $A$ that is a [right Noetherian ring](#right-noetherian-ring) and one element $x$, and $A+xA=A+Ax$, then $B$ is a [right Noetherian ring](#right-noetherian-ring). The proof uses $F_n=\sum_{i\leq n}Ax^i=\sum_{i\leq n}x^iA$ and, for each [right ideal](associative-algebra.md#right-ideal) $I$, the ascending [right ideals](associative-algebra.md#right-ideal) $L_n=\{a:ax^n\in I+F_{n-1}\}$. After these stabilize, finitely many lifts of generators for $L_0,\ldots,L_N$ generate $I$ by induction on degree. Neither unique normal forms nor an [automorphism](algebra.md#automorphism) moving coefficients is required.

#### Leading-coefficient proof for a central polynomial extension

↑ **Parent:** [Noncommutative Hilbert basis theorem](#noncommutative-hilbert-basis-theorem)

For a right ideal $I\subseteq R[t]$, let $L_d$ be the set of degree-$d$ coefficients of its elements of degree at most $d$. These are right ideals of $R$, and multiplication by the central variable makes $L_d\subseteq L_{d+1}$. They stabilize, and every $L_d$ before stabilization is finitely generated. Choose polynomial lifts of those generators. Subtracting a suitable right linear combination of the lifts, shifted by powers of $t$, cancels the leading coefficient of any element of $I$. Induction on degree proves that the finitely many chosen lifts generate $I$.

// Destination: noncommutative-algebra.bigb

#### Skew Hilbert basis theorem

↑ **Parent:** [Noncommutative Hilbert basis theorem](#noncommutative-hilbert-basis-theorem)

For an [automorphism](algebra.md#automorphism) $\sigma$ of a [left Noetherian ring](#left-noetherian-ring) $A$, the [skew polynomial ring of an automorphism](commutative-algebra.md#skew-polynomial-ring-of-an-automorphism) $A[t;\sigma]$ is left [Noetherian](algebra.md#noetherian-ring). For a [left ideal](associative-algebra.md#left-ideal) $L$, the normalized leading-coefficient ideals $I_n=\{\sigma^{-n}(a_n):\sum_{j=0}^n a_jt^j\in L\}$ form an ascending chain of [left ideals](associative-algebra.md#left-ideal) of $A$. Choose finite generating lifts through the stabilization degree. Every element of $L$ has its leading coefficient cancelled by a suitable left multiple of one of these lifts, and induction on degree proves finite generation. Passing to the [skew Laurent polynomial ring](commutative-algebra.md#skew-laurent-polynomial-ring) preserves the property by clearing negative powers. The right-sided statement follows by applying the argument to the [opposite ring](commutative-algebra.md#opposite-ring).

## Weyl algebra

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weyl_algebra)

The first Weyl algebra is $A_1(k)=k\langle x,y\rangle/(yx-xy-1)$, the algebra of polynomial-coefficient differential operators in one variable.

### Order filtration of a Weyl algebra

↑ **Parent:** [Weyl algebra](#weyl-algebra)

For the relative [differential operators](analysis.md#differential-operator) over $\mathbb C$ on a polynomial ring, coordinates have order zero and partial derivatives have order one. The [associated graded ring](commutative-algebra.md#associated-graded-ring) is $\mathbb C[x,\xi]$ with degrees zero for $x_i$ and one for $\xi_i$. This differs from the [Bernstein filtration](#bernstein-filtration), in which both sets of generators have degree one and every filtration piece is finite-dimensional.

### Simplicity of a Weyl algebra in characteristic zero

↑ **Parent:** [Weyl algebra](#weyl-algebra)

In a nonzero two-sided ideal choose an element of least [Bernstein filtration](#bernstein-filtration) degree. Commuting it with any position or differentiation generator lowers degree, so all such commutators vanish. The [ordered monomial basis of a Weyl algebra](#ordered-monomial-basis-of-a-weyl-algebra) and characteristic zero then force it to be a nonzero scalar. The ideal is the whole ring. The argument fails in positive characteristic, when powers of the generators can be central.

### Ordered monomial basis of a Weyl algebra

↑ **Parent:** [Weyl algebra](#weyl-algebra)

The defining [commutators](lie-algebra.md#commutator) $[\partial_i,x_j]=\delta_{ij}$ reorder every word into the displayed monomials. Over a characteristic-zero field, the polynomial representation proves independence: iterated commutation with the coordinate multiplications extracts a highest derivative coefficient, multiplied by the nonzero factorial $\beta!$. Hence the representation is faithful and every polynomial-coefficient operator has a unique ordered expression.

### Weyl algebra in positive characteristic

↑ **Parent:** [Weyl algebra](#weyl-algebra)

In characteristic $p>0$, multiplication by $x_i$ and formal differentiation by $x_i$ act on the displayed vector space, because differentiation preserves the ideal generated by the $p$th powers. They satisfy the [Weyl algebra](#weyl-algebra) relations and yield a nonzero module of dimension $p^n$. The central elements $x_i^p$ and $\partial_i^p$ also show why the characteristic-zero simplicity argument cannot apply. In particular the characteristic-zero [Bernstein inequality for Weyl algebra modules](associative-algebra.md#bernstein-inequality-for-weyl-algebra-modules) fails for this finite-dimensional module.

// Destination: module-theory.bigb

### Weyl algebra has no nonzero finite-dimensional modules

↑ **Parent:** [Weyl algebra](#weyl-algebra)

For the complex [Weyl algebra](#weyl-algebra) $A_n$ with $n\geq1$, a unital finite-dimensional [module](module-theory.md#module-mathematics) would give matrices satisfying $[\partial_1,x_1]=I$. Their [matrix trace](linear-algebra.md#matrix-trace) gives $0=\dim_\mathbb C M$, so the [module](module-theory.md#module-mathematics) is zero. Characteristic zero and $n\geq1$ are essential.

### Bernstein filtration

↑ **Parent:** [Weyl algebra](#weyl-algebra)

Give both position and differentiation generators of a [Weyl algebra](#weyl-algebra) degree one. The ordered [monomial](polynomial.md#monomial) [basis](vector-space.md#basis) gives $\dim F_jA_n=\binom{j+2n}{2n}$ and $\operatorname{gr}_F A_n$ equal to a polynomial ring in $2n$ variables. Commuting a filtered element with any generator lowers its degree by at least one.

## Primitive ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_ring)

A left primitive ring has a faithful simple left module.

### Jacobson density theorem

↑ **Parent:** [Primitive ring](#primitive-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobson_density_theorem)

If $V$ is a simple left $R$-module and $D=\operatorname{End}_R(V)^{\mathrm{op}}$, then every prescribed map on a finite $D$-linearly independent subset of $V$ is induced by an element of $R$.

## Morita equivalence

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Morita_equivalence)

Morita-equivalent rings have equivalent module categories. In particular, $R$ and $\operatorname{Mat}_n(R)$ are Morita equivalent.

## Jacobson radical

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobson_radical)

The Jacobson radical is the intersection of all maximal left ideals, equivalently the intersection of the annihilators of all simple left modules.

### Jacobson radical as greatest quasinilpotent ideal

↑ **Parent:** [Jacobson radical](#jacobson-radical)

The [unit criterion for the Jacobson radical](#unit-criterion-for-the-jacobson-radical) implies that every radical element is a [quasinilpotent element](banach-algebra.md#quasinilpotent-element), because $1-x/\lambda$ is invertible for every nonzero $\lambda$. Conversely, if a two-sided [ideal](commutative-algebra.md#ideal) consists of quasinilpotent elements, then $yx$ is quasinilpotent for every member $x$ and every $y\in A$. Hence $1+yx$ is invertible and $x$ lies in the [Jacobson radical](#jacobson-radical). The maximality statement concerns ideals contained in the quasinilpotent set, not the whole set itself.

### Jacobson radical is independent of handedness

↑ **Parent:** [Jacobson radical](#jacobson-radical)

The intersection of [maximal left ideals](associative-algebra.md#maximal-left-ideal) is the intersection of annihilators of [simple modules](module-theory.md#irreducible-module) on the left, hence is a two-sided [ideal](commutative-algebra.md#ideal). If $j$ belongs to it, $1-rj$ has a left inverse for every $r$. Its left inverse also differs from $1$ by a radical element and has a left inverse; this makes the original inverse two-sided. The identity $(1-ba)^{-1}=1+b(1-ab)^{-1}a$ then shows that $1-jr$ is invertible too. If $j$ were outside a [maximal right ideal](associative-algebra.md#maximal-right-ideal) $I$, one would have $1-jr\in I$ for some $r$, a contradiction. Applying the same argument to the [opposite ring](commutative-algebra.md#opposite-ring) proves equality.

### Unit criterion for the Jacobson radical

↑ **Parent:** [Jacobson radical](#jacobson-radical)

The [Jacobson radical](#jacobson-radical) is the intersection of the ideals $\operatorname{Ann}_R(S)$ over all [simple modules](module-theory.md#irreducible-module), where $\operatorname{Ann}$ is the [annihilator of a module](module-theory.md#annihilator-of-a-module), so it is a two-sided [ideal](commutative-algebra.md#ideal). If $y\in J(R)$, the [left ideal](associative-algebra.md#left-ideal) $R(1-y)$ cannot be proper, since a containing maximal left ideal would also contain $y$ and hence $1$. Thus $c(1-y)=1$ for some $c$. Now $c=1+cy$ also differs from $1$ by a radical element and has a left inverse $d$. Multiplying $c(1-y)=1$ by $d$ gives $d=1-y$, and hence $(1-y)c=1$. This proves the unit assertion. Conversely, if $x$ is outside a maximal left ideal $L$, then $ax+l=1$ for some $a\in R$, $l\in L$. Consequently $1-ax\in L$ cannot be a [unit](algebra.md#unit-in-a-ring), proving the reverse direction.

### Nilpotent ideal with semisimple quotient radical criterion

↑ **Parent:** [Jacobson radical](#jacobson-radical)

If $I$ is a [nilpotent ideal](commutative-algebra.md#nilpotent-ideal) and $J(A/I)=0$, then $I=J(A)$. Every $1-ax$, $x\in I$, has a finite geometric-series inverse, giving $I\subseteq J(A)$. The radical's image lies in $J(A/I)=0$, giving the reverse inclusion. A [semisimple algebra](associative-algebra.md#semisimple-algebra) as quotient supplies the required zero radical.

### Jacobson radical under an integral extension

↑ **Parent:** [Jacobson radical](#jacobson-radical)

For an [integral extension](commutative-algebra.md#integral-extension) $A\subseteq B$ of commutative rings,

$$
J(A)=J(B)\cap A.
$$

Contraction sends maximal ideals of $B$ to maximal ideals of $A$, while the [Lying-over theorem](commutative-algebra.md#lying-over-theorem) puts a maximal ideal of $B$ over every maximal ideal of $A$.

### Jacobson ring

↑ **Parent:** [Jacobson radical](#jacobson-radical)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobson_ring)

A commutative ring $R$ is Jacobson when every [prime ideal](commutative-algebra.md#prime-ideal) is the intersection of the maximal ideals containing it. Equivalently, for every ideal $I$, its [radical](commutative-algebra.md#radical-of-an-ideal) is the intersection of the maximal ideals containing $I$.

#### Radical equality for finitely generated integer algebras

↑ **Parent:** [Jacobson ring](#jacobson-ring)

For a [finite-type integer algebra](commutative-algebra.md#finite-type-integer-algebra), a nonnilpotent element $r$ gives a nonzero [localization of a ring](commutative-algebra.md#localization-of-a-ring) $R[1/r]$. A [maximal ideal](commutative-algebra.md#maximal-ideal) there has finite [residue field](commutative-algebra.md#residue-field) by the [finite-field theorem for finitely generated integer algebras](commutative-algebra.md#finite-field-theorem-for-finitely-generated-integer-algebras). The image of $R$ in that [field](algebra.md#field) is a finite [integral domain](commutative-algebra.md#integral-domain), hence a [field](algebra.md#field). Its kernel is therefore maximal in $R$ and avoids $r$. Nilpotents lie in every [maximal ideal](commutative-algebra.md#maximal-ideal), proving the radical equality. Applying the same argument to every prime quotient shows that these algebras are [Jacobson rings](#jacobson-ring). Merely contracting a localized [maximal ideal](commutative-algebra.md#maximal-ideal) without the finite-image argument would not prove maximality.

#### Integral extension of a Jacobson ring

↑ **Parent:** [Jacobson ring](#jacobson-ring)

Every ring integral over a [Jacobson ring](#jacobson-ring) is Jacobson. After quotienting by a prime, an integral equation for a nonzero element has nonzero constant term; choose a maximal ideal of the base avoiding that term and apply the [Lying-over theorem](commutative-algebra.md#lying-over-theorem).

## Injective module

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Injective_module)

An injective module has the extension property for homomorphisms defined on submodules.

### Injective cogenerator of abelian groups

↑ **Parent:** [Injective module](#injective-module)

The divisible group $D=\mathbb Q/\mathbb Z$ is injective: every homomorphism $n\mathbb Z\to D$ extends to $\mathbb Z$ by choosing an $n$th division of its value at $n$, and the [Baer criterion](#baer-criterion) applies. It is a cogenerator because any nonzero element generates a cyclic subgroup admitting a character nonzero on that element, and injectivity extends that character to the whole group. Consequently a map $u:T\to U$ of abelian groups is injective exactly when restriction $U^*\to T^*$ is surjective: injectivity gives extension of characters, while a nonzero kernel element is detected by a character that cannot extend along $u$.

### Local criterion for injectivity over a Noetherian ring

↑ **Parent:** [Injective module](#injective-module)

For a [Noetherian ring](algebra.md#noetherian-ring), injectivity of a [module](module-theory.md#module-mathematics) can be tested at all prime localizations. By the [Baer criterion](#baer-criterion), test $\operatorname{Ext}^1_R(R/J,M)$ for every [ideal](commutative-algebra.md#ideal) $J$. [Localization of Ext over a Noetherian ring](algebra.md#localization-of-ext-over-a-noetherian-ring) identifies its localization with the corresponding [ideal](commutative-algebra.md#ideal) test over $R_P$. Every [ideal](commutative-algebra.md#ideal) of $R_P$ is extended from its contraction, and [localization detects zero elements](commutative-algebra.md#localization-detects-zero-elements) applies to the resulting Ext [module](module-theory.md#module-mathematics) even when it is not finitely generated. These observations prove both directions.

### Baer criterion

↑ **Parent:** [Injective module](#injective-module)

This criterion characterizes an [injective module](#injective-module) using extension from ideals. A left $R$-module is injective exactly when every homomorphism from a left ideal of $R$ extends to a homomorphism from $R$.

### Bass-Papp theorem

↑ **Parent:** [Injective module](#injective-module)

A ring is left Noetherian exactly when every direct sum of injective left modules is injective.

### Divisible module

↑ **Parent:** [Injective module](#injective-module)

Over an integral domain, a module $M$ is divisible when $rM=M$ for every nonzero $r$. A [divisible group](group.md#divisible-group) is precisely a divisible $\mathbb Z$-module, and over a principal ideal domain divisibility is equivalent to injectivity.

### Injective hull

↑ **Parent:** [Injective module](#injective-module)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Injective_hull)

The injective hull of a module $M$ is a minimal injective extension of $M$ in which $M$ is an essential submodule.

#### Injective hull of an Ore domain

↑ **Parent:** [Injective hull](#injective-hull)

For a domain satisfying the left [Ore condition](#ore-condition), its [division ring](commutative-algebra.md#division-ring) of fractions $Q$ is an injective essential extension of the left regular module. For a homomorphism $f:I\to Q$ on a nonzero left ideal, choose $a\in I\setminus\{0\}$. A common left multiple $sx=ta$ gives $sf(x)=tf(a)$, hence $f(x)=xa^{-1}f(a)$; right multiplication by $a^{-1}f(a)$ extends it. The [Baer criterion](#baer-criterion) proves injectivity. Clearing a left denominator proves essentiality. The same calculation gives $\operatorname{End}_R({}_RQ)\cong Q^{\rm op}$, with the opposite ring required because right multiplications compose in reversed order.

#### Local endomorphism ring of a uniform injective module

↑ **Parent:** [Injective hull](#injective-hull)

The [injective hull](#injective-hull) of a [uniform module](module-theory.md#uniform-module) is uniform. An injective endomorphism of a uniform injective module splits its image, so its complementary summand must vanish and it is an automorphism. Consequently all nonunits are precisely the noninjective endomorphisms. Their nonzero kernels are essential; intersection of two such kernels is nonzero, making their sum noninjective. Composition on either side preserves noninjectivity, unless the other map is a unit, which merely transports the kernel. Thus the nonunits form the unique maximal ideal, and the quotient is a [division ring](commutative-algebra.md#division-ring).

## Ore condition

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ore_condition)

The Ore condition is a common-multiple condition that permits fractions to be formed in a noncommutative ring.

### Ore theorem

↑ **Parent:** [Ore condition](#ore-condition)

A multiplicative set $S$ of [regular elements of a ring](#regular-element-of-a-ring) admits a right ring of fractions exactly when it satisfies the [right Ore condition](#right-ore-condition). The resulting localization embeds the original [ring](commutative-algebra.md#ring), inverts $S$, and expresses every element as $as^{-1}$. For denominators that can be [zero divisors](mathematics.md#zero-divisor), an additional denominator reversibility condition is required.

#### Right Noetherian domains satisfy the Ore condition

↑ **Parent:** [Ore theorem](#ore-theorem)

If two nonzero principal [right ideals](associative-algebra.md#right-ideal) in a [right Noetherian domain](#right-noetherian-domain) had zero intersection, the sums $bR\oplus abR\oplus\cdots\oplus a^mbR$ would be strictly increasing. Directness follows by splitting the lowest term into $bR$ and the other terms into $aR$, then cancelling $a$ and repeating. This contradicts the [ascending chain condition](algebra.md#ascending-chain-condition). A nonzero common element $au=bv$ gives the right [Ore condition](#ore-condition). The left version follows from the [opposite ring](commutative-algebra.md#opposite-ring). Consequently a [noncommutative domain](#noncommutative-domain) [Noetherian](algebra.md#noetherian-ring) on both sides has a single [division ring](commutative-algebra.md#division-ring) of fractions with both left and right fraction presentations.

#### Left Ore fraction construction

↑ **Parent:** [Ore theorem](#ore-theorem)

For a multiplicative set $S$ of regular elements satisfying the left Ore condition, represent a fraction by $(s,a)$. Pairs $(s,a)$ and $(t,b)$ agree when there are $u,v$ with $us=vt\in S$ and $ua=vb$. Addition uses this common denominator. For multiplication choose $v\in S,c\in R$ with $va=ct$, then $(s^{-1}a)(t^{-1}b)=(vs)^{-1}cb$. The Ore condition gives common multiples for successive operations; regularity supplies cancellation. In a domain with $S$ all nonzero elements, every nonzero fraction has inverse $a^{-1}s$.

// Destination: associative-algebra.bigb

### Right Ore condition

↑ **Parent:** [Ore condition](#ore-condition)

A multiplicative subset $S\subseteq A$ with $1\in S$ and $0\notin S$ of a [ring](commutative-algebra.md#ring) $A$ satisfies the right [Ore condition](#ore-condition) if for every $a\in A$ and $s\in S$ there are $u\in S$ and $b\in A$ such that $au=sb$. For a [noncommutative domain](#noncommutative-domain), taking $S=A\setminus\{0\}$ gives a [ring](commutative-algebra.md#ring) of right fractions $as^{-1}$; every nonzero fraction is invertible. The usual additional denominator reversibility condition is automatic when the elements of $S$ are nonzero in a [noncommutative domain](#noncommutative-domain).

#### Right denominator set

↑ **Parent:** [Right Ore condition](#right-ore-condition)

A multiplicative set $S$ containing $1$ and not $0$ is a right denominator set if it satisfies the [right Ore condition](#right-ore-condition) and right reversibility: $sr=0$, with $s\in S$, implies $rt=0$ for some $t\in S$. Its [Ore localization](#ore-localization) consists of right fractions $rs^{-1}$ and has kernel $\{r:rt=0\text{ for some }t\in S\}$. This condition permits zero-divisor denominators; it is automatic for a set of [regular elements of a ring](#regular-element-of-a-ring). When all denominators are regular, the localization map is injective.

#### Classical right ring of quotients

↑ **Parent:** [Right Ore condition](#right-ore-condition)

The classical right ring of quotients inverts all [regular elements of a ring](#regular-element-of-a-ring). Existence requires the [right Ore condition](#right-ore-condition) for these denominators. The original [ring](commutative-algebra.md#ring) embeds, every regular element becomes a [unit](algebra.md#unit-in-a-ring), and every fraction has a right denominator. The [right Ore condition](#right-ore-condition) also permits finitely many fractions to be placed over a common right denominator.

#### Right Ore set

↑ **Parent:** [Right Ore condition](#right-ore-condition)

A multiplicative [subset](set.md#subset) $S$ of a [ring](commutative-algebra.md#ring) is a right Ore set if $1\in S$, $0\notin S$ and it satisfies the [right Ore condition](#right-ore-condition). In a [noncommutative domain](#noncommutative-domain), this condition lets nonzero denominators be used in [Ore localization](#ore-localization).

### Ore localization

↑ **Parent:** [Ore condition](#ore-condition)

Ore localization extends localization to suitable multiplicative subsets of noncommutative rings.

#### Classical left ring of quotients

↑ **Parent:** [Ore localization](#ore-localization)

This is the localization of a [ring](commutative-algebra.md#ring) at all its [regular elements of a ring](#regular-element-of-a-ring), with left fractions. It exists precisely when those denominators satisfy the left [Ore condition](#ore-condition). If $R$ embeds in a ring $Q$, all regular elements become units in $Q$, and every element of $Q$ is such a fraction, the Ore condition follows by writing $rc^{-1}=s^{-1}b$, which gives $sr=bc$.

##### Matrix and triangular localization over an Ore domain

↑ **Parent:** [Classical left ring of quotients](#classical-left-ring-of-quotients)

Let $A$ be a domain satisfying both Ore conditions, with quotient [division ring](commutative-algebra.md#division-ring) $K$. A matrix over $A$ is regular exactly when it is invertible over $K$: a kernel vector of a singular matrix can have its denominators cleared to give a nonzero annihilator over $A$. An upper triangular matrix is regular exactly when all diagonal entries are nonzero. Each finite list of entries of a matrix over $K$ has a common left denominator $a\in A\setminus\{0\}$. Thus it is a fraction with denominator $aI_r$, proving the displayed classical localizations. The triangular localization retains its strictly upper triangular nilpotent ideal; it is not a semisimple matrix ring.

### Left Ore set

↑ **Parent:** [Ore condition](#ore-condition)

A multiplicative subset $S$ is left Ore when, for every $s\in S$ and $r\in R$, there are $s'\in S$ and $r'\in R$ such that $s'r=r's$.

## Prime ideal of a noncommutative ring

↑ **Parent:** [Noncommutative algebra](noncommutative-algebra.md)

A proper two-sided ideal $P$ of a noncommutative ring is prime when $AB\subseteq P$ for two-sided ideals $A,B$ implies $A\subseteq P$ or $B\subseteq P$.

### Prime ring

↑ **Parent:** [Prime ideal of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_ring)

A prime ring is a nonzero [ring](commutative-algebra.md#ring) whose zero ideal is a [prime ideal of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring). Equivalently, the product of any two nonzero two-sided [ideals](commutative-algebra.md#ideal) is nonzero. This condition is weaker than absence of zero divisors: a full matrix ring over a [division ring](commutative-algebra.md#division-ring) is prime even when its size is greater than one. For a commutative [ring](commutative-algebra.md#ring), primeness is exactly being an [integral domain](commutative-algebra.md#integral-domain).

### Prime radical of a noncommutative ring

↑ **Parent:** [Prime ideal of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring)

The prime radical is the intersection of all [prime ideals of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring). For a nonzero [ring](commutative-algebra.md#ring) satisfying the [ascending chain condition](algebra.md#ascending-chain-condition) on two-sided [ideals](commutative-algebra.md#ideal), there exist [prime ideals of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring) $P_1,\ldots,P_r$ with $P_1\cdots P_r=0$. Indeed, a maximal counterexample among two-sided [ideals](commutative-algebra.md#ideal) could not itself be a [prime ideal of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring), and two larger witness [ideals](commutative-algebra.md#ideal) would contradict its maximality. Every [prime ideal of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring) contains one $P_i$, so the intersection equals $\bigcap_iP_i$, and its $r$th power is zero. This nilpotence assertion fails without a chain condition.

#### Finite minimal primes and nilpotent prime radical

↑ **Parent:** [Prime radical of a noncommutative ring](#prime-radical-of-a-noncommutative-ring)

In a [left Noetherian ring](#left-noetherian-ring), [Noetherian induction](algebra.md#noetherian-induction) shows that every proper two-sided [ideal](commutative-algebra.md#ideal) contains a finite product of [prime ideals of a noncommutative ring](#prime-ideal-of-a-noncommutative-ring) that contain it. A maximal counterexample would be nonprime and contain a product of two strictly larger ideals; their prime products give the contradiction. Every prime over the original ideal contains a factor, so the inclusion-minimal factors give all its [minimal primes over an ideal](commutative-algebra.md#minimal-prime-over-an-ideal). Replacing each factor by a minimal prime beneath it gives a product of minimal primes inside the original ideal, with repetitions allowed. Applying this to zero makes a power of the [prime radical](#prime-radical-of-a-noncommutative-ring) zero.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
