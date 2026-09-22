<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

This is [mid-edge subdivision](../../../../../mid-edge-subdivision.md), rather than a vertex-retaining refinement. Use the usual closed two-manifold mesh setting: each edge has two incident facets and each vertex has a cyclic fan. For boundary meshes, a boundary refinement rule has to be specified separately. The relevant generic-position condition excludes collapsed local tangent directions and singular regular patches.

**Topology and the [manifold](../../../../../topological-manifold.md) property.** Regard the abstract mesh as a cell decomposition of a [surface](../../../../../topological-surface.md). Join the edge midpoints in each facet. The inner polygon is the new face associated with that facet; the corner regions around an old vertex assemble into the face associated with that vertex. At an old edge midpoint, the four adjacent corner connections form a cyclic link. Thus every new interior vertex has valence four, every new edge has two incident faces, and the refined cell complex is homeomorphic to the original [surface](../../../../../topological-surface.md). If the original counts are $V,E,F$, the new counts are $E,2E,V+F$, preserving $V-E+F$. The cyclic-link argument, rather than Euler characteristic alone, verifies the local [manifold](../../../../../topological-manifold.md) condition. Convergence and local regularity, justified below, transfer this abstract [surface](../../../../../topological-surface.md) structure to the limit.

**[Convex hull](../../../../../convex-hull.md).** Each newly created point is an average of two previous points. By induction it is a [convex combination](../../../../../convex-combination.md) of original vertices. The same is true of points of any triangulation of the refined facets, and taking limits keeps them in the closed [convex hull](../../../../../convex-hull.md). Hence the entire limit stays in that hull, not necessarily inside the original nonconvex enclosed solid.

**Facet centroids.** Follow the descendant inner face of an original $n$-sided facet, with cyclic vertices $p_i$. Its vertices satisfy $p_i^{(r+1)}=(p_i^{(r)}+p_{i+1}^{(r)})/2$. Summing proves [mid-edge facet centroid invariance](../../../../../mid-edge-facet-centroid-invariance.md):

$$
\frac1n\sum_i p_i^{(r+1)}=\frac1n\sum_i p_i^{(r)}=\overline p.
$$

For a cyclic Fourier mode $e^{2\pi iji/n}$ the multiplier is $(1+e^{2\pi ij/n})/2$, whose modulus is $|\cos(\pi j/n)|<1$ for $j\ne0$. Every mean-zero mode therefore decays, so all descendant face vertices converge to $\overline p$. Consequently **the original vertex [centroid](../../../../../centroid.md) belongs to the limit [surface](../../../../../topological-surface.md)**. No planarity assumption is needed.

**Quadratic triangular pieces.** On a regular quadrilateral mesh, apply two midpoint steps. Each new point combines three old neighboring controls with weights $1/2,1/4,1/4$. For example, around a face with cyclic corners $p_{00},p_{10},p_{11},p_{01}$, the four new points are

$$
\tfrac12p_{00}+\tfrac14(p_{10}+p_{01}),\quad
\tfrac12p_{10}+\tfrac14(p_{00}+p_{11}),\quad
\tfrac12p_{11}+\tfrac14(p_{10}+p_{01}),\quad
\tfrac12p_{01}+\tfrac14(p_{00}+p_{11}).
$$

This is the binary refinement mask obtained by expanding

$$
\frac14(1+z)(1+w)(1+zw)(1+z/w),
$$

with the translation chosen to place the refined grid at quarter offsets. The limit is therefore represented by shifts of the [quadratic four-direction box spline](../../../../../quadratic-four-direction-box-spline.md) with directions $e_1,e_2,e_1+e_2,e_1-e_2$. Projection of a four-cube onto the plane has piecewise total degree $4-2=2$, and its knot grid is triangular. Coordinatewise linear combinations preserve that degree, giving parametric quadratic triangle patches. Around a nonregular center there are infinitely many shrinking rings of such patches; the isolated center is their limit, not generally part of a finite [polynomial](../../../../../polynomial-split.md) patch representation.

**Only finitely many initially possible smoothness exceptions.** Every vertex has valence four after the first step. Only the descendants of original facets and the faces created around original vertices can remain nonquadrilateral. All subsequently created faces around four-valent vertices are quadrilaterals. Thus every point except the limiting centers of those persistent nonquadrilateral faces eventually lies in a regular patch neighborhood. The number of possible exceptional centers is at most $V+F$. For the regular [box spline](../../../../../box-spline.md), any three distinct directions still span the plane, so three directions must be removed to make the remainder nonspanning. The [box spline](../../../../../box-spline.md) [continuity](../../../../../continuous-function.md) criterion gives $C^{3-2}=C^1$ across its triangle boundaries. This proves $C^1$ [continuity](../../../../../continuous-function.md) away from at most those finitely many centers.

**Removing the apparent exceptions.** Center a finite neighborhood of an $n$-sided exceptional face, and analyze a full two-step [subdivision matrix](../../../../../subdivision-matrix.md) so the mesh orientation is restored. Cyclic [Fourier basis](../../../../../fourier-basis.md) modes diagonalize its sector symmetry. The face mode has [eigenvalue](../../../../../eigenvalue.md)

$$
\alpha_j=\frac{1+\cos(2\pi j/n)}2,\qquad
\lambda=\alpha_1=\alpha_{n-1}=\cos^2(\pi/n).
$$

The local ring blocks also contribute [eigenvalues](../../../../../eigenvalue.md) $1/4$ and zero. For $n>3$, the constant mode is the single [eigenvalue](../../../../../eigenvalue.md) one, and the two first-frequency tangent modes dominate all nonconstant remaining modes. Construct their [characteristic map of a subdivision surface](../../../../../characteristic-map-of-a-subdivision-surface.md); its quadratic [derivative](../../../../../derivative.md) pieces must have a nonzero consistently oriented Jacobian, and its fundamental sector must be injective. These checks, not the [eigenvalue](../../../../../eigenvalue.md) ordering alone, give a regular chart and a continuously limiting tangent plane for generic data.

The case $n=3$ needs a separate Jordan analysis: $\lambda=1/4$ is eightfold, so the usual semisimple double-eigenvalue test does not apply. Its first-frequency Jordan chains supply the leading tangent behavior, while the other contributions become relatively negligible. Regularity and injectivity of that generalized characteristic map complete the argument. These concrete spectral and characteristic-map checks are established for this scheme in [Peters and Reif, Sections 3 and Appendix](https://www.cise.ufl.edu/research/SurfLab/pre99-papers/9697.sss.pdf). Thus **the generic limit is geometrically $C^1$ also at the exceptional centers**; compatible local charts need not preserve the original uniform refinement parameterization.

The [manifold](../../../../../topological-manifold.md) statement concerns the abstract limit [surface](../../../../../topological-surface.md) and its regular local parametrizations. It does not, from combinatorics and generic tangent data alone, prove global injectivity of the image in three-dimensional space. A particular model may require an additional global self-intersection test before claiming that its image is an embedded [manifold](../../../../../topological-manifold.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
