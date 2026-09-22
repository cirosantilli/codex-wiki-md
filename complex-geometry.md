# Complex geometry

↑ **Parent:** [Geometry and topology](geometry-and-topology.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_geometry)

**Table of contents**

- [Complex structure](#complex-structure)
  - [Space of orthogonal complex structures](#space-of-orthogonal-complex-structures)
  - [Almost complex manifold](#almost-complex-manifold)
    - [Almost complex structure from a decomposable volume form](#almost-complex-structure-from-a-decomposable-volume-form)
      - [Closed decomposable complex volume forms are integrable](#closed-decomposable-complex-volume-forms-are-integrable)
    - [Type decomposition of the complexified tangent bundle](#type-decomposition-of-the-complexified-tangent-bundle)
    - [Totally real submanifold](#totally-real-submanifold)
    - [Compatible almost complex structure](#compatible-almost-complex-structure)
      - [Contractibility of compatible almost complex structures](#contractibility-of-compatible-almost-complex-structures)
      - [Compatible triple](#compatible-triple)
      - [Metric construction of a compatible almost complex structure](#metric-construction-of-a-compatible-almost-complex-structure)
      - [Relative extension of a compatible almost complex structure](#relative-extension-of-a-compatible-almost-complex-structure)
    - [Nijenhuis tensor](#nijenhuis-tensor)
    - [Integrable almost complex structure](#integrable-almost-complex-structure)
      - [Bracket and differential-form criteria for integrability](#bracket-and-differential-form-criteria-for-integrability)
      - [Newlander-Nirenberg theorem](#newlander-nirenberg-theorem)
      - [Complex manifold](#complex-manifold)
        - [Holomorphic map between complex manifolds](#holomorphic-map-between-complex-manifolds)
        - [Smooth proper family of compact complex manifolds](#smooth-proper-family-of-compact-complex-manifolds)
        - [Irreducible analytic subvariety of a complex manifold](#irreducible-analytic-subvariety-of-a-complex-manifold)
        - [Complex surface](#complex-surface)
          - [K3 surface](#k3-surface)
            - [Fermat quartic surface](#fermat-quartic-surface)
            - [Global Torelli theorem for K3 surfaces](#global-torelli-theorem-for-k3-surfaces)
            - [K3 linear system dichotomies](#k3-linear-system-dichotomies)
            - [Trigonal linear system on a K3 surface](#trigonal-linear-system-on-a-k3-surface)
            - [Hyperelliptic linear system on a K3 surface](#hyperelliptic-linear-system-on-a-k3-surface)
            - [Elliptic pencil on a K3 surface](#elliptic-pencil-on-a-k3-surface)
              - [Monogonal linear system on a K3 surface](#monogonal-linear-system-on-a-k3-surface)
            - [Moduli space of Ricci-flat K3 metrics](#moduli-space-of-ricci-flat-k3-metrics)
            - [K3 intersection lattice](#k3-intersection-lattice)
            - [Fixed-part elimination on a K3 surface](#fixed-part-elimination-on-a-k3-surface)
            - [Self-intersection of a smooth curve on a K3 surface](#self-intersection-of-a-smooth-curve-on-a-k3-surface)
            - [Elliptic K3 surface from a quartic containing a line](#elliptic-k3-surface-from-a-quartic-containing-a-line)
        - [Hopf surface](#hopf-surface)
        - [Hartogs's extension theorem](#hartogs-s-extension-theorem)
        - [Holomorphic atlas](#holomorphic-atlas)
        - [Stein manifold](#stein-manifold)
          - [Oka-Grauert principle](#oka-grauert-principle)
          - [Cartan theorem B](#cartan-theorem-b)
        - [Structure sheaf of a complex manifold](#structure-sheaf-of-a-complex-manifold)
          - [Ideal sheaf of a point on a complex manifold](#ideal-sheaf-of-a-point-on-a-complex-manifold)
        - [Polydisc](#polydisc)
        - [Holomorphic coordinate](#holomorphic-coordinate)
        - [Holomorphic embedding](#holomorphic-embedding)
        - [Holomorphic tangent bundle](#holomorphic-tangent-bundle)
          - [Holomorphic tangent connection and mixed torsion criterion](#holomorphic-tangent-connection-and-mixed-torsion-criterion)
          - [Holomorphic cotangent bundle](#holomorphic-cotangent-bundle)
        - [Almost complex structure induced by a complex atlas](#almost-complex-structure-induced-by-a-complex-atlas)
        - [Differential form of type (p, q)](#differential-form-of-type-p-q)
          - [Real (p, p)-form](#real-p-p-form)
          - [Complex conjugation of differential-form type](#complex-conjugation-of-differential-form-type)
        - [d c operator](#d-c-operator)
        - [Holomorphic vector field](#holomorphic-vector-field)
          - [Euler vector field](#euler-vector-field)
          - [Projectivization of a linear vector field](#projectivization-of-a-linear-vector-field)
        - [Complex submanifold](#complex-submanifold)
          - [Nonsingular analytic subvariety](#nonsingular-analytic-subvariety)
          - [Smooth submanifolds with invariant complex tangent spaces are complex](#smooth-submanifolds-with-invariant-complex-tangent-spaces-are-complex)
          - [Holomorphic normal bundle](#holomorphic-normal-bundle)
            - [Normal bundle of a regular zero locus](#normal-bundle-of-a-regular-zero-locus)
            - [Normal bundle of a smooth analytic hypersurface](#normal-bundle-of-a-smooth-analytic-hypersurface)
            - [Holomorphic conormal sequence](#holomorphic-conormal-sequence)
              - [Holomorphic conormal bundle](#holomorphic-conormal-bundle)
                - [Conormal line of a smooth analytic hypersurface](#conormal-line-of-a-smooth-analytic-hypersurface)
          - [Complex analytic hypersurface](#complex-analytic-hypersurface)
            - [Local defining function of a complex analytic hypersurface](#local-defining-function-of-a-complex-analytic-hypersurface)
              - [Reduced local defining functions differ by a holomorphic unit](#reduced-local-defining-functions-differ-by-a-holomorphic-unit)
            - [Divisor on a complex manifold](#divisor-on-a-complex-manifold)
              - [Order of a meromorphic function along a hypersurface](#order-of-a-meromorphic-function-along-a-hypersurface)
              - [Principal divisor on a complex manifold](#principal-divisor-on-a-complex-manifold)
              - [Holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor)
                - [Additivity of analytic divisor line bundles](#additivity-of-analytic-divisor-line-bundles)
              - [Sheaf of meromorphic functions on a complex manifold](#sheaf-of-meromorphic-functions-on-a-complex-manifold)
                - [Divisor sheaf on a complex manifold](#divisor-sheaf-on-a-complex-manifold)
                  - [Divisor-to-Picard map](#divisor-to-picard-map)
                - [Principal part of a meromorphic function](#principal-part-of-a-meromorphic-function)
                  - [Sheaf of meromorphic principal parts](#sheaf-of-meromorphic-principal-parts)
                  - [Mittag-Leffler problem on a Riemann surface](#mittag-leffler-problem-on-a-riemann-surface)
        - [Dolbeault operator](#dolbeault-operator)
          - [Bundle-valued Dolbeault adjoint](#bundle-valued-dolbeault-adjoint)
          - [Conjugate Dolbeault operator](#conjugate-dolbeault-operator)
          - [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma)
            - [Coordinate elimination for local Dolbeault primitives](#coordinate-elimination-for-local-dolbeault-primitives)
            - [Conjugate Dolbeault-Poincaré lemma](#conjugate-dolbeault-poincare-lemma)
            - [Cauchy-Green operator](#cauchy-green-operator)
          - [Dolbeault cohomology](#dolbeault-cohomology)
            - [Dolbeault cohomology of the projective line](#dolbeault-cohomology-of-the-projective-line)
            - [Laurent gluing of Dolbeault primitives on the projective line](#laurent-gluing-of-dolbeault-primitives-on-the-projective-line)
            - [Stein vanishing for the Dolbeault cohomology of functions](#stein-vanishing-for-the-dolbeault-cohomology-of-functions)
            - [Dolbeault cohomology of the projective line times the affine line](#dolbeault-cohomology-of-the-projective-line-times-the-affine-line)
            - [Dolbeault cohomology with values in a holomorphic vector bundle](#dolbeault-cohomology-with-values-in-a-holomorphic-vector-bundle)
              - [Curvature Dolbeault class](#curvature-dolbeault-class)
                - [Čech cocycle for the curvature Dolbeault class](#cech-cocycle-for-the-curvature-dolbeault-class)
                - [Metric independence of curvature Dolbeault powers](#metric-independence-of-curvature-dolbeault-powers)
            - [Dolbeault cohomology of a complex torus](#dolbeault-cohomology-of-a-complex-torus)
            - [Bott-Chern cohomology](#bott-chern-cohomology)
              - [Bott-Chern cohomology of a compact Kähler manifold](#bott-chern-cohomology-of-a-compact-kahler-manifold)
              - [Bott-Chern Poincaré lemma](#bott-chern-poincare-lemma)
            - [Dolbeault theorem](#dolbeault-theorem)
              - [Dolbeault resolution of holomorphic differential forms](#dolbeault-resolution-of-holomorphic-differential-forms)
            - [Hodge number](#hodge-number)
              - [Hodge duality](#hodge-duality)
              - [Hodge symmetry](#hodge-symmetry)
        - [Holomorphic vector bundle](#holomorphic-vector-bundle)
          - [Unitary flat holomorphic vector bundle](#unitary-flat-holomorphic-vector-bundle)
            - [Holomorphic sections of a unitary flat bundle are parallel](#holomorphic-sections-of-a-unitary-flat-bundle-are-parallel)
          - [Degree of a holomorphic vector bundle](#degree-of-a-holomorphic-vector-bundle)
            - [Slope of a holomorphic vector bundle](#slope-of-a-holomorphic-vector-bundle)
              - [Subbundle slope bound from ambient Chern curvature](#subbundle-slope-bound-from-ambient-chern-curvature)
              - [Semistable holomorphic vector bundle](#semistable-holomorphic-vector-bundle)
          - [Holomorphic splitting of transition functions on a trivial bundle](#holomorphic-splitting-of-transition-functions-on-a-trivial-bundle)
          - [Holomorphic subbundle](#holomorphic-subbundle)
          - [Holomorphic dual vector bundle](#holomorphic-dual-vector-bundle)
          - [Sheaf of holomorphic sections of a vector bundle](#sheaf-of-holomorphic-sections-of-a-vector-bundle)
          - [Holomorphic line bundle](#holomorphic-line-bundle)
            - [Sections of the degree-one line bundle on the projective line](#sections-of-the-degree-one-line-bundle-on-the-projective-line)
            - [Two-section criterion for holomorphic triviality](#two-section-criterion-for-holomorphic-triviality)
            - [Smoothly trivial holomorphic line bundles when H01 vanishes](#smoothly-trivial-holomorphic-line-bundles-when-h01-vanishes)
            - [Meromorphic section of a holomorphic line bundle](#meromorphic-section-of-a-holomorphic-line-bundle)
            - [Principal part of a meromorphic section](#principal-part-of-a-meromorphic-section)
            - [Holomorphic exponential sequence](#holomorphic-exponential-sequence)
            - [Dolbeault partial connection](#dolbeault-partial-connection)
          - [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle)
            - [Semipositive holomorphic line bundle](#semipositive-holomorphic-line-bundle)
            - [Metric compatibility as parallelism of a Hermitian tensor](#metric-compatibility-as-parallelism-of-a-hermitian-tensor)
            - [Quotient Hermitian metric](#quotient-hermitian-metric)
            - [Positive holomorphic line bundle](#positive-holomorphic-line-bundle)
              - [Kodaira vanishing theorem](#kodaira-vanishing-theorem)
                - [Vanishing for divisor twists on a complex torus](#vanishing-for-divisor-twists-on-a-complex-torus)
              - [Spectral gap for powers of a positive line bundle](#spectral-gap-for-powers-of-a-positive-line-bundle)
              - [Kodaira embedding theorem](#kodaira-embedding-theorem)
          - [Holomorphic local trivialization](#holomorphic-local-trivialization)
          - [Holomorphic section](#holomorphic-section)
            - [Rank-one sections of two hyperplane line bundles](#rank-one-sections-of-two-hyperplane-line-bundles)
        - [Complex cylinder](#complex-cylinder)
        - [Complex torus](#complex-torus)
          - [Semipositive canonical bundle of a submanifold of a complex torus](#semipositive-canonical-bundle-of-a-submanifold-of-a-complex-torus)
          - [Period matrix of a complex torus](#period-matrix-of-a-complex-torus)
          - [Averaging Kähler forms over a complex torus](#averaging-kahler-forms-over-a-complex-torus)
          - [Affine lift of a holomorphic map between complex tori](#affine-lift-of-a-holomorphic-map-between-complex-tori)
          - [Negation map on a one-dimensional complex torus](#negation-map-on-a-one-dimensional-complex-torus)
            - [Quotient of a one-dimensional complex torus by negation](#quotient-of-a-one-dimensional-complex-torus-by-negation)
          - [Holomorphic map from the complex plane to a one-dimensional complex torus](#holomorphic-map-from-the-complex-plane-to-a-one-dimensional-complex-torus)
          - [Affine lift of a holomorphic map between one-dimensional complex tori](#affine-lift-of-a-holomorphic-map-between-one-dimensional-complex-tori)
          - [Automorphism of a one-dimensional complex torus](#automorphism-of-a-one-dimensional-complex-torus)
          - [Riemann form on a complex torus](#riemann-form-on-a-complex-torus)
            - [Integral Hermitian forms on the square complex torus](#integral-hermitian-forms-on-the-square-complex-torus)
            - [Riemann bilinear criterion for a period matrix](#riemann-bilinear-criterion-for-a-period-matrix)
            - [Polarization of a complex torus](#polarization-of-a-complex-torus)
          - [Appell–Humbert theorem](#appell-humbert-theorem)
            - [Semicharacter of a complex lattice](#semicharacter-of-a-complex-lattice)
          - [Complex subtorus](#complex-subtorus)
          - [Isogeny of complex tori](#isogeny-of-complex-tori)
        - [Hermitian manifold](#hermitian-manifold)
          - [Lefschetz operator on a Hermitian manifold](#lefschetz-operator-on-a-hermitian-manifold)
            - [Injectivity of powers of the Lefschetz operator](#injectivity-of-powers-of-the-lefschetz-operator)
          - [Fundamental form of a Hermitian manifold](#fundamental-form-of-a-hermitian-manifold)
            - [Hodge star of the fundamental Hermitian form](#hodge-star-of-the-fundamental-hermitian-form)
          - [Real (1, 1)-form](#real-1-1-form)
            - [Positive real (1, 1)-form](#positive-real-1-1-form)
              - [Wedge positivity for two positive (1, 1)-forms](#wedge-positivity-for-two-positive-1-1-forms)
        - [Kähler manifold](#kahler-manifold)
          - [Calabi-Yau threefold](#calabi-yau-threefold)
          - [Kähler cone](#kahler-cone)
            - [Kähler class](#kahler-class)
          - [Kähler metric](#kahler-metric)
            - [Hodge metric](#hodge-metric)
            - [Kähler normal holomorphic coordinates](#kahler-normal-holomorphic-coordinates)
            - [Kähler form](#kahler-form)
              - [Powers of a compact Kähler form have nonzero cohomology classes](#powers-of-a-compact-kahler-form-have-nonzero-cohomology-classes)
              - [Local real potential for a closed (1,1)-form](#local-real-potential-for-a-closed-1-1-form)
                - [Rotation-invariant Kähler potential on the complex plane](#rotation-invariant-kahler-potential-on-the-complex-plane)
                  - [Positivity criterion for a radial Kähler potential](#positivity-criterion-for-a-radial-kahler-potential)
            - [Kähler potential (complex geometry)](#kahler-potential-complex-geometry)
              - [Radial Kähler metric with Euclidean volume in complex dimension two](#radial-kahler-metric-with-euclidean-volume-in-complex-dimension-two)
          - [Kähler quotient](#kahler-quotient)
          - [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)
            - [Hard Lefschetz theorem on de Rham cohomology](#hard-lefschetz-theorem-on-de-rham-cohomology)
            - [Hard Lefschetz isomorphism on Dolbeault cohomology](#hard-lefschetz-isomorphism-on-dolbeault-cohomology)
            - [Dependence of Lefschetz maps on the Dolbeault class](#dependence-of-lefschetz-maps-on-the-dolbeault-class)
            - [Primitive differential form on a Kähler manifold](#primitive-differential-form-on-a-kahler-manifold)
              - [Primitive (1,1)-forms on a Kähler surface are anti-self-dual](#primitive-1-1-forms-on-a-kahler-surface-are-anti-self-dual)
            - [Lefschetz commutator](#lefschetz-commutator)
              - [Commutator formula for powers of the Lefschetz operator](#commutator-formula-for-powers-of-the-lefschetz-operator)
            - [Adjoint Lefschetz operator](#adjoint-lefschetz-operator)
            - [Kähler identities](#kahler-identities)
              - [Bundle-valued Kähler identities](#bundle-valued-kahler-identities)
                - [Lefschetz-Dolbeault curvature commutator](#lefschetz-dolbeault-curvature-commutator)
                  - [Flatness criterion from Lefschetz commutation](#flatness-criterion-from-lefschetz-commutation)
              - [Bochner-Kodaira-Nakano identity](#bochner-kodaira-nakano-identity)
              - [Dolbeault Laplacian](#dolbeault-laplacian)
                - [Dolbeault Green operator](#dolbeault-green-operator)
                - [Kähler Laplacian identity](#kahler-laplacian-identity)
                  - [Harmonicity of holomorphic functions on a Kähler manifold](#harmonicity-of-holomorphic-functions-on-a-kahler-manifold)
                - [Lefschetz operator preserves harmonic forms](#lefschetz-operator-preserves-harmonic-forms)
                - [Dolbeault Hodge decomposition on a compact Hermitian manifold](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold)
                  - [Complementary Dolbeault harmonic types on a Hermitian manifold](#complementary-dolbeault-harmonic-types-on-a-hermitian-manifold)
                  - [ddbar lemma](#ddbar-lemma)
                    - [Global potential for cohomologous Kähler forms](#global-potential-for-cohomologous-kahler-forms)
                    - [Harmonic orthogonality criterion for ddbar exactness](#harmonic-orthogonality-criterion-for-ddbar-exactness)
                      - [Green operator potential for ddbar exactness](#green-operator-potential-for-ddbar-exactness)
                    - [ddc lemma](#ddc-lemma)
          - [Fubini-Study metric](#fubini-study-metric)
            - [Fubini-Study form](#fubini-study-form)
              - [Integrally normalized Fubini-Study form](#integrally-normalized-fubini-study-form)
              - [Fubini-Study form from circle reduction](#fubini-study-form-from-circle-reduction)
                - [Symplectic ball chart in complex projective space](#symplectic-ball-chart-in-complex-projective-space)
                  - [Two-ball packing obstruction in the projective plane](#two-ball-packing-obstruction-in-the-projective-plane)
          - [Hodge decomposition theorem for compact Kähler manifolds](#hodge-decomposition-theorem-for-compact-kahler-manifolds)
            - [Primitive cohomology](#primitive-cohomology)
              - [Hodge–Riemann bilinear relations](#hodge-riemann-bilinear-relations)
            - [Odd Betti numbers of a compact Kähler manifold are even](#odd-betti-numbers-of-a-compact-kahler-manifold-are-even)
            - [Hodge index theorem for compact Kähler surfaces](#hodge-index-theorem-for-compact-kahler-surfaces)
        - [Canonical bundle](#canonical-bundle)
          - [Poincaré residue along a smooth hypersurface](#poincare-residue-along-a-smooth-hypersurface)
            - [Residue trivialization for a degree n+1 projective hypersurface](#residue-trivialization-for-a-degree-n-plus-1-projective-hypersurface)
          - [Holomorphic cubic differential](#holomorphic-cubic-differential)
          - [Quadratic differential](#quadratic-differential)
            - [Flat metric of a quadratic differential](#flat-metric-of-a-quadratic-differential)
              - [Area of a quadratic differential](#area-of-a-quadratic-differential)
            - [Half-translation surface](#half-translation-surface)
            - [Holomorphic quadratic differential](#holomorphic-quadratic-differential)
          - [Holomorphic differential form](#holomorphic-differential-form)
            - [Order of a zero of a differential](#order-of-a-zero-of-a-differential)
            - [Natural coordinate of a holomorphic differential](#natural-coordinate-of-a-holomorphic-differential)
            - [Holomorphic one-form](#holomorphic-one-form)
              - [Stratum of holomorphic one-forms](#stratum-of-holomorphic-one-forms)
            - [Holomorphic forms on a compact complex surface are closed](#holomorphic-forms-on-a-compact-complex-surface-are-closed)
              - [Betti and Hodge bounds for compact complex surfaces](#betti-and-hodge-bounds-for-compact-complex-surfaces)
            - [Holomorphic forms on a compact Kähler manifold are closed](#holomorphic-forms-on-a-compact-kahler-manifold-are-closed)
            - [Holomorphic de Rham complex](#holomorphic-de-rham-complex)
              - [Sheaf of holomorphic differential forms](#sheaf-of-holomorphic-differential-forms)
                - [Holomorphic p-form on a complex manifold](#holomorphic-p-form-on-a-complex-manifold)
                  - [Nonzero holomorphic top forms are not exact](#nonzero-holomorphic-top-forms-are-not-exact)
              - [Sheaf of closed holomorphic one-forms](#sheaf-of-closed-holomorphic-one-forms)
              - [Holomorphic Poincaré lemma](#holomorphic-poincare-lemma)
                - [Coordinate-integral primitive on a polydisc](#coordinate-integral-primitive-on-a-polydisc)
            - [Holomorphic differentials on a smooth plane curve](#holomorphic-differentials-on-a-smooth-plane-curve)
          - [Adjunction formula](#adjunction-formula)
            - [Smooth rational-curve self-intersection on a projective hypersurface](#smooth-rational-curve-self-intersection-on-a-projective-hypersurface)
            - [Canonical bundle of a regular projective complete intersection](#canonical-bundle-of-a-regular-projective-complete-intersection)
            - [Adjunction for a smooth submanifold](#adjunction-for-a-smooth-submanifold)
        - [First Chern class](#first-chern-class)
          - [Symplectic canonical class](#symplectic-canonical-class)
          - [Čech-de Rham curvature descent](#cech-de-rham-curvature-descent)
          - [First Chern class of a tensor product of complex line bundles](#first-chern-class-of-a-tensor-product-of-complex-line-bundles)
          - [Chern connection](#chern-connection)
            - [Torsion-free Chern tangent connection characterizes a Kähler metric](#torsion-free-chern-tangent-connection-characterizes-a-kahler-metric)
            - [Chern curvature](#chern-curvature)
            - [Chern connection component adjoint](#chern-connection-component-adjoint)
            - [Dolbeault closedness of Chern curvature](#dolbeault-closedness-of-chern-curvature)
            - [Trace of Chern curvature](#trace-of-chern-curvature)
            - [Projected Chern connection](#projected-chern-connection)
              - [Second fundamental form of a holomorphic subbundle](#second-fundamental-form-of-a-holomorphic-subbundle)
                - [Curvature formula for a holomorphic subbundle](#curvature-formula-for-a-holomorphic-subbundle)
            - [Normalized curvature form of a Hermitian holomorphic line bundle](#normalized-curvature-form-of-a-hermitian-holomorphic-line-bundle)
            - [Local formula for the Chern connection on a vector bundle](#local-formula-for-the-chern-connection-on-a-vector-bundle)
              - [Chern connection in a normal holomorphic frame](#chern-connection-in-a-normal-holomorphic-frame)
            - [Curvature difference of two Chern connections](#curvature-difference-of-two-chern-connections)
            - [Local formula for the Chern connection on a line bundle](#local-formula-for-the-chern-connection-on-a-line-bundle)
            - [Ricci form of a Kähler manifold](#ricci-form-of-a-kahler-manifold)
        - [Blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point)
          - [Projective pencil resolved by a point blowup](#projective-pencil-resolved-by-a-point-blowup)
          - [Canonical bundle formula for a point blowup](#canonical-bundle-formula-for-a-point-blowup)
            - [Anticanonical strict transform under a point blowup](#anticanonical-strict-transform-under-a-point-blowup)
          - [Exceptional divisor](#exceptional-divisor)
            - [Nontrivial powers of the exceptional line bundle of a point blowup](#nontrivial-powers-of-the-exceptional-line-bundle-of-a-point-blowup)
          - [Strict transform](#strict-transform)
          - [Pencil of plane cubics](#pencil-of-plane-cubics)
            - [Rational elliptic surface](#rational-elliptic-surface)
              - [Elliptic fibration of the rational elliptic surface](#elliptic-fibration-of-the-rational-elliptic-surface)
                - [Canonical class of the rational elliptic surface](#canonical-class-of-the-rational-elliptic-surface)
                  - [Genus formula for a multisection of the rational elliptic surface](#genus-formula-for-a-multisection-of-the-rational-elliptic-surface)

## Complex structure

↑ **Parent:** [Complex geometry](complex-geometry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_structure)

A complex structure on a real vector space or vector bundle is an endomorphism $J$ satisfying $J^2=-I$. On a [smooth manifold](differential-geometry.md#smooth-manifold), an integrable complex structure determines holomorphic coordinate charts.

### Space of orthogonal complex structures

↑ **Parent:** [Complex structure](#complex-structure)

On a Euclidean real space of dimension $2n$, an orthogonal [complex structure](#complex-structure) is an orthogonal endomorphism $J$ with $J^2=-I$. Orthogonal changes of basis act transitively on these structures, and the stabilizer of the standard structure is $U(n)$. The compact [homogeneous space](lie-theory.md#homogeneous-space) has real dimension $n(n-1)$.

// Target: geometry-and-topology.bigb

### Almost complex manifold

↑ **Parent:** [Complex structure](#complex-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Almost_complex_manifold)

An almost complex manifold is a smooth manifold $X$ with a bundle endomorphism $J:TX\to TX$ satisfying $J^2=-I$.

#### Almost complex structure from a decomposable volume form

↑ **Parent:** [Almost complex manifold](#almost-complex-manifold)

A locally decomposable complex $n$-form $\Omega$ on a real $2n$-manifold, with $\Omega\wedge\overline\Omega$ nowhere zero, determines an [almost complex structure](#almost-complex-manifold). The intrinsic rank-$n$ subbundle $W=\{\alpha\in T^*M\otimes\mathbb C:\alpha\wedge\Omega=0\}$ is locally spanned by the factors of $\Omega$. The nonvanishing condition gives $T^*M\otimes\mathbb C=W\oplus\overline W$. Set $J^*=i$ on $W$ and $J^*=-i$ on $\overline W$. This commutes with conjugation, so comes from a unique real bundle endomorphism with square $-I$.

##### Closed decomposable complex volume forms are integrable

↑ **Parent:** [Almost complex structure from a decomposable volume form](#almost-complex-structure-from-a-decomposable-volume-form)

If $\Omega=\theta_1\wedge\cdots\wedge\theta_n$ and $d\Omega=0$, differentiating $\theta_j\wedge\Omega=0$ gives $d\theta_j\wedge\Omega=0$. Only the $(0,2)$ component of $d\theta_j$ can survive this wedge product; multiplication by $\Omega$ is injective on that component. Thus no $d\theta_j$ has a $(0,2)$ part. The [bracket and differential-form criteria for integrability](#bracket-and-differential-form-criteria-for-integrability) make the induced [almost complex structure](#almost-complex-manifold) integrable. Local decomposability is part of the hypothesis and is not implied solely by nonvanishing of $\Omega\wedge\overline\Omega$.

#### Type decomposition of the complexified tangent bundle

↑ **Parent:** [Almost complex manifold](#almost-complex-manifold)

An [almost complex structure](#almost-complex-manifold) $J$ gives the $+i$ and $-i$ [eigenbundles](fiber-bundle.md#eigenbundle) of its complex-linear extension. Their projections are $(I-iJ)/2$ and $(I+iJ)/2$. For an integrable structure the first is the [holomorphic tangent bundle](#holomorphic-tangent-bundle).

#### Totally real submanifold

↑ **Parent:** [Almost complex manifold](#almost-complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Totally_real_submanifold)

In the maximal-dimension convention, a totally real submanifold of $(M,J)$ has half the real dimension of $M$ and $T_pL\cap J(T_pL)=0$. Every [Lagrangian submanifold](symplectic-geometry.md#lagrangian-submanifold) is totally real for a [compatible almost complex structure](#compatible-almost-complex-structure), but the converse fails in complex dimension at least two.

#### Compatible almost complex structure

↑ **Parent:** [Almost complex manifold](#almost-complex-manifold)

An [almost complex structure](#almost-complex-manifold) $J$ on a [symplectic manifold](symplectic-geometry.md#symplectic-manifold) $(M,\omega)$ is compatible with $\omega$ when

$$
\omega(Ju,Jv)=\omega(u,v)
$$

and $g_J(u,v)=\omega(u,Jv)$ is a positive-definite [inner product](linear-algebra.md#inner-product). Every symplectic vector bundle admits a compatible almost complex structure.

##### Contractibility of compatible almost complex structures

↑ **Parent:** [Compatible almost complex structure](#compatible-almost-complex-structure)

The [metric construction of a compatible almost complex structure](#metric-construction-of-a-compatible-almost-complex-structure) is continuous in the auxiliary [Riemannian metric](differential-geometry.md#riemannian-metric), and recovers $J$ when applied to $g_J=\omega(\cdot,J\cdot)$. Interpolating $g_J$ linearly to a fixed auxiliary metric therefore contracts the space of [compatible almost complex structures](#compatible-almost-complex-structure). In particular it is nonempty and path connected.

##### Compatible triple

↑ **Parent:** [Compatible almost complex structure](#compatible-almost-complex-structure)

A compatible triple consists of a [symplectic form](symplectic-geometry.md#symplectic-form), a [compatible almost complex structure](#compatible-almost-complex-structure), and the [Riemannian metric](differential-geometry.md#riemannian-metric) $g(u,v)=\omega(u,Jv)$. Equivalently $g(Ju,v)=\omega(u,v)$.

##### Metric construction of a compatible almost complex structure

↑ **Parent:** [Compatible almost complex structure](#compatible-almost-complex-structure)

Choose an auxiliary [Riemannian metric](differential-geometry.md#riemannian-metric) $h$ and define the skew-adjoint bundle map $A$ by $\omega(u,v)=h(Au,v)$. Then

$$
J=A(-A^2)^{-1/2}
$$

is a [compatible almost complex structure](#compatible-almost-complex-structure). The positive square root is defined fiberwise by the [spectral theorem for normal operators](hilbert-space.md#spectral-theorem-for-normal-operators), and its smooth dependence on $A$ makes $J$ smooth.

##### Relative extension of a compatible almost complex structure

↑ **Parent:** [Compatible almost complex structure](#compatible-almost-complex-structure)

If a compatible almost complex structure is prescribed along a closed [symplectic submanifold](symplectic-geometry.md#symplectic-submanifold) $N\subset M$ and preserves $TN$, it extends to one on $M$. Choose a compatible structure separately on $TN$ and its [symplectic normal bundle](symplectic-geometry.md#symplectic-normal-bundle), use the associated metric along $N$, extend that metric to $M$, and apply the [metric construction of a compatible almost complex structure](#metric-construction-of-a-compatible-almost-complex-structure).

#### Nijenhuis tensor

↑ **Parent:** [Almost complex manifold](#almost-complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nijenhuis_tensor)

The Nijenhuis tensor of an [almost complex manifold](#almost-complex-manifold) is

$$
N_J(U,V)=[JU,JV]-J[JU,V]-J[U,JV]-[U,V].
$$

It measures the failure of the $(0,1)$ tangent distribution to be closed under the [Lie bracket](lie-algebra.md#lie-bracket).

#### Integrable almost complex structure

↑ **Parent:** [Almost complex manifold](#almost-complex-manifold)

An almost complex structure is integrable when it comes from holomorphic coordinate charts. Equivalently, its Nijenhuis tensor vanishes, or the $(0,1)$ vector fields are closed under Lie bracket.

##### Bracket and differential-form criteria for integrability

↑ **Parent:** [Integrable almost complex structure](#integrable-almost-complex-structure)

For an [almost complex structure](#almost-complex-manifold), closure of $T^{1,0}$ under the [Lie bracket](lie-algebra.md#lie-bracket) is equivalent to the absence of a $(0,2)$ component in $d\alpha$ for every $(1,0)$-form $\alpha$. Conjugation exchanges the bracket condition with closure of $T^{0,1}$. For sections $U,V$ of $T^{0,1}$, the [exterior derivative](differential-form.md#exterior-derivative) identity gives $d\alpha(U,V)=-\alpha([U,V])$. Its vanishing for all $(1,0)$-forms is exactly $[U,V]\in T^{0,1}$.

##### Newlander-Nirenberg theorem

↑ **Parent:** [Integrable almost complex structure](#integrable-almost-complex-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newlander-Nirenberg_theorem)

The Newlander-Nirenberg theorem says that a smooth [almost complex structure](#almost-complex-manifold) is [integrable](#integrable-almost-complex-structure) if and only if its [Nijenhuis tensor](#nijenhuis-tensor) vanishes.

##### Complex manifold

↑ **Parent:** [Integrable almost complex structure](#integrable-almost-complex-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_manifold)

A complex $n$-manifold has charts to $\mathbb C^n$ with holomorphic transition maps. It is a real $2n$-manifold with an integrable almost complex structure.

###### Holomorphic map between complex manifolds

↑ **Parent:** [Complex manifold](#complex-manifold)

A map between [complex manifolds](#complex-manifold) is holomorphic when its local coordinate expression has holomorphic scalar components. For a smooth map, this is equivalent to its differential being complex-linear at every point. These maps compose by the chain rule. For one-dimensional manifolds this reduces to a [holomorphic map](complex-analysis.md#holomorphic-map) between [Riemann surfaces](complex-analysis.md#riemann-surfaces); the general definition also applies to multiplication and inversion on a [complex Lie group](lie-theory.md#complex-lie-group).

###### Smooth proper family of compact complex manifolds

↑ **Parent:** [Complex manifold](#complex-manifold)

A proper holomorphic submersion has compact smooth fibres, and the [Ehresmann fibration theorem](fiber-bundle.md#ehresmann-fibration-theorem) gives differentiable local trivializations. Their integral cohomology, modulo torsion, forms a [local system](ringed-space.md#local-system). If the fibres are [Kähler manifolds](#kahler-manifold), their Hodge filtrations form holomorphic subbundles and give a [variation of Hodge structure](differential-geometry.md#variation-of-hodge-structure). Properness is needed for this usual conclusion.

###### Irreducible analytic subvariety of a complex manifold

↑ **Parent:** [Complex manifold](#complex-manifold)

An analytic subvariety is a closed subset locally defined by finitely many [holomorphic functions](complex-analysis.md#holomorphic-function). It is irreducible if it is not the union of two proper closed analytic subsets. An irreducible analytic subvariety of complex codimension $k$ in an $n$-dimensional [complex manifold](#complex-manifold) has pure complex dimension $n-k$. Global irreducibility does not forbid multiple local branches at a singular point.

###### Complex surface

↑ **Parent:** [Complex manifold](#complex-manifold)

A complex surface is a [complex manifold](#complex-manifold) of complex dimension two, hence real dimension four. Compact complex surfaces need not admit a [Kähler metric](#kahler-metric); a [Hopf surface](#hopf-surface) is an example. Every [holomorphic one-form](#holomorphic-one-form) on a compact complex surface is closed, and the [Betti and Hodge bounds for compact complex surfaces](#betti-and-hodge-bounds-for-compact-complex-surfaces) still apply without Kähler assumptions.

###### K3 surface

↑ **Parent:** [Complex surface](#complex-surface)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/K3_surface)

A complex [K3 surface](#k3-surface) is a compact, simply connected [complex surface](#complex-surface) with trivial [canonical bundle](#canonical-bundle). For projective [algebraic surfaces](algebraic-geometry.md#algebraic-surface), one can equivalently require a trivial [canonical bundle](#canonical-bundle) and $H^1(X,\mathcal O_X)=0$. Nonprojective complex [K3 surfaces](#k3-surface) are also included, which is essential for the full [moduli space of Ricci-flat K3 metrics](#moduli-space-of-ricci-flat-k3-metrics).

###### Fermat quartic surface

↑ **Parent:** [K3 surface](#k3-surface)

Over $\mathbb C$, the four partial derivatives show that this projective surface is smooth. Adjunction makes its [canonical bundle](#canonical-bundle) trivial, and the hypersurface [exact sequence](homology.md#exact-sequence) gives $H^1(\mathcal O_X)=0$, so it is a [K3 surface](#k3-surface). Lines given by $x_0=\zeta x_1$, $x_2=\eta x_3$, with $\zeta^4=\eta^4=-1$, lie on it. Choosing both roots differently gives skew lines, one of which is a section of the elliptic pencil defined by planes through the other.

###### Global Torelli theorem for K3 surfaces

↑ **Parent:** [K3 surface](#k3-surface)

An integral Hodge isometry between complex [K3 surfaces](#k3-surface) which carries some [Kähler class](#kahler-class) to a Kähler class is the pullback of a unique [isomorphism](algebra.md#isomorphism) of the surfaces. A Hodge isometry without that cone condition need not itself be geometric: reflection in an effective $(-2)$-curve reverses its class and cannot be induced by an isomorphism.

###### K3 linear system dichotomies

↑ **Parent:** [K3 surface](#k3-surface)

For nef big systems on a complex [K3 surface](#k3-surface), the successive alternatives distinguish a [monogonal linear system on a K3 surface](#monogonal-linear-system-on-a-k3-surface) from a basepoint-free system; then a degree-two map from a birational map; then a projective ideal generated by quadrics from the trigonal and plane-quintic exceptions. The last alternatives must include the low-genus quartic and quadric-cubic models. The birational morphism can contract exactly the orthogonal $(-2)$-curves; it need not embed the original smooth surface.

###### Trigonal linear system on a K3 surface

↑ **Parent:** [K3 surface](#k3-surface)

For a basepoint-free nonhyperelliptic nef big divisor $D$, the trigonal condition means that its general smooth curve is a [trigonal curve](algebraic-geometry.md#trigonal-curve). An [elliptic pencil on a K3 surface](#elliptic-pencil-on-a-k3-surface) with $D\cdot E=3$ restricts to its degree-three pencil. On a smooth quartic containing a line $\Gamma$, the hyperplane class $H$ has this property for $E=H-\Gamma$.

###### Hyperelliptic linear system on a K3 surface

↑ **Parent:** [K3 surface](#k3-surface)

For a basepoint-free nef big divisor $D$, this means that the morphism given by its complete system is generically two-to-one onto its image. Equivalently, its general smooth curve is [hyperelliptic](algebraic-geometry.md#hyperelliptic-curve). A double cover of $\mathbb P^2$ branched over a smooth sextic, with the pullback of $\mathcal O(1)$, gives the degree-two example.

###### Elliptic pencil on a K3 surface

↑ **Parent:** [K3 surface](#k3-surface)

A primitive effective nef class of square zero on a complex [K3 surface](#k3-surface) defines a basepoint-free pencil with connected genus-one fibres. Its general fibre is a smooth [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve). A section is a [smooth rational curve](projective-space.md#smooth-rational-curve) $\Gamma$ with $E\cdot\Gamma=1$ and $\Gamma^2=-2$.

###### Monogonal linear system on a K3 surface

↑ **Parent:** [Elliptic pencil on a K3 surface](#elliptic-pencil-on-a-k3-surface)

For a nef big divisor, the monogonal case is the fixed-section system $|D|=\Gamma+|mE|$, where $E$ is an [elliptic pencil on a K3 surface](#elliptic-pencil-on-a-k3-surface) and $\Gamma$ is a section. Thus $D\cdot E=1$. The fixed part persists even though $D$ is nef; the general divisor is reducible. [Riemann–Roch theorem for algebraic surfaces](algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces) gives $h^0(D)=m+1=h^0(mE)$, proving the equality of systems.

###### Moduli space of Ricci-flat K3 metrics

↑ **Parent:** [K3 surface](#k3-surface)

Locally, a unit-volume [Ricci flat](differential-geometry.md#ricci-flat-manifold) metric on a [K3 surface](#k3-surface) determines a positive three-plane in its real second [cohomology](cohomology.md), with the [K3 intersection lattice](#k3-intersection-lattice) fixed. The corresponding Grassmannian has dimension $3\cdot19=57$. Allowing the volume gives one further positive real parameter; large diffeomorphisms identify lattice-equivalent descriptions. This is the same continuous moduli count as the three-torus [Narain moduli space](string-theory.md#narain-moduli-space) plus its coupling.

// Target: supersymmetry.bigb

###### K3 intersection lattice

↑ **Parent:** [K3 surface](#k3-surface)

The [cup product](cohomology.md#cup-product) on the second integral [cohomology](cohomology.md) of a complex [K3 surface](#k3-surface) is an [even unimodular lattice](linear-algebra.md#even-unimodular-lattice) of signature $(3,19)$. Here $U$ is the [hyperbolic plane](linear-algebra.md#hyperbolic-plane-quadratic-form) and $E_8(-1)$ is the negative-definite form of the [E8 lattice](linear-algebra.md#e8-lattice). In the [M-theory K3 duality](string-theory.md#m-theory-k3-duality), this lattice matches the heterotic electric charge lattice. The self-dual harmonic two-forms of a [Ricci flat](differential-geometry.md#ricci-flat-manifold) K3 metric span its positive three-plane.

###### Fixed-part elimination on a K3 surface

↑ **Parent:** [K3 surface](#k3-surface)

If $D$ is a nontrivial [nef divisor](cartier-divisor.md#nef-line-bundle) on a [K3 surface](#k3-surface) with $D^2=0$, its [complete linear system of a divisor](cartier-divisor.md#complete-linear-system-of-a-divisor) has no fixed part. Write $D=F+M$. Nefness of $D$ and $M$ gives $D\cdot F=D\cdot M=M^2=M\cdot F=F^2=0$. But a nonzero fixed part satisfies $h^0(F)=1$, while [Riemann–Roch theorem for algebraic surfaces](algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces) and [Serre duality](ringed-space.md#serre-duality) would give $h^0(F)\geq2$ if $F^2=0$. Hence $F=0$. Two movable members with no common component have intersection zero and are disjoint, so the system is [basepoint-free](cartier-divisor.md#basepoint-free-divisor) and has [Iitaka dimension](cartier-divisor.md#iitaka-dimension) one.

###### Self-intersection of a smooth curve on a K3 surface

↑ **Parent:** [K3 surface](#k3-surface)

If a smooth curve $C$ of genus $g$ lies on a [K3 surface](#k3-surface), the [adjunction formula](#adjunction-formula) and $K_X=0$ give

$$
C^2=2g-2.
$$

###### Elliptic K3 surface from a quartic containing a line

↑ **Parent:** [K3 surface](#k3-surface)

A smooth quartic surface $X\subseteq\mathbb P^3$ containing a line $L$ is a [K3 surface](#k3-surface). The pencil of planes through $L$ cuts out $L$ plus a residual plane cubic; the divisor class $H-L$ has square zero and its basepoint-free pencil defines an [elliptic fibration](algebraic-geometry.md#elliptic-surface) $X\to\mathbb P^1$.

###### Hopf surface

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopf_surface)

A primary Hopf surface is a quotient of $\mathbb C^2\setminus\{0\}$ by an infinite cyclic group generated by a suitable contracting holomorphic map; reversing the generator gives the expanding dilation description. The scalar dilation $z\mapsto2z$ gives a compact surface diffeomorphic to $S^3\times S^1$ via polar coordinates and log radius. Hence $b_1=1$. The [Betti and Hodge bounds for compact complex surfaces](#betti-and-hodge-bounds-for-compact-complex-surfaces) force $h^{1,0}=0$ and $h^{0,1}\geq1$, furnishing a strict example of $h^{1,0}<h^{0,1}$.

<h6 id="hartogs-s-extension-theorem">Hartogs's extension theorem</h6>

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hartogs's_extension_theorem)

In complex dimension at least two, a holomorphic function on a punctured coordinate ball extends holomorphically through its centre. Componentwise extension in a [holomorphic local frame](#holomorphic-local-trivialization) gives the same statement for [holomorphic sections](#holomorphic-section). This preserves global sections after removing finitely many points, but does not imply preservation of higher [sheaf cohomology](ringed-space.md#sheaf-cohomology). This analytic theorem differs from the set-theoretic [Hartogs theorem](set-theory.md#hartogs-theorem).

###### Holomorphic atlas

↑ **Parent:** [Complex manifold](#complex-manifold)

An atlas of charts into $\mathbb C^n$ whose transition maps are [biholomorphic](complex-analysis.md#biholomorphism). Their real [differentials](differential-geometry.md#differential-of-a-smooth-map) commute with multiplication by $i$, giving an [almost complex structure induced by a complex atlas](#almost-complex-structure-induced-by-a-complex-atlas).

###### Stein manifold

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stein_manifold)

A [complex manifold](#complex-manifold) is Stein if its global [holomorphic functions](complex-analysis.md#holomorphic-function) separate points, give local coordinates, and make it holomorphically convex: the holomorphic hull of every compact set is compact. Closed complex submanifolds of affine complex space are examples, including products of copies of $\mathbb C$ and $\mathbb C^*$. [Cartan theorem B](#cartan-theorem-b) makes these spaces useful for acyclic covers in [sheaf cohomology](ringed-space.md#sheaf-cohomology).

###### Oka-Grauert principle

↑ **Parent:** [Stein manifold](#stein-manifold)

For a complex Lie group, holomorphic [principal bundles](fiber-bundle.md#principal-bundle) over a [Stein manifold](#stein-manifold) are classified up to holomorphic isomorphism by their topological bundle class. In particular, a topologically trivial holomorphic [principal bundle](fiber-bundle.md#principal-bundle) over a Stein base has a global holomorphic trivialization. This supplies global complex gauges for a flat partial connection on contractible complex affine space; it does not impose prescribed behaviour at infinity.

###### Cartan theorem B

↑ **Parent:** [Stein manifold](#stein-manifold)

On a [Stein manifold](#stein-manifold) $X$, every [coherent analytic sheaf](ringed-space.md#coherent-analytic-sheaf) $\mathcal F$ has $H^q(X,\mathcal F)=0$ for $q>0$. In particular this applies to the [sheaf of holomorphic functions](#structure-sheaf-of-a-complex-manifold). If every nonempty finite intersection in an [open cover](topology.md#open-cover) is Stein, these vanishing results and the [acyclic cover theorem](ringed-space.md#leray-s-theorem) compute the corresponding [sheaf cohomology](ringed-space.md#sheaf-cohomology) from its [Čech cochain complex](ringed-space.md#cech-cochain-complex).

###### Structure sheaf of a complex manifold

↑ **Parent:** [Complex manifold](#complex-manifold)

The structure sheaf assigns to an open set its ring of [holomorphic functions](complex-analysis.md#holomorphic-function). Its invertible sections form the sheaf $\mathcal O_M^*$ of nowhere-zero [holomorphic functions](complex-analysis.md#holomorphic-function).

###### Ideal sheaf of a point on a complex manifold

↑ **Parent:** [Structure sheaf of a complex manifold](#structure-sheaf-of-a-complex-manifold)

This sheaf consists of [holomorphic functions](complex-analysis.md#holomorphic-function) vanishing at $p$ on opens containing $p$, and all [holomorphic functions](complex-analysis.md#holomorphic-function) on opens not containing $p$. Evaluation gives $0\to\mathcal I_p\to\mathcal O_M\to\mathbb C_p\to0$, with a [skyscraper sheaf](ringed-space.md#skyscraper-sheaf) as quotient. On an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve), $H^0(\mathcal I_p)=0$, $H^1(\mathcal I_p)\cong\mathbb C$, and all higher cohomology vanishes.

###### Polydisc

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polydisc)

A polydisc is a product of open discs in $\mathbb C$. It is a contractible [complex manifold](#complex-manifold), with vanishing positive-degree [de Rham cohomology](differential-form.md#de-rham-cohomology) and vanishing [Dolbeault cohomology](#dolbeault-cohomology) in positive antiholomorphic degree.

###### Holomorphic coordinate

↑ **Parent:** [Complex manifold](#complex-manifold)

A holomorphic coordinate chart on a [complex manifold](#complex-manifold) is a [biholomorphism](complex-analysis.md#biholomorphism) from an open subset of the manifold to an open subset of $\mathbb C^n$. Its component functions are holomorphic coordinates.

###### Holomorphic embedding

↑ **Parent:** [Complex manifold](#complex-manifold)

A holomorphic embedding is a [holomorphic map](complex-analysis.md#holomorphic-map) that is also a [smooth embedding](differential-geometry.md#smooth-embedding). Its image is a [complex submanifold](#complex-submanifold) and the map is a [biholomorphism](complex-analysis.md#biholomorphism) onto that image.

###### Holomorphic tangent bundle

↑ **Parent:** [Complex manifold](#complex-manifold)

The holomorphic tangent bundle of a [complex manifold](#complex-manifold) $X$ is locally spanned in [holomorphic coordinates](#holomorphic-coordinate) by $\partial/\partial z^1,\ldots,\partial/\partial z^n$. Under a holomorphic coordinate change $w=w(z)$, the [chain rule](calculus.md#chain-rule) gives

$$
\frac{\partial}{\partial z^j}
=\sum_k\frac{\partial w^k}{\partial z^j}\frac{\partial}{\partial w^k},
$$

whose coefficient matrix is holomorphic; these frames therefore define a [holomorphic vector bundle](#holomorphic-vector-bundle).

###### Holomorphic tangent connection and mixed torsion criterion

↑ **Parent:** [Holomorphic tangent bundle](#holomorphic-tangent-bundle)

A real [connection on a vector bundle](fiber-bundle.md#connection-vector-bundle) on $TM$ with $\nabla J=0$ restricts after complexification to a connection $D$ on the [holomorphic tangent bundle](#holomorphic-tangent-bundle). Conversely $D$ and its conjugate determine a unique such real connection. In holomorphic coordinates, compatibility with the holomorphic structure means $D_{\partial_{\bar z^i}}\partial_{z^j}=0$. Zero mixed [torsion tensor](fiber-bundle.md#torsion-tensor) says that this derivative equals $\nabla_{\partial_{z^j}}\partial_{\bar z^i}$; the two belong to opposite eigentypes, so both vanish. Reality proves the reverse implication. Preserving $J$ alone does not imply this condition.

###### Holomorphic cotangent bundle

↑ **Parent:** [Holomorphic tangent bundle](#holomorphic-tangent-bundle)

The dual of the [holomorphic tangent bundle](#holomorphic-tangent-bundle) is a [holomorphic vector bundle](#holomorphic-vector-bundle) with local frames $dz^1,\ldots,dz^n$. Coordinate changes have holomorphic invertible Jacobian matrices, so these frames have holomorphic transition functions. Its [holomorphic sections](#holomorphic-section) are exactly the [holomorphic one-forms](#holomorphic-one-form).

###### Almost complex structure induced by a complex atlas

↑ **Parent:** [Complex manifold](#complex-manifold)

In a holomorphic chart $z^j=x^j+iy^j$, define

$$
J\frac{\partial}{\partial x^j}=\frac{\partial}{\partial y^j},
\qquad
J\frac{\partial}{\partial y^j}=-\frac{\partial}{\partial x^j}.
$$

The derivative of every holomorphic transition map is complex linear and therefore commutes with this $J$, so the chartwise definitions glue to the intrinsic [almost complex structure](#almost-complex-manifold) of the [complex manifold](#complex-manifold).

###### Differential form of type (p, q)

↑ **Parent:** [Complex manifold](#complex-manifold)

The complexified cotangent bundle of a [complex manifold](#complex-manifold) splits as

$$
T^*X\otimes\mathbb C=(T^{1,0}X)^*\oplus(T^{0,1}X)^*.
$$

A differential form has type $(p,q)$ when it is locally a sum of terms containing $p$ factors $dz^j$ and $q$ factors $d\bar z^k$.

###### Real (p, p)-form

↑ **Parent:** [Differential form of type (p, q)](#differential-form-of-type-p-q)

A [differential form of type (p, q)](#differential-form-of-type-p-q) with equal holomorphic and antiholomorphic degrees is real when it is fixed by [complex conjugation](complex-analysis.md#complex-conjugation). For such a form, $\overline{\bar\partial\eta}=\partial\eta$, so $\bar\partial\eta=0$ implies $d\eta=0$. The converse follows from the distinct types of $\partial\eta$ and $\bar\partial\eta$.

###### Complex conjugation of differential-form type

↑ **Parent:** [Differential form of type (p, q)](#differential-form-of-type-p-q)

[Complex conjugation](complex-analysis.md#complex-conjugate) interchanges the bidegrees of complex differential forms:

$$
\overline{\Omega^{p,q}(X)}=\Omega^{q,p}(X).
$$

It also interchanges the two type components of the [exterior derivative](differential-form.md#exterior-derivative), so $\bar\partial\bar\alpha=\overline{\partial\alpha}$ and $\partial\bar\alpha=\overline{\bar\partial\alpha}$.

###### d c operator

↑ **Parent:** [Complex manifold](#complex-manifold)

With the convention $d^c=i(\bar\partial-\partial)$ and with $J$ acting on forms by applying the [complex structure](#complex-structure) to every argument,

$$
d^c=J^{-1}dJ.
$$

Indeed, $J$ acts on a $(p,q)$-form by $i^{p-q}$; conjugating $d=\partial+\bar\partial$ therefore multiplies its two type components by $-i$ and $i$, respectively.

###### Holomorphic vector field

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holomorphic_vector_field)

A holomorphic vector field is a holomorphic section of $T^{1,0}X$. In holomorphic coordinates it has the form $\sum_jf^j(z)\partial/\partial z^j$ with holomorphic coefficient functions $f^j$.

###### Euler vector field

↑ **Parent:** [Holomorphic vector field](#holomorphic-vector-field)

On a complex vector space with linear coordinates, the Euler vector field is $E=\sum_jz_j\partial_{z_j}$. It generates scalar dilations, and the [Euler homogeneous function theorem](real-analysis.md#euler-theorem-for-homogeneous-functions) says $E(f)=kf$ for a homogeneous function of degree $k$. Contracting a top form with $E$ gives a horizontal form for the quotient by nonzero scalings; descent also requires the appropriate scaling invariance.

###### Projectivization of a linear vector field

↑ **Parent:** [Holomorphic vector field](#holomorphic-vector-field)

A complex-linear endomorphism $A$ of $\mathbb C^{n+1}$ induces a [holomorphic vector field](#holomorphic-vector-field) on [Complex projective space](algebraic-topology.md#complex-projective-space) by differentiating the projective transformations $[z]\mapsto[e^{tA}z]$. Its zeroes are precisely the projective eigenlines of $A$; a diagonalizable $A$ with distinct eigenvalues therefore gives exactly $n+1$ zeroes.

###### Complex submanifold

↑ **Parent:** [Complex manifold](#complex-manifold)

A complex submanifold is locally the common zero set of holomorphic coordinates, equivalently a smooth submanifold whose tangent spaces are complex linear.

###### Nonsingular analytic subvariety

↑ **Parent:** [Complex submanifold](#complex-submanifold)

A closed analytic subset of a [complex manifold](#complex-manifold) is nonsingular when every point has a neighbourhood on which the subset is the zero set of a [holomorphic map](complex-analysis.md#holomorphic-map) of full rank along that zero set. The [holomorphic implicit function theorem](calculus.md#holomorphic-implicit-function-theorem) then makes it a local coordinate subspace. This includes a closed complex submanifold, whereas an arbitrary open piece of a complex submanifold need not be globally closed in its ambient manifold.

###### Smooth submanifolds with invariant complex tangent spaces are complex

↑ **Parent:** [Complex submanifold](#complex-submanifold)

Let $Y$ be a [embedded submanifold](differential-geometry.md#embedded-submanifold) of a [complex manifold](#complex-manifold). If its [tangent spaces](differential-geometry.md#tangent-space) are invariant under the [almost complex structure induced by a complex atlas](#almost-complex-structure-induced-by-a-complex-atlas), choose ambient [holomorphic coordinates](#holomorphic-coordinate) making its [tangent space](differential-geometry.md#tangent-space) at one point $\mathbb C^k\times0$. The first $k$ coordinates restrict to a local real [diffeomorphism](geometry-and-topology.md#diffeomorphism) by the [inverse function theorem](calculus.md#inverse-function-theorem), so $Y$ is locally the graph of a smooth function $F$. Invariance of the tangent graph gives $dF(iv)=i\,dF(v)$, the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations). Thus $F$ is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) and these graph coordinates give the induced [complex submanifold](#complex-submanifold) structure. This proves the result directly, without needing the general integrability theorem as an unproved step.

###### Holomorphic normal bundle

↑ **Parent:** [Complex submanifold](#complex-submanifold)

For a [complex submanifold](#complex-submanifold) $Y\subseteq X$, the holomorphic normal bundle is the quotient [holomorphic vector bundle](#holomorphic-vector-bundle)

$$
N_{Y/X}=TX|_Y/TY.
$$

###### Normal bundle of a regular zero locus

↑ **Parent:** [Holomorphic normal bundle](#holomorphic-normal-bundle)

The derivative of a section defining a [regular zero locus](fiber-bundle.md#regular-zero-locus) patches intrinsically along that locus because changes of trivialization introduce derivative terms multiplied by the vanishing section. Its tangent kernel and surjectivity give $N_V\cong E|_V$. Combining this with [adjunction for a smooth submanifold](#adjunction-for-a-smooth-submanifold) gives $K_V=(K_M\otimes\det E)|_V$.

###### Normal bundle of a smooth analytic hypersurface

↑ **Parent:** [Holomorphic normal bundle](#holomorphic-normal-bundle)

For a smooth [complex analytic hypersurface](#complex-analytic-hypersurface) $Y\subset X$, its [holomorphic normal bundle](#holomorphic-normal-bundle) is naturally the restriction of its [holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor):

$$
N_{Y/X}\cong\mathcal O(Y)|_Y.
$$

If reduced local defining functions satisfy $f_i=g_{ij}f_j$, then $df_i|_Y=g_{ij}df_j|_Y$. Pairing a normal vector with $df_i$ and using the reciprocal transition functions of $\mathcal O(Y)$ gives the isomorphism.

###### Holomorphic conormal sequence

↑ **Parent:** [Holomorphic normal bundle](#holomorphic-normal-bundle)

The dual of the tangent-normal sequence is the short exact sequence of [holomorphic vector bundles](#holomorphic-vector-bundle)

$$
0\longrightarrow N_{Y/X}^*\longrightarrow\Omega_X^1|_Y\longrightarrow\Omega_Y^1\longrightarrow0.
$$

###### Holomorphic conormal bundle

↑ **Parent:** [Holomorphic conormal sequence](#holomorphic-conormal-sequence)

For a [complex submanifold](#complex-submanifold) $Y\subset X$, the holomorphic conormal bundle is the annihilator of $T^{1,0}Y$ inside $\Omega_X^1|_Y$, or equivalently the dual of the [holomorphic normal bundle](#holomorphic-normal-bundle). For a smooth analytic hypersurface with local equation $f$, it is generated by $df|_Y$. It is also the locally free analytic sheaf $\mathcal I_Y/\mathcal I_Y^2$.

###### Conormal line of a smooth analytic hypersurface

↑ **Parent:** [Holomorphic conormal bundle](#holomorphic-conormal-bundle)

For reduced local equations $f_j=u_{ji}f_i$ with $u_{ji}$ a holomorphic unit, the [holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor) $[-Y]$ has local generators $f_i$ and transition $u_{ji}$. Differentiation along $Y$ gives $df_j|_Y=u_{ji}|_Y\,df_i|_Y$. Sending the restricted local generator to $df_i|_Y$ gives the conormal isomorphism. The term $f_i\,du_{ji}$ disappears only after restricting to $Y$.

###### Complex analytic hypersurface

↑ **Parent:** [Complex submanifold](#complex-submanifold)

A complex analytic hypersurface in an $n$-dimensional [complex manifold](#complex-manifold) is a closed analytic subset of pure complex codimension one. It is irreducible when it is not the union of two proper closed analytic subsets.

###### Local defining function of a complex analytic hypersurface

↑ **Parent:** [Complex analytic hypersurface](#complex-analytic-hypersurface)

A local defining function for a complex analytic hypersurface $Y$ near $x$ is a holomorphic function $f$ on a neighbourhood $U$ such that $Y\cap U=\{f=0\}$. It may be chosen reduced, with each local irreducible factor occurring once. The [local ring](commutative-algebra.md#local-ring) $\mathcal O_{X,x}$ of a complex manifold is a [regular local ring](commutative-algebra.md#regular-local-ring) and hence a [unique factorization domain](algebra.md#unique-factorization-domain); each height-one prime of the hypersurface germ is principal, and the product of generators for its finitely many local branches gives $f$.

###### Reduced local defining functions differ by a holomorphic unit

↑ **Parent:** [Local defining function of a complex analytic hypersurface](#local-defining-function-of-a-complex-analytic-hypersurface)

The [local ring](commutative-algebra.md#local-ring) of a [complex manifold](#complex-manifold) is the [unique factorization domain](algebra.md#unique-factorization-domain) of convergent power series in local coordinates. A reduced [local defining function of a complex analytic hypersurface](#local-defining-function-of-a-complex-analytic-hypersurface) has each local irreducible factor once. The analytic zero-set ideal is the radical of its [principal ideal](commutative-algebra.md#principal-ideal), and reducedness makes that [principal ideal](commutative-algebra.md#principal-ideal) radical. Thus two reduced equations for the same germ generate the same ideal and differ by a unit. A globally irreducible hypersurface may have several local branches; reducedness includes each once. Without reducedness, $f$ and $f^2$ have the same zero set and need not differ by a unit.

###### Divisor on a complex manifold

↑ **Parent:** [Complex analytic hypersurface](#complex-analytic-hypersurface)

A divisor on a [complex manifold](#complex-manifold) is a locally finite formal sum

$$
D=\sum_Yn_YY,
$$

where the $Y$ are irreducible complex analytic hypersurfaces and $n_Y\in\mathbb Z$. Products of powers of [local defining functions](#local-defining-function-of-a-complex-analytic-hypersurface) give local meromorphic equations $f_\alpha$ for $D$ whose ratios $f_\alpha/f_\beta$ are nowhere-vanishing holomorphic functions.

###### Order of a meromorphic function along a hypersurface

↑ **Parent:** [Divisor on a complex manifold](#divisor-on-a-complex-manifold)

At a generic smooth point of an irreducible [complex analytic hypersurface](#complex-analytic-hypersurface) $Y$, a nonzero [meromorphic function](isolated-singularity.md#meromorphic-function) has the form $f=t^m u$, where $t$ is a reduced transverse local equation and $u$ is a holomorphic unit. The integer $m$ is its order along $Y$: positive for a zero and negative for a pole. The [unique factorization domain](algebra.md#unique-factorization-domain) property of the [local ring](commutative-algebra.md#local-ring) of a [complex manifold](#complex-manifold) makes this independent of the equation and propagates it along $Y$. These orders are the coefficients of the [principal divisor on a complex manifold](#principal-divisor-on-a-complex-manifold) of $f$.

###### Principal divisor on a complex manifold

↑ **Parent:** [Divisor on a complex manifold](#divisor-on-a-complex-manifold)

The [divisor on a complex manifold](#divisor-on-a-complex-manifold) of a nonzero global [meromorphic function](isolated-singularity.md#meromorphic-function) records its zero and pole orders along irreducible analytic hypersurfaces. It is called principal. Its [holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor) is trivial: choosing the same global [meromorphic function](isolated-singularity.md#meromorphic-function) as the local equation on every open set gives identity transition functions. In particular, two hyperplanes in [Complex projective space](algebraic-topology.md#complex-projective-space) have isomorphic associated bundles, since the quotient of their homogeneous linear equations is a global [meromorphic function](isolated-singularity.md#meromorphic-function) with their difference as divisor.

###### Holomorphic line bundle associated to a divisor

↑ **Parent:** [Divisor on a complex manifold](#divisor-on-a-complex-manifold)

If $f_\alpha$ are local meromorphic equations for a [divisor on a complex manifold](#divisor-on-a-complex-manifold) $D$, glue holomorphic frames $e_\alpha$ by

$$
e_\alpha=(f_\beta/f_\alpha)e_\beta.
$$

The resulting holomorphic line bundle is denoted $[D]$. The expressions $f_\alpha e_\alpha$ glue to its canonical meromorphic section, whose divisor is $D$.

###### Additivity of analytic divisor line bundles

↑ **Parent:** [Holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor)

If $f_i$ and $g_i$ are local meromorphic equations for two [divisors on a complex manifold](#divisor-on-a-complex-manifold), then $f_ig_i$ defines their sum. With local frames satisfying $e_j=(f_i/f_j)e_i$, the [transition functions of a vector bundle](fiber-bundle.md#transition-function-of-a-vector-bundle) for the tensor product are the products of the two ratios, exactly those for $f_ig_i$. Multiplication of local frames therefore gives the displayed [holomorphic line bundle](#holomorphic-line-bundle) isomorphism.

###### Sheaf of meromorphic functions on a complex manifold

↑ **Parent:** [Divisor on a complex manifold](#divisor-on-a-complex-manifold)

The sheaf $\mathcal K_X$ assigns to an open subset of a [complex manifold](#complex-manifold) its [meromorphic functions](isolated-singularity.md#meromorphic-function). Its subsheaf $\mathcal K_X^*$ consists of the nonzero meromorphic functions, while $\mathcal O_X^*$ consists of the nowhere-zero [holomorphic functions](complex-analysis.md#holomorphic-function).

###### Divisor sheaf on a complex manifold

↑ **Parent:** [Sheaf of meromorphic functions on a complex manifold](#sheaf-of-meromorphic-functions-on-a-complex-manifold)

The quotient sheaf $\mathcal K_X^*/\mathcal O_X^*$ records the zero and pole orders of local nonzero [meromorphic functions](isolated-singularity.md#meromorphic-function). Each of its [global sections](ringed-space.md#global-section) is naturally a [divisor on a complex manifold](#divisor-on-a-complex-manifold) on $X$.

###### Divisor-to-Picard map

↑ **Parent:** [Divisor sheaf on a complex manifold](#divisor-sheaf-on-a-complex-manifold)

The [connecting homomorphism](homology.md#connecting-homomorphism) of

$$
0\longrightarrow\mathcal O_X^*\longrightarrow\mathcal K_X^*\longrightarrow\mathcal K_X^*/\mathcal O_X^*\longrightarrow0
$$

sends a [divisor on a complex manifold](#divisor-on-a-complex-manifold) $D$ to its [holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor) $\mathcal O(D)$ in the [Picard group](ringed-space.md#picard-group). Its kernel consists exactly of the [principal divisors](algebraic-geometry.md#principal-divisor-on-an-algebraic-curve) of global nonzero [meromorphic functions](isolated-singularity.md#meromorphic-function).

###### Principal part of a meromorphic function

↑ **Parent:** [Sheaf of meromorphic functions on a complex manifold](#sheaf-of-meromorphic-functions-on-a-complex-manifold)

At a point $x$ of a [Riemann surface](complex-analysis.md#riemann-surfaces), the principal part of a [meromorphic function](isolated-singularity.md#meromorphic-function) is the negative-degree part of its [Laurent series](analysis.md#laurent-series) in a local coordinate. It is equivalently a germ in the quotient $\mathcal K_x/\mathcal O_x$.

The principal part at a pole is the finite sum of negative-degree terms of its [Laurent series](analysis.md#laurent-series). Prescribing such parts is the problem solved by the [Mittag-Leffler theorem](isolated-singularity.md#mittag-leffler-s-theorem).

###### Sheaf of meromorphic principal parts

↑ **Parent:** [Principal part of a meromorphic function](#principal-part-of-a-meromorphic-function)

On a [Riemann surface](complex-analysis.md#riemann-surfaces), the quotient sheaf $\mathcal P=\mathcal M_X/\mathcal O_X$ records the finite negative [Laurent series](analysis.md#laurent-series) tails of meromorphic germs. At $x$, a local coordinate $t$ identifies its stalk with $\bigoplus_{m\geq1}\mathbb C t^{-m}$. As a sheaf it is the [direct sum of sheaves](algebraic-geometry.md#direct-sum-of-sheaves) $\bigoplus_x(i_x)_*\mathcal P_x$. Global sections prescribe locally finite families of principal parts, possibly infinite on a noncompact surface. The [connecting homomorphism](homology.md#connecting-homomorphism) to $H^1(X,\mathcal O_X)$ is exactly the obstruction to a global meromorphic function with those parts and no extra poles.

###### Mittag-Leffler problem on a Riemann surface

↑ **Parent:** [Principal part of a meromorphic function](#principal-part-of-a-meromorphic-function)

The Mittag-Leffler problem asks for a global [meromorphic function](isolated-singularity.md#meromorphic-function) with prescribed [principal parts](#principal-part-of-a-meromorphic-function) at a discrete collection of points. For a finite collection, those principal parts define a [Čech cocycle](ringed-space.md#cech-cocycle-condition) for the sheaf $\mathcal O$; vanishing of its class in $\check H^1(X,\mathcal O)$ is exactly the condition that the problem has a solution.

###### Dolbeault operator

↑ **Parent:** [Complex manifold](#complex-manifold)

The complexified cotangent bundle decomposes into $(1,0)$ and $(0,1)$ parts. The Dolbeault operator is the type-$(0,1)$ component of the exterior derivative, $\bar\partial:\Omega^{p,q}\to\Omega^{p,q+1}$, and integrability gives $\bar\partial^2=0$.

Together with its $(1,0)$ counterpart, the [Dolbeault operator](#dolbeault-operator) decomposes the [exterior derivative](differential-form.md#exterior-derivative) on complex differential forms.

###### Bundle-valued Dolbeault adjoint

↑ **Parent:** [Dolbeault operator](#dolbeault-operator)

Using the [bundle-valued conjugate-linear Hodge star](differential-form.md#bundle-valued-conjugate-linear-hodge-star), the [formal adjoint](hilbert-space.md#formal-adjoint) of the holomorphic bundle's [Dolbeault operator](#dolbeault-operator) is $\bar\partial_E^*=-*_{E^*}\bar\partial_{E^*}*_E$. It lowers antiholomorphic degree. Stokes applied to the coefficient-contracted form $\psi\wedge *_E\eta$ proves the integrated adjoint identity on a compact [complex manifold](#complex-manifold).

###### Conjugate Dolbeault operator

↑ **Parent:** [Dolbeault operator](#dolbeault-operator)

The conjugate [Dolbeault operator](#dolbeault-operator) is the type-$(1,0)$ component of the [exterior derivative](differential-form.md#exterior-derivative): $\partial:\mathcal A^{p,q}\to\mathcal A^{p+1,q}$. [Complex conjugation](complex-analysis.md#complex-conjugation) interchanges $\partial$ and $\bar\partial$. On a [complex manifold](#complex-manifold), $d=\partial+\bar\partial$, $\partial^2=\bar\partial^2=0$, and $\partial\bar\partial+\bar\partial\partial=0$.

<h6 id="dolbeault-poincare-lemma">Dolbeault-Poincaré lemma</h6>

↑ **Parent:** [Dolbeault operator](#dolbeault-operator)

On a sufficiently small polydisc in a [complex manifold](#complex-manifold), every $\bar\partial$-closed $(p,q)$-form with $q>0$ is locally $\bar\partial$-exact. A coefficientwise one-variable integral operator and induction over the coordinates prove the result.

###### Coordinate elimination for local Dolbeault primitives

↑ **Parent:** [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma)

For a $\bar\partial$-closed positive-antiholomorphic-degree [differential form of type (p, q)](#differential-form-of-type-p-q) on a [polydisc](#polydisc), write $\varphi=d\bar z_j\wedge\alpha+\beta$ with no $d\bar z_j$ in $\alpha,\beta$. Apply the [Cauchy-Green operator](#cauchy-green-operator) in coordinate $j$ to the coefficients of $\alpha$. Subtracting its [Dolbeault operator](#dolbeault-operator) derivative removes every $d\bar z_j$ term. Closedness then makes the remaining coefficients holomorphic in $z_j$. Eliminating successive coordinates preserves holomorphicity in earlier coordinates and produces a local primitive after finitely many steps.

<h6 id="conjugate-dolbeault-poincare-lemma">Conjugate Dolbeault-Poincaré lemma</h6>

↑ **Parent:** [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma)

On a [polydisc](#polydisc), a $\partial$-closed [differential form of type (p, q)](#differential-form-of-type-p-q) with $p>0$ is $\partial$-exact. Apply the [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma) to its complex conjugate, whose antiholomorphic degree is $p$.

###### Cauchy-Green operator

↑ **Parent:** [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma)

On a disc $D\subset\mathbb C$, the Cauchy-Green operator

$$
Tg(z)=\frac1{2\pi i}\int_D\frac{g(w)}{w-z}\,dw\wedge d\bar w
$$

is a right inverse to $\partial/\partial\bar z$ in the interior: $\partial_{\bar z}Tg=g$. Applying it to coefficients gives the local homotopy operator used in the [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma).

###### Dolbeault cohomology

↑ **Parent:** [Dolbeault operator](#dolbeault-operator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dolbeault_cohomology)

Dolbeault cohomology is

$$
H^{p,q}_{\bar\partial}(X)=\ker(\bar\partial:\Omega^{p,q}\to\Omega^{p,q+1})/\operatorname{im}(\bar\partial:\Omega^{p,q-1}\to\Omega^{p,q}).
$$

###### Dolbeault cohomology of the projective line

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

The [Dolbeault theorem](#dolbeault-theorem) identifies this group with first [Čech cohomology](ringed-space.md#cech-cohomology) of the trivial holomorphic line bundle. On the two standard affine charts, a holomorphic overlap function has a [Laurent series](analysis.md#laurent-series). Its nonnegative powers extend to the chart at zero, and its negative powers extend to the chart at infinity. Every overlap cocycle is therefore a coboundary. Consequently the [Dolbeault operator](#dolbeault-operator) from functions to $(0,1)$-forms is [surjective](algebra.md#surjective-function).

###### Laurent gluing of Dolbeault primitives on the projective line

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

For a smooth $(0,1)$-form on the [complex projective line](algebraic-topology.md#complex-projective-line), solve its [Dolbeault operator](#dolbeault-operator) equation on a disc about zero and a disc about infinity. The difference of the primitives is a [holomorphic function](complex-analysis.md#holomorphic-function) on their annular overlap. Split its [Laurent series](analysis.md#laurent-series) into a nonnegative-power part extending to the finite disc and a negative-power part extending holomorphically across infinity. Subtract the first part from the finite primitive and add the second to the infinite primitive. The results agree and define a global primitive, without [Hodge theory](differential-geometry.md#hodge-theory).

###### Stein vanishing for the Dolbeault cohomology of functions

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

On a [Stein manifold](#stein-manifold), every smooth $\bar\partial$-closed $(0,q)$-form with $q>0$ is globally $\bar\partial$-exact. The same holds componentwise for forms valued in a finite-dimensional constant vector space. Complex conjugation yields the corresponding global $\partial$ primitive for a closed $(1,0)$-form, as used in the [complex potential reduction of anti-self-dual Yang-Mills](classical-field-theory-soliton.md#complex-potential-reduction-of-anti-self-dual-yang-mills).

###### Dolbeault cohomology of the projective line times the affine line

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

For $X=\mathbb P^1\times\mathbb C$, the two standard affine charts and their intersection form an [acyclic cover](topology.md#acyclic-cover) for the [sheaves](algebraic-geometry.md#sheaf-mathematics) of holomorphic forms. Their [Čech cohomology](ringed-space.md#cech-cohomology) gives $H^{0,0}_{\bar\partial}=\mathcal O(\mathbb C)$ and $H^{2,1}_{\bar\partial}=\mathcal O(\mathbb C)$, with all other groups for $p\in\{0,2\}$ zero. For the top-form [sheaf](algebraic-geometry.md#sheaf-mathematics), the transition $d(1/z)=-z^{-2}dz$ removes every [Laurent series](analysis.md#laurent-series) power except $z^{-1}$ from the first cohomology quotient; its coefficient may be an arbitrary [entire function](complex-analysis.md#entire-function) on the affine factor.

###### Dolbeault cohomology with values in a holomorphic vector bundle

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

This is the cohomology of $\mathcal A^{p,\bullet}(X,E)$ with the bundle [Dolbeault operator](#dolbeault-operator). The [Dolbeault theorem](#dolbeault-theorem) identifies it with $H^q(X,\Omega_X^p\otimes\mathcal O(E))$. For compact Hermitian $X$, [Dolbeault Hodge decomposition](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) gives unique harmonic representatives.

###### Curvature Dolbeault class

↑ **Parent:** [Dolbeault cohomology with values in a holomorphic vector bundle](#dolbeault-cohomology-with-values-in-a-holomorphic-vector-bundle)

[Chern curvature](#chern-curvature) defines $\alpha(E)=[\Theta]\in H^1(M,\Omega_M^1\otimes\operatorname{End}E)$. If two metrics give connections differing by $a$, then $\Theta_1-\Theta_0=\bar\partial_{\operatorname{End}E}a$. Thus this [vector-bundle curvature](fiber-bundle.md#curvature-form) class depends on the holomorphic bundle rather than the chosen metric.

<h6 id="cech-cocycle-for-the-curvature-dolbeault-class">Čech cocycle for the curvature Dolbeault class</h6>

↑ **Parent:** [Curvature Dolbeault class](#curvature-dolbeault-class)

In frames with $e^{(\beta)}=g_{\alpha\beta}e^{(\alpha)}$ and input-index connection matrices, the [Chern connection](#chern-connection) has $\theta_\beta-g_{\alpha\beta}\theta_\alpha g_{\alpha\beta}^{-1}=\sigma_{\alpha\beta}$. These holomorphic one-forms, interpreted in the beta frame, satisfy the transported [Čech cocycle condition](ringed-space.md#cech-cocycle-condition) because $g_{\alpha\gamma}=g_{\beta\gamma}g_{\alpha\beta}$. Local primitives of curvature differ by this cocycle. A holomorphic frame change $e'_\alpha=u_\alpha e_\alpha$ adds the [Čech coboundary](ringed-space.md#cech-coboundary) of $u_\alpha^{-1}\partial u_\alpha$, so the resulting [curvature Dolbeault class](#curvature-dolbeault-class) is intrinsic.

###### Metric independence of curvature Dolbeault powers

↑ **Parent:** [Curvature Dolbeault class](#curvature-dolbeault-class)

Composition of [endomorphisms](algebra.md#endomorphism) and [wedge product of differential forms](differential-form.md#wedge-product-of-differential-forms) give the class $[\Theta^k]\in H^k(M,\Omega_M^k\otimes\operatorname{End}E)$. Even total degree of [vector-bundle curvature](fiber-bundle.md#curvature-form) and the noncommutative telescoping identity give $\Theta_1^k-\Theta_0^k=\bar\partial\sum_{j=0}^{k-1}\Theta_1^j a\Theta_0^{k-1-j}$ whenever $\Theta_1-\Theta_0=\bar\partial a$. Thus all powers are metric independent; no commutativity of [endomorphisms](algebra.md#endomorphism) is assumed.

###### Dolbeault cohomology of a complex torus

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

For a [complex torus](#complex-torus) $X=V/\Lambda$ of complex dimension $g$, constant forms give a natural isomorphism $H^{p,q}_{\bar\partial}(X)\cong\bigwedge^pV^*\otimes\bigwedge^q\overline{V^*}$. A flat [Kähler metric](#kahler-metric) and the [Dolbeault Hodge decomposition](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) prove that these constant forms are precisely the harmonic representatives. Thus $h^{p,q}=\binom gp\binom gq$ for $0\leq p,q\leq g$, and zero otherwise.

###### Bott-Chern cohomology

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

For a [complex manifold](#complex-manifold), Bott-Chern cohomology is

$$
H_{BC}^{p,q}(M)=\frac{\ker\partial\cap\ker\bar\partial\subseteq\mathcal A^{p,q}(M)}{\partial\bar\partial\mathcal A^{p-1,q-1}(M)}.
$$

Its classes are represented by $d$-closed forms of pure type. A natural map sends a Bott-Chern class to its [Dolbeault cohomology](#dolbeault-cohomology) class.

<h6 id="bott-chern-cohomology-of-a-compact-kahler-manifold">Bott-Chern cohomology of a compact Kähler manifold</h6>

↑ **Parent:** [Bott-Chern cohomology](#bott-chern-cohomology)

For a compact [Kähler manifold](#kahler-manifold), the natural map $H_{BC}^{p,q}\to H_{\bar\partial}^{p,q}$ is an isomorphism. The [Kähler Laplacian identity](#kahler-laplacian-identity) makes the harmonic representative of every [Dolbeault cohomology](#dolbeault-cohomology) class $d$-closed, giving surjectivity, and the [ddbar lemma](#ddbar-lemma) gives injectivity.

<h6 id="bott-chern-poincare-lemma">Bott-Chern Poincaré lemma</h6>

↑ **Parent:** [Bott-Chern cohomology](#bott-chern-cohomology)

On a [polydisc](#polydisc), $H_{BC}^{p,q}=0$ for $p,q>0$. A [Poincaré lemma](differential-form.md#poincare-lemma) primitive for a closed pure-type form can be modified by exact terms until only bidegrees $(p-1,q)$ and $(p,q-1)$ remain. The [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma) and [conjugate Dolbeault-Poincaré lemma](#conjugate-dolbeault-poincare-lemma) then make the original form $\partial\bar\partial$-exact.

###### Dolbeault theorem

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dolbeault_theorem)

For the sheaf $\Omega^p$ of holomorphic $p$-forms on a [complex manifold](#complex-manifold), the [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma) makes

$$
0\longrightarrow\Omega^p\longrightarrow\mathcal A^{p,0}\xrightarrow{\bar\partial}\mathcal A^{p,1}\xrightarrow{\bar\partial}\cdots
$$

a resolution by [fine sheaves](ringed-space.md#fine-sheaf). Taking [global sections](ringed-space.md#global-section) therefore gives the natural isomorphism

$$
H^q(X,\Omega^p)\cong H_{\bar\partial}^{p,q}(X).
$$

###### Dolbeault resolution of holomorphic differential forms

↑ **Parent:** [Dolbeault theorem](#dolbeault-theorem)

The [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma) makes this a locally exact complex of [sheaves](algebraic-geometry.md#sheaf-mathematics), with degree-zero kernel the [holomorphic differential forms](#holomorphic-differential-form). The [sheaves](algebraic-geometry.md#sheaf-mathematics) of smooth forms are [fine sheaves](ringed-space.md#fine-sheaf) by a [partition of unity](differential-geometry.md#partition-of-unity). The [acyclic resolution theorem](ringed-space.md#acyclic-resolution-theorem) therefore computes the cohomology of $\Omega^p$ by the global [Dolbeault operator](#dolbeault-operator) complex.

###### Hodge number

↑ **Parent:** [Dolbeault cohomology](#dolbeault-cohomology)

The Hodge number of a compact complex manifold is $h^{p,q}=\dim_{\mathbb C}H^{p,q}_{\bar\partial}(X)$.

For a compact [Kähler manifold](#kahler-manifold), these dimensions are the graded dimensions in its [Hodge structure](differential-geometry.md#hodge-structure).

###### Hodge duality

↑ **Parent:** [Hodge number](#hodge-number)

On a compact [Kähler manifold](#kahler-manifold) of complex dimension $n$, the [conjugate-linear Hodge star](differential-form.md#conjugate-linear-hodge-star) gives a bijection of harmonic forms in complementary bidegrees. The [Dolbeault Hodge decomposition](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) identifies these harmonic spaces with [Dolbeault cohomology](#dolbeault-cohomology) and yields the displayed equality.

###### Hodge symmetry

↑ **Parent:** [Hodge number](#hodge-number)

On a compact [Kähler manifold](#kahler-manifold), complex conjugation commutes with the real [Hodge Laplacian](differential-form.md#hodge-laplacian) and exchanges harmonic forms of bidegrees $(p,q)$ and $(q,p)$. The identification of [Dolbeault cohomology](#dolbeault-cohomology) with harmonic forms therefore gives the symmetry of [Hodge numbers](#hodge-number).

###### Holomorphic vector bundle

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holomorphic_vector_bundle)

A holomorphic vector bundle is a complex [vector bundle](fiber-bundle.md#vector-bundle) whose local trivializations have holomorphic transition functions.

###### Unitary flat holomorphic vector bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

A [unitary representation](representation-theory.md#unitary-representation) of the [fundamental group](algebraic-topology.md#fundamental-group) of a connected [complex manifold](#complex-manifold) gives a bundle $(\widetilde X\times V)/\pi_1X$ with locally constant unitary transition matrices. Its induced flat [unitary connection](fiber-bundle.md#unitary-connection) has $(0,1)$ part equal to its [Dolbeault operator](#dolbeault-operator), so it is the [Chern connection](#chern-connection) for the induced Hermitian metric. On a [compact Riemann surface](complex-analysis.md#compact-riemann-surface), zero curvature gives degree zero; the subbundle curvature inequality makes the bundle semistable.

###### Holomorphic sections of a unitary flat bundle are parallel

↑ **Parent:** [Unitary flat holomorphic vector bundle](#unitary-flat-holomorphic-vector-bundle)

In a local parallel orthonormal frame a [holomorphic section](#holomorphic-section) has holomorphic coefficients $f_j$. Its squared norm satisfies $\partial_z\partial_{\bar z}\sum_j|f_j|^2=\sum_j|f'_j|^2\ge0$. On a compact connected complex curve, integration of the Laplacian makes the right side zero. Thus every coefficient is locally constant and the section is parallel. A global parallel section is determined by a vector fixed by all monodromy operators, and every such vector gives a global section.

###### Degree of a holomorphic vector bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

On a [compact Riemann surface](complex-analysis.md#compact-riemann-surface), the degree of a [holomorphic vector bundle](#holomorphic-vector-bundle) is the [degree of a line bundle](ringed-space.md#degree-of-a-line-bundle) of its [determinant line bundle](fiber-bundle.md#determinant-line-bundle). A [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle) and its [Chern connection](#chern-connection) express this degree by the trace-curvature integral. The value is independent of the metric because the normalized trace curvature represents the [First Chern class](#first-chern-class).

###### Slope of a holomorphic vector bundle

↑ **Parent:** [Degree of a holomorphic vector bundle](#degree-of-a-holomorphic-vector-bundle)

The slope of a nonzero [holomorphic vector bundle](#holomorphic-vector-bundle) on a [compact Riemann surface](complex-analysis.md#compact-riemann-surface) is its [degree of a holomorphic vector bundle](#degree-of-a-holomorphic-vector-bundle) divided by its [rank of a vector bundle](fiber-bundle.md#rank-of-a-vector-bundle). It measures degree per fibre dimension. Comparing subbundle slopes defines [semistable holomorphic vector bundles](#semistable-holomorphic-vector-bundle).

###### Subbundle slope bound from ambient Chern curvature

↑ **Parent:** [Slope of a holomorphic vector bundle](#slope-of-a-holomorphic-vector-bundle)

Fix a [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle) $E$ over a [compact Riemann surface](complex-analysis.md#compact-riemann-surface) and a positive area form $\omega$. Write $iF_E=K\omega$ for its [Chern curvature](#chern-curvature). If every eigenvalue of the Hermitian endomorphism $K$ is at most $C$, the [curvature formula for a holomorphic subbundle](#curvature-formula-for-a-holomorphic-subbundle) gives $\deg F\le\operatorname{rank}(F)C\int_X\omega/(2\pi)$. The second-fundamental-form term is nonpositive. Compactness supplies a finite $C$ independent of the subbundle. If $F_E=0$, every subbundle has nonpositive degree.

###### Semistable holomorphic vector bundle

↑ **Parent:** [Slope of a holomorphic vector bundle](#slope-of-a-holomorphic-vector-bundle)

A positive-rank [holomorphic vector bundle](#holomorphic-vector-bundle) on a [compact Riemann surface](complex-analysis.md#compact-riemann-surface) is semistable when every nonzero proper [holomorphic subbundle](#holomorphic-subbundle) has slope at most its own. Equivalently one tests coherent subsheaves: saturation on a smooth curve preserves rank, increases degree, and gives a subbundle with torsion-free quotient. Strict inequality defines stability, which is stronger.

###### Holomorphic splitting of transition functions on a trivial bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

For a holomorphically [trivial vector bundle](fiber-bundle.md#trivial-vector-bundle), choose a global [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) [bundle frame](fiber-bundle.md#frame-of-a-vector-bundle). Let the columns of $H_\alpha$ be the coordinates of that frame in the prescribed frame over $U_\alpha$. If fiber coordinates transform as $s_\beta=F_{\alpha\beta}s_\alpha$, then $H_\beta=F_{\alpha\beta}H_\alpha$. Each [matrix](vector-space.md#matrix) is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) and invertible, giving the displayed splitting. Conversely such [matrices](vector-space.md#matrix) give agreeing global [holomorphic sections](#holomorphic-section) forming a frame. Topological triviality alone does not supply this conclusion.

// Destination: electromagnetism.bigb

###### Holomorphic subbundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

A holomorphic subbundle of a [holomorphic vector bundle](#holomorphic-vector-bundle) is a constant-rank [vector subbundle](fiber-bundle.md#vector-subbundle) which is locally spanned by a holomorphic linearly independent family of sections and whose inclusion is a [holomorphic bundle map](fiber-bundle.md#holomorphic-bundle-map). It has an induced [holomorphic vector bundle](#holomorphic-vector-bundle) structure. A varying-rank coherent subsheaf is not generally a subbundle.

###### Holomorphic dual vector bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

Dualize the fibres of a [holomorphic vector bundle](#holomorphic-vector-bundle). If its transitions are $g_{ij}$, the dual transitions are $g_{ij}^{-T}$, which are holomorphic and preserve the evaluation pairing. These define the natural holomorphic structure on the smooth [dual bundle](fiber-bundle.md#dual-bundle).

###### Sheaf of holomorphic sections of a vector bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

For a [holomorphic vector bundle](#holomorphic-vector-bundle) $E$, $\mathcal O(E)(U)$ is its space of [holomorphic sections](#holomorphic-section) on $U$, with their restrictions. It is the kernel of the bundle [Dolbeault operator](#dolbeault-operator) on smooth sections.

###### Holomorphic line bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holomorphic_line_bundle)

A holomorphic line bundle is a complex line bundle with holomorphic local trivializations and holomorphic nonvanishing transition functions.

###### Sections of the degree-one line bundle on the projective line

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

A global [holomorphic section](#holomorphic-section) of $\mathcal O(1)$ on $\mathbb{CP}^1$ is a linear homogeneous polynomial in the two projective coordinates. On one patch its coefficient is an entire [function](function.md) $p(\lambda)$; regularity on the other patch says $p(\lambda)/\lambda$ is regular at infinity. Hence $p$ has at most linear growth. [Cauchy estimates](analysis.md#cauchy-estimate) make its second and higher [derivatives](calculus.md#derivative) zero, so $p=a+b\lambda$. The same argument entrywise applies to matrix-valued sections and makes the logarithmic [derivative](calculus.md#derivative) in the [Penrose-Ward correspondence](general-relativity.md#penrose-ward-correspondence) linear in the primed [two-component spinor](connection-1-form.md#two-component-spinor).

###### Two-section criterion for holomorphic triviality

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

On a compact connected [complex manifold](#complex-manifold), pair nonzero [holomorphic sections](#holomorphic-section) of a [holomorphic line bundle](#holomorphic-line-bundle) and its [holomorphic dual vector bundle](#holomorphic-dual-vector-bundle). Their product is a global [holomorphic function](complex-analysis.md#holomorphic-function), hence constant by the [maximum modulus principle](complex-analysis.md#maximum-modulus-principle). The [identity theorem](complex-analysis.md#identity-theorem) makes their nonvanishing loci dense, so this constant is nonzero. Both sections are consequently nowhere zero and trivialize their bundles. Conversely, the constant section of a trivial bundle and its dual provide the two sections.

###### Smoothly trivial holomorphic line bundles when H01 vanishes

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

A nowhere-zero smooth section $s$ of a [holomorphic line bundle](#holomorphic-line-bundle) writes its [Dolbeault operator](#dolbeault-operator) as $\bar\partial_Ls=a\otimes s$. Its integrability gives $\bar\partial a=0$. If $H^{0,1}(X)=0$, then $a=\bar\partial f$ globally. The section $e^{-f}s$ is nowhere zero and [holomorphic](complex-analysis.md#complex-differentiability-at-a-point). This argument requires no [compactness](topology.md#compact-space) and explicitly constructs the [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) trivialization.

###### Meromorphic section of a holomorphic line bundle

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

In a [holomorphic local frame](#holomorphic-local-trivialization), a meromorphic section has a meromorphic scalar coefficient; the coefficients transform by the bundle's [transition functions of a vector bundle](fiber-bundle.md#transition-function-of-a-vector-bundle). A nonzero meromorphic section has a [divisor on a complex manifold](#divisor-on-a-complex-manifold) recording its zero and pole orders.

###### Principal part of a meromorphic section

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

For a [holomorphic line bundle](#holomorphic-line-bundle) on a complex curve, a meromorphic section modulo sections holomorphic through a point is its principal part. In a local coordinate and [holomorphic local frame](#holomorphic-local-trivialization) it is represented by finitely many negative powers. A vanishing $H^1(X,\mathcal O(E))$ permits prescribed principal parts, by a cutoff followed by solving a global [Dolbeault operator](#dolbeault-operator) equation.

###### Holomorphic exponential sequence

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

For the [structure sheaf of a complex manifold](#structure-sheaf-of-a-complex-manifold), local holomorphic logarithms give the [short exact sequence of sheaves](algebraic-geometry.md#short-exact-sequence-of-sheaves)

$$
0\to\underline{\mathbb Z}\to\mathcal O_M\xrightarrow{\exp(2\pi i\,\cdot)}\mathcal O_M^*\to1.
$$

The connecting map $H^1(M,\mathcal O_M^*)\to H^2(M,\mathbb Z)$ sends a [holomorphic line bundle](#holomorphic-line-bundle) to its [First Chern class](#first-chern-class). In particular, it is onto when $H^2(M,\mathcal O_M)=0$.

###### Dolbeault partial connection

↑ **Parent:** [Holomorphic line bundle](#holomorphic-line-bundle)

A Dolbeault partial connection obeys $\bar\partial_E(fs)=\bar\partial f\otimes s+f\bar\partial_Es$. Its square is a tensorial $(0,2)$-form with values in $\operatorname{End}E$; it vanishes for the canonical partial connection of a holomorphic bundle.

###### Hermitian metric on a holomorphic vector bundle

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

A Hermitian metric on a [holomorphic vector bundle](#holomorphic-vector-bundle) $E\to X$ is a smoothly varying positive-definite [Hermitian form](linear-algebra.md#hermitian-form) $h_x$ on every complex fiber $E_x$.

Such a metric makes the underlying smooth bundle a [Hermitian vector bundle](fiber-bundle.md#hermitian-vector-bundle).

###### Semipositive holomorphic line bundle

↑ **Parent:** [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle)

A [holomorphic line bundle](#holomorphic-line-bundle) is semipositive if it admits a smooth [Hermitian metric](#hermitian-metric-on-a-holomorphic-vector-bundle) whose normalized [Chern curvature](#chern-curvature) form is semipositive. Tensoring a [positive holomorphic line bundle](#positive-holomorphic-line-bundle) with a nonnegative integer power of a semipositive one remains positive, because their curvature forms add. This smooth-metric property is stronger than simply having a nef numerical class.

###### Metric compatibility as parallelism of a Hermitian tensor

↑ **Parent:** [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle)

With a [Hermitian form](linear-algebra.md#hermitian-form) linear in its first slot, $H(s\otimes\bar t)=h(s,t)$ is a complex-linear dual tensor. The original connection, its [conjugate connection](fiber-bundle.md#conjugate-connection), the [tensor product connection](fiber-bundle.md#tensor-product-connection) and the [dual connection](fiber-bundle.md#dual-connection) induce $D_0$. Its derivative is $(D_{0,V}H)(s\otimes\bar t)=Vh(s,t)-h(D_Vs,t)-h(s,D_Vt)$. Consequently $D_0H=0$ is exactly metric compatibility.

###### Quotient Hermitian metric

↑ **Parent:** [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle)

For a smooth subbundle $S$ of a [Hermitian vector bundle](fiber-bundle.md#hermitian-vector-bundle) $E$, [orthogonal projection](hilbert-space.md#orthogonal-projection) identifies $E/S$ smoothly with $S^\perp$. The quotient metric is $h_Q([v],[w])=h_E((I-\pi_S)v,(I-\pi_S)w)$. It is independent of representatives and positive definite. For a holomorphic subbundle the resulting smooth quotient metric is defined on the holomorphic quotient, but the orthogonal identification itself need not be holomorphic.

###### Positive holomorphic line bundle

↑ **Parent:** [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle)

A [holomorphic line bundle](#holomorphic-line-bundle) is positive when it admits a [Hermitian metric](#hermitian-metric-on-a-holomorphic-vector-bundle) whose [Chern connection](#chern-connection) has positive curvature form $iF_\nabla$, equivalently when $iF_\nabla$ is a [positive real (1, 1)-form](#positive-real-1-1-form).

The positive-curvature definition uses a [positive real (1, 1)-form](#positive-real-1-1-form).

###### Kodaira vanishing theorem

↑ **Parent:** [Positive holomorphic line bundle](#positive-holomorphic-line-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kodaira_vanishing_theorem)

On a compact [Kähler manifold](#kahler-manifold) $X$, if $P$ is a [positive holomorphic line bundle](#positive-holomorphic-line-bundle), then $H^i(X,K_X\otimes P)=0$ for $i>0$. The canonical-bundle twist is part of the hypothesis and conclusion; positivity alone does not remove it on a general manifold. For a [complex torus](#complex-torus), the [canonical bundle](#canonical-bundle) is trivial, so higher cohomology of a positive line bundle vanishes without an additional twist.

###### Vanishing for divisor twists on a complex torus

↑ **Parent:** [Kodaira vanishing theorem](#kodaira-vanishing-theorem)

Let $L$ be positive and $V$ a closed smooth hypersurface in a [complex torus](#complex-torus). The [semipositive canonical bundle of a submanifold of a complex torus](#semipositive-canonical-bundle-of-a-submanifold-of-a-complex-torus) makes $P_a=(L\otimes\mathcal O(aV))|_V$ positive. Since $K_V=\mathcal O(V)|_V$, the restriction of the $a$-th ambient twist is $K_V\otimes P_{a-1}$ when $a\geq1$. Apply the [Kodaira vanishing theorem](#kodaira-vanishing-theorem) on $V$, and use $0\to L((a-1)V)\to L(aV)\to L(aV)|_V\to0$ and its long exact sequence to induct from the positive bundle $L$ on the torus. No unproved ambient positivity of $\mathcal O(V)$ is needed.

###### Spectral gap for powers of a positive line bundle

↑ **Parent:** [Positive holomorphic line bundle](#positive-holomorphic-line-bundle)

For a positive Hermitian [holomorphic line bundle](#holomorphic-line-bundle) on compact $X$, using its curvature as the [Kähler form](#kahler-form), a linear lower bound in $k$ for the full [Dolbeault Laplacian](#dolbeault-laplacian) on positive antiholomorphic degrees rules out harmonic forms for sufficiently large $k$. The [Dolbeault theorem](#dolbeault-theorem) and [Dolbeault Hodge decomposition](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) then imply $H^{q>0}(X,L^k)=0$.

###### Kodaira embedding theorem

↑ **Parent:** [Positive holomorphic line bundle](#positive-holomorphic-line-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kodaira_embedding_theorem)

The Kodaira embedding theorem says that a compact [complex manifold](#complex-manifold) carrying a [positive holomorphic line bundle](#positive-holomorphic-line-bundle) is projective: sufficiently large [tensor powers](linear-algebra.md#tensor-power) of the bundle have global holomorphic sections defining a [holomorphic embedding](#holomorphic-embedding) into [Complex projective space](algebraic-topology.md#complex-projective-space). Conversely, the restriction of $\mathcal O(1)$ gives a positive line bundle on every projective complex manifold.

###### Holomorphic local trivialization

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

A holomorphic local trivialization of a rank-$r$ [holomorphic vector bundle](#holomorphic-vector-bundle) $E\to X$ is a [biholomorphic](complex-analysis.md#biholomorphism) bundle map $E|_U\to U\times\mathbb C^r$ that is complex linear on each fiber. Equivalently, it is a local frame of holomorphic sections.

###### Holomorphic section

↑ **Parent:** [Holomorphic vector bundle](#holomorphic-vector-bundle)

A section of a [holomorphic vector bundle](#holomorphic-vector-bundle) is holomorphic when its coordinate functions in every [holomorphic local trivialization](#holomorphic-local-trivialization) are holomorphic.

It is a [section of a fiber bundle](fiber-bundle.md#section-fiber-bundle) satisfying holomorphicity.

###### Rank-one sections of two hyperplane line bundles

↑ **Parent:** [Holomorphic section](#holomorphic-section)

A section of $\mathcal O(1)\oplus\mathcal O(1)$ on the [complex projective line](algebraic-topology.md#complex-projective-line) is a pair of homogeneous linear forms $\ell_1=aZ_0+bZ_1$, $\ell_2=cZ_0+dZ_1$. It vanishes at exactly one projective point precisely when its coefficient matrix has rank one, equivalently $ad-bc=0$ and the matrix is nonzero. Its kernel is then one line in $\mathbb C^2$. Equivalently, $s=v\ell$ for a constant nonzero vector $v$ and one nonzero linear form $\ell$. Rank two gives no zero, while rank zero gives the identically zero section.

###### Complex cylinder

↑ **Parent:** [Complex manifold](#complex-manifold)

A complex cylinder is a quotient $\mathbb C/\mathbb Z\tau$ by one nonzero complex translation. Unlike a compact [complex torus](#complex-torus), it is biholomorphic to $\mathbb C^*$ through a suitable exponential map.

###### Complex torus

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_torus)

A complex torus is a quotient $\mathbb C^n/\Lambda$ by a discrete subgroup $\Lambda\cong\mathbb Z^{2n}$ spanning $\mathbb C^n$ over $\mathbb R$. Translation-invariant [differential forms](differential-form.md) descend to the quotient.

###### Semipositive canonical bundle of a submanifold of a complex torus

↑ **Parent:** [Complex torus](#complex-torus)

The tangent bundle of a [complex torus](#complex-torus) is holomorphically trivial with a flat [Hermitian metric](#hermitian-metric-on-a-holomorphic-vector-bundle). Apply the [curvature formula for a holomorphic subbundle](#curvature-formula-for-a-holomorphic-subbundle) to $TV\subset TM|_V$: its determinant dual $K_V$ has semipositive curvature. For a closed smooth hypersurface, [adjunction for a smooth submanifold](#adjunction-for-a-smooth-submanifold) identifies $K_V$ with the restriction of its [divisor line bundle](cartier-divisor.md#divisor-line-bundle). Thus a positive ambient line bundle remains positive on the hypersurface after tensoring by any nonnegative power of the restricted divisor bundle.

###### Period matrix of a complex torus

↑ **Parent:** [Complex torus](#complex-torus)

With a chosen lattice basis and complex coordinates on $\mathbb C^n$, the columns of the period matrix are the coordinate vectors of the lattice generators. It identifies a real coordinate vector $t$ on the universal covering space with $z=\Omega t$.

<h6 id="averaging-kahler-forms-over-a-complex-torus">Averaging Kähler forms over a complex torus</h6>

↑ **Parent:** [Complex torus](#complex-torus)

Averaging a [Kähler form](#kahler-form) over translations with normalized [Haar measure](measure-theory.md#haar-measure) gives an invariant [Kähler form](#kahler-form) in the same [de Rham cohomology](differential-form.md#de-rham-cohomology) class. Positivity is preserved by averaging positive values on $(v,Jv)$, and the class is unchanged because translations are homotopic to the identity. Thus any [Hodge metric](#hodge-metric) on a [complex torus](#complex-torus) can be replaced by an invariant one.

###### Affine lift of a holomorphic map between complex tori

↑ **Parent:** [Complex torus](#complex-torus)

Every [holomorphic map](complex-analysis.md#holomorphic-map) $V_1/\Lambda_1\to V_2/\Lambda_2$ lifts to $z\mapsto Az+x$, where $A$ is a [complex-linear map](vector-space.md#complex-linear-map) satisfying $A\Lambda_1\subseteq\Lambda_2$. Period differences of a lift lie in the discrete target [Euclidean lattice](fourier-analysis.md#euclidean-lattice), so its derivative is periodic. Boundedness on a compact fundamental domain and the [Liouville theorem](complex-analysis.md#liouville-theorem) make this derivative constant. The linear map is unique, and the translation vector is determined modulo $\Lambda_2$.

###### Negation map on a one-dimensional complex torus

↑ **Parent:** [Complex torus](#complex-torus)

Negation is a biholomorphic involution of $E=\mathbb C/\Lambda$. Its fixed points satisfy $2z\in\Lambda$, so they are indexed by the four elements of $\tfrac12\Lambda/\Lambda$.

###### Quotient of a one-dimensional complex torus by negation

↑ **Parent:** [Negation map on a one-dimensional complex torus](#negation-map-on-a-one-dimensional-complex-torus)

Away from the four fixed points, negation acts freely and the quotient map is a holomorphic double covering. Near a fixed point, an invariant coordinate is $w=z^2$, so the quotient extends across the image as a Riemann surface and the map has ramification index two. The [Riemann-Hurwitz formula](complex-analysis.md#riemann-hurwitz-formula) gives

$$
0=2(2g-2)+4,
$$

hence the quotient has genus zero and is biholomorphic to the [Riemann sphere](complex-analysis.md#riemann-sphere).

###### Holomorphic map from the complex plane to a one-dimensional complex torus

↑ **Parent:** [Complex torus](#complex-torus)

Every [holomorphic map](complex-analysis.md#holomorphic-map) $f:\mathbb C\to\mathbb C/\Lambda$ is constant or surjective. It lifts to an entire function $F:\mathbb C\to\mathbb C$. If $F$ is nonconstant, the [Little Picard theorem](complex-analysis.md#little-picard-theorem) says it omits at most one point, while every fiber of $\mathbb C\to\mathbb C/\Lambda$ is an infinite lattice coset; hence every point of the torus has a preimage under $f$.

###### Affine lift of a holomorphic map between one-dimensional complex tori

↑ **Parent:** [Complex torus](#complex-torus)

Let $\pi_\Lambda:\mathbb C\to\mathbb C/\Lambda$ and $\pi_{\Lambda'}:\mathbb C\to\mathbb C/\Lambda'$ be the [universal covering maps](algebraic-topology.md#universal-cover) of two one-dimensional [complex tori](#complex-torus). Every [holomorphic map](complex-analysis.md#holomorphic-map) $f:\mathbb C/\Lambda\to\mathbb C/\Lambda'$ has a [holomorphic lift between one-dimensional complex tori](#affine-lift-of-a-holomorphic-map-between-one-dimensional-complex-tori) $F:\mathbb C\to\mathbb C$ satisfying $\pi_{\Lambda'}\circ F=f\circ\pi_\Lambda$, and every such lift is an [affine function](vector-space.md#affine-function)

$$
F(z)=az+b
$$

with $a\Lambda\subseteq\Lambda'$. Indeed, for $\lambda\in\Lambda$, the continuous function $F(z+\lambda)-F(z)$ takes values in the discrete set $\Lambda'$ and is therefore constant. Hence $F'$ is $\Lambda$-periodic. It is bounded on a compact [fundamental parallelogram](complex-analysis.md#fundamental-parallelogram-of-a-period-lattice) and therefore on the [complex plane](complex-analysis.md#complex-plane), so the [Liouville theorem](complex-analysis.md#liouville-theorem) makes $F'$ constant. If $f$ preserves the identity and the lift is chosen with $F(0)=0$, then $b=0$ and the lift is a [linear map](vector-space.md#linear-map).

###### Automorphism of a one-dimensional complex torus

↑ **Parent:** [Complex torus](#complex-torus)

Every identity-preserving [biholomorphism](complex-analysis.md#biholomorphism) of $\mathbb C/\Lambda$ lifts to multiplication by a nonzero [complex number](complex-analysis.md#complex-number) $\zeta$ satisfying $\zeta\Lambda=\Lambda$. Relative to a $\mathbb Z$-basis of $\Lambda$, multiplication by $\zeta$ is represented by a [unimodular matrix](linear-algebra.md#unimodular-matrix) $A\in\operatorname{GL}_2(\mathbb Z)$. Its real [determinant](linear-algebra.md#determinant) is $|\zeta|^2$, while complex multiplication preserves orientation, so $\det A=1$ and $|\zeta|=1$. The [Cayley-Hamilton theorem](mathematics.md#cayley-hamilton-theorem) gives

$$
\zeta^2-\operatorname{tr}(A)\zeta+1=0.
$$

Consequently $2\operatorname{Re}\zeta=\operatorname{tr}(A)\in\{-2,-1,0,1,2\}$, and $\zeta$ is a [root of unity](algebra.md#root-of-unity) of order $1$, $2$, $3$, $4$, or $6$.

###### Riemann form on a complex torus

↑ **Parent:** [Complex torus](#complex-torus)

A Riemann form on $V/\Gamma$ is a Hermitian form $H$ whose imaginary part is integer-valued on $\Gamma\times\Gamma$. Its imaginary part is equivalently an integral alternating form compatible with the complex structure.

###### Integral Hermitian forms on the square complex torus

↑ **Parent:** [Riemann form on a complex torus](#riemann-form-on-a-complex-torus)

On $\mathbb C/(\mathbb Z+\mathbb Zi)$, a [Hermitian form](linear-algebra.md#hermitian-form) linear in its first argument has integral imaginary part on the [period lattice](complex-analysis.md#period-lattice) exactly when its real scalar coefficient is integral. Positivity is equivalent to $t>0$. The associated [holomorphic line bundle](#holomorphic-line-bundle) has degree $t$ because its [First Chern class](#first-chern-class) is represented by $(it/2)dz\wedge d\overline z$. In particular the oriented Chern pairing is minus the imaginary part under this convention.

###### Riemann bilinear criterion for a period matrix

↑ **Parent:** [Riemann form on a complex torus](#riemann-form-on-a-complex-torus)

A [complex torus](#complex-torus) with [period matrix of a complex torus](#period-matrix-of-a-complex-torus) $\Omega$ admits a [Hodge metric](#hodge-metric) precisely when there is a nonsingular integral skew-symmetric matrix $Q$ satisfying the displayed conditions. The entries of $Q$ are the periods of the invariant [Kähler form](#kahler-form) over lattice two-tori. The first condition imposes type $(1,1)$, and the second imposes positivity; the factor $-i$ corresponds to the convention $\omega(v,Jv)>0$.

###### Polarization of a complex torus

↑ **Parent:** [Riemann form on a complex torus](#riemann-form-on-a-complex-torus)

A polarization of a complex torus is a positive Riemann form, equivalently the first Chern class of an ample line bundle. It is principal when its alternating form identifies the lattice with its dual.

<h6 id="appell-humbert-theorem">Appell–Humbert theorem</h6>

↑ **Parent:** [Complex torus](#complex-torus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Appell–Humbert_theorem)

The Appell–Humbert theorem classifies holomorphic line bundles on a complex torus by a Riemann form together with a compatible semicharacter of its lattice.

###### Semicharacter of a complex lattice

↑ **Parent:** [Appell–Humbert theorem](#appell-humbert-theorem)

For an integral alternating form $E$ arising as the imaginary part of a [Hermitian form](linear-algebra.md#hermitian-form), a semicharacter satisfies $\alpha(\lambda+\mu)=e^{\pi iE(\lambda,\mu)}\alpha(\lambda)\alpha(\mu)$. The [Appell–Humbert theorem](#appell-humbert-theorem) uses this datum together with the [Hermitian form](linear-algebra.md#hermitian-form) to specify a [holomorphic line bundle](#holomorphic-line-bundle) on a [complex torus](#complex-torus). The ratio of two semicharacters is an ordinary unitary [group homomorphism](group-theory.md#group-homomorphism). On the square [period lattice](complex-analysis.md#period-lattice), with $H(z,w)=z\overline w$, all semicharacters are $\alpha(m+ni)=(-1)^{mn}u^m v^n$ for $u,v\in U(1)$.

###### Complex subtorus

↑ **Parent:** [Complex torus](#complex-torus)

A complex subtorus of $V/\Gamma$ is a connected closed complex Lie subgroup. It has the form $V'/\Gamma'$ for a complex subspace $V'\subseteq V$ such that $\Gamma'=V'\cap\Gamma$ is a full lattice in $V'$.

###### Isogeny of complex tori

↑ **Parent:** [Complex torus](#complex-torus)

An isogeny of complex tori is a surjective holomorphic homomorphism with finite kernel. On universal covers it comes from a complex-linear map carrying one lattice into the other with finite index.

###### Hermitian manifold

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hermitian_manifold)

A Hermitian manifold is a [complex manifold](#complex-manifold) whose tangent bundle carries a smoothly varying positive-definite [Hermitian form](linear-algebra.md#hermitian-form). Its real part is a [Riemannian metric](differential-geometry.md#riemannian-metric) invariant under the [complex structure](#complex-structure) $J$.

###### Lefschetz operator on a Hermitian manifold

↑ **Parent:** [Hermitian manifold](#hermitian-manifold)

Exterior multiplication by the fundamental $(1,1)$-form of a [Hermitian manifold](#hermitian-manifold) raises bidegree by $(1,1)$. Its pointwise [formal adjoint](hilbert-space.md#formal-adjoint) lowers bidegree by $(1,1)$. On a [Kähler manifold](#kahler-manifold) this is the [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold), but its pointwise algebraic properties do not require the form to be closed.

###### Injectivity of powers of the Lefschetz operator

↑ **Parent:** [Lefschetz operator on a Hermitian manifold](#lefschetz-operator-on-a-hermitian-manifold)

The [Hermitian Lefschetz operator](#lefschetz-operator-on-a-hermitian-manifold) has injective powers in the indicated range. The [commutator formula for powers of the Lefschetz operator](#commutator-formula-for-powers-of-the-lefschetz-operator) proves this by induction on $r+k$: a form in the kernel can be written as $L\alpha$ using injectivity of the smaller power, and the lower-degree form $\alpha$ is then in the kernel of another power covered by the induction hypothesis.

###### Fundamental form of a Hermitian manifold

↑ **Parent:** [Hermitian manifold](#hermitian-manifold)

For the underlying [Riemannian metric](differential-geometry.md#riemannian-metric) $g$ and [complex structure](#complex-structure) $J$, the fundamental form is $\omega(u,v)=g(Ju,v)$. It is a [real (1, 1)-form](#real-1-1-form). In complex dimension $n$, the compatible orientation has [Riemannian volume form](differential-geometry.md#riemannian-volume-form) $\omega^n/n!$, and its [Hodge star operator](differential-form.md#hodge-star-operator) satisfies

$$
*\omega=\frac{\omega^{n-1}}{(n-1)!}.
$$

###### Hodge star of the fundamental Hermitian form

↑ **Parent:** [Fundamental form of a Hermitian manifold](#fundamental-form-of-a-hermitian-manifold)

In an adapted real orthonormal coframe, the [fundamental form of a Hermitian manifold](#fundamental-form-of-a-hermitian-manifold) is $\omega=\sum_j e^j\wedge f^j$ and the [Riemannian volume form](differential-geometry.md#riemannian-volume-form) is $\omega^n/n!$. The complex-linear [Hodge star](differential-form.md#hodge-star-operator) sends each summand to the product of all the other oriented two-dimensional factors. Summation gives the displayed formula, valid for every [Hermitian manifold](#hermitian-manifold), without a [Kähler](#kahler-manifold) assumption.

###### Real (1, 1)-form

↑ **Parent:** [Hermitian manifold](#hermitian-manifold)

A [differential form of type (p, q)](#differential-form-of-type-p-q) $\varphi$ of type $(1,1)$ is real when $\bar\varphi=\varphi$. Locally this is equivalent to

$$
\varphi=i\sum_{j,k}h_{j\bar k}\,dz^j\wedge d\bar z^k
$$

for a Hermitian matrix $(h_{j\bar k})$.

###### Positive real (1, 1)-form

↑ **Parent:** [Real (1, 1)-form](#real-1-1-form)

A real $(1,1)$-form $\varphi$ is positive when

$$
-i\varphi(\xi,\bar\xi)>0
$$

for every nonzero tangent vector $\xi$ of type $(1,0)$. Equivalently, the local Hermitian matrix in the representation $\varphi=i h_{j\bar k}dz^j\wedge d\bar z^k$ is positive definite.

###### Wedge positivity for two positive (1, 1)-forms

↑ **Parent:** [Positive real (1, 1)-form](#positive-real-1-1-form)

If $\varphi$ and $\psi$ are positive real $(1,1)$-forms and $\xi,\eta$ are linearly independent tangent vectors of type $(1,0)$, then

$$
(\varphi\wedge\psi)(\xi,\eta,\bar\xi,\bar\eta)>0.
$$

After simultaneous diagonalization by congruence, with positive diagonal entries $a_j,b_j$, the left side is

$$
\sum_{j<k}(a_jb_k+a_kb_j)|\xi_j\eta_k-\xi_k\eta_j|^2,
$$

which is positive because some $2\times2$ minor is nonzero.

<h6 id="kahler-manifold">Kähler manifold</h6>

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_manifold)

A Kähler manifold is a complex manifold with a positive real closed $(1,1)$-form $\omega$. The associated Riemannian metric is $g(u,v)=\omega(u,Jv)$.

###### Calabi-Yau threefold

↑ **Parent:** [Kähler manifold](#kahler-manifold)

Here a Calabi-Yau threefold is a compact complex three-dimensional [Kähler manifold](#kahler-manifold) with trivial [canonical bundle](#canonical-bundle) and $H^1(M,\mathbb C)=0$. The [Hodge decomposition theorem for compact Kähler manifolds](#hodge-decomposition-theorem-for-compact-kahler-manifolds) gives $H^1(M,\mathcal O_M)=0$, and [Serre duality for compact complex manifolds](ringed-space.md#serre-duality-for-compact-complex-manifolds) then gives $H^2(M,\mathcal O_M)=0$. This supplies a positive integral Kähler class and hence a projective embedding.

<h6 id="kahler-cone">Kähler cone</h6>

↑ **Parent:** [Kähler manifold](#kahler-manifold)

The Kähler cone of a compact [Kähler manifold](#kahler-manifold) is the open cone of real $(1,1)$ cohomology classes represented by positive closed $(1,1)$ forms. If every real degree-two cohomology class has type $(1,1)$, density of rational classes supplies a rational Kähler class. An integral multiple is the [First Chern class](#first-chern-class) of a positive [holomorphic line bundle](#holomorphic-line-bundle), and the [Kodaira embedding theorem](#kodaira-embedding-theorem) implies projectivity.

<h6 id="kahler-class">Kähler class</h6>

↑ **Parent:** [Kähler cone](#kahler-cone)

The [de Rham cohomology](differential-form.md#de-rham-cohomology) class of a [Kähler form](#kahler-form) is a Kähler class. Such classes form the [Kähler cone](#kahler-cone). They have positive integral on every complex curve, and their top self-intersection is positive.

<h6 id="kahler-metric">Kähler metric</h6>

↑ **Parent:** [Kähler manifold](#kahler-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_metric)

Locally, a Kähler metric is the complex Hessian $g_{i\bar j}=\partial_i\partial_{\bar j}K$ of a real Kähler potential. Adding a holomorphic function and its complex conjugate to $K$ leaves the metric unchanged.

###### Hodge metric

↑ **Parent:** [Kähler metric](#kahler-metric)

A Hodge metric is a [Kähler metric](#kahler-metric) whose [Kähler form](#kahler-form) represents an [integral cohomology](cohomology.md#integral-cohomology) class in real [de Rham cohomology](differential-form.md#de-rham-cohomology). Equivalently, its periods over integral two-cycles are integers. Some conventions require the class of $\omega/(2\pi)$ to be integral instead; this changes the normalization but not existence.

<h6 id="kahler-normal-holomorphic-coordinates">Kähler normal holomorphic coordinates</h6>

↑ **Parent:** [Kähler metric](#kahler-metric)

At any point of a [Kähler manifold](#kahler-manifold), a complex-linear coordinate change normalizes the Hermitian metric matrix. Closedness makes its holomorphic first derivatives symmetric in the two unbarred indices. A quadratic holomorphic coordinate change removes those derivatives, and Hermitian symmetry removes the antiholomorphic derivatives. Conversely, having this first-order normalization at every point makes the [fundamental Hermitian form](#fundamental-form-of-a-hermitian-manifold) closed.

<h6 id="kahler-form">Kähler form</h6>

↑ **Parent:** [Kähler metric](#kahler-metric)

For a [Kähler metric](#kahler-metric) $g$ with [complex structure](#complex-structure) $J$, the associated real two-form is $\omega(u,v)=g(Ju,v)$. It has type $(1,1)$, is positive in the sense $\omega(v,Jv)=g(v,v)>0$ for $v\ne0$, and is closed. Conversely a real closed positive $(1,1)$ form determines a [Kähler metric](#kahler-metric). A local [geometric Kähler potential](#kahler-potential-complex-geometry) writes it as $i\partial\bar\partial\varphi$.

<h6 id="powers-of-a-compact-kahler-form-have-nonzero-cohomology-classes">Powers of a compact Kähler form have nonzero cohomology classes</h6>

↑ **Parent:** [Kähler form](#kahler-form)

On a nonempty compact [Kähler manifold](#kahler-manifold) of complex dimension $n$, the [Kähler form](#kahler-form) is closed and $\int_X\omega^n>0$. If $\omega^k=d\eta$ for $1\leq k\leq n$, then $\omega^n=d(\eta\wedge\omega^{n-k})$; [Stokes theorem](calculus.md#stokes-theorem) contradicts the positive integral. Thus the [de Rham cohomology](differential-form.md#de-rham-cohomology) is nonzero in every even degree through $2n$.

<h6 id="local-real-potential-for-a-closed-1-1-form">Local real potential for a closed (1,1)-form</h6>

↑ **Parent:** [Kähler form](#kahler-form)

For a closed real $(1,1)$ form, the [Poincaré lemma](differential-form.md#poincare-lemma) gives a real one-form $\eta$ with $d\eta=\omega$. Its $(0,1)$ part is $\bar\partial$-closed, so the [Dolbeault-Poincaré lemma](#dolbeault-poincare-lemma) gives $\eta^{0,1}=\bar\partial\psi$. Reality gives $\eta^{1,0}=\partial\bar\psi$, hence $\omega=i\partial\bar\partial(2\operatorname{Im}\psi)$. Positivity is a separate requirement for this form to define a metric.

<h6 id="rotation-invariant-kahler-potential-on-the-complex-plane">Rotation-invariant Kähler potential on the complex plane</h6>

↑ **Parent:** [Local real potential for a closed (1,1)-form](#local-real-potential-for-a-closed-1-1-form)

A smooth real rotation-invariant potential is constant on every positive-radius circle, so its logarithmic-radius function $u$ is smooth on $\mathbb R$. Off the origin, $f_{z\bar z}=e^{-t}u''(t)$. Since $f$ is smooth on the entire plane, this coefficient extends smoothly through the origin. A finite [Taylor expansion](calculus.md#taylor-expansion), rather than a convergent series assumption, gives $f(z)=f(0)+b|z|^2+O(|z|^4)$.

<h6 id="positivity-criterion-for-a-radial-kahler-potential">Positivity criterion for a radial Kähler potential</h6>

↑ **Parent:** [Rotation-invariant Kähler potential on the complex plane](#rotation-invariant-kahler-potential-on-the-complex-plane)

For a potential already smooth on all of $\mathbb C$, the associated form is a [Kähler form](#kahler-form) exactly when the displayed two positivity conditions hold. The first gives a positive metric coefficient off the origin; the second is positivity of $f_{z\bar z}(0)$. The associated real metric is $2f_{z\bar z}(dx^2+dy^2)$. Positivity away from the origin alone permits a degenerate metric at the origin.

<h6 id="kahler-potential-complex-geometry">Kähler potential (complex geometry)</h6>

↑ **Parent:** [Kähler metric](#kahler-metric)

A [geometric Kähler potential](#kahler-potential-complex-geometry) is locally a real smooth function $\varphi$ with $\omega=i\partial\bar\partial\varphi$ for the [Kähler form](#kahler-form). Its complex Hessian must be positive definite to define a [Kähler metric](#kahler-metric). Conventions sometimes absorb a factor of $1/2$ into $\varphi$. Potentials differing by the real part of a [holomorphic function](complex-analysis.md#holomorphic-function) determine the same form. This topic concerns ordinary [complex geometry](complex-geometry.md); the existing undisambiguated [Kähler potential](supersymmetry.md#kahler-potential) entry concerns superfields.

<h6 id="radial-kahler-metric-with-euclidean-volume-in-complex-dimension-two">Radial Kähler metric with Euclidean volume in complex dimension two</h6>

↑ **Parent:** [Kähler potential (complex geometry)](#kahler-potential-complex-geometry)

For $s=|z_1|^2+|z_2|^2>0$ and $a>0$, a [geometric Kähler potential](#kahler-potential-complex-geometry) with derivative $\varphi'(s)=\sqrt{s^2+a^2}/(2s)$ defines a [Kähler metric](#kahler-metric) on $\mathbb C^2\setminus\{0\}$. Its tangential and radial [eigenvalues](linear-operator-theory.md#eigenvalue) are $\sqrt{s^2+a^2}/(2s)$ and $s/(2\sqrt{s^2+a^2})$. Their product is $1/4$, giving the same [Riemannian volume form](differential-geometry.md#riemannian-volume-form) as $\omega_0=(i/2)\sum dz_j\wedge d\bar z_j$, although the metric is different. This construction makes preservation of volume compatible with anisotropic stretching.

<h6 id="kahler-quotient">Kähler quotient</h6>

↑ **Parent:** [Kähler manifold](#kahler-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_quotient)

A Kähler quotient imposes a moment-map level condition and divides by the compact symmetry group. Under suitable stability assumptions it is equivalent to a quotient by the complexified group and inherits a Kähler metric away from singular orbits.

<h6 id="lefschetz-operator-of-a-kahler-manifold">Lefschetz operator of a Kähler manifold</h6>

↑ **Parent:** [Kähler manifold](#kahler-manifold)

The Lefschetz operator of a [Kähler manifold](#kahler-manifold) is exterior multiplication by its Kähler form,

$$
L\alpha=\omega\wedge\alpha.
$$

Its formal adjoint is denoted by $\Lambda=L^*$ and lowers the bidegree of a [differential form](differential-form.md) by $(1,1)$.

This wedge operator participates in the [Kähler identities](#kahler-identities); the theorem on integral $(1,1)$ classes is a different result.

###### Hard Lefschetz theorem on de Rham cohomology

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)

For a compact [Kähler manifold](#kahler-manifold) of complex dimension $n$, wedging with the $(n-k)$th power of its [Kähler class](#kahler-class) is the displayed [isomorphism](algebra.md#isomorphism) for $0\leq k\leq n$. The [Hard Lefschetz isomorphism on Dolbeault cohomology](#hard-lefschetz-isomorphism-on-dolbeault-cohomology) and [Hodge decomposition theorem for compact Kähler manifolds](#hodge-decomposition-theorem-for-compact-kahler-manifolds) give the result by summing the bidegrees. In particular, $L:H^k\to H^{k+2}$ is [injective](algebra.md#injective-function) when $k<n$: if $L\alpha=0$, then $L^{n-k}\alpha=0$. Hence $b_k\leq b_{k+2}$ below the middle dimension.

###### Hard Lefschetz isomorphism on Dolbeault cohomology

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)

On a compact [Kähler manifold](#kahler-manifold), the [Lefschetz operator preserves harmonic forms](#lefschetz-operator-preserves-harmonic-forms), so the indicated power acts on harmonic representatives of [Dolbeault cohomology](#dolbeault-cohomology). It is injective by [injectivity of powers of the Lefschetz operator](#injectivity-of-powers-of-the-lefschetz-operator); [Hodge symmetry](#hodge-symmetry) and [Hodge duality](#hodge-duality) make its finite-dimensional source and target have equal dimension, so it is an isomorphism.

###### Dependence of Lefschetz maps on the Dolbeault class

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)

Wedge multiplication by a closed $(1,1)$ form induces maps on [Dolbeault cohomology](#dolbeault-cohomology). If $\omega'-\omega=\bar\partial\theta$, then $(\omega')^k-\omega^k=\bar\partial(\theta\wedge\sum_{j=0}^{k-1}(\omega')^j\wedge\omega^{k-1-j})$. Wedging with a closed representative shows that the maps agree. For a change of [Kähler metric potential](#kahler-potential-complex-geometry), take $\theta=-i\partial f$.

<h6 id="primitive-differential-form-on-a-kahler-manifold">Primitive differential form on a Kähler manifold</h6>

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)

For degree $k\leq n$, a form is primitive if $\Lambda\alpha=0$, equivalently $L^{n-k+1}\alpha=0$. In middle degree $k=n$ this is equivalent to $L\alpha=0$. On a compact [Kähler manifold](#kahler-manifold), the same definitions apply to cohomology via [harmonic differential forms](differential-form.md#harmonic-differential-form).

<h6 id="primitive-1-1-forms-on-a-kahler-surface-are-anti-self-dual">Primitive (1,1)-forms on a Kähler surface are anti-self-dual</h6>

↑ **Parent:** [Primitive differential form on a Kähler manifold](#primitive-differential-form-on-a-kahler-manifold)

On a complex two-dimensional [Kähler manifold](#kahler-manifold), a primitive $(1,1)$ form satisfies $*\alpha=-\alpha$, making it an [anti-self-dual differential form](differential-form.md#anti-self-dual-differential-form). For a nonzero real primitive harmonic form on a compact surface, $\int\alpha\wedge\alpha=-\|\alpha\|_{L^2}^2<0$.

###### Lefschetz commutator

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)

In complex dimension $n$, the [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold) and [adjoint Lefschetz operator](#adjoint-lefschetz-operator) satisfy $[\Lambda,L]=(n-k)\operatorname{id}$ on degree $k$. In middle degree, this yields $\|L\alpha\|^2=\|\Lambda\alpha\|^2$.

###### Commutator formula for powers of the Lefschetz operator

↑ **Parent:** [Lefschetz commutator](#lefschetz-commutator)

For the [Hermitian Lefschetz operator](#lefschetz-operator-on-a-hermitian-manifold) on a complex $n$-manifold, the [Lefschetz commutator](#lefschetz-commutator) and the [commutator derivation identity](lie-algebra.md#commutator-derivation-identity) imply this formula. When expanding a product commutator, one must evaluate $[L,\Lambda]$ on the degree after the powers of $L$ to its right have acted.

###### Adjoint Lefschetz operator

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)

The adjoint of $L=\omega\wedge-$ lowers real degree by two and bidegree by $(1,1)$. On a compact [Kähler manifold](#kahler-manifold) it acts on cohomology through [harmonic differential forms](differential-form.md#harmonic-differential-form), because it commutes with the [Hodge Laplacian](differential-form.md#hodge-laplacian). It does not generally preserve all closed forms.

<h6 id="kahler-identities">Kähler identities</h6>

↑ **Parent:** [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_identities)

For the [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold) and its adjoint, the Kähler identities include

$$
[\Lambda,\partial]=i\bar\partial^*,\qquad
[\Lambda,\bar\partial]=-i\partial^*,\qquad
[L,\partial^*]=i\bar\partial,\qquad
[L,\bar\partial^*]=-i\partial.
$$

<h6 id="bundle-valued-kahler-identities">Bundle-valued Kähler identities</h6>

↑ **Parent:** [Kähler identities](#kahler-identities)

On a [Kähler manifold](#kahler-manifold) the [Chern connection](#chern-connection) components satisfy $[\Lambda,\bar\partial_E]=-i(D'_E)^*$ and $[\Lambda,D'_E]=i\bar\partial_E^*$. Holomorphic normal coordinates and a [Chern connection in a normal holomorphic frame](#chern-connection-in-a-normal-holomorphic-frame) reduce them to the scalar identities pointwise. Closedness of the Kähler form also gives $[\Lambda,\bar\partial_E^*]=0$.

###### Lefschetz-Dolbeault curvature commutator

↑ **Parent:** [Bundle-valued Kähler identities](#bundle-valued-kahler-identities)

For a Hermitian holomorphic bundle over a [Kähler manifold](#kahler-manifold), let $\Theta$ act by exterior multiplication. The [bundle-valued Kähler identities](#bundle-valued-kahler-identities) give $[\Lambda,\Delta_{\bar\partial}]=-i(\Theta\wedge-)^*$, and taking adjoints yields $[\Delta_{\bar\partial},L]=i\Theta\wedge-$. This measures the failure of the bundle-valued [Dolbeault Laplacian](#dolbeault-laplacian) to commute with the Lefschetz operator.

###### Flatness criterion from Lefschetz commutation

↑ **Parent:** [Lefschetz-Dolbeault curvature commutator](#lefschetz-dolbeault-curvature-commutator)

The Lefschetz operator commutes with the bundle-valued [Dolbeault Laplacian](#dolbeault-laplacian) on the entire smooth form space exactly when the [Chern connection](#chern-connection) is flat. The [Lefschetz-Dolbeault curvature commutator](#lefschetz-dolbeault-curvature-commutator) gives one direction. Conversely test its curvature-wedge operator on degree-zero sections with arbitrary prescribed values at any point to force every [vector-bundle curvature](fiber-bundle.md#curvature-form) [endomorphism](algebra.md#endomorphism) to vanish.

###### Bochner-Kodaira-Nakano identity

↑ **Parent:** [Kähler identities](#kahler-identities)

For the [Chern connection](#chern-connection) of a Hermitian [holomorphic vector bundle](#holomorphic-vector-bundle) on a [Kähler manifold](#kahler-manifold), the two [Dolbeault Laplacians](#dolbeault-laplacian) differ by $[iF\wedge,\Lambda]$, where $F$ is its [curvature form of a connection](fiber-bundle.md#curvature-form) and $\Lambda$ is the [adjoint Lefschetz operator](#adjoint-lefschetz-operator). The curvature term controls vanishing estimates.

###### Dolbeault Laplacian

↑ **Parent:** [Kähler identities](#kahler-identities)

The Dolbeault Laplacian is $\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial$. On a [Kähler manifold](#kahler-manifold), the [Kähler identities](#kahler-identities) imply

$$
\Delta_d=2\Delta_\partial=2\Delta_{\bar\partial}.
$$

###### Dolbeault Green operator

↑ **Parent:** [Dolbeault Laplacian](#dolbeault-laplacian)

On a compact [Hermitian manifold](#hermitian-manifold) without boundary, this operator is the inverse of the [Dolbeault Laplacian](#dolbeault-laplacian) on the orthogonal complement of its harmonic forms and is zero on the harmonic space. Elliptic theory gives $\Delta_{\bar\partial}G=G\Delta_{\bar\partial}=I-H$, with $H$ the harmonic projection, and ensures that $G$ sends smooth forms to smooth forms. It commutes with $\bar\partial$ and $\bar\partial^*$; their commutation with the Laplacian and orthogonality to its kernel give this by uniqueness of the inverse. If $\eta$ is $\bar\partial$-exact, then $\eta=\bar\partial\bar\partial^*G\eta$. On a [Kähler manifold](#kahler-manifold), the same operator serves the holomorphic Laplacian because $\Delta_\partial=\Delta_{\bar\partial}$.

<h6 id="kahler-laplacian-identity">Kähler Laplacian identity</h6>

↑ **Parent:** [Dolbeault Laplacian](#dolbeault-laplacian)

On a [Kähler manifold](#kahler-manifold), expanding $d=\partial+\bar\partial$ and using the [Kähler identities](#kahler-identities) makes the mixed anticommutators vanish and gives $\Delta_\partial=\Delta_{\bar\partial}$. Therefore

$$
\Delta_d=2\Delta_{\bar\partial}=2\Delta_\partial.
$$

<h6 id="harmonicity-of-holomorphic-functions-on-a-kahler-manifold">Harmonicity of holomorphic functions on a Kähler manifold</h6>

↑ **Parent:** [Kähler Laplacian identity](#kahler-laplacian-identity)

The [Kähler Laplacian identity](#kahler-laplacian-identity) $\Delta_d^{\mathrm H}=2\Delta_{\bar\partial}$ implies that every [holomorphic function](complex-analysis.md#holomorphic-function) on a [Kähler manifold](#kahler-manifold) is a [harmonic function](partial-differential-equation.md#harmonic-function). On functions, $\bar\partial u=0$ and $\bar\partial^*u=0$ by degree, so both terms of the [Dolbeault Laplacian](#dolbeault-laplacian) vanish. Compactness is unnecessary. Changing the sign convention for the scalar Laplacian does not change this conclusion.

###### Lefschetz operator preserves harmonic forms

↑ **Parent:** [Dolbeault Laplacian](#dolbeault-laplacian)

On a [Kähler manifold](#kahler-manifold), the [Lefschetz operator of a Kähler manifold](#lefschetz-operator-of-a-kahler-manifold) $L=\omega\wedge-$ commutes with the [Dolbeault Laplacian](#dolbeault-laplacian):

$$
[L,\Delta_{\bar\partial}]=0.
$$

Consequently, if $\alpha$ is $\Delta_{\bar\partial}$-harmonic, then every $\alpha\wedge\omega^k=L^k\alpha$ is also harmonic.

###### Dolbeault Hodge decomposition on a compact Hermitian manifold

↑ **Parent:** [Dolbeault Laplacian](#dolbeault-laplacian)

For a compact [Hermitian manifold](#hermitian-manifold), elliptic theory gives the orthogonal decomposition

$$
\Omega^{p,q}
=\mathcal H^{p,q}_{\bar\partial}
\oplus\bar\partial\Omega^{p,q-1}
\oplus\bar\partial^*\Omega^{p,q+1}.
$$

The harmonic space $\mathcal H^{p,q}_{\bar\partial}=\ker\Delta_{\bar\partial}$ is finite-dimensional and represents [Dolbeault cohomology](#dolbeault-cohomology).

###### Complementary Dolbeault harmonic types on a Hermitian manifold

↑ **Parent:** [Dolbeault Hodge decomposition on a compact Hermitian manifold](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold)

On a compact [Hermitian manifold](#hermitian-manifold) of complex dimension $n$, $C\alpha=*\bar\alpha$, with complex-linear [Hodge star](differential-form.md#hodge-star-operator), is a conjugate-linear bijection from [Dolbeault Laplacian](#dolbeault-laplacian) harmonic $(p,q)$-forms to harmonic $(n-p,n-q)$-forms. The identities $\bar\partial^*=-*\partial*$ and $*^2=(-1)^{p+q}$ show that $\bar\partial\alpha=\bar\partial^*\alpha=0$ implies the same two equations for $C\alpha$. Its square is $(-1)^{p+q}$. Thus these harmonic spaces have equal complex dimension even without the [Kähler](#kahler-manifold) condition. The natural map is conjugate-linear, not complex-linear.

###### ddbar lemma

↑ **Parent:** [Dolbeault Hodge decomposition on a compact Hermitian manifold](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold)

On a compact [Kähler manifold](#kahler-manifold), a pure-type differential form that is $d$-closed and is either $\partial$-exact or $\bar\partial$-exact is $\partial\bar\partial$-exact. In particular, if $\eta$ is $\bar\partial$-exact and $\partial\eta=0$, then

$$
\eta=\bar\partial\partial\phi
$$

for a form $\phi$ of bidegree one lower in each component.

<h6 id="global-potential-for-cohomologous-kahler-forms">Global potential for cohomologous Kähler forms</h6>

↑ **Parent:** [Ddbar lemma](#ddbar-lemma)

On a compact [Kähler manifold](#kahler-manifold), the difference of cohomologous [Kähler forms](#kahler-form) is a real, [de Rham cohomology](differential-form.md#de-rham-cohomology) exact $(1,1)$-form. The [ddbar lemma](#ddbar-lemma) gives $\widetilde\omega-\omega=\partial\bar\partial h$. Reality implies $\partial\bar\partial\bar h=-(\widetilde\omega-\omega)$, so $f=(h-\bar h)/(2i)$ is real and has the displayed potential equation. The difference of two real potentials is a [pluriharmonic function](partial-differential-equation.md#pluriharmonic-function), hence constant on each connected component. On a connected manifold the only ambiguity is one additive constant.

###### Harmonic orthogonality criterion for ddbar exactness

↑ **Parent:** [Ddbar lemma](#ddbar-lemma)

If $\alpha$ is a $d$-closed $(p,q)$-form on a compact [Kähler manifold](#kahler-manifold), then $\alpha$ is [ddbar lemma](#ddbar-lemma) exact if and only if it is orthogonal to every [harmonic differential form](differential-form.md#harmonic-differential-form) of type $(p,q)$. The forward implication follows by integration by parts. For the reverse implication, [Dolbeault Hodge decomposition](#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) first makes $\alpha$ $\bar\partial$-exact, and the ddbar lemma then makes it $\partial\bar\partial$-exact.

###### Green operator potential for ddbar exactness

↑ **Parent:** [Harmonic orthogonality criterion for ddbar exactness](#harmonic-orthogonality-criterion-for-ddbar-exactness)

For a $d$-closed pure-type form $\alpha$ orthogonal to [harmonic forms](differential-form.md#harmonic-differential-form) on a [compact](topology.md#compact-space) [Kähler manifold](#kahler-manifold), let $G_{\bar\partial}$ be the inverse of the [Dolbeault Laplacian](#dolbeault-laplacian) on the harmonic complement, zero on the harmonic space. The [Kähler Laplacian identity](#kahler-laplacian-identity) makes it commute with $\partial$ and $\bar\partial$. Thus $\alpha=\bar\partial\bar\partial^*G_{\bar\partial}\alpha$ and $G_{\bar\partial}\alpha=\partial\partial^*G_{\bar\partial}^2\alpha$. The mixed anticommutator $\bar\partial^*\partial+\partial\bar\partial^*=0$ gives $\alpha=\partial\bar\partial\beta$. This is an explicit potential for the [ddbar lemma](#ddbar-lemma), with one lower degree of each type; using the inverse of the [Hodge Laplacian](differential-form.md#hodge-laplacian) instead multiplies the displayed expression by four.

###### ddc lemma

↑ **Parent:** [Ddbar lemma](#ddbar-lemma)

On a compact [Kähler manifold](#kahler-manifold), if a differential form $\alpha$ is $d$-closed and $d^c$-exact, then it is $dd^c$-exact: there is a form $\beta$ two degrees lower such that $\alpha=dd^c\beta$. This real-form statement is equivalent, after decomposing by type, to the [ddbar lemma](#ddbar-lemma).

###### Fubini-Study metric

↑ **Parent:** [Kähler manifold](#kahler-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fubini–Study_metric)

The Fubini-Study metric is the standard unitary-invariant [Kähler metric](#kahler-metric) on [Complex projective space](algebraic-topology.md#complex-projective-space), induced from the unit sphere by the [Hopf fibration](algebraic-topology.md#hopf-fibration). Its associated [Kähler form](#kahler-form) is the [Fubini-Study form](#fubini-study-form); scaling conventions determine the area of a projective line.

###### Fubini-Study form

↑ **Parent:** [Fubini-Study metric](#fubini-study-metric)

The Fubini-Study form is the standard Kähler form on complex projective space. With the integral normalization, $[\omega_{FS}/(2\pi)]=c_1(\mathcal O(1))$.

The two-form is associated with the [Fubini-Study metric](#fubini-study-metric).

###### Integrally normalized Fubini-Study form

↑ **Parent:** [Fubini-Study form](#fubini-study-form)

The form $\omega_{\rm int}=\frac{i}{2\pi}\partial\bar\partial\log(1+\sum|z_j|^2)$ patches on [Complex projective space](algebraic-topology.md#complex-projective-space). The dual tautological metric on $\mathcal O(1)$ identifies it with normalized [Chern curvature](#chern-curvature), so $[\omega_{\rm int}]=c_1(\mathcal O(1))$. With the unnormalized convention $i\partial\bar\partial\log(1+\sum|z_j|^2)$, divide by $2\pi$ to obtain this integral class.

###### Fubini-Study form from circle reduction

↑ **Parent:** [Fubini-Study form](#fubini-study-form)

The scalar [circle group](lie-theory.md#circle-group) action on $\mathbb C^{n+1}$ with the [standard symplectic form](symplectic-geometry.md#standard-symplectic-form) has [moment map](symplectic-geometry.md#moment-map) $\mu=-|z|^2/2$ in the convention $\iota_{X_H}\omega=dH$. Reduction of the radius-$R$ sphere gives [Complex projective space](algebraic-topology.md#complex-projective-space) and the form $\omega_R=(iR^2/2)\partial\bar\partial\log(1+|w|^2)$. Its area on a [complex projective line](algebraic-topology.md#complex-projective-line) is $\pi R^2$. Thus $R=\sqrt2$ yields the [Fubini-Study form](#fubini-study-form) normalized to projective-line area $2\pi$, while $R=1$ yields half that form. The [Hopf fibration](algebraic-topology.md#hopf-fibration) identifies the quotient.

###### Symplectic ball chart in complex projective space

↑ **Parent:** [Fubini-Study form from circle reduction](#fubini-study-form-from-circle-reduction)

Normalize the [Fubini-Study form](#fubini-study-form) so that a [complex projective line](algebraic-topology.md#complex-projective-line) has [symplectic area](symplectic-geometry.md#symplectic-area) $\pi$. The displayed map takes the unit [symplectic ball](symplectic-geometry.md#symplectic-ball) in $\mathbb C^n$ diffeomorphically onto the complement of the last-coordinate hyperplane. Its lift to the unit sphere has last coordinate positive real, so that coordinate contributes zero to the pulled-back [standard symplectic form](symplectic-geometry.md#standard-symplectic-form). The map is therefore a [symplectomorphism](symplectic-geometry.md#symplectomorphism).

###### Two-ball packing obstruction in the projective plane

↑ **Parent:** [Symplectic ball chart in complex projective space](#symplectic-ball-chart-in-complex-projective-space)

Two disjoint [symplectic balls](symplectic-geometry.md#symplectic-ball) of radii $r_1,r_2$ embedding into the unit four-ball must satisfy the displayed inequality. Extend their transported standard [complex structures](#complex-structure) on smaller concentric balls to a [compatible almost complex structure](#compatible-almost-complex-structure) on the projective plane. A degree-one [J-holomorphic curve](symplectic-geometry.md#pseudoholomorphic-curve) through both centres has area $\pi$. The [Monotonicity theorem for a J-holomorphic curve](symplectic-geometry.md#monotonicity-theorem-for-a-j-holomorphic-curve) bounds its area in each smaller ball below by $\pi\rho_i^2$. Disjointness allows these bounds to be added; letting $\rho_i$ increase to $r_i$ proves the result.

<h6 id="hodge-decomposition-theorem-for-compact-kahler-manifolds">Hodge decomposition theorem for compact Kähler manifolds</h6>

↑ **Parent:** [Kähler manifold](#kahler-manifold)

For a compact Kähler manifold,

$$
H^k_{dR}(X;\mathbb C)=\bigoplus_{p+q=k}H^{p,q}_{\bar\partial}(X),
$$

and every class has a unique harmonic representative of each type.

This is the compact Kähler specialization of [Hodge theory](differential-geometry.md#hodge-theory).

###### Primitive cohomology

↑ **Parent:** [Hodge decomposition theorem for compact Kähler manifolds](#hodge-decomposition-theorem-for-compact-kahler-manifolds)

For a compact [Kähler manifold](#kahler-manifold) of complex dimension $d$ and $k\le d$, this is the cohomology killed by the indicated power of a [Kähler class](#kahler-class). The Hodge–Riemann bilinear relations polarize its [Hodge structure](differential-geometry.md#hodge-structure). On a [K3 surface](#k3-surface), primitive degree-two cohomology is the orthogonal complement of the chosen positive class.

<h6 id="hodge-riemann-bilinear-relations">Hodge–Riemann bilinear relations</h6>

↑ **Parent:** [Primitive cohomology](#primitive-cohomology)

For a nonzero primitive class $v\in H^{p,q}$ of degree $k=p+q$ on a compact [Kähler manifold](#kahler-manifold) of complex dimension $d$, the displayed expression is positive. Together with orthogonality of complementary Hodge bidegrees, this makes primitive cohomology a [polarized Hodge structure](differential-geometry.md#polarized-hodge-structure) when the [Kähler class](#kahler-class) is rational, after clearing denominators. Positivity on the full cohomology requires the signs prescribed by its primitive decomposition.

<h6 id="odd-betti-numbers-of-a-compact-kahler-manifold-are-even">Odd Betti numbers of a compact Kähler manifold are even</h6>

↑ **Parent:** [Hodge decomposition theorem for compact Kähler manifolds](#hodge-decomposition-theorem-for-compact-kahler-manifolds)

The [Kähler Laplacian identity](#kahler-laplacian-identity) makes the space of complex [harmonic differential forms](differential-form.md#harmonic-differential-form) of degree $r$ the direct sum of its $(p,q)$ parts with $p+q=r$. Conjugation identifies the $(p,q)$ and $(q,p)$ harmonic spaces. If $r$ is odd these are distinct and pair off, so the [Betti number](homology.md#betti-number) in degree $r$ is even. This is a topological obstruction to existence of a [Kähler metric](#kahler-metric), exhibited by a [Hopf surface](#hopf-surface) with first Betti number one.

<h6 id="hodge-index-theorem-for-compact-kahler-surfaces">Hodge index theorem for compact Kähler surfaces</h6>

↑ **Parent:** [Hodge decomposition theorem for compact Kähler manifolds](#hodge-decomposition-theorem-for-compact-kahler-manifolds)

On a connected compact [Kähler manifold](#kahler-manifold) of complex dimension two, the [intersection form](homology.md#intersection-form) restricted to real $(1,1)$ cohomology has [signature](linear-algebra.md#signature-of-a-quadratic-form) $(1,h^{1,1}-1)$. The Kähler class spans a positive line, and its orthogonal complement consists of primitive classes, which are negative definite. Thus a [totally isotropic subspace](linear-algebra.md#totally-isotropic-subspace) of real $(1,1)$ cohomology has dimension at most one.

###### Canonical bundle

↑ **Parent:** [Complex manifold](#complex-manifold)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_bundle)

The canonical bundle of a complex $n$-manifold is the holomorphic line bundle $K_X=\bigwedge^n(T^{1,0}X)^*$.

<h6 id="poincare-residue-along-a-smooth-hypersurface">Poincaré residue along a smooth hypersurface</h6>

↑ **Parent:** [Canonical bundle](#canonical-bundle)

If a meromorphic top form has at most a simple pole along a smooth [complex analytic hypersurface](#complex-analytic-hypersurface) $Y=\{z=0\}$, write $\alpha=(dz/z)\wedge\beta$ with $\beta$ holomorphic. Its residue is $\beta|_Y$, a holomorphic section of the [canonical bundle](#canonical-bundle) $K_Y$. A change of defining coordinate $t=az$, with $a$ holomorphic and nonzero, changes $dt/t$ by the holomorphic form $da/a$ and leaves this restriction invariant. Placing the normal factor first fixes the sign convention.

<h6 id="residue-trivialization-for-a-degree-n-plus-1-projective-hypersurface">Residue trivialization for a degree n+1 projective hypersurface</h6>

↑ **Parent:** [Poincaré residue along a smooth hypersurface](#poincare-residue-along-a-smooth-hypersurface)

For a smooth hypersurface $Y=\{f=0\}\subset\mathbb{CP}^n$ of degree $n+1$, let $E=\sum z_i\partial_{z_i}$ and $\Omega=dz_0\wedge\cdots\wedge dz_n$. The meromorphic form $(\iota_E\Omega)/f$ descends to projective space because its scaling weights cancel and it is horizontal. Its [Poincaré residue](#poincare-residue-along-a-smooth-hypersurface) is a nowhere-zero section of $K_Y$. On the chart $z_j=1$, with remaining coordinates $t_1,\ldots,t_n$ in original-index order and $F=f|_{z_j=1}$, it is $(-1)^{j+r-1}(dt_1\wedge\cdots\widehat{dt_r}\cdots\wedge dt_n)/F_{t_r}$ wherever $F_{t_r}\ne0$. Thus $K_Y\cong\mathcal O_Y$.

###### Holomorphic cubic differential

↑ **Parent:** [Canonical bundle](#canonical-bundle)

A section of the cube of the [canonical bundle](#canonical-bundle), locally $c=\phi(z)\,dz^3$ with [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) coefficient. The [flat coordinates](#natural-coordinate-of-a-holomorphic-differential) obtained by integrating cube roots have transitions $w\mapsto\zeta w+b$, $\zeta^3=1$; general real-linear deformations do not preserve these as [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) transitions.

###### Quadratic differential

↑ **Parent:** [Canonical bundle](#canonical-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_differential)

A section of the square of the [canonical bundle](#canonical-bundle), locally $q=\phi(z)\,dz^2$; its coefficient changes by the square of the coordinate [derivative](calculus.md#derivative). A [holomorphic quadratic differential](#holomorphic-quadratic-differential) has [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) coefficient, and its [flat metric of a quadratic differential](#flat-metric-of-a-quadratic-differential) is $|q|^{1/2}$.

###### Flat metric of a quadratic differential

↑ **Parent:** [Quadratic differential](#quadratic-differential)

For $q=\phi(z)\,dz^2$, the length element is $|\phi(z)|^{1/2}|dz|$, locally Euclidean in [flat coordinates](#natural-coordinate-of-a-holomorphic-differential). Zeros give cone points, not punctures. Its infimal length in a [homotopy class](algebraic-topology.md#homotopy-class) need not determine the hyperbolic length of that class.

###### Area of a quadratic differential

↑ **Parent:** [Flat metric of a quadratic differential](#flat-metric-of-a-quadratic-differential)

The area of the [flat metric of a quadratic differential](#flat-metric-of-a-quadratic-differential) is $\int_X|q|$. Multiplying $q$ by a scalar $a$ multiplies this area by $|a|$ and lengths by $|a|^{1/2}$. It is preserved by the [SL2R action on differentials](complex-analysis.md#sl2r-action-on-differentials).

###### Half-translation surface

↑ **Parent:** [Quadratic differential](#quadratic-differential)

A surface with local Euclidean charts whose changes of coordinate are $w\mapsto\pm w+b$, outside finitely many cone points. A nonzero [holomorphic quadratic differential](#holomorphic-quadratic-differential) defines such a surface; a zero of order $m$ has [cone angle](differential-geometry.md#cone-angle) $(m+2)\pi$.

###### Holomorphic quadratic differential

↑ **Parent:** [Quadratic differential](#quadratic-differential)

A [quadratic differential](#quadratic-differential) with [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) local coefficients. If it is nonzero, its zeros have total order $4g-4$ on a [compact](topology.md#compact-space) [genus](topology.md#genus-of-a-surface)-$g$ [Riemann surface](complex-analysis.md#riemann-surfaces). Away from its zeros, a nonzero differential has [flat coordinates](#natural-coordinate-of-a-holomorphic-differential) whose changes of coordinate have the form $w\mapsto\pm w+c$.

###### Holomorphic differential form

↑ **Parent:** [Canonical bundle](#canonical-bundle)

On a [Riemann surface](complex-analysis.md#riemann-surfaces), a holomorphic differential form is a holomorphic section of the [canonical bundle](#canonical-bundle). In a local complex coordinate $z$ it has the form $f(z)\,dz$ with $f$ holomorphic.

###### Order of a zero of a differential

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

If a local [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) $r$-differential is $z^m u(z)\,dz^r$, where $u(0)\ne0$, its [zero order](#order-of-a-zero-of-a-differential) is $m$. The order is unchanged by a [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) coordinate change with nonzero [derivative](calculus.md#derivative). For a [holomorphic one-form](#holomorphic-one-form) the [cone angle](differential-geometry.md#cone-angle) is $2\pi(m+1)$, and for a [holomorphic quadratic differential](#holomorphic-quadratic-differential) it is $(m+2)\pi$.

###### Natural coordinate of a holomorphic differential

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

For a nonvanishing local $m$-differential $\phi(z)\,dz^m$, choose $w=\int\phi^{1/m}\,dz$. Then the differential is $dw^m$. Different root choices give $w\mapsto\zeta w+b$, $\zeta^m=1$. For $m=1,2$ the permitted linear parts are translations or signs, producing [translation surfaces](complex-analysis.md#translation-surface) and [half-translation surfaces](#half-translation-surface).

###### Holomorphic one-form

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

A section $\omega$ of the [canonical bundle](#canonical-bundle) of a [Riemann surface](complex-analysis.md#riemann-surfaces), locally $\omega=\phi(z)\,dz$ with [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) $\phi$. A nonzero form on a [compact](topology.md#compact-space) [genus](topology.md#genus-of-a-surface)-$g$ surface has total [zero order](#order-of-a-zero-of-a-differential) $2g-2$. Its integral supplies [flat coordinates](#natural-coordinate-of-a-holomorphic-differential) away from zeros.

###### Stratum of holomorphic one-forms

↑ **Parent:** [Holomorphic one-form](#holomorphic-one-form)

The locus of nonzero [holomorphic one-forms](#holomorphic-one-form) with a fixed list of zero multiplicities $k_1,\ldots,k_r$, summing to $2g-2$. The [SL2R action on differentials](complex-analysis.md#sl2r-action-on-differentials) preserves this list. For example $\mathcal H(2)$ and $\mathcal H(1,1)$ are distinct [genus](topology.md#genus-of-a-surface)-two strata.

###### Holomorphic forms on a compact complex surface are closed

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

On a compact complex surface, the claim also holds without a Kähler metric. For a holomorphic one-form $\alpha$, let $\beta=d\alpha$. It is a closed holomorphic two-form, and the [Stokes theorem](calculus.md#stokes-theorem) gives $\int\beta\wedge\bar\beta=\int d(\alpha\wedge\bar\beta)=0$. Positivity of $\beta\wedge\bar\beta$ forces $\beta=0$. Functions are constant on each connected component, and holomorphic two-forms are closed by dimension.

###### Betti and Hodge bounds for compact complex surfaces

↑ **Parent:** [Holomorphic forms on a compact complex surface are closed](#holomorphic-forms-on-a-compact-complex-surface-are-closed)

Closed [holomorphic one-forms](#holomorphic-one-form) inject into [de Rham cohomology](differential-form.md#de-rham-cohomology): an exact one would have a global holomorphic primitive and hence vanish. If a holomorphic class equals an antiholomorphic class, their difference is $df$, and $\partial\bar\partial f=0$; compact pluriharmonic rigidity makes both forms vanish. Their direct sum gives the lower bound. The [sheaf of closed holomorphic one-forms](#sheaf-of-closed-holomorphic-one-forms) exact sequence gives $0\to H^0(\Omega^1)\to H^1(\mathbb C)\to H^1(\mathcal O)$, yielding the upper bound and $h^{1,0}\leq h^{0,1}$. These inequalities do not require a [Kähler manifold](#kahler-manifold).

<h6 id="holomorphic-forms-on-a-compact-kahler-manifold-are-closed">Holomorphic forms on a compact Kähler manifold are closed</h6>

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

A holomorphic $(p,0)$ form is annihilated by $\bar\partial$ and, by bidegree, by $\bar\partial^*$. The [Kähler Laplacian identity](#kahler-laplacian-identity) makes it harmonic for $d$, hence $d$-closed on a compact [Kähler manifold](#kahler-manifold).

###### Holomorphic de Rham complex

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

This complex has the sheaves $\Omega_M^p$ of [holomorphic differential forms](#holomorphic-differential-form) and differential $\partial$. By the [holomorphic Poincaré lemma](#holomorphic-poincare-lemma), it resolves the complex [constant sheaf](algebraic-geometry.md#constant-sheaf).

###### Sheaf of holomorphic differential forms

↑ **Parent:** [Holomorphic de Rham complex](#holomorphic-de-rham-complex)

On a [complex manifold](#complex-manifold), $\Omega_X^p$ is the [sheaf](algebraic-geometry.md#sheaf-mathematics) of holomorphic degree-$p$ forms. It is the kernel of the [Dolbeault operator](#dolbeault-operator) on $\mathcal A^{p,0}$. The [Dolbeault theorem](#dolbeault-theorem) computes its [sheaf cohomology](ringed-space.md#sheaf-cohomology) using smooth forms.

###### Holomorphic p-form on a complex manifold

↑ **Parent:** [Sheaf of holomorphic differential forms](#sheaf-of-holomorphic-differential-forms)

A [differential form of type (p, q)](#differential-form-of-type-p-q) of type $(p,0)$ is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) when its local coefficients in [holomorphic coordinates](#holomorphic-coordinate) are [holomorphic functions](complex-analysis.md#holomorphic-function), equivalently $\bar\partial\alpha=0$. It need not be $d$-closed on every [complex manifold](#complex-manifold). Top-degree [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) forms are closed by bidegree. On a [compact](topology.md#compact-space) [complex surface](#complex-surface), [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) forms of all degrees are closed, even without a [Kähler metric](#kahler-metric).

###### Nonzero holomorphic top forms are not exact

↑ **Parent:** [Holomorphic p-form on a complex manifold](#holomorphic-p-form-on-a-complex-manifold)

On a [compact](topology.md#compact-space) [complex manifold](#complex-manifold) of complex dimension $n$, a [holomorphic p-form on a complex manifold](#holomorphic-p-form-on-a-complex-manifold) of degree $n$ is $d$-closed. The form $i^{n^2}\alpha\wedge\bar\alpha$ is a nonnegative volume density, positive wherever $\alpha\ne0$: in [holomorphic coordinates](#holomorphic-coordinate) it equals $2^n|f|^2dx_1\wedge dy_1\wedge\cdots\wedge dx_n\wedge dy_n$ for $\alpha=f\,dz_1\wedge\cdots\wedge dz_n$. If $\alpha=d\beta$, its integral would vanish by the [Stokes theorem](calculus.md#stokes-theorem), contradicting this positivity. No [Kähler metric](#kahler-metric) is needed.

###### Sheaf of closed holomorphic one-forms

↑ **Parent:** [Holomorphic de Rham complex](#holomorphic-de-rham-complex)

The sheaf is $\mathcal Z_M^1=\ker(\partial:\Omega_M^1\to\Omega_M^2)$. The [holomorphic Poincaré lemma](#holomorphic-poincare-lemma) gives $0\to\underline{\mathbb C}\to\mathcal O_M\xrightarrow{\partial}\mathcal Z_M^1\to0$. On a compact complex surface its [long exact sequence in sheaf cohomology](ringed-space.md#long-exact-sequence-in-sheaf-cohomology) yields $0\to H^0(M,\Omega_M^1)\to H^1(M,\mathbb C)\to H^1(M,\mathcal O_M)$.

<h6 id="holomorphic-poincare-lemma">Holomorphic Poincaré lemma</h6>

↑ **Parent:** [Holomorphic de Rham complex](#holomorphic-de-rham-complex)

On a star-shaped holomorphic coordinate neighbourhood, a closed [holomorphic differential form](#holomorphic-differential-form) of positive degree has a holomorphic primitive. Radial integration gives the homotopy operator. This proves exactness of the [holomorphic de Rham complex](#holomorphic-de-rham-complex) on stalks.

###### Coordinate-integral primitive on a polydisc

↑ **Parent:** [Holomorphic Poincaré lemma](#holomorphic-poincare-lemma)

For a closed [holomorphic one-form](#holomorphic-one-form) $\sum b_kdz_k$ on a polydisc, the displayed coordinate-path integral is a [holomorphic function](complex-analysis.md#holomorphic-function). Differentiating in $z_j$ gives the $k=j$ endpoint term; for $k>j$ use $\partial_jb_k=\partial_kb_j$ and integrate that derivative. The resulting sum telescopes to $b_j(z)$. Thus $\partial F=\sum b_kdz_k$, giving an explicit degree-one proof of the [holomorphic Poincaré lemma](#holomorphic-poincare-lemma).

###### Holomorphic differentials on a smooth plane curve

↑ **Parent:** [Holomorphic differential form](#holomorphic-differential-form)

If $f(x,y)=0$ has a smooth projective completion of degree $d$ and $f_y\ne0$, then its holomorphic differentials have basis

$$
x^iy^j\frac{dx}{f_y},
\qquad i,j\geq0,\quad i+j\leq d-3.
$$

The equality $f_xdx+f_ydy=0$ gives the equivalent expressions $-x^iy^jdy/f_x$.

###### Adjunction formula

↑ **Parent:** [Canonical bundle](#canonical-bundle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adjunction_formula)

For a smooth hypersurface $X$ in a complex manifold $Y$,

$$
K_X\cong(K_Y\otimes\mathcal O_Y(X))|_X.
$$

###### Smooth rational-curve self-intersection on a projective hypersurface

↑ **Parent:** [Adjunction formula](#adjunction-formula)

For a degree-$d$ smooth surface $X\subset\mathbb P^3$ and a smooth rational curve $C$ of degree $a$, the [canonical bundle](#canonical-bundle) is $K_X=\mathcal O_X(d-4)$. The [adjunction formula](#adjunction-formula) gives $(K_X+C)\cdot C=-2$, hence $C^2=-2-(d-4)a$. In particular a line has self-intersection $2-d$.

###### Canonical bundle of a regular projective complete intersection

↑ **Parent:** [Adjunction formula](#adjunction-formula)

For regular homogeneous equations of degrees $d_1,\ldots,d_r$ in $\mathbb P^n$, the [normal bundle of a regular zero locus](#normal-bundle-of-a-regular-zero-locus) is $\bigoplus_i\mathcal O(d_i)|_V$. The [Euler sequence](algebraic-geometry.md#euler-sequence) gives $K_{\mathbb P^n}=\mathcal O(-n-1)$, hence $K_V=\mathcal O(\sum_i d_i-n-1)|_V$. Equations with unreduced multiplicities do not have this conclusion for the underlying reduced submanifold.

###### Adjunction for a smooth submanifold

↑ **Parent:** [Adjunction formula](#adjunction-formula)

For a smooth complex submanifold $V\subset M$, the tangent exact sequence gives $\det TM|_V=\det TV\otimes\det N_V$. Dualizing yields $K_V=K_M|_V\otimes\det N_V$. This form of [adjunction formula](#adjunction-formula) applies in any codimension.

###### First Chern class

↑ **Parent:** [Complex manifold](#complex-manifold)

The first Chern class classifies complex line bundles topologically. For a Hermitian holomorphic line bundle with Chern curvature $F_\nabla$, Chern-Weil theory gives $c_1(E)=[iF_\nabla/(2\pi)]$.

###### Symplectic canonical class

↑ **Parent:** [First Chern class](#first-chern-class)

The symplectic canonical class is the negative [First Chern class](#first-chern-class) of the tangent bundle for a [compatible almost complex structure](#compatible-almost-complex-structure). The [contractibility of compatible almost complex structures](#contractibility-of-compatible-almost-complex-structures) makes it independent of that choice. It is the class appearing in the [symplectic adjunction formula](symplectic-geometry.md#symplectic-adjunction-formula).

<h6 id="cech-de-rham-curvature-descent">Čech-de Rham curvature descent</h6>

↑ **Parent:** [First Chern class](#first-chern-class)

For line-bundle transition functions $g_{ij}=e^{2\pi i f_{ij}}$, the integer cocycle is $c=\delta f$. Connection forms satisfy $A_j-A_i=2\pi i\,df_{ij}$. Set $B=-A/(2\pi i)$ and $F=i\Theta/(2\pi)$. In the Čech-de Rham total complex, $F-c=D_{\rm tot}(B-f)$, so the normalized [vector-bundle curvature](fiber-bundle.md#curvature-form) represents the image of the integral [First Chern class](#first-chern-class). Curvature cannot detect integral torsion.

###### First Chern class of a tensor product of complex line bundles

↑ **Parent:** [First Chern class](#first-chern-class)

The [First Chern class](#first-chern-class) turns the [tensor product of vector bundles](fiber-bundle.md#tensor-product-of-vector-bundles) of [complex line bundles](fiber-bundle.md#complex-line-bundle) into addition in integral [cohomology](cohomology.md). This follows by computing the universal [complex line bundle](fiber-bundle.md#complex-line-bundle) on the product of two [Complex projective spaces](algebraic-topology.md#complex-projective-space) and restricting to each factor. The proof retains [torsion elements](group-theory.md#torsion-element), which differential forms alone cannot detect.

###### Chern connection

↑ **Parent:** [First Chern class](#first-chern-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chern_connection)

The Chern connection is the unique connection on a Hermitian holomorphic bundle compatible with both its metric and holomorphic structure. Its curvature has type $(1,1)$.

<h6 id="torsion-free-chern-tangent-connection-characterizes-a-kahler-metric">Torsion-free Chern tangent connection characterizes a Kähler metric</h6>

↑ **Parent:** [Chern connection](#chern-connection)

For a [Hermitian metric](#hermitian-metric-on-a-holomorphic-vector-bundle) on a [complex manifold](#complex-manifold), the [Chern connection](#chern-connection) on its [holomorphic tangent bundle](#holomorphic-tangent-bundle) corresponds to a real metric-compatible connection preserving the [almost complex structure](#almost-complex-manifold). Its mixed torsion vanishes, and in holomorphic coordinates its remaining coefficients are $\Gamma^k_{ij}=h^{k\bar l}\partial_i h_{j\bar l}$. Symmetry in $i,j$ is equivalent to $\partial\omega=0$; its conjugate gives $d\omega=0$. Thus zero torsion is exactly the [Kähler metric](#kahler-metric) condition, and then uniqueness identifies this connection with the [Levi-Civita connection](general-relativity.md#levi-civita-connection).

###### Chern curvature

↑ **Parent:** [Chern connection](#chern-connection)

The [vector-bundle curvature](fiber-bundle.md#curvature-form) of the unique metric-compatible holomorphic Chern connection is an endomorphism-valued form of type $(1,1)$. It is Dolbeault closed and represents the [curvature Dolbeault class](#curvature-dolbeault-class). Its trace gives normalized first-Chern forms, while its full [endomorphism](algebra.md#endomorphism) action enters the [Lefschetz-Dolbeault curvature commutator](#lefschetz-dolbeault-curvature-commutator).

###### Chern connection component adjoint

↑ **Parent:** [Chern connection](#chern-connection)

For the $(1,0)$ component of a [Chern connection](#chern-connection), $(D'_E)^*=-*_{E^*}D'_{E^*}*_E$, where the middle operator is the corresponding component of the dual [Chern connection](#chern-connection). This is the holomorphic-degree counterpart of the [bundle-valued Dolbeault adjoint](#bundle-valued-dolbeault-adjoint).

###### Dolbeault closedness of Chern curvature

↑ **Parent:** [Chern connection](#chern-connection)

In a [holomorphic local frame](#holomorphic-local-trivialization) the Chern matrix is $A=H^{-1}\partial H$. The identity $\partial A+A\wedge A=0$ gives [vector-bundle curvature](fiber-bundle.md#curvature-form) $\Theta=\bar\partial A$ of type $(1,1)$. Therefore $\bar\partial_{\operatorname{End}E}\Theta=0$, allowing the [vector-bundle curvature](fiber-bundle.md#curvature-form) to represent a bundle-valued Dolbeault class.

###### Trace of Chern curvature

↑ **Parent:** [Chern connection](#chern-connection)

In a [holomorphic local frame](#holomorphic-local-trivialization), a [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle) has matrix $h$. The [trace](linear-algebra.md#matrix-trace) of its [Chern connection](#chern-connection) curvature is $\bar\partial\partial\log\det h$. A frame change multiplies $\det h$ by the squared modulus of a holomorphic unit, whose logarithm has vanishing mixed derivative. For two metrics, the quotient of their determinants is a global positive function, and the trace curvatures differ by the [exterior derivative](differential-form.md#exterior-derivative) of its logarithmic $\partial$-derivative.

###### Projected Chern connection

↑ **Parent:** [Chern connection](#chern-connection)

If $S$ is a holomorphic subbundle of a [Hermitian vector bundle](fiber-bundle.md#hermitian-vector-bundle) $E$, its induced [Chern connection](#chern-connection) is $D_S=\pi_SD_E$ on sections of $S$. [Orthogonal projection](hilbert-space.md#orthogonal-projection) preserves [metric compatibility](fiber-bundle.md#metric-compatibility), and holomorphicity of $S$ preserves the required $(0,1)$ operator. Uniqueness of the [Chern connection](#chern-connection) therefore identifies the projected connection.

###### Second fundamental form of a holomorphic subbundle

↑ **Parent:** [Projected Chern connection](#projected-chern-connection)

For a holomorphic subbundle $S\subset E$ and quotient $Q=E/S$, the second fundamental form is $A(s)=(I-\pi_S)D_Es$. The [Leibniz rule](calculus.md#leibniz-rule) gives $A(fs)=fA(s)$, and holomorphicity of the subbundle makes its $(0,1)$ part vanish. Thus $A\in\mathcal A^{1,0}(\operatorname{Hom}(S,Q))$: the form factor is a [cotangent bundle](symplectic-geometry.md#cotangent-bundle), not a tangent bundle.

###### Curvature formula for a holomorphic subbundle

↑ **Parent:** [Second fundamental form of a holomorphic subbundle](#second-fundamental-form-of-a-holomorphic-subbundle)

In an adapted smooth unitary frame with input-index connection convention, the [Chern connection](#chern-connection) matrix has blocks $(\theta_F,B;-\overline B^t,\theta_Q)$, where the [second fundamental form of a holomorphic subbundle](#second-fundamental-form-of-a-holomorphic-subbundle) $B$ has type $(1,0)$. The [Cartan curvature equation with input indices](fiber-bundle.md#cartan-curvature-equation-with-input-indices) gives the displayed formula. If the ambient curvature is zero, $\Theta_F(X,\overline X)=-B(X)B(X)^\dagger$ is negative semidefinite. Dualizing the [determinant line bundle](fiber-bundle.md#determinant-line-bundle) therefore gives semipositive curvature.

###### Normalized curvature form of a Hermitian holomorphic line bundle

↑ **Parent:** [Chern connection](#chern-connection)

For a [holomorphic local frame](#holomorphic-local-trivialization) $e$ with $h_e=h(e,e)>0$, this form is

$$
\omega_{(L,h)}=-\frac{i}{2\pi}\partial\bar\partial\log h_e.
$$

It is a closed [real (1, 1)-form](#real-1-1-form) representing the [First Chern class](#first-chern-class). A positive [Hermitian metric](#hermitian-metric-on-a-holomorphic-vector-bundle) makes it a [positive real (1, 1)-form](#positive-real-1-1-form). Replacing $h$ by $e^{-u}h$ adds $(i/(2\pi))\partial\bar\partial u$ to the form.

###### Local formula for the Chern connection on a vector bundle

↑ **Parent:** [Chern connection](#chern-connection)

In a [holomorphic local frame](#holomorphic-local-trivialization) of a Hermitian [holomorphic vector bundle](#holomorphic-vector-bundle), let $H$ be the matrix of its [Hermitian metric on a holomorphic vector bundle](#hermitian-metric-on-a-holomorphic-vector-bundle). With the convention $\nabla e=eA$, the [Chern connection](#chern-connection) has

$$
A=H^{-1}\partial H.
$$

The condition $\nabla^{0,1}=\bar\partial_E$ forces $A$ to have type $(1,0)$, while [metric compatibility](fiber-bundle.md#metric-compatibility) forces this formula, proving both existence and uniqueness.

###### Chern connection in a normal holomorphic frame

↑ **Parent:** [Local formula for the Chern connection on a vector bundle](#local-formula-for-the-chern-connection-on-a-vector-bundle)

At any point of a Hermitian [holomorphic vector bundle](#holomorphic-vector-bundle) one may choose a [holomorphic local frame](#holomorphic-local-trivialization) with $H=I$ and $\partial H=0$. First normalize $H$ by a constant frame change, then prescribe a holomorphic matrix's first jet to cancel $H^{-1}\partial H$. The Chern matrix vanishes there. This frame reduces first-order bundle identities at that point to scalar identities.

###### Curvature difference of two Chern connections

↑ **Parent:** [Chern connection](#chern-connection)

Let $D_1$ and $D_2$ be [Chern connections](#chern-connection) on the same [holomorphic vector bundle](#holomorphic-vector-bundle), possibly for different [Hermitian metrics](#hermitian-metric-on-a-holomorphic-vector-bundle), and put $a=D_1-D_2$. Then $a$ has type $(1,0)$ and

$$
F_{D_1}-F_{D_2}=\bar\partial_{\operatorname{End}E}a.
$$

Indeed, the [curvature difference formula](fiber-bundle.md#curvature-difference-formula) has only types $(2,0)$ and $(1,1)$; both Chern curvatures have type $(1,1)$, so the $(2,0)$ part vanishes and the remaining part is $D_2^{0,1}a=\bar\partial_{\operatorname{End}E}a$.

###### Local formula for the Chern connection on a line bundle

↑ **Parent:** [Chern connection](#chern-connection)

Let $e$ be a [holomorphic local frame](#holomorphic-local-trivialization) of a Hermitian holomorphic line bundle and put $h=h(e,e)$. The [Chern connection](#chern-connection) and its curvature are locally

$$
\nabla e=(\partial\log h)e,
\qquad
F_\nabla=\bar\partial\partial\log h=-\partial\bar\partial\log h.
$$

Thus $F_\nabla$ has type $(1,1)$. Because the connection is [unitary](fiber-bundle.md#unitary-connection), $\bar F_\nabla=-F_\nabla$, so $iF_\nabla$ is a [real (1, 1)-form](#real-1-1-form).

<h6 id="ricci-form-of-a-kahler-manifold">Ricci form of a Kähler manifold</h6>

↑ **Parent:** [Chern connection](#chern-connection)

The Ricci form is the real curvature form $iF_\nabla$ of the Chern connection on $T^{1,0}X$. In complex dimension one, $\rho=K\omega=\frac12\operatorname{Scal}\,\omega$.

###### Blowup of a complex manifold at a point

↑ **Parent:** [Complex manifold](#complex-manifold)

The blowup replaces a point of a complex $n$-manifold by the projective space of complex tangent directions $\mathbb{CP}^{n-1}$. A biholomorphism carrying one center to another lifts to a biholomorphism of their blowups.

It is the point-center case of [blowup of an algebraic variety](algebraic-geometry.md#blowing-up-algebraic-geometry), also interpreted analytically.

###### Projective pencil resolved by a point blowup

↑ **Parent:** [Blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point)

The [holomorphic map](complex-analysis.md#holomorphic-map) $[Z_0:Z_1:Z_2]\mapsto[Z_1:Z_2]$ on $\mathbb{CP}^2\setminus\{[1:0:0]\}$ records the line through the missing point and the input point. Its graph closure is the incidence surface $Z_1b=Z_2a$ in $\mathbb{CP}^2\times\mathbb{CP}^1$, the [blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point). Projection to $[a:b]$ extends the pencil holomorphically. On the [exceptional divisor](#exceptional-divisor) it is the identity map on the projective tangent directions.

###### Canonical bundle formula for a point blowup

↑ **Parent:** [Blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point)

For the [blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point) in complex dimension $n$, the differential gives a section of $K_{\widetilde M}\otimes(\phi^*K_M)^{-1}$ whose [divisor on a complex manifold](#divisor-on-a-complex-manifold) is $(n-1)E$. Indeed, a local chart has $x_i=u$ and $x_j=ut_j$ for $j\ne i$, so its [Jacobian determinant](calculus.md#jacobian-determinant) is $\pm u^{n-1}$. The [holomorphic line bundle associated to a divisor](#holomorphic-line-bundle-associated-to-a-divisor) then gives the formula for the [canonical bundle](#canonical-bundle).

###### Anticanonical strict transform under a point blowup

↑ **Parent:** [Canonical bundle formula for a point blowup](#canonical-bundle-formula-for-a-point-blowup)

Let $Y$ be a smooth [complex analytic hypersurface](#complex-analytic-hypersurface) through the blowup centre with $[-Y]\cong K_X$. Its multiplicity at that point is one, so $\sigma^*Y=\widetilde Y+E$. Combining this with the [canonical bundle formula for a point blowup](#canonical-bundle-formula-for-a-point-blowup) gives $[-\widetilde Y]\cong K_{\widetilde X}\otimes[E]^{\otimes(2-n)}$. The [nontrivial powers of the exceptional line bundle of a point blowup](#nontrivial-powers-of-the-exceptional-line-bundle-of-a-point-blowup) prove the equivalence for $n\ge2$. On a [compact](topology.md#compact-space) complex curve the premise cannot hold for an irreducible hypersurface: it is one point, so its negative divisor has degree $-1$, whereas the [canonical bundle](#canonical-bundle) has even degree $2g-2$.

###### Exceptional divisor

↑ **Parent:** [Blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exceptional_divisor)

The exceptional divisor of the [blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point) $p$ is the fiber over $p$. In complex dimension $n$ it is naturally the projective space $\mathbb P(T_pX)\cong\mathbb{CP}^{n-1}$ of tangent directions at the center.

###### Nontrivial powers of the exceptional line bundle of a point blowup

↑ **Parent:** [Exceptional divisor](#exceptional-divisor)

For the [blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point) in dimension $n\ge2$, the [exceptional divisor](#exceptional-divisor) is $\mathbb{CP}^{n-1}$ and $[E]|_E=\mathcal O_E(-1)$. The local blowup is the total space of the tautological [line bundle](ringed-space.md#line-bundle), so its zero section has that [normal bundle](algebraic-geometry.md#normal-bundle). Restricting a power to a [projective line](finite-group-theory.md#projective-line) inside $E$ gives degree $-r$; a trivial bundle has degree zero. This proves that no nonzero power of $[E]$ is trivial, without assuming global projectivity of the original manifold.

###### Strict transform

↑ **Parent:** [Blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strict_transform)

The strict transform of a subvariety $Y$ under a blowup $\sigma:\widetilde X\to X$ is the closure of $\sigma^{-1}(Y\setminus Z)$, where $Z$ is the center. Its total transform also contains the [exceptional divisor](#exceptional-divisor) with the multiplicity with which $Y$ passes through $Z$.

###### Pencil of plane cubics

↑ **Parent:** [Blowup of a complex manifold at a point](#blowup-of-a-complex-manifold-at-a-point)

A pencil generated by cubic forms $F_0,F_1$ is the one-parameter family $sF_0+tF_1=0$ indexed by $[s:t]\in\mathbb{CP}^1$. A general pair has nine transverse base points.

###### Rational elliptic surface

↑ **Parent:** [Pencil of plane cubics](#pencil-of-plane-cubics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_elliptic_surface)

Blowing up the nine base points of a general [pencil of plane cubics](#pencil-of-plane-cubics) produces the rational elliptic surface

$$
E(1)=\{([z],[s:t])\in\operatorname{Bl}_B\mathbb{CP}^2\times\mathbb{CP}^1:sF_0(z)+tF_1(z)=0\}.
$$

###### Elliptic fibration of the rational elliptic surface

↑ **Parent:** [Rational elliptic surface](#rational-elliptic-surface)

Projection to $[s:t]$ gives an elliptic fibration with connected cubic fibers. Each of the nine [exceptional divisors](#exceptional-divisor) maps isomorphically to $\mathbb{CP}^1$ and is therefore a holomorphic section.

###### Canonical class of the rational elliptic surface

↑ **Parent:** [Elliptic fibration of the rational elliptic surface](#elliptic-fibration-of-the-rational-elliptic-surface)

Writing $H$ for the pullback of a line and $E_1,\ldots,E_9$ for the exceptional classes, a fiber has class $F=3H-\sum_iE_i$, while the blowup formula gives

$$
K_{E(1)}=-3H+\sum_iE_i=-F.
$$

###### Genus formula for a multisection of the rational elliptic surface

↑ **Parent:** [Canonical class of the rational elliptic surface](#canonical-class-of-the-rational-elliptic-surface)

If a smooth connected complex curve $C\subset E(1)$ satisfies $C^2=k$ and has degree $d=C\cdot F$ over the base, the [adjunction formula](#adjunction-formula) gives

$$
2g(C)-2=C^2+K_{E(1)}\cdot C=k-d,
\qquad
g(C)=1+\frac{k-d}{2}.
$$

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Kähler potential (complex geometry)](#kahler-potential-complex-geometry)
