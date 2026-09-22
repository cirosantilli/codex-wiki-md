# Abelian variety

↑ **Parent:** [Algebraic group](algebraic-geometry.md#algebraic-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abelian_variety)

An abelian variety is a complete connected group variety. Despite its name, commutativity follows from completeness and the rigidity lemma.

**Table of contents**

- [Prime-to-characteristic torsion of an abelian variety](#prime-to-characteristic-torsion-of-an-abelian-variety)
- [Jacobian variety](#jacobian-variety)
  - [Torelli theorem](#torelli-theorem)
  - [Universal property of the Jacobian variety](#universal-property-of-the-jacobian-variety)
  - [Theta divisor](#theta-divisor)
    - [Riemann vanishing theorem](#riemann-vanishing-theorem)
      - [Theta pullback zero-divisor identity](#theta-pullback-zero-divisor-identity)
      - [Vector of Riemann constants](#vector-of-riemann-constants)
    - [Gauss map of a theta divisor](#gauss-map-of-a-theta-divisor)
      - [Branch locus of the theta Gauss map](#branch-locus-of-the-theta-gauss-map)
    - [Riemann singularity theorem](#riemann-singularity-theorem)
      - [Schur complement presentation of a theta singularity](#schur-complement-presentation-of-a-theta-singularity)
      - [Tangent cone to a theta divisor](#tangent-cone-to-a-theta-divisor)
    - [Theta autoduality of a Jacobian](#theta-autoduality-of-a-jacobian)
    - [Restriction of the theta divisor to an Abel curve](#restriction-of-the-theta-divisor-to-an-abel-curve)
    - [Determinant description of the theta divisor](#determinant-description-of-the-theta-divisor)
      - [Invertible cup-product direction for a line bundle on a curve](#invertible-cup-product-direction-for-a-line-bundle-on-a-curve)
      - [Evaluation determinant on a product of curves](#evaluation-determinant-on-a-product-of-curves)
        - [Torsion trivialization in a determinant quotient](#torsion-trivialization-in-a-determinant-quotient)
  - [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve)
    - [Derivative of the Abelian sum map](#derivative-of-the-abelian-sum-map)
      - [Repeated-point Abel differential formula](#repeated-point-abel-differential-formula)
- [Curve generation criterion for an abelian variety](#curve-generation-criterion-for-an-abelian-variety)
- [Dual abelian variety](#dual-abelian-variety)
  - [Weil pairing for an abelian variety](#weil-pairing-for-an-abelian-variety)
  - [Poincaré line bundle](#poincare-line-bundle)
- [Mumford rigidity lemma](#mumford-rigidity-lemma)
- [Invariant differential on a group scheme](#invariant-differential-on-a-group-scheme)
- [Theorem of the Cube](#theorem-of-the-cube)
  - [Arithmetic cube identity for Weil heights](#arithmetic-cube-identity-for-weil-heights)
  - [Cohomological proof of the cube theorem for elliptic curves](#cohomological-proof-of-the-cube-theorem-for-elliptic-curves)
  - [Bilinear cross-effect of a line bundle on an abelian variety](#bilinear-cross-effect-of-a-line-bundle-on-an-abelian-variety)
  - [Theorem of the square](#theorem-of-the-square)
    - [Homomorphism associated to a line bundle on an abelian variety](#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)
      - [Line bundle translation stabilizer](#line-bundle-translation-stabilizer)
      - [Identity component of the Picard group](#identity-component-of-the-picard-group)
        - [Seesaw theorem](#seesaw-theorem)

## Prime-to-characteristic torsion of an abelian variety

↑ **Parent:** [Abelian variety](abelian-variety.md)

If $N$ is invertible in the base [field](algebra.md#field), multiplication by $N$ on an [abelian variety](abelian-variety.md) is finite étale: its differential is $N$ times the identity, and properness turns its zero-dimensional fibres into finite fibres. The [Theorem of the Cube](#theorem-of-the-cube) gives $[N]^*L\cong L^{N^2}$ for a symmetric [ample line bundle](ringed-space.md#ample-line-bundle). Top [intersection products](algebraic-geometry.md#intersection-product-of-cartier-divisors) give degree $N^{2\dim A}$. For each prime power $\ell^r\mid N$, the kernels killed by $\ell^s$ have orders $\ell^{2s\dim A}$; the classification of [finite abelian groups](group.md#finite-abelian-group) forces $2\dim A$ cyclic factors of length $r$. Combining the prime powers gives the displayed group.

## Jacobian variety

↑ **Parent:** [Abelian variety](abelian-variety.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobian_variety)

The [Jacobian variety](#jacobian-variety) of a smooth projective [algebraic curve](algebraic-geometry.md#algebraic-curve) parametrizes degree-zero [line bundles](ringed-space.md#line-bundle). Its dimension is the genus of the [algebraic curve](algebraic-geometry.md#algebraic-curve). An effective degree-$d$ [Cartier divisor](cartier-divisor.md) defines a point in a degree-$d$ torsor through the [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve). The [theta divisor](#theta-divisor) induces an isomorphism with the [dual abelian variety](#dual-abelian-variety).

### Torelli theorem

↑ **Parent:** [Jacobian variety](#jacobian-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Torelli_theorem)

A [smooth projective curve](projective-space.md#smooth-projective-curve) over the [complex numbers](complex-analysis.md#complex-number) is determined up to isomorphism by its [Jacobian variety](#jacobian-variety) together with its canonical principal [polarization of a complex torus](complex-geometry.md#polarization-of-a-complex-torus). For genus at least three, the [branch locus of the theta Gauss map](#branch-locus-of-the-theta-gauss-map) recovers the canonical curve by [projective biduality theorem](projective-space.md#projective-biduality-theorem), or recovers the canonical [rational normal curve](projective-space.md#rational-normal-curve) and the branch points of a [hyperelliptic curve](algebraic-geometry.md#hyperelliptic-curve). In genus two the [theta divisor](#theta-divisor) itself is the curve; in genus one the [Jacobian variety](#jacobian-variety) is the curve after choosing an origin. The polarization is essential data in this statement.

### Universal property of the Jacobian variety

↑ **Parent:** [Jacobian variety](#jacobian-variety)

For a smooth connected projective curve $C$ with chosen basepoint $p$, the [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve) $i_p:C\to J(C)$ sends $q$ to $[q-p]$. Every morphism $g:C\to A$ to an [abelian variety](abelian-variety.md) with $g(p)=0$ factors uniquely through a homomorphism $J(C)\to A$. This universal property converts a curve embedded in an abelian variety into a homomorphism from its Jacobian.

### Theta divisor

↑ **Parent:** [Jacobian variety](#jacobian-variety)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theta_divisor)

The [theta divisor](#theta-divisor) consists of degree-$g-1$ [line bundles](ringed-space.md#line-bundle) with a nonzero [global section](ringed-space.md#global-section). It is the irreducible image of the [symmetric product of a curve](algebraic-geometry.md#symmetric-product-of-a-curve) $C^{(g-1)}$, with its reduced [Cartier divisor](cartier-divisor.md) structure. The [determinant description of the theta divisor](#determinant-description-of-the-theta-divisor) supplies equations, multiplicities and pullbacks in families.

#### Riemann vanishing theorem

↑ **Parent:** [Theta divisor](#theta-divisor)

For the period matrix of a genus-$g$ [compact Riemann surface](complex-analysis.md#compact-riemann-surface), there is a vector $\kappa$ depending on the marking and base point such that the [Riemann theta function](modular-function.md#riemann-theta-function) vanishes exactly on this translate of the image of the [Abelian sum map](#abel-map-of-an-algebraic-curve). Pairing sides of the cut surface proves that a nonzero pullback $\theta(u(p)-z)$ has a degree-$g$ zero [divisor](number-theory.md#divisor) whose Abel sum is $z+\kappa$. At a theta zero that pullback includes the base point. Irreducibility and dimension of the effective-divisor locus give equality of supports; the primitive [First Chern class](complex-geometry.md#first-chern-class) of the theta [line bundle](ringed-space.md#line-bundle) makes the [divisor](number-theory.md#divisor) reduced.

##### Theta pullback zero-divisor identity

↑ **Parent:** [Riemann vanishing theorem](#riemann-vanishing-theorem)

If $p\mapsto\theta(u(p)-z)$ is not identically zero, its zero [divisor](number-theory.md#divisor) $D_z$ has these properties. The logarithmic derivative changes by $-2\pi i\omega_j$ across the paired $b_j$ translation, giving zero count $g$. For a variation of $z$, the logarithm changes there by $2\pi i\delta z_j$; integrating by parts in the first-moment contour integral gives $\delta\operatorname{AJ}(D_z)=\delta z$. Thus the difference is constant. Weighted zero [divisors](number-theory.md#divisor), rather than a distinct-zero assumption, make the statement valid at collisions.

##### Vector of Riemann constants

↑ **Parent:** [Riemann vanishing theorem](#riemann-vanishing-theorem)

The vector of [Riemann constants](#vector-of-riemann-constants) is the parameter-independent class obtained from the zeros of $p\mapsto\theta(u(p)-z)$ using the displayed formula. Under this sign convention the [theta divisor](#theta-divisor) is $W_{g-1}-\kappa$. It depends on the base point and normalized symplectic marking; some accounts use its negative. Changing the marking or sign convention must also change the translation formula consistently.

#### Gauss map of a theta divisor

↑ **Parent:** [Theta divisor](#theta-divisor)

Translate the tangent hyperplane at a smooth point of the [theta divisor](#theta-divisor) to the identity of the [Jacobian variety](#jacobian-variety). Its annihilator defines the Gauss map. At $L=\mathcal O_X(D)$ with $h^0(L)=1$, the [derivative of the Abelian sum map](#derivative-of-the-abelian-sum-map) identifies this annihilator with the unique line $H^0(K_X(-D))$. Thus $\Gamma(L)=[\omega]$ implies $D\le\operatorname{div}(\omega)$. This connects the intrinsic geometry of the [theta divisor](#theta-divisor) to the [canonical map](algebraic-geometry.md#canonical-map) of the curve.

##### Branch locus of the theta Gauss map

↑ **Parent:** [Gauss map of a theta divisor](#gauss-map-of-a-theta-divisor)

Normalize the target in the [function field](algebraic-geometry.md#function-field-of-an-algebraic-variety) of the generically finite [Gauss map of a theta divisor](#gauss-map-of-a-theta-divisor); its finite map has an intrinsic branch locus. For a nonhyperelliptic [smooth projective curve](projective-space.md#smooth-projective-curve), this locus is the [projective dual variety](projective-space.md#projective-dual-variety) of the canonical curve. For a [hyperelliptic curve](algebraic-geometry.md#hyperelliptic-curve) of genus at least three, it is the union of the dual hypersurface of its canonical [rational normal curve](projective-space.md#rational-normal-curve) and the $2g+2$ hyperplanes corresponding to branch points. Locally, ramification exchanges two roots of a hyperplane section, or exchanges the two lifts of a root passing through a branch point. Biduality then recovers the curve or its double-cover data.

#### Riemann singularity theorem

↑ **Parent:** [Theta divisor](#theta-divisor)

For a [compact Riemann surface](complex-analysis.md#compact-riemann-surface) of genus $g\ge1$, the [theta divisor](#theta-divisor) in $\operatorname{Pic}^{g-1}(X)$ has the displayed multiplicity. A local [determinant description of the theta divisor](#determinant-description-of-the-theta-divisor) reduces to an $r$ by $r$ [matrix](vector-space.md#matrix) vanishing at $L$, where $r=h^0(L)$. Its linear term is cup product with a tangent class in $H^1(\mathcal O_X)$. The [invertible cup-product direction for a line bundle on a curve](#invertible-cup-product-direction-for-a-line-bundle-on-a-curve) shows that its [determinant](linear-algebra.md#determinant) has order exactly $r$. Consequently the [singular locus](algebraic-geometry.md#singular-locus) consists precisely of classes with at least two independent [global sections](ringed-space.md#global-section).

##### Schur complement presentation of a theta singularity

↑ **Parent:** [Riemann singularity theorem](#riemann-singularity-theorem)

For a square evaluation matrix representing a degree-$g-1$ [line bundle](ringed-space.md#line-bundle) $L$, remove an invertible minor of size $N-h^0(L)$. [Holomorphic](complex-analysis.md#complex-differentiability-at-a-point) row and column operations leave a square matrix $M$ of size $r=h^0(L)$ with zero constant term. Its linear part in a tangent direction $\xi\in H^1(\mathcal O_X)$ is $\xi\smile-:H^0(L)\to H^1(L)$. The [invertible cup-product direction for a line bundle on a curve](#invertible-cup-product-direction-for-a-line-bundle-on-a-curve) makes the leading degree-$r$ [determinant](linear-algebra.md#determinant) nonzero, establishing order exactly $r$ rather than just a lower bound.

##### Tangent cone to a theta divisor

↑ **Parent:** [Riemann singularity theorem](#riemann-singularity-theorem)

The [tangent cone to a theta divisor](#tangent-cone-to-a-theta-divisor) at a degree-$g-1$ [line bundle](ringed-space.md#line-bundle) $L$ is cut out in $H^1(\mathcal O_X)$ by the [determinant](linear-algebra.md#determinant) of $\xi\smile-:H^0(L)\to H^1(L)$. Under [Serre duality](ringed-space.md#serre-duality) its [matrix](vector-space.md#matrix) entries are $\langle\xi,s_i t_j\rangle$ for bases of $H^0(L)$ and $H^0(K_X\otimes L^{-1})$. For $h^0(L)=1$, its tangent hyperplane is annihilated by the nonzero [holomorphic differential form](complex-geometry.md#holomorphic-differential-form) $s_1t_1$.

#### Theta autoduality of a Jacobian

↑ **Parent:** [Theta divisor](#theta-divisor)

For $T_q(x)=x+q$, the [homomorphism associated to a line bundle on an abelian variety](#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety) gives $\lambda_\Theta(q)=T_q^*\mathcal O(\Theta)\otimes\mathcal O(\Theta)^{-1}$. Restrict to the negative [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve). The [restriction of the theta divisor to an Abel curve](#restriction-of-the-theta-divisor-to-an-abel-curve) identifies this restriction with the degree-zero class $q$. Pullback of algebraically trivial [line bundles](ringed-space.md#line-bundle) does not change when the embedding is translated. Thus pullback $\rho:\widehat{J(C)}\to J(C)$ satisfies $\rho\lambda_\Theta=1$. Equal dimensions and properness make $\lambda_\Theta$ an isomorphism, including on schemes, rather than only on closed points.

#### Restriction of the theta divisor to an Abel curve

↑ **Parent:** [Theta divisor](#theta-divisor)

For a degree-$g$ [divisor class](algebraic-geometry.md#divisor-class) $D$ with $h^0(\mathcal O_C(D))=1$, let $D_0$ be its unique effective representative. Under $\phi_D(P)=[D-P]$, evaluation of the unique [global section](ringed-space.md#global-section) gives $\phi_D^*\Theta=D_0$, including multiplicities. If $h^0(\mathcal O_C(D))\ge2$, every evaluation kernel is nonzero and the entire curve lies in the [theta divisor](#theta-divisor). These restrictions also show that $h^0(\mathcal O(\Theta))=1$: after pulling back to a dominant product of curves, the ratio of any section to the defining section of the [theta divisor](#theta-divisor) is constant on each general coordinate curve, hence constant everywhere.

#### Determinant description of the theta divisor

↑ **Parent:** [Theta divisor](#theta-divisor)

Choose an effective [Cartier divisor](cartier-divisor.md) $E$ of degree at least $g$ on a smooth projective genus-$g$ [algebraic curve](algebraic-geometry.md#algebraic-curve). For a family $M$ of degree-$g-1$ [line bundles](ringed-space.md#line-bundle), the evaluation map from $\pi_*M(E)$ to $\pi_*(M(E)|_E)$ is between [vector bundles](fiber-bundle.md#vector-bundle) of the same rank. Its [determinant](linear-algebra.md#determinant) vanishes exactly when $H^0(C,M)$ is nonzero. Changing $E$ changes the presentation by cancelling an invertible determinant factor; the zero [Cartier divisor](cartier-divisor.md) is the [theta divisor](#theta-divisor). At a point with $h^0(M)=h^1(M)=1$, the derivative is the cup-product map $H^1(\mathcal O_C)\to\operatorname{Hom}(H^0(M),H^1(M))$. By [Serre duality](ringed-space.md#serre-duality) it is nonzero, since the product of nonzero sections of $M$ and $K_C\otimes M^{-1}$ is nonzero. Hence this [Cartier divisor](cartier-divisor.md) is generically reduced.

##### Invertible cup-product direction for a line bundle on a curve

↑ **Parent:** [Determinant description of the theta divisor](#determinant-description-of-the-theta-divisor)

Suppose a [line bundle](ringed-space.md#line-bundle) $L$ of degree $g-1$ on a [smooth projective curve](projective-space.md#smooth-projective-curve) has $h^0(L)=h^1(L)=r$. Choose $r$ distinct points where evaluation is invertible for both $H^0(L)$ and $H^0(K_X\otimes L^{-1})$. Such choices exist simultaneously: each [determinant](linear-algebra.md#determinant) defines a nonempty open subset of $X^r$, since independent sections cannot vanish at every point. Let $\xi\in H^1(\mathcal O_X)=H^0(K_X)^*$ be a sum of nonzero weighted evaluation functionals at these points. The [Serre duality](ringed-space.md#serre-duality) [matrix](vector-space.md#matrix) of $\xi\smile-$ factors as the product of the two invertible evaluation [matrices](vector-space.md#matrix) and an invertible diagonal [matrix](vector-space.md#matrix). Its [determinant](linear-algebra.md#determinant) is nonzero. This gives the nonzero leading [determinant](linear-algebra.md#determinant) needed for the [Riemann singularity theorem](#riemann-singularity-theorem).

##### Evaluation determinant on a product of curves

↑ **Parent:** [Determinant description of the theta divisor](#determinant-description-of-the-theta-divisor)

On $C\times C^n$, let $\Gamma_i$ be the graph of the $i$th coordinate and $D=\sum_i\Gamma_i$. Successive restriction exact sequences give

$$
\det\pi_*(L|_D)\cong\bigotimes_i\operatorname{pr}_i^*L\otimes\mathcal O\left(-\sum_{i<j}\Delta_{ij}\right).
$$

When $h^0(L)=n$ and $h^1(L)=0$, the [determinant](linear-algebra.md#determinant) of evaluation vanishes at tuples where $H^0(L(-D))$ is nonzero. On distinct points it is the ordinary evaluation [determinant](linear-algebra.md#determinant); the diagonal factors remove its forced zero when two points coincide. This explains why the formula remains valid at repeated points, using jets instead of repeated evaluations.

###### Torsion trivialization in a determinant quotient

↑ **Parent:** [Evaluation determinant on a product of curves](#evaluation-determinant-on-a-product-of-curves)

Evaluation [determinants](linear-algebra.md#determinant) for $L\otimes P$ and $L$ have a quotient which is a rational section of $\bigotimes_i\operatorname{pr}_i^*P$, not intrinsically a scalar. If $P^N\cong\mathcal O_C$, its $N$th power becomes a [rational function](isolated-singularity.md#rational-function) after choosing that trivialization. In [Cartier divisor](cartier-divisor.md) notation, write $P=\mathcal O_C(p)$ and $\operatorname{div}(h)=Np$. With raw meromorphic evaluations the scalar expression is $r^N\prod_i h(z_i)$. The extra product accounts for the line-bundle frames; it is suppressed when evaluation already uses compatible torsion trivializations.

### Abel map of an algebraic curve

↑ **Parent:** [Jacobian variety](#jacobian-variety)

The [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve) sends an effective [Cartier divisor](cartier-divisor.md) $D$ to its [line bundle](ringed-space.md#line-bundle) $\mathcal O_C(D)$. Its scheme fibre over a [line bundle](ringed-space.md#line-bundle) $L$ is the [projective space](projective-space.md) of one-dimensional subspaces of $H^0(C,L)$. This follows in families: a relative effective [Cartier divisor](cartier-divisor.md) in the fixed class determines a nowhere fibre-zero section of $L$ up to a [line bundle](ringed-space.md#line-bundle) from the parameter space, equivalently a line subbundle of $H^0(C,L)\otimes\mathcal O_T$. Thus the scheme fibre is smooth, not merely reduced on its points. The dimensions can nevertheless jump, so the [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve) need not be a smooth morphism.

#### Derivative of the Abelian sum map

↑ **Parent:** [Abel map of an algebraic curve](#abel-map-of-an-algebraic-curve)

For an effective [divisor on an algebraic curve](algebraic-geometry.md#divisor-on-an-algebraic-curve) $D$ on a [smooth projective curve](projective-space.md#smooth-projective-curve), the [Zariski tangent space](algebraic-geometry.md#zariski-tangent-space) to its [symmetric product of a curve](algebraic-geometry.md#symmetric-product-of-a-curve) is $H^0(\mathcal O_D(D))$. The derivative of the [Abelian sum map](#abel-map-of-an-algebraic-curve) is the [connecting homomorphism](homology.md#connecting-homomorphism) of $0\to\mathcal O_X\to\mathcal O_X(D)\to\mathcal O_D(D)\to0$. Its dual under [Serre duality](ringed-space.md#serre-duality) is restriction of [holomorphic differential forms](complex-geometry.md#holomorphic-differential-form) to $D$, including all jets at repeated points. Hence its rank is $\deg D+1-h^0(\mathcal O_X(D))$, and its image annihilates $H^0(K_X(-D))$.

##### Repeated-point Abel differential formula

↑ **Parent:** [Derivative of the Abelian sum map](#derivative-of-the-abelian-sum-map)

At a multiplicity-$r$ point, choose a local parameter and elementary symmetric coordinates $e_1,\ldots,e_r$ for the nearby roots. The tangent [principal part](complex-geometry.md#principal-part-of-a-meromorphic-function) is $v=\sum_{k=1}^r(-1)^{k-1}\delta e_k z^{-k}$. [Newton's identities](polynomial.md#newton-s-identities) give $d(\sum z_i^k)=(-1)^{k-1}k\,d e_k$. Expanding the primitive of a [holomorphic one-form](complex-geometry.md#holomorphic-one-form) proves the [residue](analysis.md#residue) formula, including its sign. The dual map is restriction to the length-$r$ scheme, so it sees all jets through order $r-1$.

## Curve generation criterion for an abelian variety

↑ **Parent:** [Abelian variety](abelian-variety.md)

A smooth projective curve $C\subset A$ generates $A$ by its point differences if and only if it meets every prime [Weil divisor](algebraic-geometry.md#weil-divisor). If a prime [Weil divisor](algebraic-geometry.md#weil-divisor) avoids $C$, its restriction to $C$ has degree zero; [constancy of line bundle degree in a family](ringed-space.md#constancy-of-line-bundle-degree-in-a-family) shows that every translate either contains $C$ or misses it. This forces invariance under $C-C$ and puts the generated subgroup inside the [line bundle translation stabilizer](#line-bundle-translation-stabilizer). If this subgroup were all of $A$, the divisor would be algebraically trivial, contradicting its positive intersection with an [ample line bundle](ringed-space.md#ample-line-bundle). Conversely a proper closed generated subgroup admits a disjoint divisor by the [pole divisor avoiding a fiber](projective-space.md#pole-divisor-avoiding-a-fiber) construction, after translating the fiber to contain $C$.

## Dual abelian variety

↑ **Parent:** [Abelian variety](abelian-variety.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_abelian_variety)

The dual of an [abelian variety](abelian-variety.md) represents algebraically trivial [line bundles](ringed-space.md#line-bundle) rigidified at the origin. Its group law is [tensor product](linear-algebra.md#tensor-product). A [group homomorphism](group-theory.md#group-homomorphism) $f:A\to B$ induces $\widehat f:\widehat B\to\widehat A$ by pullback of these [line bundles](ringed-space.md#line-bundle).

### Weil pairing for an abelian variety

↑ **Parent:** [Dual abelian variety](#dual-abelian-variety)

For an [abelian variety](abelian-variety.md) and an integer $N$ invertible in the base [field](algebra.md#field), a torsion [line bundle](ringed-space.md#line-bundle) $M\in\widehat A[N]$ has trivial pullback by $[N]$. Choose a trivialization. The descent action of the kernel $A[N]$ on that trivial [line bundle](ringed-space.md#line-bundle) acts through a character $\chi_M:A[N]\to\mu_N$. Define $e_N(P,M)=\chi_M(P)$. This is independent of rescaling the trivialization and bilinear under translation and [tensor product](linear-algebra.md#tensor-product). A trivial character descends the trivial bundle, so $M$ is trivial. Since both groups have order $N^{2\dim A}$, the character map is an isomorphism and the [Weil pairing for an abelian variety](#weil-pairing-for-an-abelian-variety) is perfect. The [theta autoduality of a Jacobian](#theta-autoduality-of-a-jacobian) turns it into a pairing on two copies of the [Jacobian variety](#jacobian-variety)'s torsion group.

<h3 id="poincare-line-bundle">Poincaré line bundle</h3>

↑ **Parent:** [Dual abelian variety](#dual-abelian-variety)

The normalized universal [line bundle](ringed-space.md#line-bundle) restricts to the class $\xi$ on $A\times\{\xi\}$ and is trivialized on both zero sections. For a [line bundle](ringed-space.md#line-bundle) $L$ on an [abelian variety](abelian-variety.md), its [homomorphism associated to a line bundle on an abelian variety](#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety) satisfies

$$
(\operatorname{id},\phi_L)^*P_A\cong m^*L\otimes p_1^*L^{-1}\otimes p_2^*L^{-1}
$$

as [Picard group](ringed-space.md#picard-group) classes. A choice of trivialization of $L_0$ normalizes the right side; uniqueness then follows from the [Seesaw theorem](#seesaw-theorem).

## Mumford rigidity lemma

↑ **Parent:** [Abelian variety](abelian-variety.md)

One form of Mumford's rigidity lemma says that if $X$ is complete, $Y$ is connected, and a morphism $f:X\times Y\to Z$ maps one fiber $X\times\{y_0\}$ to a point, then $f$ factors through the projection to $Y$ under the usual pointed hypotheses.

## Invariant differential on a group scheme

↑ **Parent:** [Abelian variety](abelian-variety.md)

Translation identifies the cotangent sheaf of a group scheme with the constant bundle determined by its cotangent space at the identity:

$$
\Omega_{G/k}\cong\mathcal O_G\otimes_k\Omega_{G/k}(e).
$$

## Theorem of the Cube

↑ **Parent:** [Abelian variety](abelian-variety.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theorem_of_the_Cube)

The Theorem of the Cube says that the third finite difference of a line bundle on an abelian variety is trivial. On $X^3$, it is the alternating tensor product of the pullbacks along the seven nonempty partial-sum maps.

### Arithmetic cube identity for Weil heights

↑ **Parent:** [Theorem of the Cube](#theorem-of-the-cube)

For a [line bundle](ringed-space.md#line-bundle) on an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) over a [number field](algebraic-number-theory.md#number-field), the geometric cube identity remains exact as a line-bundle identity. The [Weil height machine](algebraic-number-theory.md#weil-height-machine) translates it into the displayed bounded-error identity for a chosen logarithmic height, uniformly on the rational triples. This distinction is essential: arbitrary naive heights do not obey an exact quadratic identity. Dividing the identity for $2^nP,2^nQ,2^nR$ by $4^n$ produces an exact identity for the [canonical height of an elliptic curve](normalization-of-an-algebraic-curve.md#canonical-height-of-an-elliptic-curve).

### Cohomological proof of the cube theorem for elliptic curves

↑ **Parent:** [Theorem of the Cube](#theorem-of-the-cube)

If a [line bundle](ringed-space.md#line-bundle) on $E^3$ is trivial on each zero-coordinate face, its [First Chern class](complex-geometry.md#first-chern-class) vanishes: the integral second cohomology consists of single-factor second cohomology and cross-products of first cohomology from pairs, and each summand is detected on a coordinate face. The [holomorphic exponential sequence](complex-geometry.md#holomorphic-exponential-sequence) then puts the bundle in $\operatorname{Pic}^0(E^3)$. The decomposition of first cohomology, including [Dolbeault cohomology](complex-geometry.md#dolbeault-cohomology), identifies this group with $\operatorname{Pic}^0(E)^3$. Triviality on the three coordinate axes makes all three factors trivial. Applying this cube principle to the alternating partial-sum pullbacks proves the usual addition-map [Theorem of the Cube](#theorem-of-the-cube).

### Bilinear cross-effect of a line bundle on an abelian variety

↑ **Parent:** [Theorem of the Cube](#theorem-of-the-cube)

For [group homomorphisms](group-theory.md#group-homomorphism) $f,g:A\to B$, this [Picard group](ringed-space.md#picard-group) class is symmetric and additive in both arguments. The [Theorem of the Cube](#theorem-of-the-cube) says precisely that the third additive difference of $h\mapsto[h^*L]$ vanishes, proving additivity of the cross-effect. The [Poincaré line bundle](#poincare-line-bundle) expresses it as $(f,\phi_Lg)^*P_B$, so it depends only on the [Néron-Severi group](ringed-space.md#neron-severi-group) class of $L$. Its associated homomorphism is $\widehat f\phi_Lg+\widehat g\phi_Lf$.

### Theorem of the square

↑ **Parent:** [Theorem of the Cube](#theorem-of-the-cube)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Theorem_of_the_square)

For a line bundle $L$ on an abelian variety and points $x,y$,

$$
T_{x+y}^*L\otimes L\cong T_x^*L\otimes T_y^*L.
$$

#### Homomorphism associated to a line bundle on an abelian variety

↑ **Parent:** [Theorem of the square](#theorem-of-the-square)

For a line bundle $L$ on an abelian variety $X$,

$$
\phi_L:X(k)\to\operatorname{Pic}X,
\qquad x\mapsto T_x^*L\otimes L^{-1},
$$

is a homomorphism by the [Theorem of the square](#theorem-of-the-square).

##### Line bundle translation stabilizer

↑ **Parent:** [Homomorphism associated to a line bundle on an abelian variety](#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)

For a [line bundle](ringed-space.md#line-bundle) $L$ on an [abelian variety](abelian-variety.md) $A$, this closed subgroup consists of $a$ such that $T_a^*L\cong L$. It is a stabilizer of a [Picard group](ringed-space.md#picard-group) class, which need not be the same as the stabilizer of an individual [Weil divisor](algebraic-geometry.md#weil-divisor) representing that class.

##### Identity component of the Picard group

↑ **Parent:** [Homomorphism associated to a line bundle on an abelian variety](#homomorphism-associated-to-a-line-bundle-on-an-abelian-variety)

For an abelian variety,

$$
\operatorname{Pic}^0X=\{L\in\operatorname{Pic}X:\phi_L=0\}
$$

is the subgroup of translation-invariant line bundles.

###### Seesaw theorem

↑ **Parent:** [Identity component of the Picard group](#identity-component-of-the-picard-group)

The seesaw theorem determines a line bundle on a product from its restrictions to fibers: if it is trivial on all fibers over one factor and on one transverse section, then it is trivial.

## ↑ Ancestors (7)

1. [Algebraic group](algebraic-geometry.md#algebraic-group)
2. [Algebraic variety](algebraic-geometry.md#algebraic-variety)
3. [Algebraic geometry](algebraic-geometry.md)
4. [Geometry and topology](geometry-and-topology.md)
5. [Area of mathematics](mathematics.md#area-of-mathematics)
6. [Mathematics](mathematics.md)
7. [Codex Wiki](README.md)

## ← Incoming links (23)

- [Abelian surface](algebraic-geometry.md#abelian-surface)
- [Complex multiplication](algebraic-geometry.md#complex-multiplication)
- [Dual abelian variety](#dual-abelian-variety)
- [Isogeny](algebraic-geometry.md#isogeny)
- [Line bundle translation stabilizer](#line-bundle-translation-stabilizer)
- [Multiplication-by-n morphism](ringed-space.md#multiplication-by-n-morphism)
- [Néron–Tate height](algebraic-number-theory.md#neron-tate-height)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-25.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-18.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-18.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-159.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-159.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-126.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-126.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-126.md#4/i/solution)
- [Poincaré line bundle](#poincare-line-bundle)
- [Prime-to-characteristic torsion of an abelian variety](#prime-to-characteristic-torsion-of-an-abelian-variety)
- [Tate module](representation-theory.md#tate-module)
- [Universal property of the Jacobian variety](#universal-property-of-the-jacobian-variety)
- [Weil–Châtelet group](galois-theory.md#weil-chatelet-group)
- [Weil pairing for an abelian variety](#weil-pairing-for-an-abelian-variety)
