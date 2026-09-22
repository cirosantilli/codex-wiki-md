<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An error of order $\epsilon$ in a squared [singular value](../../../../../singular-value.md) can become an error of order $\sqrt\epsilon$ after taking its square root. To keep $A$ nonsingular as required, take $0<\epsilon<1/2$ and

$$
A=\operatorname{diag}(1,\epsilon),\qquad
\widehat V=I_2,\qquad
\widehat\Sigma=\operatorname{diag}(1,\sqrt{\epsilon^2+\epsilon}).
$$

Then $\|A\|_2=1$, and the computed [eigendecomposition](../../../../../spectral-decomposition.md) has exactly the permitted [backward error](../../../../../backward-error.md):

$$
\|A^TA-\widehat V\widehat\Sigma^2\widehat V^T\|_2
=\|\operatorname{diag}(0,-\epsilon)\|_2=\epsilon.
$$

Nevertheless the second computed [singular value](../../../../../singular-value.md) has error

$$
\sqrt{\epsilon^2+\epsilon}-\epsilon
=\sqrt\epsilon\bigl(\sqrt{1+\epsilon}-\sqrt\epsilon\bigr)
\sim\sqrt\epsilon.
$$

By the [singular value perturbation bound](../../../../../singular-value-perturbation-bound.md), every product with these computed [singular values](../../../../../singular-value.md) and exactly [orthonormal](../../../../../orthonormal-set.md) outer factors has [spectral norm](../../../../../matrix-2-norm.md) error at least this large. In particular, even the favorable choice $\widehat U=I_2$ gives

$$
\boxed{\|A-\widehat U\widehat\Sigma\widehat V^T\|_2
=\sqrt{\epsilon^2+\epsilon}-\epsilon\sim\sqrt\epsilon},
$$

which has no uniform $O(\epsilon)$ bound in [big O notation](../../../../../big-o-notation.md). Therefore [backward stability](../../../../../backward-stability.md) for the [eigendecomposition](../../../../../spectral-decomposition.md) of the [Gram matrix](../../../../../gram-matrix.md) does not imply [backward stability](../../../../../backward-stability.md) for the [singular value decomposition](../../../../../singular-value-decomposition.md).

There is a related loss of [orthonormality](../../../../../orthonormal-set.md) in the raw formula: evaluating $A\widehat V\widehat\Sigma^{-1}$ exactly for these perturbed factors gives $\operatorname{diag}(1,\epsilon/\sqrt{\epsilon^2+\epsilon})$, whose second column has length tending to zero. Its product with $\widehat\Sigma\widehat V^T$ equals $A$, but its diagonal factors are consequently not a [singular value decomposition](../../../../../singular-value-decomposition.md). The paper's idealized [orthonormality](../../../../../orthonormal-set.md) assumption lets us isolate the unavoidable [singular value](../../../../../singular-value.md) error even if this additional problem is repaired.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
