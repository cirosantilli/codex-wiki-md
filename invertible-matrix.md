# Invertible matrix

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Invertible_matrix)

An $n$-by-$n$ [square matrix](square-matrix.md) $A$ over a [field](field.md) is invertible when it has a two-sided [matrix inverse](matrix-inverse.md). Equivalently, its [linear map](linear-map.md) $x\mapsto Ax$ is a [bijection](bijection.md): every output comes from exactly one input. For a [square matrix](square-matrix.md), the following conditions are equivalent:

$$
A\text{ is invertible}
\iff\operatorname{rank}A=n
\iff\ker A=\{0\}
\iff\det A\ne0
\iff Ax=b\text{ has exactly one solution for every }b.
$$

Here [matrix rank](matrix-rank.md) $n$ means both [full column rank](full-column-rank.md) and [full row rank](full-row-rank.md). The square hypothesis matters: a rectangular [matrix](matrix.md) can have [full column rank](full-column-rank.md) without reaching every output, or [full row rank](full-row-rank.md) without determining every input.[Strang, MIT 18.06 Lecture 3: multiplication and inverse matrices](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/resources/lecture-3-multiplication-and-inverse-matrices/)

The equivalences explain why invertibility is a question about retaining information. A [trivial kernel](trivial-kernel.md) makes the [linear map](linear-map.md) [injective](injective-function.md); the [rank-nullity theorem](rank-nullity-theorem.md) then gives [matrix rank](matrix-rank.md) $n$, so its columns form a [basis](basis.md) and the [linear map](linear-map.md) is also [surjective](surjective-function.md). Assigning to each output its unique input gives a [linear map](linear-map.md): the preimage of $\alpha b+\beta c$ is $\alpha A^{-1}b+\beta A^{-1}c$. The [determinant](determinant.md) is nonzero precisely when the columns are [linearly independent](linear-independence.md). Thus algebraic solvability and independent directions describe the same phenomenon; over the [real numbers](real-number.md), nonzero [oriented volume](oriented-volume.md) supplies its geometric interpretation.

**Table of contents**

- [Singular matrix](singular-matrix.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (50)

- [Change-of-basis matrix](change-of-basis-matrix.md)
- [Column rank](column-rank.md)
- [Covector transformation under a change of basis](covector-transformation-under-a-change-of-basis.md)
- [Determinant](determinant.md)
- [Diagonal scaling of Gershgorin discs](diagonal-scaling-of-gershgorin-discs.md)
- [Diagonalizable matrix](diagonalizable-matrix.md)
- [Gershgorin circle theorem](gershgorin-circle-theorem.md)
- [Hessian matrix](hessian-matrix.md)
- [LU decomposition](lu-decomposition.md)
- [Matrix congruence](matrix-congruence.md)
- [Matrix determinant lemma](matrix-determinant-lemma.md)
- [Matrix inverse](matrix-inverse.md)
- [Matrix of a bilinear form](matrix-of-a-bilinear-form.md)
- [Matrix trace](matrix-trace.md)
- [Minimal polynomial of an invertible matrix](minimal-polynomial-of-an-invertible-matrix.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
- [Nondegenerate critical point](nondegenerate-critical-point.md)
- [Nondegenerate stationary point of a phase](nondegenerate-stationary-point-of-a-phase.md)
- [Padé identification of a Radau stability function](pade-identification-of-a-radau-stability-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-87/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/2b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-20/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/2b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/7b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2/12g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/7c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/2c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/11g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-115/1/c/solution.md)
- [Pivot element](pivot-element.md)
- [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
- [Row rank](row-rank.md)
- [Sherman–Morrison formula](sherman-morrison-formula.md)
- [Singular matrix](singular-matrix.md)
- [Singular value](singular-value.md)
- [Trivial kernel](trivial-kernel.md)
- [Unique minimizer of a positive-definite quadratic function](unique-minimizer-of-a-positive-definite-quadratic-function.md)
- [Unit triangular matrix](unit-triangular-matrix.md)
- [Zero-pivot failure of tridiagonal elimination](zero-pivot-failure-of-tridiagonal-elimination.md)
