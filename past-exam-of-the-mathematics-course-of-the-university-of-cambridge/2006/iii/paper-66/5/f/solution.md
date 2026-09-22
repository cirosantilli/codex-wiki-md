<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose coefficients using the local [subdivision matrix](../../../../../../subdivision-matrix.md), not just by copying a pleasant-looking regular stencil. Because the grids alternate, form the matrix $S_n$ for a complete two-step cycle around the valence-$n$ [extraordinary subdivision vertex](../../../../../../extraordinary-subdivision-vertex.md), retaining a large enough neighborhood that it maps into itself. The three local coefficients enter this matrix through the specified vertex and face rules.

First require constant reproduction and commutation with [affine maps](../../../../../../affine-map.md): every target stencil must sum to one, and the valence-four rules must reduce to the regular ones already found. A propagation mask need not itself sum to one. For example, with an old-vertex target rule $V'=a_nV+c_n\sum_{j=1}^nV_j$, normalization requires $a_n+nc_n=1$; a face-centroid target rule separately has corner weights summing to one. If face weights depend on incident valences, impose their sum on each actual face, rather than incorrectly using a propagation-column normalization. Rotational and reflection symmetry around the vertex should preserve an isotropic treatment of its sectors. Nonnegative coefficients are desirable for [convex hull](../../../../../../convex-hull.md) bounds and stability, although they are not by themselves a smoothness proof.

For convergence, seek a simple [eigenvalue](../../../../../../eigenvalue.md) one corresponding to the constant [eigenvector](../../../../../../eigenvector.md), with all remaining [eigenvalues](../../../../../../eigenvalue.md) of modulus below one. For a well-defined tangent plane, seek two independent, semisimple tangent modes with a common positive subdominant [eigenvalue](../../../../../../eigenvalue.md):

$$
1>\lambda_1=\lambda_2=\lambda>\max_{j\geq3}|\lambda_j|.
$$

The angular modes should be the first sine and cosine modes around the ring. On the regular lattice the full two-step tangent scale is $1/2$, which provides a useful consistency check. These requirements suppress persistent unwanted modes and ensure that generic first-order geometry is dominated by a two-dimensional tangent space.

Then check that the [characteristic map of a subdivision surface](../../../../../../characteristic-map-of-a-subdivision-surface.md) built from those tangent [eigenvectors](../../../../../../eigenvector.md) is regular and injective on the punctured neighborhood. **A dominant tangent pair together with a regular, nonfolding characteristic map is the crucial $C^1$ target; eigenvalues alone are insufficient.** This check rules out folds or vanishing tangent area that a spectrum cannot detect. For reasonable curvature behavior, also try to keep second-order modes at or below $\lambda^2$ in modulus, with equality and appropriate mode structure when nonzero finite curvature is desired. Avoid negative or complex modes that produce visible alternating ripples, excessive shrinkage and strongly anisotropic shape response.

These are selection criteria, not a uniquely determined triple of coefficients. The disappearance of extraordinary faces after one step simplifies the subsequent local matrix, but the extraordinary vertex remains and its smoothness still needs these tests. In particular, the regular $C^4$ result cannot simply be assigned to arbitrary valence.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
