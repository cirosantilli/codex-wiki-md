<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $u\in W^{1,2}(B_2(0))$ is nonnegative [almost everywhere](../../../../../../almost-everywhere.md), and that the real coefficient [matrix](../../../../../../matrix.md) $A=(a^{ij})$ is measurable and satisfies, for almost every $x$ and every $\xi\in\mathbb R^n$,

$$
\xi\cdot A(x)\xi\geq\lambda|\xi|^2,\qquad
|A(x)\xi|\leq\Lambda|\xi|,
\qquad 0<\lambda\leq\Lambda<\infty.
$$

The [operator norm](../../../../../../operator-norm.md) bound controls all coefficients, including any antisymmetric part. For a [symmetric matrix](../../../../../../symmetric-matrix.md), these assumptions are exactly the usual lower and upper quadratic-form bounds. The [weak solution](../../../../../../weak-solution.md) condition is

$$
\int_{B_2}a^{ij}D_j uD_i\zeta=0\qquad(\zeta\in C_c^\infty(B_2)).
$$

Then the [Harnack inequality for uniformly elliptic divergence-form equations](../../../../../../harnack-inequality-for-uniformly-elliptic-divergence-form-equations.md) is

$$
\boxed{\operatorname*{ess\,sup}_{B_1}u\leq C(n,\Lambda/\lambda)\operatorname*{ess\,inf}_{B_1}u.}
$$

**A nonnegative weak solution has its supremum controlled by its infimum on the smaller ball.** The [De Giorgi-Nash-Moser theorem](../../../../../../de-giorgi-nash-moser-theorem.md) supplies a [Hölder continuous function](../../../../../../holder-condition.md) representative, for which ordinary supremum and infimum can replace the [essential supremum](../../../../../../essential-supremum.md) and [essential infimum](../../../../../../essential-infimum.md). Nonnegativity and the larger ball are essential hypotheses; there is no differentiability requirement on the coefficients.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
