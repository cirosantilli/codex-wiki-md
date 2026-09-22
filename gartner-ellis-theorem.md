<h1 id="gartner-ellis-theorem">Gärtner–Ellis theorem</h1>

↑ **Parent:** [Large deviation principle](large-deviation-principle.md)

Let $X_N\in\mathbb R^d$ and $a_N\to\infty$. Define the scaled [cumulant-generating function](cumulant-generating-function.md)

$$
\Lambda_N(\theta)=a_N^{-1}\log\mathbb E e^{a_N\langle\theta,X_N\rangle}.
$$

Suppose its pointwise limit $\Lambda$ exists, is [lower semicontinuous](lower-semicontinuity.md), has $0$ in the interior of its effective domain, and is essentially smooth: it is differentiable on that interior, which is nonempty, and its gradient norm diverges at every finite boundary point approached from the interior. Then $X_N$ satisfies a [large deviation principle](large-deviation-principle.md) with [good rate function](good-rate-function.md) given by the [Legendre-Fenchel transform](convex-conjugate.md)

$$
\Lambda^*(x)=\sup_\theta\{\langle\theta,x\rangle-\Lambda(\theta)\}.
$$

The [Chernoff bound](chernoff-bound.md) supplies the upper estimate. The lower estimate uses [exponential tilting](exponential-tilting.md) at a parameter whose gradient selects the required mean; essential smoothness supplies the boundary approximation needed for the full lower bound. A finite boundary slope can leave an affine branch of $\Lambda^*$ outside this argument, so a separate lower-bound proof is then necessary.

## ↑ Ancestors (7)

1. [Large deviation principle](large-deviation-principle.md)
2. [Convergence of random variables](convergence-of-random-variables-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Essential smoothness of a convex function](essential-smoothness-of-a-convex-function.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-26/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/4/a/solution.md)
- [Poisson moderate deviation principle](poisson-moderate-deviation-principle.md)
