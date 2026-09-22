# Exponential map of a Lie group

↑ **Parent:** [Lie group](lie-group.md)

For any [Lie group](lie-group.md), the [Exponential map of a Lie group](exponential-map-of-a-lie-group.md) is defined by $\exp(X)=\gamma_X(1)$, where $\gamma_X$ is the [one-parameter subgroup](one-parameter-subgroup.md) with initial [tangent vector](tangent-vector.md) $X$. For a [Matrix Lie group](matrix-lie-group.md), it is the [matrix exponential](matrix-exponential.md) $\exp X=\sum_{n\geq0}X^n/n!$. Its [differential](differential-of-a-smooth-map.md) at zero is the identity, so the [inverse function theorem](inverse-function-theorem.md) supplies a [local exponential chart](local-exponential-chart.md). A small transformation can therefore be encoded by a [vector](vector.md) in the [Lie algebra](lie-algebra-split.md). See [MIT 18.745, Lecture 7, Definition 7.2 and Theorem 7.5](https://ocw.mit.edu/courses/18-745-lie-groups-and-lie-algebras-i-fall-2020/mit18_745_f20_lec07.pdf).

Local invertibility makes no promise about a global inverse. In the planar [rotation](rotation-mathematics.md) example, $\exp((\theta+2\pi k)J)=\exp(\theta J)$ for every integer $k$, so the [Exponential map of a Lie group](exponential-map-of-a-lie-group.md) is surjective onto $SO(2)$ but not injective. Restricting to $-\pi<\theta<\pi$ gives unique angles for every [rotation](rotation-mathematics.md) except $R_\pi=-I$. The omitted half-turn exposes the cut needed for this single angle chart.

Surjectivity can also fail, even in a connected [Lie group](lie-group.md). The [matrix](matrix.md) $A=\operatorname{diag}(-2,-1/2)$ lies in the [special linear group](special-linear-group.md) $SL_2(\mathbb R)$ but has no real [matrix logarithm](matrix-logarithm.md): any logarithm must commute with $A$, hence preserve each of its distinct real [eigenvectors](eigenvector.md), where exponentiating a real scalar gives a positive number. See the [exponential-surjectivity obstruction from distinct negative eigenvalues](exponential-surjectivity-obstruction-from-distinct-negative-eigenvalues.md). These two examples distinguish two different global obstacles: repeated parameters and unreachable elements. The [Exponential map of a Lie group](exponential-map-of-a-lie-group.md) remains locally effective in both settings.

**Table of contents**

- [Additivity of the Lie exponential map](additivity-of-the-lie-exponential-map.md)
- [Lie product formula in a Lie group](lie-product-formula-in-a-lie-group.md)
- [Naturality of the Lie group exponential](naturality-of-the-lie-group-exponential.md)
- [Local exponential chart](local-exponential-chart.md)

## ↑ Ancestors (7)

1. [Lie group](lie-group.md)
2. [Lie theory](lie-theory-split.md)
3. [Diagonal dominance](diagonal-dominance.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Additivity of the Lie exponential map](additivity-of-the-lie-exponential-map.md)
- [Exponential map of a Lie group](exponential-map-of-a-lie-group.md)
- [Lie algebra of a closed subgroup](lie-algebra-of-a-closed-subgroup.md)
- [Lie theory](lie-theory-split.md)
- [Local exponential chart](local-exponential-chart.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-102/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-131/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-302/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-302/1/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-302/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-302/1/e/solution.md)
- [Real special linear group of degree two](real-special-linear-group-of-degree-two.md)
