# Differential form

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Differential_form)

A differential form is an alternating covariant tensor field designed for coordinate-independent integration.

**Table of contents**

- [Integration on an oriented manifold](#integration-on-an-oriented-manifold)
- [Comass](#comass)
- [Integral pairing of complex top forms](#integral-pairing-of-complex-top-forms)
- [Differential three-form](#differential-three-form)
  - [Eleven-dimensional three-form action variation](#eleven-dimensional-three-form-action-variation)
- [Vector-bundle-valued differential form](#vector-bundle-valued-differential-form)
  - [Sheaf of vector-bundle-valued differential forms](#sheaf-of-vector-bundle-valued-differential-forms)
- [Sheaf of smooth differential forms](#sheaf-of-smooth-differential-forms)
  - [Sheaf of differential forms of type (p, q)](#sheaf-of-differential-forms-of-type-p-q)
- [Volume form](#volume-form)
  - [Metric volume form](#metric-volume-form)
  - [Area form](#area-form)
  - [Metric volume tensor](#metric-volume-tensor)
  - [Volume-preserving vector field](#volume-preserving-vector-field)
    - [Boundary obstruction for commuting volume-preserving vector fields](#boundary-obstruction-for-commuting-volume-preserving-vector-fields)
- [2-form](#2-form)
- [Wedge product of differential forms](#wedge-product-of-differential-forms)
  - [Exterior multiplication](#exterior-multiplication)
- [Pullback of a differential form](#pullback-of-a-differential-form)
- [Interior product](#interior-product)
- [One-form](#one-form)
  - [Pointwise representation of one-forms by vector-field functionals](#pointwise-representation-of-one-forms-by-vector-field-functionals)
- [Exterior derivative](#exterior-derivative)
  - [Uniqueness of the exterior derivative from its axioms](#uniqueness-of-the-exterior-derivative-from-its-axioms)
  - [Exterior derivative of a one-form evaluated on vector fields](#exterior-derivative-of-a-one-form-evaluated-on-vector-fields)
  - [Generalized Stokes theorem](#generalized-stokes-theorem)
  - [Closed and exact differential forms](#closed-and-exact-differential-forms)
    - [Closed differential form](#closed-differential-form)
      - [Nonexact angular one-form](#nonexact-angular-one-form)
      - [Closed differential one-form](#closed-differential-one-form)
        - [Closed one-forms on the two-sphere are exact](#closed-one-forms-on-the-two-sphere-are-exact)
        - [Averaging closed one-forms on a surface unit tangent bundle](#averaging-closed-one-forms-on-a-surface-unit-tangent-bundle)
      - [Poincaré lemma](#poincare-lemma)
        - [Relative Poincaré lemma](#relative-poincare-lemma)
        - [Radial homotopy operator](#radial-homotopy-operator)
          - [Degree-zero correction to radial homotopy](#degree-zero-correction-to-radial-homotopy)
          - [Radial homotopy primitive near a zero section](#radial-homotopy-primitive-near-a-zero-section)
        - [Green-theorem proof of exactness on a disc](#green-theorem-proof-of-exactness-on-a-disc)
        - [Local potential of a closed differential one-form](#local-potential-of-a-closed-differential-one-form)
      - [Exact differential form](#exact-differential-form)
        - [de Rham cohomology](#de-rham-cohomology)
          - [Relative de Rham complex](#relative-de-rham-complex)
          - [Degree-zero de Rham cohomology](#degree-zero-de-rham-cohomology)
          - [de Rham cohomology of a finite disjoint union](#de-rham-cohomology-of-a-finite-disjoint-union)
          - [de Rham theorem](#de-rham-theorem)
          - [Top de Rham cohomology of a compact connected oriented manifold](#top-de-rham-cohomology-of-a-compact-connected-oriented-manifold)
          - [First de Rham cohomology of the two-sphere](#first-de-rham-cohomology-of-the-two-sphere)
          - [de Rham cohomology of a finite quotient](#de-rham-cohomology-of-a-finite-quotient)
          - [Top-degree de Rham cohomology](#top-degree-de-rham-cohomology)
            - [Top-degree de Rham cohomology of a compact Lie group](#top-degree-de-rham-cohomology-of-a-compact-lie-group)
          - [Averaging differential forms over the circle](#averaging-differential-forms-over-the-circle)
            - [de Rham cohomology of a product with a circle](#de-rham-cohomology-of-a-product-with-a-circle)
          - [Homotopy invariance of de Rham cohomology](#homotopy-invariance-of-de-rham-cohomology)
          - [Mayer--Vietoris sequence for de Rham cohomology](#mayer-vietoris-sequence-for-de-rham-cohomology)
            - [Suspension isomorphism for top de Rham cohomology of spheres](#suspension-isomorphism-for-top-de-rham-cohomology-of-spheres)
- [Hodge star operator](#hodge-star-operator)
  - [Conjugate-linear Hodge star](#conjugate-linear-hodge-star)
    - [Bundle-valued conjugate-linear Hodge star](#bundle-valued-conjugate-linear-hodge-star)
  - [Hodge splitting of Euclidean two-forms](#hodge-splitting-of-euclidean-two-forms)
    - [Wedge orthogonality of opposite-duality two-forms](#wedge-orthogonality-of-opposite-duality-two-forms)
  - [Adjoint of the Hodge star on middle-degree forms](#adjoint-of-the-hodge-star-on-middle-degree-forms)
  - [Hodge star on middle-degree differential forms is conformally invariant](#hodge-star-on-middle-degree-differential-forms-is-conformally-invariant)
  - [Complex Hodge star operator](#complex-hodge-star-operator)
    - [Hodge star eigenvalues on graded differential forms](#hodge-star-eigenvalues-on-graded-differential-forms)
    - [Hodge star on top holomorphic forms](#hodge-star-on-top-holomorphic-forms)
  - [Self-dual differential form](#self-dual-differential-form)
    - ['t Hooft symbol](#t-hooft-symbol)
    - [Self-dual frame in complex Euclidean coordinates](#self-dual-frame-in-complex-euclidean-coordinates)
  - [Anti-self-dual differential form](#anti-self-dual-differential-form)
    - [Exact anti-self-dual form on a compact four-manifold](#exact-anti-self-dual-form-on-a-compact-four-manifold)
  - [Codifferential](#codifferential)
    - [Hodge integration by parts in arbitrary degree](#hodge-integration-by-parts-in-arbitrary-degree)
    - [Hodge integration by parts for one-forms](#hodge-integration-by-parts-for-one-forms)
    - [Coclosed differential form](#coclosed-differential-form)
  - [Hodge Laplacian](#hodge-laplacian)
    - [Poisson equation for differential forms](#poisson-equation-for-differential-forms)
      - [Solvability condition for the Hodge Poisson equation](#solvability-condition-for-the-hodge-poisson-equation)
        - [Affine space of solutions of the Hodge Poisson equation](#affine-space-of-solutions-of-the-hodge-poisson-equation)
    - [Bochner-Weitzenbock formula for one-forms](#bochner-weitzenbock-formula-for-one-forms)
      - [Harmonic one-forms are parallel under nonnegative Ricci curvature](#harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature)
        - [Dimension bound for harmonic one-forms under nonnegative Ricci curvature](#dimension-bound-for-harmonic-one-forms-under-nonnegative-ricci-curvature)
          - [Betti-number obstruction to nonnegative Ricci curvature](#betti-number-obstruction-to-nonnegative-ricci-curvature)
    - [Hodge star commutes with the Hodge Laplacian](#hodge-star-commutes-with-the-hodge-laplacian)
    - [Nonnegativity of the Hodge Laplacian](#nonnegativity-of-the-hodge-laplacian)
    - [Green operator of the Hodge Laplacian](#green-operator-of-the-hodge-laplacian)
  - [Harmonic differential form](#harmonic-differential-form)
    - [Harmonic top-degree forms on a closed oriented manifold](#harmonic-top-degree-forms-on-a-closed-oriented-manifold)
    - [Harmonic one-form](#harmonic-one-form)
    - [Harmonic forms are fixed by a connected isometric group action](#harmonic-forms-are-fixed-by-a-connected-isometric-group-action)
    - [Hodge decomposition theorem](#hodge-decomposition-theorem)
      - [Representing functionals on harmonic forms by wedge pairing](#representing-functionals-on-harmonic-forms-by-wedge-pairing)
        - [Ambiguity of harmonic wedge-pairing representatives](#ambiguity-of-harmonic-wedge-pairing-representatives)
      - [Self-dual primitive of an exact three-form](#self-dual-primitive-of-an-exact-three-form)
- [Exact differential](#exact-differential)
- [Lie derivative of a differential form](#lie-derivative-of-a-differential-form)
  - [Cartan's magic formula](#cartan-s-magic-formula)

## Integration on an oriented manifold

↑ **Parent:** [Differential form](differential-form.md)

A compactly supported top-degree [differential form](differential-form.md) on an oriented smooth [manifold](topology.md#topological-manifold) is integrated using orientation-preserving coordinates and a [partition of unity](differential-geometry.md#partition-of-unity). The coordinate [change of variables](calculus.md#change-of-variables-formula) formula makes the result independent of the choices. More generally, a form is integrated over a lower-dimensional oriented submanifold by its [pullback](category.md#pullback-category-theory). The [Generalized Stokes theorem](#generalized-stokes-theorem) states $\int_M d\beta=\int_{\partial M}\beta$ with the induced boundary orientation. Integrating a [closed differential form](#closed-differential-form) over a closed cycle depends only on its [homology class](homology.md#homology-class), since its integral over a boundary vanishes.

## Comass

↑ **Parent:** [Differential form](differential-form.md)

The comass is the operator norm of a differential form restricted to simple unit tangent multivectors. Reversing orientation gives the equivalent two-sided bound. It differs from the Euclidean norm of all the form's components. The [calibration](differential-geometry.md#calibration-differential-geometry) bound uses comass because tangent planes are represented by simple multivectors.

## Integral pairing of complex top forms

↑ **Parent:** [Differential form](differential-form.md)

For a smooth form $\theta=g\,dz_1\wedge\cdots\wedge dz_n$ of type $(n,0)$, the complex orientation gives $i^{n^2}\theta\wedge\overline\theta=2^n|g|^2\,dx_1\wedge dy_1\wedge\cdots\wedge dx_n\wedge dy_n$. Consequently its integral on a compact [complex manifold](complex-geometry.md#complex-manifold) is positive unless $\theta$ vanishes identically. Applying [Stokes theorem](calculus.md#stokes-theorem) to $d(\psi\wedge\overline{d\psi})$ proves that a [holomorphic differential form](complex-geometry.md#holomorphic-differential-form) of degree $n-1$ on a compact complex $n$-manifold is closed, without requiring a [Kähler metric](complex-geometry.md#kahler-metric).

## Differential three-form

↑ **Parent:** [Differential form](differential-form.md)

A differential three-form is a smooth, totally antisymmetric covariant tensor of rank three. For a [Killing-Yano two-form](riemannian-geometry.md#killing-yano-two-form), its [covariant derivative](general-relativity.md#covariant-derivative) is such a tensor, because it is antisymmetric in the first two and last two slots.

### Eleven-dimensional three-form action variation

↑ **Parent:** [Differential three-form](#differential-three-form)

For a [differential three-form](#differential-three-form) $A$ with $F=dA$ on an oriented eleven-dimensional [manifold](topology.md#topological-manifold), varying $\int(\tfrac12F\wedge\star F+F\wedge F\wedge A)$ with fixed metric gives $\delta S=\int\delta A\wedge(d\star F+3F\wedge F)$ up to a boundary term. Indeed $d(\delta A\wedge F\wedge A)=d\delta A\wedge F\wedge A-\delta A\wedge F\wedge F$, so the two differentiated $F$ factors and the differentiated $A$ factor contribute equally. The shift $A\mapsto A+d\Lambda$ changes the density by $d(F\wedge F\wedge\Lambda)$, preserving the field equation.

## Vector-bundle-valued differential form

↑ **Parent:** [Differential form](differential-form.md)

A smooth section of $\bigwedge^k(T^*X\otimes\mathbb C)\otimes E$ is a differential form with values in the complex [vector bundle](fiber-bundle.md#vector-bundle) $E$. A [connection on a vector bundle](fiber-bundle.md#connection-vector-bundle) extends to these forms by the graded Leibniz rule.

### Sheaf of vector-bundle-valued differential forms

↑ **Parent:** [Vector-bundle-valued differential form](#vector-bundle-valued-differential-form)

For a [holomorphic vector bundle](complex-geometry.md#holomorphic-vector-bundle) $E$, this [sheaf](algebraic-geometry.md#sheaf-mathematics) assigns to $U$ the smooth $E$-valued [differential forms of type (p, q)](complex-geometry.md#differential-form-of-type-p-q) on $U$. Its [Dolbeault operator](complex-geometry.md#dolbeault-operator) acts coefficientwise in a [holomorphic local frame](complex-geometry.md#holomorphic-local-trivialization) and squares to zero.

## Sheaf of smooth differential forms

↑ **Parent:** [Differential form](differential-form.md)

On a [smooth manifold](differential-geometry.md#smooth-manifold), $\mathcal A^k(U)$ is the space of smooth complex-valued degree-$k$ [differential forms](differential-form.md) on $U$. Restriction of forms supplies the [sheaf](algebraic-geometry.md#sheaf-mathematics) maps. Smooth [partitions of unity](differential-geometry.md#partition-of-unity) make this a [fine sheaf](ringed-space.md#fine-sheaf).

### Sheaf of differential forms of type (p, q)

↑ **Parent:** [Sheaf of smooth differential forms](#sheaf-of-smooth-differential-forms)

On a [complex manifold](complex-geometry.md#complex-manifold), this [sheaf](algebraic-geometry.md#sheaf-mathematics) consists of smooth [differential forms of type (p, q)](complex-geometry.md#differential-form-of-type-p-q). The [type decomposition of the complexified tangent bundle](complex-geometry.md#type-decomposition-of-the-complexified-tangent-bundle) gives $\mathcal A^k=\bigoplus_{p+q=k}\mathcal A^{p,q}$.

## Volume form

↑ **Parent:** [Differential form](differential-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volume_form)

A volume form is a nowhere-vanishing differential form of top degree on an oriented manifold. A metric supplies the canonical local density $\sqrt{|\det g|}$ and hence a metric volume form after choosing orientation.

### Metric volume form

↑ **Parent:** [Volume form](#volume-form)

On an oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the metric volume form is the [volume form](#volume-form) taking value one on positively oriented orthonormal frames. In an oriented [manifold chart](differential-geometry.md#manifold-chart) it has the displayed expression. Under an orientation-preserving coordinate change with Jacobian $A$, $\det g$ acquires the factor $(\det A)^2$, precisely matching the transformation of the top [exterior product](linear-algebra.md#exterior-product). Thus the expressions agree on chart overlaps. Orientation is needed to make a globally positive form, though the volume density exists without it.

### Area form

↑ **Parent:** [Volume form](#volume-form)

The oriented metric [volume form](#volume-form) on a two-dimensional surface. On the unit [sphere](geometry-and-topology.md#sphere) with standard orientation, $\omega=\sin\theta\,d\theta\wedge d\varphi$ and $\int\omega=4\pi$. Its [pullback of a differential form](#pullback-of-a-differential-form) under a map measures signed local area.

### Metric volume tensor

↑ **Parent:** [Volume form](#volume-form)

On an oriented $d$-dimensional [pseudo-Riemannian manifold](differential-geometry.md#pseudo-riemannian-manifold), the metric volume tensor is the totally antisymmetric [tensor](linear-algebra.md#tensor) with $\epsilon_{1\ldots d}=\sqrt{|\det g|}$ in positively oriented coordinates. It supplies the components of the [volume form](#volume-form). It differs from the coordinate [Levi-Civita symbol](calculus.md#levi-civita-symbol), whose entries are just $0,1,-1$. Raising indices with a [Lorentzian metric](general-relativity.md#lorentzian-metric) can change signs; the metric, dimension and orientation must be specified.

### Volume-preserving vector field

↑ **Parent:** [Volume form](#volume-form)

A [vector field](calculus.md#vector-field) preserves a chosen [volume form](#volume-form) $\omega$ when its [local flow](differential-geometry.md#local-flow) pulls $\omega$ back to itself. Infinitesimally this is $\mathcal L_X\omega=0$, using the [Lie derivative](#lie-derivative-of-a-differential-form). The condition depends on the chosen volume form.

#### Boundary obstruction for commuting volume-preserving vector fields

↑ **Parent:** [Volume-preserving vector field](#volume-preserving-vector-field)

Suppose a nonempty compact $(n+1)$-manifold with a [volume form](#volume-form) has $n$ pointwise independent [volume-preserving vector fields](#volume-preserving-vector-field) that commute and are tangent to its boundary. If restriction $H^1_{\rm dR}(M)\to H^1_{\rm dR}(\partial M)$ is injective, the boundary must have at least two connected components.

Indeed $\eta=\iota_{X_1}\cdots\iota_{X_n}\omega$ is nowhere zero. [Cartan's magic formula](#cartan-s-magic-formula) and commutation show $d\eta=0$, while boundary tangency gives $j^*\eta=0$. Injectivity in [de Rham cohomology](#de-rham-cohomology) makes $\eta=df$. On a connected boundary $f$ is constant; a maximum or minimum differing from that boundary value would be an interior [critical point](analysis.md#critical-point), contradicting $df\ne0$. Empty boundary is also impossible.

## 2-form

↑ **Parent:** [Differential form](differential-form.md)

A 2-form is an alternating covariant tensor field of rank two. Curvature forms and electromagnetic field strengths are standard examples.

## Wedge product of differential forms

↑ **Parent:** [Differential form](differential-form.md)

The wedge product is the alternating tensor product of differential forms. It is associative and graded-commutative and satisfies the graded Leibniz rule for the exterior derivative.

### Exterior multiplication

↑ **Parent:** [Wedge product of differential forms](#wedge-product-of-differential-forms)

Exterior multiplication by a fixed [differential form](differential-form.md) is the linear operator taking the [wedge product of differential forms](#wedge-product-of-differential-forms) on the left. For a one-form $\omega$, it raises degree by one. Anticommutativity gives $e(\omega)e(\eta)+e(\eta)e(\omega)=0$ for one-forms. On the [exterior algebra](linear-algebra.md#exterior-algebra) of an inner product space, pairing this operation with contraction produces [Clifford multiplication](algebra.md#clifford-multiplication) $c(v)=e(v^\flat)-\iota_v$.

## Pullback of a differential form

↑ **Parent:** [Differential form](differential-form.md)

A smooth map $\phi:M\to N$ pulls a differential form on $N$ back to one on $M$ by applying $d\phi$ to each vector argument. Pullback commutes with wedge products and the exterior derivative.

It is the alternating-tensor case of [pullback](differential-geometry.md#pullback-differential-geometry).

## Interior product

↑ **Parent:** [Differential form](differential-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interior_product)

The interior product contracts a differential form with a vector field in its first argument:

$$
(\iota_X\alpha)(X_2,\ldots,X_k)=\alpha(X,X_2,\ldots,X_k).
$$

## One-form

↑ **Parent:** [Differential form](differential-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-form)

A differential 1-form is a smooth section of the [cotangent bundle](symplectic-geometry.md#cotangent-bundle); it assigns a [covector](linear-algebra.md#covector) to every point of a [smooth manifold](differential-geometry.md#smooth-manifold).

### Pointwise representation of one-forms by vector-field functionals

↑ **Parent:** [One-form](#one-form)

Let $W$ consist of real-linear maps $\alpha$ from smooth [vector fields](calculus.md#vector-field) to smooth functions such that $X_p=0$ implies $\alpha(X)(p)=0$. These are exactly evaluations by smooth [differential one-forms](#one-form). Define $\omega_p(v)=\alpha(X)(p)$ using any global field with $X_p=v$; the vanishing condition makes it well-defined. Bump-extended local frame vectors make its coefficients smooth. Also $\alpha(fX)(p)=f(p)\alpha(X)(p)$, so real linearity and pointwise vanishing automatically give $C^\infty$-linearity. The evaluation correspondence is a natural module isomorphism.

## Exterior derivative

↑ **Parent:** [Differential form](differential-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exterior_derivative)

The exterior derivative is the unique graded derivation $d:\Omega^p(M)\to\Omega^{p+1}(M)$ that agrees with the differential on functions and satisfies $d^2=0$.

### Uniqueness of the exterior derivative from its axioms

↑ **Parent:** [Exterior derivative](#exterior-derivative)

An $\mathbb R$-linear degree-one [graded derivation](commutative-algebra.md#graded-derivation) of the [exterior algebra](linear-algebra.md#exterior-algebra) of smooth [differential forms](differential-form.md) that equals the differential on functions and squares to zero is unique. A [smooth bump function](partial-differential-equation.md#smooth-bump-function) and the [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) first establish locality. Then $d(dx^i)=0$, and applying the [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) to $\alpha=\sum_Ia_Idx^I$ gives the displayed coordinate formula. The [chain rule](calculus.md#chain-rule) makes that formula coordinate-independent.

### Exterior derivative of a one-form evaluated on vector fields

↑ **Parent:** [Exterior derivative](#exterior-derivative)

For a smooth one-form $\alpha$ and smooth [vector fields](calculus.md#vector-field) $X,Y$,

$$
d\alpha(X,Y)=X(\alpha(Y))-Y(\alpha(X))-\alpha([X,Y]).
$$

In coordinates the derivatives of the components of $X,Y$ cancel against the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields), leaving $(\partial_i\alpha_j-\partial_j\alpha_i)X^iY^j$. This formula extends the coordinate definition of the [exterior derivative](#exterior-derivative) to arbitrary frames.

### Generalized Stokes theorem

↑ **Parent:** [Exterior derivative](#exterior-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generalized_Stokes_theorem)

If $X$ is an oriented $n$-manifold with boundary, $F:\partial X\hookrightarrow X$ is the inclusion, and $\omega$ is a compactly supported $(n-1)$-form, then

$$
\int_Xd\omega=\int_{\partial X}F^*\omega,
$$

where the boundary has the [outward-normal-first boundary orientation](differential-geometry.md#outward-normal-first-boundary-orientation). A subordinate [partition of unity](differential-geometry.md#partition-of-unity) reduces the theorem to the fundamental theorem of calculus in oriented coordinate half-spaces; local finiteness and compact support ensure that only finitely many terms contribute.

### Closed and exact differential forms

↑ **Parent:** [Exterior derivative](#exterior-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_and_exact_differential_forms)

A [closed differential form](#closed-differential-form) satisfies $d\alpha=0$; an [exact differential form](#exact-differential-form) has $\alpha=d\beta$. The identity $d^2=0$ makes every exact form closed. Global failure of the converse is measured by [de Rham cohomology](#de-rham-cohomology); the [Poincaré lemma](#poincare-lemma) gives the local converse in positive degrees.

#### Closed differential form

↑ **Parent:** [Closed and exact differential forms](#closed-and-exact-differential-forms)

A differential form $\alpha$ is closed when $d\alpha=0$.

##### Nonexact angular one-form

↑ **Parent:** [Closed differential form](#closed-differential-form)

On the [punctured plane](complex-analysis.md#punctured-complex-plane), this [one-form](#one-form) is closed and locally the differential of the polar angle. Its [line integral](calculus.md#line-integral) around a closed curve is $2\pi$ times the [winding number](complex-analysis.md#winding-number). A once-winding circle therefore has nonzero integral, proving that no global single-valued angle potential exists and the form is not an [exact differential form](#exact-differential-form).

##### Closed differential one-form

↑ **Parent:** [Closed differential form](#closed-differential-form)

A [differential one-form](#one-form) is closed when its [exterior derivative](#exterior-derivative) vanishes. In coordinates, $\eta=\eta_i dx^i$ is closed exactly when $\partial_i\eta_j=\partial_j\eta_i$. The [Poincaré lemma](#poincare-lemma) makes it locally an [exact differential form](#exact-differential-form), but global exactness can fail through nonzero integrals around closed curves.

###### Closed one-forms on the two-sphere are exact

↑ **Parent:** [Closed differential one-form](#closed-differential-one-form)

Remove the north pole and south pole separately. Each resulting chart is diffeomorphic to the plane, so the [Poincaré lemma](#poincare-lemma) supplies local primitives of a closed one-form. Their difference has zero derivative on the connected overlap and is constant. Adjust one primitive by that constant and glue. This proves exactness without assuming a prior computation of [de Rham cohomology](#de-rham-cohomology).

###### Averaging closed one-forms on a surface unit tangent bundle

↑ **Parent:** [Closed differential one-form](#closed-differential-one-form)

Average a closed one-form over fibre rotations. The average differs from the original by an exact form because each rotation is isotopic to the identity; the [Cartan formula for the Lie derivative](#cartan-s-magic-formula) supplies an explicit homotopy integral. Its vertical value $a$ is constant, since closedness and rotational invariance give $da=0$. Subtracting $a\omega$ leaves a basic form $\pi^*\xi$, and closedness gives $d\xi=aK\Omega_a$. For a zero-flux magnetic field, the Liouville mean of $\zeta(X+fV)$ is zero: the directional mean of $\xi(v)$ vanishes, the vertical mean is $2\pi a\int f\Omega_a$, and the coboundary has zero mean by volume preservation.

<h5 id="poincare-lemma">Poincaré lemma</h5>

↑ **Parent:** [Closed differential form](#closed-differential-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_lemma)

Every smooth [closed differential form](#closed-differential-form) of positive degree is locally an [exact differential form](#exact-differential-form). On a coordinate ball centered at zero, put $F_t(x)=tx$ and let $R=x^i\partial_i$ be the radial [vector field](calculus.md#vector-field). Define the degree-lowering operator

$$
K\alpha=\int_0^1t^{-1}F_t^*(\iota_R\alpha)\,dt.
$$

For a $p$-form with $p>0$, the integrand has a factor $t^{p-1}$ in its coordinate coefficients and is smooth at zero. [Cartan's magic formula](#cartan-s-magic-formula) and differentiation of the [pullback of a differential form](#pullback-of-a-differential-form) give $\partial_t(F_t^*\alpha)=t^{-1}F_t^*(d\iota_R\alpha+\iota_Rd\alpha)$. Integrating from zero to one gives $dK\alpha+Kd\alpha=\alpha$, since $F_0^*\alpha=0$ in positive degree. If $d\alpha=0$, take $\beta=K\alpha$. The [local potential of a closed differential one-form](#local-potential-of-a-closed-differential-one-form) gives the explicit degree-one construction. Global exactness can fail through nonzero periods, measured by [de Rham cohomology](#de-rham-cohomology).

<h6 id="relative-poincare-lemma">Relative Poincaré lemma</h6>

↑ **Parent:** [Poincaré lemma](#poincare-lemma)

Let a neighborhood of a submanifold retract onto it by fiberwise radial contraction in a [tubular neighborhood](differential-geometry.md#tubular-neighborhood). If a [closed differential form](#closed-differential-form) $\beta$ pulls back to zero on the submanifold, the radial homotopy formula gives $\beta=d\alpha$, with $\alpha$ vanishing along the zero section. Applying the homotopy operator to $\beta$ gives the primitive directly. This is the relative ingredient in the [relative Moser theorem](symplectic-geometry.md#relative-moser-theorem).

###### Radial homotopy operator

↑ **Parent:** [Poincaré lemma](#poincare-lemma)

On a star-shaped domain, let $\rho_t(x)=tx$ and $R=\sum x_j\partial_{x_j}$. On positive-degree [differential forms](differential-form.md), $H\alpha=\int_0^1\rho_t^*(\iota_R\alpha)\,dt/t$ satisfies $dH+Hd=\mathrm{id}-\rho_0^*$. It gives a primitive of every closed positive-degree form. On a star-shaped domain in a complex vector space, contraction with the two type components of $R$ shows that $H$ sends type $(p,q)$ into $(p-1,q)\oplus(p,q-1)$. There is no primitive assertion for a nonzero constant function.

###### Degree-zero correction to radial homotopy

↑ **Parent:** [Radial homotopy operator](#radial-homotopy-operator)

For radial contraction on a star-shaped domain, the homotopy formula is the identity in positive form degrees because pullback by the constant map vanishes there. On functions it is $h_1df=f-f(0)$. A nonzero constant is a counterexample to the uncorrected degree-zero identity. The [Poincaré lemma](#poincare-lemma) is therefore an exactness assertion in positive degrees, while closed degree-zero forms are locally constant.

###### Radial homotopy primitive near a zero section

↑ **Parent:** [Radial homotopy operator](#radial-homotopy-operator)

On a fiberwise star-shaped neighborhood, let $H_s$ scale fibers by $s$ and let $E$ be the radial [vector field](calculus.md#vector-field). For a [closed differential form](#closed-differential-form) $\delta$ with zero pullback to the [zero section](fiber-bundle.md#zero-section-of-a-vector-bundle), the homotopy primitive $\eta=\int_0^1s^{-1}H_s^*(\iota_E\delta)\,ds$ satisfies $d\eta=\delta$. For a two-form, it vanishes as an ambient covector along that section, providing the fixed-submanifold condition in the [relative Moser theorem](symplectic-geometry.md#relative-moser-theorem).

###### Green-theorem proof of exactness on a disc

↑ **Parent:** [Poincaré lemma](#poincare-lemma)

On a star-shaped planar domain containing zero, let $\eta$ be a smooth [closed differential one-form](#closed-differential-one-form) and set $f(x)=\int_{[0,x]}\eta$. [Green theorem](calculus.md#green-theorem) on the triangle with vertices $0,x,x+h$ gives $f(x+h)-f(x)=\int_{[x,x+h]}\eta$. Dividing by a displacement and taking its [limit](calculus.md#limit-of-a-function) proves $df=\eta$. Thus every such form is an [exact differential form](#exact-differential-form), a degree-one version of the [Poincaré lemma](#poincare-lemma) which uses only the planar integral theorem.

###### Local potential of a closed differential one-form

↑ **Parent:** [Poincaré lemma](#poincare-lemma)

For a smooth [differential one-form](#one-form) $\alpha=\alpha_i(x)dx^i$ with $d\alpha=0$, take a [manifold chart](differential-geometry.md#manifold-chart) identifying a neighborhood with a ball centered at zero, and set $\Phi(x)=\int_0^1x^i\alpha_i(sx)\,ds$. Closedness means $\partial_j\alpha_i=\partial_i\alpha_j$. Consequently

$$
\partial_j\Phi=\int_0^1\bigl[\alpha_j(sx)+s x^i\partial_j\alpha_i(sx)\bigr]ds=\int_0^1\frac d{ds}\bigl[s\alpha_j(sx)\bigr]ds=\alpha_j(x).
$$

Thus $d\Phi=\alpha$ in any dimension. This is the one-form case of the [Poincaré lemma](#poincare-lemma), and applies to spacetime as well as three-dimensional [vector calculus](calculus.md#vector-calculus). A global potential need not exist on a domain with nonzero periods.

##### Exact differential form

↑ **Parent:** [Closed differential form](#closed-differential-form)

A differential form is exact when it is the exterior derivative of a form of one lower degree. Since $d^2=0$, every exact form is closed.

###### de Rham cohomology

↑ **Parent:** [Exact differential form](#exact-differential-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/de_Rham_cohomology)

The $p$th de Rham cohomology group is the quotient of closed $p$-forms by exact $p$-forms.

###### Relative de Rham complex

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

For a holomorphic submersion, relative differential forms are forms modulo those containing a base differential. The relative exterior derivative gives a complex whose fibrewise hypercohomology is complex cohomology for a smooth proper family. Its filtration by degree defines the [Hodge filtration](differential-geometry.md#hodge-filtration); retaining exactly one base differential in the absolute complex constructs the [Gauss–Manin connection](differential-geometry.md#gauss-manin-connection).

###### Degree-zero de Rham cohomology

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

There are no exact forms in degree zero. A [smooth function](analysis.md#smooth-function) has zero [exterior derivative](#exterior-derivative) precisely when it is [locally constant](calculus.md#locally-constant-function), so $H^0_{\mathrm{dR}}(M)$ is the space of [locally constant functions](calculus.md#locally-constant-function). On a connected nonempty [smooth manifold](differential-geometry.md#smooth-manifold), it is $\mathbb R$. An overlapping cover by two connected open subsets therefore does not give the direct-sum formula for [de Rham cohomology of a finite disjoint union](#de-rham-cohomology-of-a-finite-disjoint-union): restriction sends a constant to equal constants on both pieces.

###### de Rham cohomology of a finite disjoint union

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

Restriction of [differential forms](differential-form.md) to the finitely many open and closed components gives an isomorphism of cochain complexes $\Omega^*(\bigsqcup M_j)\cong\bigoplus_j\Omega^*(M_j)$. Piecewise forms glue because there are no overlaps, and the [exterior derivative](#exterior-derivative) acts componentwise. Taking the quotient of [closed differential forms](#closed-differential-form) by [exact differential forms](#exact-differential-form) proves the displayed [de Rham cohomology](#de-rham-cohomology) isomorphism. For an infinite [disjoint union](set-theory.md#disjoint-union), forms and cohomology give products instead.

###### de Rham theorem

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

The complex of smooth [differential forms](differential-form.md) resolves the constant complex sheaf by the [Poincaré lemma](#poincare-lemma) and consists of fine sheaves. Its global cohomology therefore agrees with [sheaf cohomology](ringed-space.md#sheaf-cohomology) of that constant sheaf. A good-cover [Čech-de Rham double complex](ringed-space.md#cech-de-rham-double-complex) gives an explicit comparison, used in [Čech-de Rham curvature descent](complex-geometry.md#cech-de-rham-curvature-descent).

###### Top de Rham cohomology of a compact connected oriented manifold

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

For a compact connected oriented boundaryless $n$-dimensional [smooth manifold](differential-geometry.md#smooth-manifold), choose a [Riemannian metric](differential-geometry.md#riemannian-metric). Harmonic functions are constant because $\langle f,\Delta f\rangle=\|df\|^2$, and [Hodge star commutes with the Hodge Laplacian](#hodge-star-commutes-with-the-hodge-laplacian). Thus the [Hodge star operator](#hodge-star-operator) identifies the constant functions with the [harmonic differential forms](#harmonic-differential-form) of top degree, exactly $\mathbb R\omega_g$. The [Hodge decomposition theorem](#hodge-decomposition-theorem) identifies these with the top [de Rham cohomology](#de-rham-cohomology). The [metric volume form](#metric-volume-form) has nonzero class by [Stokes theorem](calculus.md#stokes-theorem). The harmonic-representative theorem is stated in [Denis Auroux's Hodge theory lecture](https://www.ocw.mit.edu/courses/18-966-geometry-of-manifolds-spring-2007/d6848bb391c032ef27993e984fef4558_lect15.pdf).

###### First de Rham cohomology of the two-sphere

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

A [closed differential form](#closed-differential-form) of degree one on the [two-sphere](geometry-and-topology.md#two-sphere) has primitives on its north-punctured and south-punctured charts by the [Poincaré lemma](#poincare-lemma). The overlap is connected, so their difference is constant. Adjust one constant and glue the primitives. Thus every closed one-form is an [exact differential form](#exact-differential-form), proving the first [de Rham cohomology](#de-rham-cohomology) vanishes.

###### de Rham cohomology of a finite quotient

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

For a free smooth action of a [finite group](group.md#finite-group) $G$ on a [smooth manifold](differential-geometry.md#smooth-manifold) $M$, the quotient projection induces

$$
H^p_{\mathrm{dR}}(M/G)\cong H^p_{\mathrm{dR}}(M)^G.
$$

Invariant [differential forms](differential-form.md) descend uniquely through local inverse branches of the [covering map](algebraic-topology.md#covering-space). Averaging by $|G|^{-1}\sum_{g\in G}g^*$ commutes with the [exterior derivative](#exterior-derivative), produces invariant representatives of invariant classes, and produces an invariant primitive for every invariant exact form. Hence taking invariant forms and taking invariant [cohomology](cohomology.md) give the same result over the real numbers.

###### Top-degree de Rham cohomology

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

On a [compact](topology.md#compact-space) [connected](geometry-and-topology.md#connected-space) oriented $n$-dimensional [smooth manifold](differential-geometry.md#smooth-manifold) without boundary, integration is a [linear isomorphism](vector-space.md#linear-isomorphism) $H^n_{\mathrm{dR}}(M)\to\mathbb R$. Thus two top-degree [differential forms](differential-form.md) have the same [de Rham cohomology](#de-rham-cohomology) class exactly when their integrals agree.

###### Top-degree de Rham cohomology of a compact Lie group

↑ **Parent:** [Top-degree de Rham cohomology](#top-degree-de-rham-cohomology)

A compact [Lie group](lie-theory.md#lie-group) has finitely many [connected components](geometry-and-topology.md#connected-component), each an oriented compact manifold of dimension $n$. Componentwise integration identifies its [top-degree de Rham cohomology](#top-degree-de-rham-cohomology) with one real coordinate per component. For a connected group, if top-degree classes are represented by invariant forms, the [invariant volume form on a Lie group](lie-theory.md#invariant-volume-form-on-a-lie-group) spans the cohomology: invariant top forms are one-dimensional, and its positive integral proves that its class is nonzero by the [Generalized Stokes theorem](#generalized-stokes-theorem). A disconnected group cannot have an invariant representative of every top-degree class, since left translations permute its components. For example, $S^1\times\mathbb Z/2$ has two independent degree-one classes but only one independent invariant top form.

###### Averaging differential forms over the circle

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

Let $S^1$ act on $M\times S^1$ by rotation of the second factor. Averaging a [differential form](differential-form.md) over this action is a cochain map. Every rotation is [homotopic](algebraic-topology.md#homotopy) to the identity through smooth rotations, and integrating [Cartan's magic formula](#cartan-s-magic-formula) along them gives a [cochain homotopy](homology.md#cochain-homotopy) between the averaging map and the identity. Consequently every [de Rham cohomology](#de-rham-cohomology) class has a rotation-invariant representative, and an invariant exact form has an invariant primitive obtained by averaging any primitive.

###### de Rham cohomology of a product with a circle

↑ **Parent:** [Averaging differential forms over the circle](#averaging-differential-forms-over-the-circle)

Choose a closed one-form $\nu$ on $S^1$ with integral one and let $p:M\times S^1\to M$ be projection. Every rotation-invariant $k$-form is uniquely

$$
p^*\alpha+p^*\beta\wedge\nu,
\qquad
\alpha\in\Omega^k(M),\quad\beta\in\Omega^{k-1}(M).
$$

The [exterior derivative](#exterior-derivative) acts componentwise. Averaging therefore proves that

$$
([\alpha],[\beta])\longmapsto[p^*\alpha+p^*\beta\wedge\nu]
$$

is the displayed isomorphism.

###### Homotopy invariance of de Rham cohomology

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

Smoothly homotopic maps induce the same map on de Rham cohomology. Integrating [Cartan's magic formula](#cartan-s-magic-formula) along a homotopy gives a cochain homotopy

$$
F_1^*-F_0^*=dK+Kd.
$$

<h6 id="mayer-vietoris-sequence-for-de-rham-cohomology">Mayer--Vietoris sequence for de Rham cohomology</h6>

↑ **Parent:** [de Rham cohomology](#de-rham-cohomology)

For an open cover $X=U\cup V$, restriction of forms gives a short exact sequence of cochain complexes

$$
0\to\Omega^*(X)\to\Omega^*(U)\oplus\Omega^*(V)\to\Omega^*(U\cap V)\to0,
$$

and hence a long exact sequence in de Rham cohomology.

###### Suspension isomorphism for top de Rham cohomology of spheres

↑ **Parent:** [Mayer--Vietoris sequence for de Rham cohomology](#mayer-vietoris-sequence-for-de-rham-cohomology)

Cover the [sphere](geometry-and-topology.md#sphere) by complements of its two poles. Each open set is contractible, and their intersection deformation retracts to the equatorial [sphere](geometry-and-topology.md#sphere). The [Poincaré lemma](#poincare-lemma) and [homotopy invariance of de Rham cohomology](#homotopy-invariance-of-de-rham-cohomology) make the two neighboring groups in the [Mayer--Vietoris sequence for de Rham cohomology](#mayer-vietoris-sequence-for-de-rham-cohomology) zero, so its connecting map is an [isomorphism](algebra.md#isomorphism). Its inverse takes a top-degree form to the difference of its local primitives on the equator, up to the connecting-map sign convention.

## Hodge star operator

↑ **Parent:** [Differential form](differential-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hodge_star_operator)

On an oriented Riemannian $n$-manifold, the Hodge star is determined by

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle\,\omega_g.
$$

It maps $p$-forms to $(n-p)$-forms and satisfies $*^2=(-1)^{p(n-p)}$ on $p$-forms.

### Conjugate-linear Hodge star

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

For a [Hermitian manifold](complex-geometry.md#hermitian-manifold) with the pointwise [Hermitian inner product](linear-algebra.md#hermitian-form) linear in the first variable, define the conjugate-linear star by $\alpha\wedge *\beta=\langle\alpha,\beta\rangle\,\omega^n/n!$. It is the usual real [Hodge star operator](#hodge-star-operator) extended complex-linearly and then composed with complex conjugation. It has the displayed bidegree and satisfies $*^2=(-1)^{p+q}$ on $(p,q)$-forms.

#### Bundle-valued conjugate-linear Hodge star

↑ **Parent:** [Conjugate-linear Hodge star](#conjugate-linear-hodge-star)

For inner products linear in the first argument, define $*_E$ by contraction in $\psi\wedge *_E\eta=(\psi,\eta)dV$. It is conjugate-linear and takes $(p,q)$-forms with values in $E$ to $(n-p,n-q)$-forms with values in $E^*$. With induced dual metrics, $*_{E^*}*_E=(-1)^{p+q}$.

### Hodge splitting of Euclidean two-forms

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

On an oriented [Euclidean metric](differential-geometry.md#euclidean-metric) four-space, the [Hodge star operator](#hodge-star-operator) on two-forms is an orthogonal involution. Its two eigenspaces each have dimension three. A [self-dual two-form](#self-dual-differential-form) has eigenvalue $+1$, while an [anti-self-dual two-form](#anti-self-dual-differential-form) has eigenvalue $-1$. The splitting uses the metric-normalized [Riemannian volume form](differential-geometry.md#riemannian-volume-form); an arbitrarily rescaled volume in the defining wedge identity would rescale the operator itself.

#### Wedge orthogonality of opposite-duality two-forms

↑ **Parent:** [Hodge splitting of Euclidean two-forms](#hodge-splitting-of-euclidean-two-forms)

The [Hodge star operator](#hodge-star-operator) is self-adjoint on real two-forms in four Euclidean dimensions, so its opposite eigenspaces are orthogonal. Since $H\wedge G=\langle H,*G\rangle\operatorname{vol}_g$, a [self-dual two-form](#self-dual-differential-form) and an [anti-self-dual two-form](#anti-self-dual-differential-form) also have zero [wedge product of differential forms](#wedge-product-of-differential-forms). Applied to Lie-algebra components with an invariant pairing, this identity eliminates mixed terms from the [Yang-Mills action](relativistic-quantum-field.md#yang-mills-action).

### Adjoint of the Hodge star on middle-degree forms

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

On $m$-forms in an oriented Riemannian manifold of dimension $2m$, the [Hodge star operator](#hodge-star-operator) is orthogonal and satisfies $*^2=(-1)^{m^2}$. Hence

$$
*^\dagger=*^{-1}=(-1)^{m^2}*.
$$

It is self-adjoint when $m$ is even and skew-adjoint when $m$ is odd.

### Hodge star on middle-degree differential forms is conformally invariant

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

If a metric in dimension $n$ is rescaled by $\widetilde g=e^{2\omega}g$, then its Hodge star on $p$-forms satisfies $\widetilde *=e^{(n-2p)\omega}*$. The exponent vanishes for middle-degree forms with $n=2p$, so their self-dual and anti-self-dual subspaces depend only on the conformal class.

### Complex Hodge star operator

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

The Hodge star extends complex-linearly to complex differential forms. With the Hermitian pointwise inner product, it is characterized by

$$
\alpha\wedge *\bar\beta=\langle\alpha,\beta\rangle\,\operatorname{vol}_g.
$$

On a [Hermitian manifold](complex-geometry.md#hermitian-manifold) it maps forms of type $(p,q)$ to forms of type $(n-q,n-p)$.

#### Hodge star eigenvalues on graded differential forms

↑ **Parent:** [Complex Hodge star operator](#complex-hodge-star-operator)

Use the complex-linear [Hodge star operator](#hodge-star-operator) on the direct sum of all form degrees. Its square on degree $r$ is $(-1)^{r(n-r)}$. In positive odd dimension this is always one; in positive even dimension its sign is positive on even-degree forms and negative on odd-degree forms. Complementary basis wedges provide both roots of each sign, so the displayed [eigenvalues](linear-operator-theory.md#eigenvalue) all occur. On a single degree the [Hodge star operator](#hodge-star-operator) is an endomorphism only in middle degree; on middle degree $m$ in dimension $2m$ its possible [eigenvalues](linear-operator-theory.md#eigenvalue) are $\pm1$ for even $m$ and $\pm i$ for odd $m$.

#### Hodge star on top holomorphic forms

↑ **Parent:** [Complex Hodge star operator](#complex-hodge-star-operator)

For the complex-linear [Hodge star operator](#hodge-star-operator) and complex orientation on a [Hermitian manifold](complex-geometry.md#hermitian-manifold) of complex dimension $n$, every $(n,0)$-form has the displayed eigenvalue. In an adapted orthonormal real coframe, each factor $dx_j+i\,dy_j$ has two-dimensional star eigenvalue $-i$. Regrouping the $n$ factors introduces $(-1)^{n(n-1)/2}$, giving $(-1)^{n(n+1)/2}i^n$. This is a pointwise metric identity; the metric need not be [Kähler](complex-geometry.md#kahler-manifold).

### Self-dual differential form

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

On an oriented Riemannian four-manifold, a two-form $\alpha$ is self-dual when $*\alpha=\alpha$.

On an oriented Riemannian four-manifold, a [two-form](#2-form) is self-dual when $*\alpha=\alpha$. Here $*$ is the [Hodge star operator](#hodge-star-operator).

#### 't Hooft symbol

↑ **Parent:** [Self-dual differential form](#self-dual-differential-form)

For the orientation $dx^1\wedge dx^2\wedge dx^3\wedge dx^4$, define $\eta^a_{ij}=\epsilon_{aij}$, $\eta^a_{i4}=\delta_{ai}$, and extend antisymmetrically. The three forms $\tfrac12\eta^a_{\mu\nu}dx^\mu\wedge dx^\nu$ are self-dual. Reversing the sign of the components involving index four gives the anti-self-dual symbols $\bar\eta$. They identify the two three-dimensional eigenspaces of the [Hodge star](#hodge-star-operator) on [differential two-forms](#2-form) and give compact formulas for the [BPST instanton](classical-field-theory-soliton.md#bpst-instanton).

#### Self-dual frame in complex Euclidean coordinates

↑ **Parent:** [Self-dual differential form](#self-dual-differential-form)

For $w=x^1+ix^2$, $z=x^3+ix^4$ and the standard oriented [Euclidean metric](differential-geometry.md#euclidean-metric), the real and imaginary parts of $dw\wedge dz$, together with $i(dw\wedge d\bar w+dz\wedge d\bar z)$, span the [self-dual two-forms](#self-dual-differential-form). The printed complex four-form $dw\wedge dz\wedge d\bar w\wedge d\bar z$ is four times the metric [volume form](#volume-form) and gives the same [orientation](algebraic-topology.md#orientation-of-a-simplex).

### Anti-self-dual differential form

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

On an oriented Riemannian four-manifold, a two-form $\alpha$ is anti-self-dual when $*\alpha=-\alpha$.

On an oriented Riemannian four-manifold, a [two-form](#2-form) is anti-self-dual when $*\alpha=-\alpha$. Here $*$ is the [Hodge star operator](#hodge-star-operator).

#### Exact anti-self-dual form on a compact four-manifold

↑ **Parent:** [Anti-self-dual differential form](#anti-self-dual-differential-form)

If an exact two-form $\beta=d\alpha$ on a compact oriented Riemannian four-manifold is anti-self-dual, then

$$
0=\int_Md(\alpha\wedge d\alpha)=\int_M\beta\wedge\beta=-\lVert\beta\rVert_{L^2}^2,
$$

so $\beta=0$.

### Codifferential

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

The codifferential is the formal $L^2$ adjoint of the exterior derivative. On $p$-forms in dimension $n$, one convention is

$$
\delta=(-1)^{n(p+1)+1}*d*.
$$

#### Hodge integration by parts in arbitrary degree

↑ **Parent:** [Codifferential](#codifferential)

On a closed oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), let $\alpha$ have degree $r-1$ and $\beta$ degree $r$. The [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) and [Stokes theorem](calculus.md#stokes-theorem) give $\int d\alpha\wedge*\beta=(-1)^r\int\alpha\wedge d*\beta$. The [codifferential](#codifferential) convention $\delta\beta=(-1)^{n(r+1)+1}*d*\beta$, combined with the square of the [Hodge star](#hodge-star-operator), gives $*\delta\beta=(-1)^rd*\beta$. This proves that the [codifferential](#codifferential) is the [formal adjoint](hilbert-space.md#formal-adjoint) of the [exterior derivative](#exterior-derivative). A boundary requires the corresponding boundary term or specified boundary conditions.

#### Hodge integration by parts for one-forms

↑ **Parent:** [Codifferential](#codifferential)

On an oriented boundaryless [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), apply [Stokes theorem](calculus.md#stokes-theorem) to the compactly supported form $f*\alpha$. The [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) gives $\int df\wedge*\alpha=-\int f\,d*\alpha$. The [Hodge star operator](#hodge-star-operator) identifies these top forms with the scalar integrands displayed above. This proves that the [codifferential](#codifferential) on one-forms is $\delta=-*d*$, the [formal adjoint](hilbert-space.md#formal-adjoint) of the [exterior derivative](#exterior-derivative). Compact support of $f$ suffices.

#### Coclosed differential form

↑ **Parent:** [Codifferential](#codifferential)

A [differential form](differential-form.md) is coclosed when its [codifferential](#codifferential) vanishes. On a closed [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), a form is a [harmonic differential form](#harmonic-differential-form) exactly when it is both a [closed differential form](#closed-differential-form) and coclosed: the identity $\langle\Delta\alpha,\alpha\rangle=\|d\alpha\|^2+\|\delta\alpha\|^2$ proves the converse as well as necessity.

### Hodge Laplacian

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

The Hodge Laplacian acts on differential forms by $\Delta=d\delta+\delta d$. On a compact manifold,

$$
\langle\Delta\alpha,\alpha\rangle
=\lVert d\alpha\rVert^2+\lVert\delta\alpha\rVert^2.
$$

It is one of the [Laplace operators in differential geometry](differential-geometry.md#laplace-operators-in-differential-geometry).

#### Poisson equation for differential forms

↑ **Parent:** [Hodge Laplacian](#hodge-laplacian)

This [Poisson equation](partial-differential-equation.md#poisson-equation) uses the [Hodge Laplacian](#hodge-laplacian) on [differential forms](differential-form.md). On a closed [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the obstruction to solving it is the component of the source along [harmonic differential forms](#harmonic-differential-form). The [Green operator of the Hodge Laplacian](#green-operator-of-the-hodge-laplacian) supplies a solution when that component vanishes.

##### Solvability condition for the Hodge Poisson equation

↑ **Parent:** [Poisson equation for differential forms](#poisson-equation-for-differential-forms)

The [Poisson equation for differential forms](#poisson-equation-for-differential-forms) on a closed oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) is solvable exactly when its source is $L^2$-orthogonal to every [harmonic differential form](#harmonic-differential-form) of the same degree. Necessity follows from the [formal adjoint](hilbert-space.md#formal-adjoint) identity $\langle\Delta\alpha,h\rangle=\langle\alpha,\Delta h\rangle=0$. For sufficiency, the [Green operator of the Hodge Laplacian](#green-operator-of-the-hodge-laplacian) gives $\alpha=G\beta$, since $\Delta G=I-P_{\mathcal H}$.

###### Affine space of solutions of the Hodge Poisson equation

↑ **Parent:** [Solvability condition for the Hodge Poisson equation](#solvability-condition-for-the-hodge-poisson-equation)

When the [Poisson equation for differential forms](#poisson-equation-for-differential-forms) has one solution $\alpha_0$, all solutions are its translates by the [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) of the [Hodge Laplacian](#hodge-laplacian), namely the [harmonic differential forms](#harmonic-differential-form). The [Hodge decomposition theorem](#hodge-decomposition-theorem) identifies this translation [vector space](vector-space.md) canonically with [de Rham cohomology](#de-rham-cohomology). There is no preferred affine origin until an extra normalization is chosen; orthogonality to harmonic forms picks the Green-operator solution.

#### Bochner-Weitzenbock formula for one-forms

↑ **Parent:** [Hodge Laplacian](#hodge-laplacian)

For a real one-form $\alpha$, the [Hodge Laplacian](#hodge-laplacian) differs from the [rough Laplacian](fiber-bundle.md#rough-laplacian) by the action of [Ricci curvature](second-fundamental-form.md#ricci-curvature): $(\operatorname{Ric}\cdot\alpha)(X)=\alpha(\operatorname{Ric}^{\sharp}X)$, where $g(\operatorname{Ric}^{\sharp}X,Y)=\operatorname{Ric}(X,Y)$. Equivalently, with the nonnegative scalar Laplacian convention,

$$
\tfrac12\Delta|\alpha|^2=\langle\Delta\alpha,\alpha\rangle-|\nabla\alpha|^2-\operatorname{Ric}(\alpha^{\sharp},\alpha^{\sharp}).
$$

##### Harmonic one-forms are parallel under nonnegative Ricci curvature

↑ **Parent:** [Bochner-Weitzenbock formula for one-forms](#bochner-weitzenbock-formula-for-one-forms)

On a closed [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) with nonnegative [Ricci curvature](second-fundamental-form.md#ricci-curvature), integration of the [Bochner-Weitzenbock formula for one-forms](#bochner-weitzenbock-formula-for-one-forms) for a [harmonic one-form](#harmonic-one-form) gives

$$
0=\|\nabla\alpha\|_{L^2}^2+\int_M\operatorname{Ric}(\alpha^{\sharp},\alpha^{\sharp})\,d\mathrm{vol}_g.
$$

Both terms are nonnegative, so $\nabla\alpha=0$. Riemannian volume density makes the argument valid even without orientation.

###### Dimension bound for harmonic one-forms under nonnegative Ricci curvature

↑ **Parent:** [Harmonic one-forms are parallel under nonnegative Ricci curvature](#harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature)

On a compact connected [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) without boundary with nonnegative [Ricci curvature](second-fundamental-form.md#ricci-curvature), the [Bochner formula for one-forms](#bochner-weitzenbock-formula-for-one-forms) makes every [harmonic one-form](#harmonic-one-form) parallel. Evaluation at any point is then injective: a parallel form that is zero there stays zero along every path. Hence $\dim\mathcal H^1(M)\le\dim M$. Flat tori attain equality. Positive-definite [Ricci curvature](second-fundamental-form.md#ricci-curvature) at even one point instead forces $\mathcal H^1=0$, because the Bochner integral makes its Ricci contraction vanish everywhere.

###### Betti-number obstruction to nonnegative Ricci curvature

↑ **Parent:** [Dimension bound for harmonic one-forms under nonnegative Ricci curvature](#dimension-bound-for-harmonic-one-forms-under-nonnegative-ricci-curvature)

On a closed connected [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) with nonnegative [Ricci curvature](second-fundamental-form.md#ricci-curvature), [harmonic one-forms are parallel under nonnegative Ricci curvature](#harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature). Evaluation at one point injects their space into the [cotangent space](differential-geometry.md#cotangent-space). The [Hodge decomposition theorem](#hodge-decomposition-theorem) identifies its dimension with the first [Betti number](homology.md#betti-number), giving $b_1(M)\le\dim M$. For example, a genus-two closed orientable surface times a [circle](topology.md#circle) has dimension three and first [Betti number](homology.md#betti-number) five, so no [Riemannian metric](differential-geometry.md#riemannian-metric) on that product has nonnegative [Ricci curvature](second-fundamental-form.md#ricci-curvature).

#### Hodge star commutes with the Hodge Laplacian

↑ **Parent:** [Hodge Laplacian](#hodge-laplacian)

On an oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the [codifferential](#codifferential) convention $\delta=(-1)^{n(p+1)+1}*d*$ and $*^2=(-1)^{p(n-p)}$ give $d*\alpha=(-1)^p*\delta\alpha$ and $\delta*\alpha=(-1)^{p+1}*d\alpha$. Applying these twice proves the displayed identity. Thus the [Hodge star operator](#hodge-star-operator) preserves [harmonic differential forms](#harmonic-differential-form) even without compactness.

#### Nonnegativity of the Hodge Laplacian

↑ **Parent:** [Hodge Laplacian](#hodge-laplacian)

On a compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) without boundary, the [codifferential](#codifferential) is the $L^2$ [adjoint operator](hilbert-space.md#adjoint-operator) of the [exterior derivative](#exterior-derivative). Consequently

$$
\langle\Delta\alpha,\alpha\rangle_{L^2}
=\lVert d\alpha\rVert_{L^2}^2+\lVert\delta\alpha\rVert_{L^2}^2\geq0.
$$

Every [eigenvalue](linear-operator-theory.md#eigenvalue) of the Hodge Laplacian is therefore nonnegative.

#### Green operator of the Hodge Laplacian

↑ **Parent:** [Hodge Laplacian](#hodge-laplacian)

On a compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), the Green operator $G$ is the inverse of the [Hodge Laplacian](#hodge-laplacian) on the orthogonal complement of harmonic forms and is zero on harmonic forms. If $H$ is harmonic projection, then

$$
\Delta G=G\Delta=1-H.
$$

It commutes with every differential operator that commutes with $\Delta$.

### Harmonic differential form

↑ **Parent:** [Hodge star operator](#hodge-star-operator)

A differential form is harmonic when it lies in the kernel of the Hodge Laplacian $\Delta=d\delta+\delta d$. On a compact manifold, this is equivalent to $d\alpha=0$ and $\delta\alpha=0$.

Its relation to cohomology is part of [Hodge theory](differential-geometry.md#hodge-theory).

#### Harmonic top-degree forms on a closed oriented manifold

↑ **Parent:** [Harmonic differential form](#harmonic-differential-form)

On a connected compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) without boundary, a top-degree form is $f\operatorname{vol}_g$. Its exterior derivative is automatically zero, and the Hodge codifferential vanishes exactly when $df=0$. Thus it is harmonic exactly when $f$ is constant. Equivalently the [Hodge star operator](#hodge-star-operator) identifies this space with harmonic functions. Without connectedness the dimension is the number of connected components.

#### Harmonic one-form

↑ **Parent:** [Harmonic differential form](#harmonic-differential-form)

A harmonic one-form is a [differential one-form](#one-form) $\alpha$ satisfying $\Delta\alpha=0$ for the [Hodge Laplacian](#hodge-laplacian). On a [closed manifold](differential-geometry.md#closed-manifold), the [Hodge decomposition theorem](#hodge-decomposition-theorem) identifies these forms with degree-one [de Rham cohomology](#de-rham-cohomology). The [Bochner-Weitzenbock formula for one-forms](#bochner-weitzenbock-formula-for-one-forms) implies that [harmonic one-forms are parallel under nonnegative Ricci curvature](#harmonic-one-forms-are-parallel-under-nonnegative-ricci-curvature).

#### Harmonic forms are fixed by a connected isometric group action

↑ **Parent:** [Harmonic differential form](#harmonic-differential-form)

On a closed oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), a smooth isometric action of a connected [Lie group](lie-theory.md#lie-group) fixes every [harmonic differential form](#harmonic-differential-form). Each group element is connected to the identity through a smooth path, so its action is smoothly homotopic to the identity and fixes [de Rham cohomology](#de-rham-cohomology). Isometries preserve the [Hodge Laplacian](#hodge-laplacian); uniqueness of the harmonic representative, from the [Hodge decomposition theorem](#hodge-decomposition-theorem), then makes each form itself fixed.

#### Hodge decomposition theorem

↑ **Parent:** [Harmonic differential form](#harmonic-differential-form)

On a compact oriented Riemannian manifold,

$$
\Omega^p=\mathcal H^p\oplus d\Omega^{p-1}\oplus\delta\Omega^{p+1}
$$

as an $L^2$-orthogonal direct sum. Every de Rham cohomology class consequently has a unique harmonic representative.

This orthogonal-splitting theorem is one result of [Hodge theory](differential-geometry.md#hodge-theory).

##### Representing functionals on harmonic forms by wedge pairing

↑ **Parent:** [Hodge decomposition theorem](#hodge-decomposition-theorem)

On a compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) without boundary, every real linear functional on $\mathcal H^p$ has a unique $L^2$ representing [harmonic form](#harmonic-differential-form) $h_f$: $f(\varphi)=\langle\varphi,h_f\rangle_{L^2}$. If $h_a$ is an orthonormal harmonic basis, then $h_f=\sum_af(h_a)h_a$. The [Hodge star](#hodge-star-operator) gives a harmonic $(n-p)$-form $\psi_0=*h_f$ satisfying $f(\varphi)=\int_M\varphi\wedge\psi_0$. The [ambiguity of harmonic wedge-pairing representatives](#ambiguity-of-harmonic-wedge-pairing-representatives) describes all smooth representatives with this same functional.

###### Ambiguity of harmonic wedge-pairing representatives

↑ **Parent:** [Representing functionals on harmonic forms by wedge pairing](#representing-functionals-on-harmonic-forms-by-wedge-pairing)

On a compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) without boundary, a smooth $(n-p)$-form $\chi$ annihilates all harmonic $p$-forms under wedge integration exactly when its harmonic projection vanishes. Indeed $\int_M\varphi\wedge\chi=\langle*\varphi,\chi\rangle_{L^2}$, and the [Hodge star](#hodge-star-operator) maps $\mathcal H^p$ isomorphically onto $\mathcal H^{n-p}$. By the [Hodge decomposition theorem](#hodge-decomposition-theorem), this annihilator is

$$
d\Omega^{n-p-1}\oplus\delta\Omega^{n-p+1}.
$$

Thus both exact and coexact additions are allowed; a harmonic representative is unique. The potentials of these additions need not be unique, and out-of-range degree spaces are zero. For a concrete coexact ambiguity, take the [torus](topology.md#torus) $(\mathbb R/2\pi\mathbb Z)^2$ with metric $dx^2+dy^2$. The form $\chi=\delta(\sin y\,dx\wedge dy)=\cos y\,dx$ annihilates every harmonic one-form by orthogonality, yet $d\chi=\sin y\,dx\wedge dy$ is nonzero. Thus an annihilating representative need not even be closed, let alone exact.

##### Self-dual primitive of an exact three-form

↑ **Parent:** [Hodge decomposition theorem](#hodge-decomposition-theorem)

On a compact oriented [Riemannian manifold](riemannian-geometry.md#riemannian-manifold) of dimension four without boundary, every exact three-form has a [self-dual two-form](#self-dual-differential-form) primitive. Write $\beta=d\omega$ and use the [Hodge decomposition theorem](#hodge-decomposition-theorem) to split $\omega=h+d\xi+\delta\psi$. Then $\beta=d\delta\psi$. For $a=\delta\psi$, the [codifferential](#codifferential) identity $\delta=-*d*$ and the fact $*^2=1$ on two-forms give $*a=-d*\psi$, so $d*a=0$. Thus $\sigma=a+*a$ satisfies $*\sigma=\sigma$ and $d\sigma=\beta$. It is twice the self-dual projection of $a$, rather than the projection itself.

## Exact differential

↑ **Parent:** [Differential form](differential-form.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exact_differential)

An exact differential is the differential $df$ of a scalar potential and integrates to zero around every closed curve.

## Lie derivative of a differential form

↑ **Parent:** [Differential form](differential-form.md)

The Lie derivative of a differential form measures its infinitesimal change under the flow generated by a vector field.

<h3 id="cartan-s-magic-formula">Cartan's magic formula</h3>

↑ **Parent:** [Lie derivative of a differential form](#lie-derivative-of-a-differential-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cartan's_magic_formula)

The [Lie derivative of a differential form](#lie-derivative-of-a-differential-form) satisfies $\mathcal L_X=d\iota_X+\iota_Xd$. Both sides agree on [functions](function.md). On a [differential 1-form](#one-form) $\eta$, evaluation at a [vector field](calculus.md#vector-field) $Y$ gives $X(\eta(Y))-\eta([X,Y])$ on both sides, by the definition of the [exterior derivative](#exterior-derivative) and the [Lie bracket of vector fields](differential-geometry.md#lie-bracket-of-vector-fields). Both operators are degree-zero [derivations of an algebra](associative-algebra.md#derivation-of-an-algebra) on the [exterior algebra](linear-algebra.md#exterior-algebra). Agreement on [functions](function.md) and coordinate [differential 1-forms](#one-form) therefore proves agreement on every [differential form](differential-form.md). Since $d^2=0$, the formula also gives $\mathcal L_Xd=d\mathcal L_X$, so the [Lie derivative of a differential form](#lie-derivative-of-a-differential-form) commutes with the [exterior derivative](#exterior-derivative).

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (88)

- [A-hat form](geometry-and-topology.md#a-hat-form)
- [Averaging differential forms over the circle](#averaging-differential-forms-over-the-circle)
- [Calibrated geometry](differential-geometry.md#calibrated-geometry)
- [Calibration (differential geometry)](differential-geometry.md#calibration-differential-geometry)
- [Cartan's magic formula](#cartan-s-magic-formula)
- [Coclosed differential form](#coclosed-differential-form)
- [Complex torus](complex-geometry.md#complex-torus)
- [de Rham cohomology of a finite disjoint union](#de-rham-cohomology-of-a-finite-disjoint-union)
- [de Rham cohomology of a finite quotient](#de-rham-cohomology-of-a-finite-quotient)
- [de Rham theorem](#de-rham-theorem)
- [Differential of a smooth function](differential-geometry.md#differential-of-a-smooth-function)
- [Distance between two uniform points in a three-dimensional ball](continuous-probability-distribution.md#distance-between-two-uniform-points-in-a-three-dimensional-ball)
- [Endomorphism-valued exterior product](fiber-bundle.md#endomorphism-valued-exterior-product)
- [Exterior multiplication](#exterior-multiplication)
- [Hodge theory](differential-geometry.md#hodge-theory)
- [Integration on an oriented manifold](#integration-on-an-oriented-manifold)
- [Invariant primitive under a finite group action](homology.md#invariant-primitive-under-a-finite-group-action)
- [Killing-Yano tensor](riemannian-geometry.md#killing-yano-tensor)
- [Laplace operators in differential geometry](differential-geometry.md#laplace-operators-in-differential-geometry)
- [Lefschetz operator of a Kähler manifold](complex-geometry.md#lefschetz-operator-of-a-kahler-manifold)
- [Lie derivative of a tensor field](fiber-bundle.md#lie-derivative-of-a-tensor-field)
- [Modified Helmholtz closed spectral one-form](partial-differential-equation.md#modified-helmholtz-closed-spectral-one-form)
- [Orientation of a smooth manifold](differential-geometry.md#orientation-of-a-smooth-manifold)
- [Oriented atlas](differential-geometry.md#oriented-atlas)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-15.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-71.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3.md#3a/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3.md#3a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-14.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-57.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-14.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58.md#7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-18.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-20.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-57.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-15.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-86.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-19.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-15.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-14.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-17.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-17.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-50.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-17.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-50.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-51.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-17.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-18.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-115.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-308.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-140.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-115.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-115.md#1/a/solution)
- [Poisson equation for differential forms](#poisson-equation-for-differential-forms)
- [Radial-gauge potential for a divergence-free magnetic field](electromagnetism.md#radial-gauge-potential-for-a-divergence-free-magnetic-field)
- [Radial homotopy operator](#radial-homotopy-operator)
- [Right-invariant differential form](lie-theory.md#right-invariant-differential-form)
- [Sheaf of smooth differential forms](#sheaf-of-smooth-differential-forms)
- [Symplectic volume form](symplectic-geometry.md#symplectic-volume-form)
- [Tensor bundle](fiber-bundle.md#tensor-bundle)
- [Time-dependent vector field](calculus.md#time-dependent-vector-field)
- [Top-degree de Rham cohomology](#top-degree-de-rham-cohomology)
- [Uniqueness of the exterior derivative from its axioms](#uniqueness-of-the-exterior-derivative-from-its-axioms)
