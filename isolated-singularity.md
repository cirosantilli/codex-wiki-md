# Isolated singularity

↑ **Parent:** [Complex analysis](complex-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isolated_singularity)

An isolated singularity at $a$ is a point at which a function is not holomorphic although it is holomorphic throughout some punctured neighbourhood of $a$.

**Table of contents**

- [Classification of isolated singularities](#classification-of-isolated-singularities)
  - [Removable singularity](#removable-singularity)
    - [Riemann removable singularity theorem](#riemann-removable-singularity-theorem)
    - [Removable singularity at infinity](#removable-singularity-at-infinity)
    - [Uniform L2 circle bound for a removable singularity](#uniform-l2-circle-bound-for-a-removable-singularity)
  - [Pole](#pole)
    - [Simple pole](#simple-pole)
    - [Double pole](#double-pole)
    - [Meromorphic function](#meromorphic-function)
      - [Spherical derivative of a meromorphic function](#spherical-derivative-of-a-meromorphic-function)
        - [Finite spherical area criterion for an isolated singularity](#finite-spherical-area-criterion-for-an-isolated-singularity)
      - [Algebraic addition theorem](#algebraic-addition-theorem)
        - [Simply periodic entire function without an algebraic addition theorem](#simply-periodic-entire-function-without-an-algebraic-addition-theorem)
      - [Meromorphic functions on the sphere are rational](#meromorphic-functions-on-the-sphere-are-rational)
      - [Mittag-Leffler's theorem](#mittag-leffler-s-theorem)
      - [Polynomial growth forces a meromorphic function to be rational](#polynomial-growth-forces-a-meromorphic-function-to-be-rational)
      - [Nevanlinna theory](#nevanlinna-theory)
        - [Ahlfors covering surface theory](#ahlfors-covering-surface-theory)
          - [Length-area exhaustion of the complex plane](#length-area-exhaustion-of-the-complex-plane)
          - [Ahlfors second fundamental theorem](#ahlfors-second-fundamental-theorem)
            - [Ahlfors five islands theorem](#ahlfors-five-islands-theorem)
          - [Island of a meromorphic function](#island-of-a-meromorphic-function)
            - [Simple island](#simple-island)
          - [Average sheet number](#average-sheet-number)
        - [Nevanlinna second main theorem](#nevanlinna-second-main-theorem)
          - [Nevanlinna second main theorem in the unit disc](#nevanlinna-second-main-theorem-in-the-unit-disc)
          - [Five values force infinitely many simple preimages](#five-values-force-infinitely-many-simple-preimages)
        - [Nevanlinna logarithmic derivative lemma](#nevanlinna-logarithmic-derivative-lemma)
          - [Derivative growth outside a finite-measure set](#derivative-growth-outside-a-finite-measure-set)
        - [Nevanlinna ramification index](#nevanlinna-ramification-index)
        - [Nevanlinna deficiency](#nevanlinna-deficiency)
          - [Simultaneous deficiency and ramification for an exponential polynomial](#simultaneous-deficiency-and-ramification-for-an-exponential-polynomial)
        - [Nevanlinna first main theorem](#nevanlinna-first-main-theorem)
        - [Nevanlinna characteristic](#nevanlinna-characteristic)
          - [Growth order of a meromorphic function](#growth-order-of-a-meromorphic-function)
            - [Counting-order exceptions for a finite-order meromorphic function](#counting-order-exceptions-for-a-finite-order-meromorphic-function)
          - [Rational composition law for the Nevanlinna characteristic](#rational-composition-law-for-the-nevanlinna-characteristic)
        - [Nevanlinna integrated counting function](#nevanlinna-integrated-counting-function)
          - [Truncated Nevanlinna counting function](#truncated-nevanlinna-counting-function)
        - [Nevanlinna proximity function](#nevanlinna-proximity-function)
      - [Meromorphic function as a holomorphic map to the Riemann sphere](#meromorphic-function-as-a-holomorphic-map-to-the-riemann-sphere)
        - [Single-pole criterion for a spherical coordinate](#single-pole-criterion-for-a-spherical-coordinate)
      - [Rational map (complex analysis)](#rational-map-complex-analysis)
        - [Rational covering maps of the projective line](#rational-covering-maps-of-the-projective-line)
        - [Common-factor reduction of a rational map](#common-factor-reduction-of-a-rational-map)
        - [Rotational symmetry of a rational map](#rotational-symmetry-of-a-rational-map)
          - [Axially equivariant monomial rational map](#axially-equivariant-monomial-rational-map)
        - [Wronskian of a rational map](#wronskian-of-a-rational-map)
        - [Angular Jacobian of a rational map](#angular-jacobian-of-a-rational-map)
      - [Rational function](#rational-function)
        - [Padé approximant](#pade-approximant)
        - [Partial fraction decomposition](#partial-fraction-decomposition)
          - [Reciprocal-polynomial root identities](#reciprocal-polynomial-root-identities)
        - [Order of vanishing](#order-of-vanishing)
    - [Exponential of a pole is an essential singularity](#exponential-of-a-pole-is-an-essential-singularity)
  - [Essential singularity](#essential-singularity)
    - [Casorati-Weierstrass theorem](#casorati-weierstrass-theorem)
- [Non-isolated singularity](#non-isolated-singularity)
  - [Reciprocal cosine with accumulating poles](#reciprocal-cosine-with-accumulating-poles)
- [Zeros and poles](#zeros-and-poles)

## Classification of isolated singularities

↑ **Parent:** [Isolated singularity](isolated-singularity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classification_of_isolated_singularities)

An isolated singularity is removable, a pole, or essential according as its Laurent principal part has zero, finitely many nonzero, or infinitely many nonzero terms.

### Removable singularity

↑ **Parent:** [Classification of isolated singularities](#classification-of-isolated-singularities)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Removable_singularity)

An isolated singularity is removable when the function extends holomorphically across it, equivalently when its Laurent series has no negative-power terms.

#### Riemann removable singularity theorem

↑ **Parent:** [Removable singularity](#removable-singularity)

A holomorphic function bounded on a punctured neighbourhood extends holomorphically across the puncture.

This criterion characterizes a [removable singularity](#removable-singularity) of a holomorphic function; the criterion is a theorem about the singularity type.

#### Removable singularity at infinity

↑ **Parent:** [Removable singularity](#removable-singularity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Removable_singularity_at_infinity)

A holomorphic function tending to a finite limit at infinity becomes holomorphic at zero after reciprocal substitution.

#### Uniform L2 circle bound for a removable singularity

↑ **Parent:** [Removable singularity](#removable-singularity)

If $f$ is holomorphic on $0<|z|<R$ and

$$
\sup_{0<r<R}\int_0^{2\pi}|f(re^{i\theta})|^2\,d\theta<\infty,
$$

then the singularity at zero is removable. The Laurent coefficient formula and Cauchy--Schwarz give $|a_{-k}|=O(r^k)$ for each $k\geq1$, so every principal-part coefficient vanishes as $r\downarrow0$.

### Pole

↑ **Parent:** [Classification of isolated singularities](#classification-of-isolated-singularities)

A function has a pole of order $k$ at $a$ when $(z-a)^kf(z)$ extends holomorphically and is nonzero at $a$.

A [pole](#pole) is the negative-order case in the [zeros and poles](#zeros-and-poles) classification of a meromorphic function.

#### Simple pole

↑ **Parent:** [Pole](#pole)

A simple pole is a pole of order one. Its [residue](analysis.md#residue) is the nonzero value of the holomorphic extension of $(z-a)f(z)$ at the pole.

#### Double pole

↑ **Parent:** [Pole](#pole)

A double pole is a [pole](#pole) of order two. If $f(z)=g(z)/(z-a)^2$ with $g$ holomorphic near $a$, then $\operatorname{Res}_{z=a}f=g'(a)$.

#### Meromorphic function

↑ **Parent:** [Pole](#pole)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Meromorphic_function)

A meromorphic function is [holomorphic](complex-analysis.md#holomorphic-function) except at isolated [poles](#pole). Equivalently, it is locally a quotient of two holomorphic functions whose denominator is not identically zero.

##### Spherical derivative of a meromorphic function

↑ **Parent:** [Meromorphic function](#meromorphic-function)

For a [meromorphic function](#meromorphic-function) viewed as a [holomorphic map](complex-analysis.md#holomorphic-map) to the unit [Riemann sphere](complex-analysis.md#riemann-sphere), this is the length density of the pulled-back spherical metric. Its square is the pulled-back area density. At a [pole](#pole) use the coordinate $1/f$, which gives the same density. Some conventions omit the factor two and use a sphere of area $\pi$; all area normalizations must then change accordingly.

###### Finite spherical area criterion for an isolated singularity

↑ **Parent:** [Spherical derivative of a meromorphic function](#spherical-derivative-of-a-meromorphic-function)

A [meromorphic function](#meromorphic-function) on a punctured disk has finite pulled-back spherical area precisely when it extends to the [Riemann sphere](complex-analysis.md#riemann-sphere) at the puncture. A removable singularity or [pole](#pole) gives a smooth spherical extension and finite area. At an [essential singularity](#essential-singularity), the meromorphic version of the [Great Picard theorem](complex-analysis.md#great-picard-theorem) gives infinitely many preimages of all but at most two spherical targets. The [area formula](calculus.md#area-formula-geometric-measure-theory) then makes the area infinite. The logarithmically weighted annular area divided by $\log(1/r)$ tends to the total unweighted area divided by $4\pi$, by averaging a nondecreasing area function.

##### Algebraic addition theorem

↑ **Parent:** [Meromorphic function](#meromorphic-function)

A [meromorphic function](#meromorphic-function) $f$ has an [algebraic addition theorem](#algebraic-addition-theorem) if some nonzero [polynomial](polynomial.md) $P\in\mathbb C[U,V,W]$ satisfies $P(f(z),f(w),f(z+w))=0$ wherever the three values are finite. For a [polynomial](polynomial.md) $f$ of degree $d>0$, take roots $z_i$ of $f(z)-U$ and $w_j$ of $f(w)-V$; the product $\prod_{i,j}(W-f(z_i+w_j))$ has [polynomial](polynomial.md) coefficients in $U,V$ by the [Fundamental theorem of symmetric polynomials](polynomial.md#fundamental-theorem-of-symmetric-polynomials), is monic in $W$, and supplies an addition relation. An [elliptic function](complex-analysis.md#elliptic-function) also has such a relation, by finite [algebraic extension](algebra.md#algebraic-extension) of its [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety) and the [Weierstrass elliptic function](complex-analysis.md#weierstrass-elliptic-function) addition formula.

###### Simply periodic entire function without an algebraic addition theorem

↑ **Parent:** [Algebraic addition theorem](#algebraic-addition-theorem)

The displayed [entire function](complex-analysis.md#entire-function) has exactly the periods $2\pi i\mathbb Z$: a period $c$ would make $e^z(e^c-1)$ a constant integer multiple of $2\pi i$, forcing $e^c=1$. If a [polynomial](polynomial.md) addition relation existed, specialize its middle argument at a point with $e^c=\alpha>0$ irrational, avoiding the finitely many specializations making the entire [polynomial](polynomial.md) vanish. With $t=e^z$, the relation becomes a nonzero finite sum of exponentials $e^{(m+\alpha n)t}$. These real exponents are distinct, so the largest one dominates as $t\to+\infty$, a contradiction. This demonstrates that an [algebraic addition theorem](#algebraic-addition-theorem) is stronger than simple periodicity.

##### Meromorphic functions on the sphere are rational

↑ **Parent:** [Meromorphic function](#meromorphic-function)

[Poles](#pole) are isolated, including in the coordinate $w=1/z$ around infinity. [Compactness](topology.md#compact-space) of the [Riemann sphere](complex-analysis.md#riemann-sphere) therefore leaves only finitely many [poles](#pole). Subtract the finite principal parts at finite [poles](#pole) and the [polynomial](polynomial.md) principal part at infinity. The remainder is entire with a finite limit at infinity, hence bounded and constant by [Liouville's theorem](complex-analysis.md#liouville-theorem). The original function is a sum of a [polynomial](polynomial.md) and finitely many partial fractions, so is rational.

<h5 id="mittag-leffler-s-theorem">Mittag-Leffler's theorem</h5>

↑ **Parent:** [Meromorphic function](#meromorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mittag-Leffler's_theorem)

[Mittag-Leffler's theorem](#mittag-leffler-s-theorem) prescribes the [principal parts](complex-geometry.md#principal-part-of-a-meromorphic-function) of a [meromorphic function](#meromorphic-function). Given an [open subset](topology.md#open-set) $D$ of the complex plane, a subset $A$ having no accumulation point in $D$, and a finite sum of negative powers $P_a(z)=\sum_{j=1}^{m_a}c_{a,j}(z-a)^{-j}$ for each $a\in A$, there is a [meromorphic function](#meromorphic-function) on $D$ with exactly these [principal parts](complex-geometry.md#principal-part-of-a-meromorphic-function) and no other [poles](#pole). The difference of any two such [meromorphic functions](#meromorphic-function) is a [holomorphic function](complex-analysis.md#holomorphic-function) on $D$, because their [principal parts](complex-geometry.md#principal-part-of-a-meromorphic-function) cancel at every prescribed [pole](#pole).

##### Polynomial growth forces a meromorphic function to be rational

↑ **Parent:** [Meromorphic function](#meromorphic-function)

A [meromorphic function](#meromorphic-function) on the plane with $|f(z)|\leq C|z|^n$ outside a disc has no poles there and only finitely many poles inside. Subtract their finite [principal parts](complex-geometry.md#principal-part-of-a-meromorphic-function) to obtain an [entire function](complex-analysis.md#entire-function). For $n\geq0$, [Cauchy estimates](analysis.md#cauchy-estimate) make every derivative of order above $n$ vanish, so the remainder is a polynomial. For $n<0$ the remainder tends to zero at infinity and is zero by [Liouville theorem](complex-analysis.md#liouville-theorem). Adding back the principal parts gives a [rational function](#rational-function) in either case.

##### Nevanlinna theory

↑ **Parent:** [Meromorphic function](#meromorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nevanlinna_theory)

Nevanlinna theory studies the growth and value distribution of [meromorphic functions](#meromorphic-function) through their integrated pole counts and logarithmic proximity to target values. The [Nevanlinna characteristic](#nevanlinna-characteristic) combines both quantities, while the [Nevanlinna first main theorem](#nevanlinna-first-main-theorem) compares it with the corresponding counts and proximity for any fixed target.

###### Ahlfors covering surface theory

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

This theory compares the area, boundary length and [Euler characteristic](homology.md#euler-characteristic) of a surface mapped holomorphically to another surface, using the pulled-back metric. It extends covering-degree and [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) estimates when some boundary maps into the interior of the target. The [Ahlfors second fundamental theorem](#ahlfors-second-fundamental-theorem) and [Ahlfors five islands theorem](#ahlfors-five-islands-theorem) are important consequences.

###### Length-area exhaustion of the complex plane

↑ **Parent:** [Ahlfors covering surface theory](#ahlfors-covering-surface-theory)

For a nonconstant [meromorphic function](#meromorphic-function) on the plane, let $S(R)$ be its normalized pulled-back spherical area on $|z|<R$, and $L(R)$ the spherical length of its boundary image counted with [multiplicity](polynomial.md#multiplicity-mathematics). The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $L(R)^2\le8\pi^2R S'(R)$. If $L/S$ stayed above a positive constant for all large $R$, integration of $(1/S)'\le-c/R$ would make $1/S$ negative. Thus there are arbitrarily large radii with $L/S$ arbitrarily small, even when the total area is finite.

###### Ahlfors second fundamental theorem

↑ **Parent:** [Ahlfors covering surface theory](#ahlfors-covering-surface-theory)

For a finite simply connected covering surface over the [Riemann sphere](complex-analysis.md#riemann-sphere) and $q\ge3$ fixed separated [Jordan domains](topology.md#jordan-domain), let $n_j$ count its simply connected islands over the $j$th domain once each, regardless of mapping degree. Let $S$ be its [average sheet number](#average-sheet-number) and $L$ its spherical boundary length. The displayed inequality holds with $h$ depending only on the target domains. For regular bordered surfaces $f:X\to Y$, a general formulation is $\max\{-\chi(X),0\}\ge-S\chi(Y)-hL$, where $L$ counts only the boundary mapped into the interior of $Y$ and $\chi$ is the modern [Euler characteristic](homology.md#euler-characteristic). The boundary error disappears for an actual [branched covering](algebraic-topology.md#branched-covering). The covering-surface formulation is explained in [https://www.math.purdue.edu/~eremenko/dvi/ahl.pdf](https://www.math.purdue.edu/~eremenko/dvi/ahl.pdf) ; the simply connected island estimate is also recorded in Lemma 2 of [https://pdfs.semanticscholar.org/d247/562607e237af7c8fc6e683b77be6b94829fa.pdf](https://pdfs.semanticscholar.org/d247/562607e237af7c8fc6e683b77be6b94829fa.pdf) .

###### Ahlfors five islands theorem

↑ **Parent:** [Ahlfors second fundamental theorem](#ahlfors-second-fundamental-theorem)

Every nonconstant [meromorphic function](#meromorphic-function) on the complex plane has a [simple island](#simple-island) over at least one of any five [Jordan domains](topology.md#jordan-domain) on the [Riemann sphere](complex-analysis.md#riemann-sphere) with disjoint closures. The [Ahlfors second fundamental theorem](#ahlfors-second-fundamental-theorem), area comparison over target domains, and a [length-area exhaustion of the complex plane](#length-area-exhaustion-of-the-complex-plane) prove this: without a simple island every counted island has degree at least two, forcing $3S\le(5/2)S+O(L)$.

###### Island of a meromorphic function

↑ **Parent:** [Ahlfors covering surface theory](#ahlfors-covering-surface-theory)

An island over a [Jordan domain](topology.md#jordan-domain) $D$ is a relatively compact component $U$ of its inverse image on which the [meromorphic function](#meromorphic-function) is a [proper map](cohomology.md#proper-map) onto $D$. A component reaching the boundary of the source is instead a peninsula. The island has an integer mapping degree; degree one means that the map is a [biholomorphism](complex-analysis.md#biholomorphism). A simply connected island can have larger degree and need not be a simple island.

###### Simple island

↑ **Parent:** [Island of a meromorphic function](#island-of-a-meromorphic-function)

A simple island is an [island of a meromorphic function](#island-of-a-meromorphic-function) of mapping degree one. It is mapped [biholomorphically](complex-analysis.md#biholomorphism) onto the target [Jordan domain](topology.md#jordan-domain). This is stronger than the source island being simply connected.

###### Average sheet number

↑ **Parent:** [Ahlfors covering surface theory](#ahlfors-covering-surface-theory)

For a [holomorphic map](complex-analysis.md#holomorphic-map) between metric [Riemann surfaces](complex-analysis.md#riemann-surfaces), the average sheet number is the pulled-back source area divided by the target area. The [area formula](calculus.md#area-formula-geometric-measure-theory) identifies it with the average number of preimages counted with [multiplicity](polynomial.md#multiplicity-mathematics). The same definition over a target region $D$ gives $S_D=A_f(f^{-1}D)/A(D)$.

###### Nevanlinna second main theorem

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

For distinct fixed target values and a nonconstant [meromorphic function](#meromorphic-function), the truncated second main theorem has the displayed form, with $S_f=O(\log^+T_f+\log r)$ outside a set of finite linear measure. The [truncated Nevanlinna counting function](#truncated-nevanlinna-counting-function) retains only one unit at each preimage. For finite-order functions the error is $O(\log r)$; for transcendental functions it is $o(T_f)$ along the nonexceptional radii.

###### Nevanlinna second main theorem in the unit disc

↑ **Parent:** [Nevanlinna second main theorem](#nevanlinna-second-main-theorem)

For a nonconstant [meromorphic function](#meromorphic-function) on the [unit disc](topology.md#unit-disc) and $q\ge3$ distinct spherical values, this version of the [Nevanlinna second main theorem](#nevanlinna-second-main-theorem) holds outside a set $E$ with $\int_Edr/(1-r)<\infty$, as $r\uparrow1$. The [truncated Nevanlinna counting function](#truncated-nevanlinna-counting-function) counts distinct preimages rather than [multiplicity](polynomial.md#multiplicity-mathematics). The boundary-distance error is essential and need not be small relative to the characteristic. It follows from the disk [Nevanlinna logarithmic derivative lemma](#nevanlinna-logarithmic-derivative-lemma) and the growth lemma in the variable $\log(1/(1-r))$. The disk error estimate and weighted exceptional-set argument appear in [https://mathweb.tifr.res.in/Documents/Publications/Lectures/tifr17.pdf](https://mathweb.tifr.res.in/Documents/Publications/Lectures/tifr17.pdf) .

###### Five values force infinitely many simple preimages

↑ **Parent:** [Nevanlinna second main theorem](#nevanlinna-second-main-theorem)

If a transcendental [meromorphic function](#meromorphic-function) had only finitely many simple preimages over each of five distinct finite values, their simple counting functions would be $O(\log r)$. The displayed [multiplicity](polynomial.md#multiplicity-mathematics) inequality and the [Nevanlinna first main theorem](#nevanlinna-first-main-theorem) would bound the truncated sum by $5T_f/2+O(\log r)$. The [Nevanlinna second main theorem](#nevanlinna-second-main-theorem) requires at least $3T_f$ up to its $o(T_f)$ error, a contradiction. Thus at least one value has infinitely many simple preimages; four other values can remain totally ramified.

###### Nevanlinna logarithmic derivative lemma

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

For a nonconstant [meromorphic function](#meromorphic-function) on the plane, the displayed estimate holds outside an exceptional set of radii of finite linear measure, for large $r$. The [logarithmic derivative](analytic-number-theory.md#logarithmic-derivative) has only simple principal parts at zeros and [poles](#pole); [Poisson-Jensen formula](complex-analysis.md#poisson-jensen-formula) estimates and control of increasing auxiliary growth functions produce the logarithmic error. It supplies the error term in the [Nevanlinna second main theorem](#nevanlinna-second-main-theorem).

###### Derivative growth outside a finite-measure set

↑ **Parent:** [Nevanlinna logarithmic derivative lemma](#nevanlinna-logarithmic-derivative-lemma)

For a nonnegative increasing continuously differentiable function not identically zero, choose $x_0$ with $\phi(x_0)>0$. On $I=\{x\ge x_0:\phi'>\phi^2\}$, $1<\phi'/\phi^2$. Thus $|I|\le\int_{x_0}^\infty\phi'/\phi^2\le1/\phi(x_0)$. Adding the finite initial interval controls all exceptions. For the zero function there are none. Taking logarithms turns [derivative](calculus.md#derivative) growth into logarithmic auxiliary-function growth in value-distribution estimates.

###### Nevanlinna ramification index

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

The [Nevanlinna ramification index](#nevanlinna-ramification-index) is the normalized lower limiting integrated excess [multiplicity](polynomial.md#multiplicity-mathematics) over a target value, with [pole](#pole) orders used for infinity. It is an asymptotic value-distribution quantity, distinct from the integer [ramification index of a holomorphic map](complex-analysis.md#ramification-index-of-a-holomorphic-map) at one source point. It can be positive even when the target has positive [Nevanlinna deficiency](#nevanlinna-deficiency).

###### Nevanlinna deficiency

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

For a nonconstant [meromorphic function](#meromorphic-function), its deficiency at a point of the [Riemann sphere](complex-analysis.md#riemann-sphere) is the displayed asymptotic proportion missing from the full [Nevanlinna integrated counting function](#nevanlinna-integrated-counting-function). The [Nevanlinna first main theorem](#nevanlinna-first-main-theorem) bounds $N(r;a)$ by $T_f(r)+O(1)$ and identifies deficiency with the lower limiting normalized proximity. An omitted value has deficiency one.

###### Simultaneous deficiency and ramification for an exponential polynomial

↑ **Parent:** [Nevanlinna deficiency](#nevanlinna-deficiency)

The [rational composition law for the Nevanlinna characteristic](#rational-composition-law-for-the-nevanlinna-characteristic) gives $T_f(r)=3r/\pi+O(1)$. Its zeros are precisely $2\pi i\mathbb Z$, all of [multiplicity](polynomial.md#multiplicity-mathematics) two, so $N(r;0)=2r/\pi+O(\log r)$ and $\overline N(r;0)=r/\pi+O(\log r)$. Hence both its [Nevanlinna deficiency](#nevanlinna-deficiency) and [Nevanlinna ramification index](#nevanlinna-ramification-index) at zero equal one third.

###### Nevanlinna first main theorem

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

For a fixed finite target $a$, the displayed identity compares growth with proximity to and occurrences of $a$. If $g(z)=cz^\nu(1+O(z))$ near zero, where $\nu$ is its signed zero order, the exact reciprocal identity is $T(r,g)-T(r,1/g)=\log|c|$. It follows by factoring out zeros and poles on a disc, applying the [mean value property for harmonic functions](partial-differential-equation.md#mean-value-property-for-harmonic-functions) to the remaining nonvanishing factor, and using $\log^+u-\log^+(1/u)=\log u$. Translation changes $T$ by a bounded amount, proving the general assertion.

###### Nevanlinna characteristic

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

The characteristic of a [meromorphic function](#meromorphic-function) is the sum of its [Nevanlinna proximity function](#nevanlinna-proximity-function) and [Nevanlinna integrated counting function](#nevanlinna-integrated-counting-function). It treats large values and actual poles together. Replacing $f$ by $f-a$ changes the characteristic by at most $\log(1+|a|)$.

###### Growth order of a meromorphic function

↑ **Parent:** [Nevanlinna characteristic](#nevanlinna-characteristic)

The growth order of a [meromorphic function](#meromorphic-function) is the upper power exponent of its [Nevanlinna characteristic](#nevanlinna-characteristic), with constants assigned order zero. It is different from the local signed order at a zero or [pole](#pole). A [Nevanlinna integrated counting function](#nevanlinna-integrated-counting-function) has an analogous growth order. The [Nevanlinna first main theorem](#nevanlinna-first-main-theorem) bounds every counting order by the function order.

###### Counting-order exceptions for a finite-order meromorphic function

↑ **Parent:** [Growth order of a meromorphic function](#growth-order-of-a-meromorphic-function)

At most two values can have counting order smaller than a positive finite function order. Otherwise the [Nevanlinna second main theorem](#nevanlinna-second-main-theorem) with three such values bounds the characteristic by a smaller power outside a finite-length exceptional set. Monotonicity extends this bound to all large radii by choosing a good radius in $[r,r+1]$, contradicting the original order. Order zero is immediate from nonnegativity and the first theorem.

###### Rational composition law for the Nevanlinna characteristic

↑ **Parent:** [Nevanlinna characteristic](#nevanlinna-characteristic)

For a degree-$d$ [rational function](#rational-function) $U$ of the [Riemann sphere](complex-analysis.md#riemann-sphere), choose relatively prime homogeneous [polynomials](polynomial.md) $(P,Q)$ of degree $d$. Their joint norm on the unit three-sphere has positive lower and finite upper bounds. Thus $\log\|(P,Q)(v)\|-d\log\|v\|$ is bounded. Averaging over a circle using a nonvanishing entire homogeneous lift of a [meromorphic function](#meromorphic-function) proves the displayed law for the spherical characteristic. [Jensen's formula](complex-analysis.md#jensen-s-formula) and $0\le\tfrac12\log(1+x^2)-\log^+x\le\tfrac12\log2$ show that it also holds for the ordinary [Nevanlinna characteristic](#nevanlinna-characteristic).

###### Nevanlinna integrated counting function

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

The number $n(t,f)$ counts [poles](#pole) in $|z|<t$ with [multiplicity](polynomial.md#multiplicity-mathematics), and $n(0,f)$ is the pole order at zero. Thus $N(r,f)=n(0,f)\log r+\sum_{0<|p|<r}\log(r/|p|)$. Applying this to $1/(f-a)$ counts occurrences of the value $a$.

###### Truncated Nevanlinna counting function

↑ **Parent:** [Nevanlinna integrated counting function](#nevanlinna-integrated-counting-function)

The truncated counting function counts each distinct $a$-point of a [meromorphic function](#meromorphic-function) once, rather than with its local [multiplicity](polynomial.md#multiplicity-mathematics). It uses the same logarithmic radial weights as the [Nevanlinna integrated counting function](#nevanlinna-integrated-counting-function), including an origin contribution $\log r$ when appropriate. The difference $N-\overline N$ measures integrated excess [multiplicity](polynomial.md#multiplicity-mathematics).

###### Nevanlinna proximity function

↑ **Parent:** [Nevanlinna theory](#nevanlinna-theory)

Here $\log^+x=\max(0,\log x)$. The function $m(r,f)$ measures logarithmic proximity of $f$ to infinity. For a finite target $a$, proximity is $m(r,1/(f-a))$. Logarithmic singularities on a circle are integrable.

##### Meromorphic function as a holomorphic map to the Riemann sphere

↑ **Parent:** [Meromorphic function](#meromorphic-function)

A meromorphic function on a [Riemann surface](complex-analysis.md#riemann-surfaces) is equivalently a holomorphic map to the [Riemann sphere](complex-analysis.md#riemann-sphere), with every pole mapped to infinity. Composition with a rational self-map of the sphere is again such a holomorphic map.

###### Single-pole criterion for a spherical coordinate

↑ **Parent:** [Meromorphic function as a holomorphic map to the Riemann sphere](#meromorphic-function-as-a-holomorphic-map-to-the-riemann-sphere)

A nonconstant [meromorphic function](#meromorphic-function) on a compact [Riemann surface](complex-analysis.md#riemann-surfaces) with exactly one [simple pole](#simple-pole) gives a degree-one holomorphic map to the sphere. A degree-one map is a [biholomorphism](complex-analysis.md#biholomorphism). The surface therefore has genus zero and the function is a global rational coordinate.

##### Rational map (complex analysis)

↑ **Parent:** [Meromorphic function](#meromorphic-function)

A rational map of the [Riemann sphere](complex-analysis.md#riemann-sphere) is a quotient of two complex polynomials, extended to infinity. A nonconstant map has a well-defined positive degree and is a branched covering of the sphere.

###### Rational covering maps of the projective line

↑ **Parent:** [Rational map (complex analysis)](#rational-map-complex-analysis)

A degree-$m$ [rational map](#rational-map-complex-analysis) of the [complex projective line](algebraic-topology.md#complex-projective-line) is represented by two degree-at-most-$m$ polynomials without a common root, modulo common scalar multiplication. This is an open set of $\mathbb{CP}^{2m+1}$. Quotienting by domain [Möbius transformations](group-theory.md#mobius-transformation) subtracts three complex dimensions, giving real dimension $4m-4$ for degree $m\geq2$. These are the local covering parameters of a multiple-covered [J-holomorphic sphere](symplectic-geometry.md#j-holomorphic-sphere).

###### Common-factor reduction of a rational map

↑ **Parent:** [Rational map (complex analysis)](#rational-map-complex-analysis)

Cancel the common polynomial factors of $p$ and $q$ before computing the [degree of a rational map of the Riemann sphere](complex-analysis.md#degree-of-a-rational-map-of-the-riemann-sphere). Removable common zeros do not contribute sheets. The reduced maximum polynomial degree is the number of inverse images of a generic target value, counted with positive holomorphic local degrees.

###### Rotational symmetry of a rational map

↑ **Parent:** [Rational map (complex analysis)](#rational-map-complex-analysis)

Rotations of the domain and target [Riemann spheres](complex-analysis.md#riemann-sphere) act as [Möbius transformations](group-theory.md#mobius-transformation) represented by [SU(2) matrices](topological-group.md#su-2-matrix). A combined symmetry requires the equivariance identity $R(gz)=hR(z)$ for the corresponding transformations. Symmetry of the [Wronskian of a rational map](#wronskian-of-a-rational-map) alone is insufficient: it tests the ramification directions, not the entire map. Target rotations preserve the [angular Jacobian of a rational map](#angular-jacobian-of-a-rational-map), so an equivariant map has a domain-invariant angular density.

###### Axially equivariant monomial rational map

↑ **Parent:** [Rotational symmetry of a rational map](#rotational-symmetry-of-a-rational-map)

For positive integer $n$, $R(e^{i\alpha}z)=e^{in\alpha}R(z)$ and $R(1/z)=1/R(z)$. For $n>1$ its [angular Jacobian of a rational map](#angular-jacobian-of-a-rational-map) vanishes at the poles and has axial symmetry. Its combined rotational group is the group of [rotations preserving an axis](linear-algebra.md#rotations-preserving-an-axis); for $n=1$ it enlarges to all domain rotations paired with identical target rotations.

###### Wronskian of a rational map

↑ **Parent:** [Rational map (complex analysis)](#rational-map-complex-analysis)

For a reduced [rational map](#rational-map-complex-analysis) $R=p/q$, its derivative is $W/q^2$ with $W=p'q-pq'$. Away from target-coordinate poles, the zeros of this [Wronskian](differential-equation.md#wronskian) identify its [ramification points of a holomorphic map](complex-analysis.md#ramification-point-of-a-holomorphic-map); at a pole use the reciprocal coordinate $q/p$. A pole of order $m$ contributes ramification order $m-1$, and infinity must also be checked in local coordinates. For degree $N$ the [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) gives total ramification $2N-2$. The affine polynomial $W$ can have fewer finite zeros because some ramification lies at infinity. In the [rational map approximation for Skyrmions](classical-field-theory-soliton.md#rational-map-approximation-for-skyrmions), these directions have zero angular baryon density.

###### Angular Jacobian of a rational map

↑ **Parent:** [Rational map (complex analysis)](#rational-map-complex-analysis)

For a nonconstant [rational map](#rational-map-complex-analysis) between round unit [Riemann spheres](complex-analysis.md#riemann-sphere), $R^*d\Omega=J_Rd\Omega$. Counting inverse images with multiplicity gives $\int J_Rd\Omega=4\pi\deg R$. The [Jacobian determinant](calculus.md#jacobian-determinant) vanishes at [ramification points of a holomorphic map](complex-analysis.md#ramification-point-of-a-holomorphic-map), but the integral still records the global [degree of a holomorphic map](complex-analysis.md#degree-of-a-holomorphic-map).

##### Rational function

↑ **Parent:** [Meromorphic function](#meromorphic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_function)

A rational function is a quotient $p/q$ of [polynomials](polynomial.md), with $q$ nonzero. After cancelling common factors, it defines a [holomorphic map](complex-analysis.md#holomorphic-map) from the [Riemann sphere](complex-analysis.md#riemann-sphere) to itself.

<h6 id="pade-approximant">Padé approximant</h6>

↑ **Parent:** [Rational function](#rational-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Padé_approximant)

A Padé approximant is a [rational function](#rational-function) with numerator degree at most $m$ and denominator degree at most $n$, normalized by $Q_n(0)=1$, such that $Q_n(z)f(z)-P_m(z)=O(z^{m+n+1})$ near zero, when such an approximant exists. For the [exponential function](calculus.md#exponential-function), its $[1/1]$ approximant is $(1+z/2)/(1-z/2)$. Applying this rational function to a matrix gives the [Crank-Nicolson method](numerical-analysis.md#crank-nicolson-method). Diagonal and subdiagonal approximants also give stability functions of [Gauss collocation methods](numerical-analysis.md#gauss-legendre-method) and [Radau IIA methods](numerical-analysis.md#radau-iia-method) respectively.

###### Partial fraction decomposition

↑ **Parent:** [Rational function](#rational-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_fraction_decomposition)

Over a field in which the denominator splits, a proper rational function is a sum of terms $c/(x-a)^k$. The coefficient at a simple pole $a$ is obtained by multiplying by $x-a$ and evaluating at $a$.

###### Reciprocal-polynomial root identities

↑ **Parent:** [Partial fraction decomposition](#partial-fraction-decomposition)

Let $P$ be a monic [polynomial](polynomial.md) of positive degree $m\ge1$ with distinct [roots of a polynomial](polynomial.md#root-of-a-polynomial) $r_j$. The [partial fraction decomposition](#partial-fraction-decomposition)

$$
\frac1{P(z)}=\sum_{j=1}^m\frac1{P'(r_j)(z-r_j)}
$$

follows by matching the simple pole residues; the difference is entire and vanishes at infinity. Comparing its expansion there gives $\sum_jr_j^\ell/P'(r_j)=0$ for $0\le\ell<m-1$ and $\sum_jr_j^{m-1}/P'(r_j)=1$. These identities give the continuity and derivative jumps needed for constant-coefficient [Green functions](analysis.md#green-s-function).

###### Order of vanishing

↑ **Parent:** [Rational function](#rational-function)

The order of vanishing of a nonzero [rational function](#rational-function) $f$ at a point $p$ is the exponent of a local parameter in its local factorization. A negative order is the order of a pole.

The local multiplicity in [zeros and poles](#zeros-and-poles) is positive for a zero and negative for a pole; it is zero at a regular nonvanishing point.

#### Exponential of a pole is an essential singularity

↑ **Parent:** [Pole](#pole)

If $f$ has a pole at $a$, then $e^f$ has an essential singularity there. The exponential series produces infinitely many negative Laurent powers from the nonzero principal part of $f$.

### Essential singularity

↑ **Parent:** [Classification of isolated singularities](#classification-of-isolated-singularities)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Essential_singularity)

An isolated singularity is essential when its Laurent series has infinitely many nonzero negative-power terms.

#### Casorati-Weierstrass theorem

↑ **Parent:** [Essential singularity](#essential-singularity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Casorati–Weierstrass_theorem)

Near an isolated [essential singularity](#essential-singularity), a [holomorphic function](complex-analysis.md#holomorphic-function) has dense image in the complex plane. If it avoided a disk about $w$, then $1/(f-w)$ would be bounded and extend across the singularity by the [Riemann removable singularity theorem](#riemann-removable-singularity-theorem). If its extended value is nonzero, $f$ extends holomorphically; if zero, its finite-order zero makes $f$ a pole. Either contradicts an essential singularity.

## Non-isolated singularity

↑ **Parent:** [Isolated singularity](isolated-singularity.md)

A singularity is non-isolated when every punctured neighbourhood contains another singularity. An accumulation point of poles or essential singularities cannot itself be classified as a removable singularity, pole, or isolated essential singularity.

### Reciprocal cosine with accumulating poles

↑ **Parent:** [Non-isolated singularity](#non-isolated-singularity)

The function $1/\cos(1/z)$ has simple [poles](#pole) at $z=1/[\pi(n+1/2)]$, accumulating at zero. Its origin is therefore a [non-isolated singularity](#non-isolated-singularity), despite the underlying cosine of $1/z$ having an isolated essential singularity.

## Zeros and poles

↑ **Parent:** [Isolated singularity](isolated-singularity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zeros_and_poles)

[Zeros and poles](#zeros-and-poles) describe the positive and negative local orders of a meromorphic function. Locally $f(z)=(z-a)^m g(z)$ with $g$ holomorphic and nonzero at $a$: $m>0$ is a zero, $m<0$ is a pole, and $m=0$ is a regular nonzero value. A [simple pole](#simple-pole) has $m=-1$, and the [order of vanishing](#order-of-vanishing) records $m$.

## ↑ Ancestors (5)

1. [Complex analysis](complex-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#13e/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3.md#23f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#12g/a/solution)
- [Residue](analysis.md#residue)
