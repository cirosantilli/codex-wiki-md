<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $S_+^{n-1}$ be the nonnegative portion of the [unit sphere](../../../../unit-sphere.md) specified in the paper. If $Ax=0$ for some $x\in S_+^{n-1}$, then this nonzero [vector](../../../../vector.md) is an [eigenvector](../../../../eigenvector.md) with [eigenvalue](../../../../eigenvalue.md) zero, which already proves the assertion.

Otherwise $Ax\ne0$ for every $x\in S_+^{n-1}$, and

$$
T(x)=\frac{Ax}{|Ax|}
$$

is a [continuous map](../../../../continuous-map.md) from $S_+^{n-1}$ to itself. Indeed, every entry of $Ax$ is nonnegative because $A$ is a [nonnegative matrix](../../../../nonnegative-matrix.md) and every entry of $x$ is nonnegative. By the supplied [homeomorphism](../../../../homeomorphism.md) $h:\mathbb B^{n-1}\to S_+^{n-1}$, the [continuous map](../../../../continuous-map.md) $h^{-1}Th$ maps the finite-dimensional [closed unit ball](../../../../closed-unit-ball.md) into itself. The [Brouwer fixed-point theorem](../../../../brouwer-fixed-point-theorem.md) supplies a [fixed point](../../../../fixed-point.md), hence $T(x_*)=x_*$ for some $x_*\in S_+^{n-1}$. Therefore

$$
\boxed{Ax_*=\lambda x_*,\qquad x_*\ne0,\qquad\lambda=|Ax_*|>0.}
$$

Together with the zero case this proves that $A$ has a nonnegative [eigenvalue](../../../../eigenvalue.md), with a nonnegative [eigenvector](../../../../eigenvector.md). For $n=1$, the auxiliary [closed unit ball](../../../../closed-unit-ball.md) is the one-point space $\mathbb B^0$ and the argument remains valid. No claim of strict positivity of every entry of the [eigenvector](../../../../eigenvector.md) is needed.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
