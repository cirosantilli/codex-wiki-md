# Moore-Penrose inverse

↑ **Parent:** [Matrix inverse](matrix-inverse-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moore-Penrose_inverse)

The [Moore-Penrose inverse](moore-penrose-inverse.md) extends the useful part of a [matrix inverse](matrix-inverse-split.md) to rectangular and singular [matrices](matrix.md). A [linear system](system-of-linear-equations.md) $Ax=b$ may have no exact solution, or may have many. The [pseudoinverse](moore-penrose-inverse.md) resolves both ambiguities: $x_*=A^+b$ is the [minimum-norm least-squares solution](minimum-norm-least-squares-solution.md). First minimize the [Euclidean norm](euclidean-norm.md) $\|Ax-b\|_2$; among all [vectors](vector.md) attaining that minimum, choose the one with smallest [Euclidean norm](euclidean-norm.md) $\|x\|_2$. It does not pretend that inconsistent equations can all be satisfied.

For $A\in\mathbb C^{m\times n}$, its [Moore-Penrose inverse](moore-penrose-inverse.md) is the unique $n\times m$ [matrix](matrix.md) satisfying the four [Penrose equations](penrose-equations.md). The [singular value decomposition](singular-value-decomposition.md) gives a direct construction:

$$
A=U\Sigma V^*,
\qquad
\boxed{A^+=V\Sigma^+U^*.}
$$

Here $U,V$ are [unitary matrices](unitary-matrix.md), the star is the [conjugate transpose](conjugate-transpose.md), and $\Sigma^+$ is the $n\times m$ rectangular [diagonal matrix](diagonal-matrix.md) obtained by replacing each nonzero [singular value](singular-value.md) $\sigma_j$ by $1/\sigma_j$ and leaving zeros at zero. Over the [real numbers](real-number.md), use [orthogonal matrices](orthogonal-matrix.md) and [transposes](transpose.md). The [pseudoinverse](moore-penrose-inverse.md) reverses the stretches that can be reversed; it discards output components the original [linear map](linear-map.md) cannot produce and does not invent an input component in its [kernel](kernel-of-a-linear-map-split.md). [Strang, MIT 18.06SC: Left and Right Inverses; Pseudoinverse](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/resources/mit18_06scf11_ses3-8sum/)

The two products have especially clear meanings:

$$
AA^+=P_{\operatorname{ran}A},
\qquad
A^+A=P_{(\ker A)^\perp}.
$$

They are [orthogonal projection matrices](orthogonal-projection-matrix.md): $AA^+$ selects the producible part of an output, while $A^+A$ selects the detectable part of an input. They are generally not [identity matrices](identity-matrix.md). For an [invertible matrix](invertible-matrix.md), both are identities and $A^+=A^{-1}$.

This gives a useful order of operations for [least-squares solutions](least-squares-solution-of-a-linear-inverse-problem.md): project the requested output onto the [column space](column-space.md), then invert the restriction of $A$ from $(\ker A)^\perp$ to its [column space](column-space.md). Adding a [kernel](kernel-of-a-linear-map-split.md) [vector](vector.md) leaves the residual unchanged but increases the squared [Euclidean norm](euclidean-norm.md) by the [Pythagorean theorem in an inner-product space](pythagorean-theorem-in-an-inner-product-space.md), because $A^+b$ is [orthogonal](orthogonal-vectors.md) to that [kernel](kernel-of-a-linear-map-split.md). The [pseudoinverse](moore-penrose-inverse.md) therefore provides one canonical answer without hiding either lost information or irreconcilable data.

The name records a history with several contributors. E. H. Moore gave an earlier generalization in 1920; M. H. Pearl's 1966 paper records that work, Arne Bjerhammar's 1951 rediscovery for maximal-rank rectangular [matrices](matrix.md), and Roger Penrose's independent 1955 treatment. [Pearl, On generalized inverses of matrices (1966), introduction and references 6–9](https://www.cambridge.org/core/journals/mathematical-proceedings-of-the-cambridge-philosophical-society/article/abs/on-generalized-inverses-of-matrices/9CD637F604C76ECD8D03AC029212D56E) Penrose's original paper proves existence and uniqueness from the four [Penrose equations](penrose-equations.md) for arbitrary complex [matrices](matrix.md), including rectangular ones. [Penrose, A generalized inverse for matrices (1955), Theorem 1, pp. 406–408](https://faculty.kfupm.edu.sa/math/jaafarm/lec-notes/Moore-Pinrose.pdf)

**Table of contents**

- [Overdetermined least-squares example](overdetermined-least-squares-example.md)
- [Underdetermined minimum-norm example](underdetermined-minimum-norm-example.md)
- [Small singular values in the Moore-Penrose inverse](small-singular-values-in-the-moore-penrose-inverse.md)
- [Moore--Penrose inverse of a Hilbert-space operator](moore-penrose-inverse-of-a-hilbert-space-operator.md)
- [Penrose equations](penrose-equations.md)
- [Reverse-order law for the Moore--Penrose inverse](reverse-order-law-for-the-moore-penrose-inverse.md)

## ↑ Ancestors (6)

1. [Matrix inverse](matrix-inverse-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Incidence pseudoinverse decomposition](incidence-pseudoinverse-decomposition.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/1/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-225/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-205/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-326/3/c/solution.md)
- [Penrose equations](penrose-equations.md)
- [Rank-deficient ordinary least squares](rank-deficient-ordinary-least-squares.md)
- [Square-root investment-consumption value](square-root-investment-consumption-value.md)
- [Underdetermined minimum-norm example](underdetermined-minimum-norm-example.md)
- [Vanishing-penalty ridge limit](vanishing-penalty-ridge-limit.md)
