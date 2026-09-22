# Null weight in a contour Laplace representation

↑ **Parent:** [Laplace integral solution](laplace-integral-solution.md)

A null weight contributes zero to a [Laplace integral](laplace-integral.md) on its domain of convergence. It can be added to a weight without changing the represented [function](function-split.md), so an integration-by-parts [differential equation](differential-equation-split.md) for the weight is not an unconditional uniqueness theorem.

For example, let $\Gamma$ enter along angle $\pi/3$ from infinity to zero and leave along angle $2\pi/3$ to infinity. The entire weight $h(\zeta)=e^{\zeta^2}$ is null for every complex $z$. Throughout the wedge between those rays, $\operatorname{Re}(\zeta^2)\leq-r^2/2$; the factor $e^{z\zeta}$ is dominated by this quadratic decay. Closing the contour by a large circular arc and applying the [Cauchy integral theorem](cauchy-s-integral-theorem.md) therefore proves the zero integral. All derivatives with respect to $z$ converge locally uniformly as well.

On the same contour, the quartic weight $e^{\zeta^4/4}$ gives a nontrivial entire solution. Its rays can be deformed within the [quartic decay sectors for a contour integral](quartic-decay-sectors-for-a-contour-integral.md) to angles $\pi/4$ and $3\pi/4$, where the value at $z=0$ is $-\sqrt2\,4^{-3/4}\Gamma(1/4)\ne0$. Adding the null weight changes neither this integral nor its vanishing endpoint terms, but the sum does not satisfy $g'=\zeta^3g$. Thus the usual Laplace method selects a convenient weight by cancelling the interior integrand separately; a necessity claim needs additional injectivity assumptions.

## ↑ Ancestors (8)

1. [Laplace integral solution](laplace-integral-solution.md)
2. [Laplace integral](laplace-integral.md)
3. [Laplace's method](laplace-s-method.md)
4. [Asymptotic expansion](asymptotic-expansion-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-applied-complex-variables-course-of-the-university-of-oxford/2011/3/a/solution.md)
- [Solution](past-exam-of-the-perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford/2009/b/5/ii/solution.md)
