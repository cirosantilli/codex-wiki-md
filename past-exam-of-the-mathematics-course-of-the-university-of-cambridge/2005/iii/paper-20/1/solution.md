<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The central problem of [spectral geometry](../../../../../spectral-geometry.md) is how much of a [Riemannian metric](../../../../../riemannian-metric.md) is determined by the [eigenvalues](../../../../../eigenvalue.md), with [multiplicities](../../../../../multiplicity-mathematics.md), of its [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md). For a membrane with fixed [boundary](../../../../../boundary-of-a-set.md), the squared vibration frequencies are proportional to the [Dirichlet eigenvalues](../../../../../dirichlet-eigenvalue.md). Kac's [1966 paper](https://www.math.ucdavis.edu/~saito/courses/ACHA.READ.F03/kac-drum.pdf) brought this inverse problem into focus: the full sequence of frequencies might encode a domain's shape, but recovering a few geometric quantities is much weaker than recovering an [isometry](../../../../../isometry.md) class.

The first major line of development extracts geometric information from spectral sums. On a smooth [closed](../../../../../closed-set.md) $d$-dimensional [manifold](../../../../../topological-manifold.md), the [heat trace](../../../../../heat-trace.md) has the short-time expansion

$$
Z(t)=\sum_j e^{-t\lambda_j}\sim(4\pi t)^{-d/2}\left(\operatorname{Vol}(M)+\frac t6\int_M R\,dV+\cdots\right),
$$

where $\lambda_j$ are the nonnegative [eigenvalues](../../../../../eigenvalue.md) of $P=-\Delta$ and $R$ is [scalar curvature](../../../../../scalar-curvature.md). The coefficients are [heat invariants](../../../../../heat-invariants.md), formed by integrating local curvature expressions. They recover dimension, [Riemannian volume](../../../../../riemannian-volume.md) and total [scalar curvature](../../../../../scalar-curvature.md). For smooth planar domains with the [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md),

$$
Z(t)=\frac{\operatorname{Area}(\Omega)}{4\pi t}-\frac{\operatorname{Length}(\partial\Omega)}{8\sqrt{\pi t}}+O(1).
$$

Thus [area](../../../../../surface-area.md) and [boundary](../../../../../boundary-of-a-set.md) length are audible. The constant term also contains topological information through [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), with corner corrections when the [boundary](../../../../../boundary-of-a-set.md) is polygonal. The [Weyl law](../../../../../weyl-law.md) is the corresponding leading eigenvalue-counting result. Neither the leading term nor the whole list of local heat coefficients automatically reconstructs global geometry.

In the 1970s, the [wave trace](../../../../../wave-trace.md) introduced a complementary link with global [closed geodesics](../../../../../closed-geodesic.md). The [distribution](../../../../../distribution-mathematical-analysis.md)

$$
W(t)=\sum_j e^{it\sqrt{\lambda_j}}
$$

is spectral, while its singularities are governed by periodic [geodesic](../../../../../geodesic.md) motion. The [1975 Duistermaat-Guillemin work](https://link.springer.com/article/10.1007/BF01405172) made this relationship precise. Its [trace](../../../../../matrix-trace.md) formula places singularities at [geodesic](../../../../../geodesic.md) lengths and computes their coefficients under suitable clean or nondegenerate hypotheses. When a coefficient is nonzero, the corresponding length is audible. Possible cancellation must be addressed before identifying the entire [length spectrum](../../../../../length-spectrum.md) with the singular support. This approach led to [spectral rigidity](../../../../../spectral-rigidity.md) questions, rather than just the recovery of integral curvature quantities.

The second main line constructs counterexamples to metric determination. A precedent was the [1964 flat-torus example](https://doi.org/10.1073/pnas.51.4.542): different sixteen-dimensional [Euclidean lattices](../../../../../euclidean-lattice.md) could give the same [Laplacian eigenvalues](../../../../../laplacian-eigenvalue.md). Subsequent lattice constructions lowered the dimension; [Conway and Sloane's 1992 work](https://academic.oup.com/imrn/article-abstract/1992/4/93/660616) exhibited four-dimensional [Euclidean lattices](../../../../../euclidean-lattice.md) with matching [lattice theta series](../../../../../theta-series-of-a-euclidean-lattice.md). For a [flat torus](../../../../../flat-torus.md) $\mathbb R^d/\Lambda$, the spectrum is the multiset $4\pi^2|\xi|^2$ for $\xi\in\Lambda^*$, so equality of [lattice theta series](../../../../../theta-series-of-a-euclidean-lattice.md) of the [dual lattices](../../../../../dual-lattice.md) gives [isospectrality](../../../../../isospectral-manifolds.md) even when the [Euclidean lattices](../../../../../euclidean-lattice.md) are not related by an [orthogonal transformation](../../../../../orthogonal-transformation.md).

A systematic geometric construction arrived with the [Sunada theorem in 1985](https://annals.math.princeton.edu/1985/121-1/p04). For a common Riemannian cover with finite [isometry](../../../../../isometry.md) [group](../../../../../group-split.md) $T$, [almost conjugate subgroups](../../../../../gassmann-equivalence.md) have the same number of invariant vectors in each [Laplacian](../../../../../laplacian.md) [eigenspace](../../../../../eigenspace.md). Their freely acting quotients are therefore [isospectral manifolds](../../../../../isospectral-manifolds.md). This reduces an analytic equality to a finite-group representation identity. It produces many examples on surfaces and in higher dimensions, but nonconjugacy of the [subgroups](../../../../../subgroup.md) must be supplemented by an argument excluding extra quotient [isometries](../../../../../isometry.md). [Transplantation theorem](../../../../../transplantation-theorem.md) provides an explicit version: piecewise [eigenfunctions](../../../../../eigenfunction.md) are recombined by a fixed invertible linear transformation that respects the gluing and [boundary conditions](../../../../../boundary-condition.md).

The planar problem itself was answered negatively by [Gordon, Webb and Wolpert in 1992](https://arxiv.org/abs/math/9207215): noncongruent simply connected polygonal plane domains have equal Dirichlet spectra. This is stronger than counterexamples among abstract [manifolds](../../../../../topological-manifold.md) or [flat tori](../../../../../flat-torus.md), since these are genuine two-dimensional planar membranes. It does not settle every restricted version, such as asking for two domains within a specified smooth or convex class.

By the 1990s, [isospectrality](../../../../../isospectral-manifolds.md) was also known to coexist with continuous metric variation and changes in local geometry. For example, [a 1997 construction](https://arxiv.org/abs/dg-ga/9710004) gives continuous isospectral families on products of spheres and [tori](../../../../../torus.md) whose members need not be locally [isometric](../../../../../isometry.md); in some examples the maximum [scalar curvature](../../../../../scalar-curvature.md) changes. Conversely, rigidity and [compactness](../../../../../compact-space.md) results show that an isospectral class is not unrestricted. The [1988 surface compactness theorem](https://doi.org/10.1016/0022-1236(88)90071-7) makes fixed-spectrum sets of [closed](../../../../../closed-set.md) orientable surface metrics [compact](../../../../../compact-space.md) modulo [diffeomorphisms](../../../../../diffeomorphism.md). [Compactness](../../../../../compact-space.md) does not mean there is only one metric, or even finitely many metrics. By 2005, the subject therefore combined local [heat invariants](../../../../../heat-invariants.md), global [geodesic](../../../../../geodesic.md) information, group-theoretic constructions, explicit [transplantation](../../../../../transplantation-theorem.md) and geometric rigidity. **The spectrum determines substantial geometry, while generally failing to determine the full metric.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
