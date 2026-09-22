<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Count scalar additions, subtractions, multiplications and divisions for the specific [triangle-triangle intersection algorithm](../../../../../../triangle-triangle-intersection-algorithm.md) above; comparisons and index selection are separate. Computing one plane [normal vector](../../../../../../normal-vector.md) uses two vector differences, costing six subtractions, and one [cross product](../../../../../../cross-product.md), costing six multiplications and three subtractions. The three vertex-to-plane evaluations use nine further coordinate subtractions and three [dot products](../../../../../../dot-product.md), each with three multiplications and two additions. The first rejection test therefore costs

$$
\boxed{6+9+9+3(5)=39\text{ arithmetic operations}.}
$$

For randomly located [triangles](../../../../../../triangle.md) of characteristic size $a$ in a box of size $H\gg a$, a second [triangle](../../../../../../triangle.md) straddles the first triangle's plane only when its position is in a slab of relative thickness $O(a/H)$. Consequently the first plane test rejects almost every pair: the expected arithmetic count for this implementation is $39+O(a/H)$, with the constant in the remainder determined by the subsequent branches. This is an average count, rather than the assertion that every input needs 39 operations.

For a generic surviving noncoplanar pair, the symmetric plane test costs another 39 operations, the [cross product](../../../../../../cross-product.md) $N_A\times N_B$ costs nine, and each of the four slice endpoints needs five scalar operations in the selected coordinate: one subtraction and division for the interpolation fraction, then one subtraction, multiplication and addition for the coordinate. Thus this branch uses

$$
\boxed{39+39+9+4(5)=107\text{ operations}.}
$$

A fully executed coplanar test can use six planar edge directions. Each needs two subtractions to form its perpendicular and six two-dimensional [dot products](../../../../../../dot-product.md), costing $2+6(3)=20$ operations. Including both plane tests and the parallelism [cross product](../../../../../../cross-product.md) gives an upper count $78+9+120=207$ before any early exit. Contact and degeneracy can shorten or change these counts. Precomputed [normal vectors](../../../../../../normal-vector.md) or a preliminary [axis-aligned bounding box](../../../../../../axis-aligned-bounding-box.md) test also change the answer: the latter uses only comparisons after its coordinate extrema are available. **The relevant small-triangle average is 39 operations for the specified plane-first implementation; a generic complete test uses 107.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
