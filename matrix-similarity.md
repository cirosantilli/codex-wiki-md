# Matrix similarity

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_similarity)

Two [square matrices](square-matrix.md) $A,B$ over the same [field](field.md) are similar if $B=S^{-1}AS$ for an [invertible matrix](invertible-matrix.md) $S$. They can describe one [linear operator](linear-operator.md) using two different [ordered bases](ordered-basis.md), with the same [basis](basis.md) used for input and output in each description. Fix the convention $x=Sy$: $x$ is the old [coordinate vector](coordinate-vector.md), $y$ the new [coordinate vector](coordinate-vector.md), and the columns of $S$ are the new [basis vectors](basis-vector.md) in old [coordinates](coordinate-linear-algebra.md). This is the convention of the [change-of-basis matrix](change-of-basis-matrix.md).[§3D, Theorem 3.84, printed p. 93: change-of-basis formula; the matrix there converts in the opposite direction to our $S$](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

For a concrete [linear operator](linear-operator.md) on the physical plane, let $T$ double horizontal components and multiply vertical components by five. In the old [standard basis](standard-basis.md) $\mathcal E=(e_1,e_2)$, its [matrix of a linear map](matrix-representation-of-a-linear-map.md) is $A=\operatorname{diag}(2,5)$. Choose the new [ordered basis](ordered-basis.md) $\mathcal F=(b_1,b_2)$ with $b_1=e_1$, $b_2=e_1+e_2$. Then

$$
S=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad
S^{-1}=\begin{pmatrix}1&-1\\0&1\end{pmatrix},\qquad
B=S^{-1}AS=\begin{pmatrix}2&-3\\0&5\end{pmatrix}.
$$

The second column of $B$ says $T(b_2)=-3b_1+5b_2=2e_1+5e_2$. Its off-diagonal entry records how the chosen [basis vectors](basis-vector.md) describe the output; the physical [linear operator](linear-operator.md) still stretches along the old horizontal and vertical directions.

Take the physical [vector](vector.md) $p=2e_1+e_2=b_1+b_2$. Its two [coordinate vectors](coordinate-vector.md), and the two descriptions of $T(p)$, are

$$
x=\begin{pmatrix}2\\1\end{pmatrix},\qquad y=\begin{pmatrix}1\\1\end{pmatrix},\qquad
Ax=\begin{pmatrix}4\\5\end{pmatrix},\qquad By=\begin{pmatrix}-1\\5\end{pmatrix}.
$$

Reconstruction gives $T(p)=4e_1+5e_2=-b_1+5b_2$. The output [coordinate vectors](coordinate-vector.md) differ, but the endpoint in the physical plane is the same.

<a id="image-one-linear-operator-and-the-same-two-physical-vectors-described-in-a-standard-basis-and-an-oblique-basis"></a>
![](matrix-similarity-physical-bases.png)

**[Figure 21](#image-one-linear-operator-and-the-same-two-physical-vectors-described-in-a-standard-basis-and-an-oblique-basis). One linear operator and the same two physical vectors described in a standard basis and an oblique basis**. Both panels use the same physical plane and scale. The blue arrow is $p$, and the orange arrow is $T(p)$. Dotted paths reconstruct them from their respective [basis vectors](basis-vector.md); the right grid follows $b_1=e_1$, $b_2=e_1+e_2$.

This is why [matrix similarity](matrix-similarity.md) is useful: a convenient [basis](basis.md) can simplify calculations without changing the [linear operator](linear-operator.md). A [diagonalizable matrix](diagonalizable-matrix.md) can be replaced by a [diagonal matrix](diagonal-matrix.md), making repeated application a calculation with powers of its [eigenvalues](eigenvalue.md). In the example, $A$ makes the two independent stretch factors visible, while $B$ expresses the same action in directions chosen for another purpose. [Matrix similarity invariants](matrix-similarity-invariants.md) separate properties of the [linear operator](linear-operator.md) from features of its address system.

**Table of contents**

- [Matrix similarity invariants](matrix-similarity-invariants.md)
- [Eigenvectors under similarity](eigenvectors-under-similarity.md)
- [Same eigenvalues do not imply similarity](same-eigenvalues-do-not-imply-similarity.md)
- [Similarity transformation](similarity-transformation.md)
  - [Similarity and the coordinate metric](similarity-and-the-coordinate-metric.md)
  - [Positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md)
  - [Every automorphism of a full matrix algebra is inner](every-automorphism-of-a-full-matrix-algebra-is-inner.md)
- [Transpose similarity](transpose-similarity.md)
- [Real similarity from complex similarity](real-similarity-from-complex-similarity.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Change-of-basis matrix](change-of-basis-matrix.md)
- [Diagonal scaling of Gershgorin discs](diagonal-scaling-of-gershgorin-discs.md)
- [Householder transformation](householder-transformation.md)
- [Invertible anticommuting matrices have even dimension and zero traces](invertible-anticommuting-matrices-have-even-dimension-and-zero-traces.md)
- [Matrix congruence](matrix-congruence.md)
- [Matrix of a bilinear form](matrix-of-a-bilinear-form.md)
- [Matrix similarity](matrix-similarity.md)
- [Matrix similarity invariants](matrix-similarity-invariants.md)
- [Matrix trace](matrix-trace.md)
- [Module isomorphism](module-isomorphism.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/10h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/7b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/8b/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/8b/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-1/8b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/11e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/section-b/7/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/18/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/5/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/5/b/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/6/c/solution.md)
- [Same eigenvalues do not imply similarity](same-eigenvalues-do-not-imply-similarity.md)
- [Similarity and the coordinate metric](similarity-and-the-coordinate-metric.md)
- [Similarity transformation](similarity-transformation.md)
- [Singular value decomposition](singular-value-decomposition.md)
