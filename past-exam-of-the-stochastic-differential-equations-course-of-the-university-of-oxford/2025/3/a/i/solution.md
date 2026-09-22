<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the diffusion and [drift coefficients](../../../../../drift-coefficient.md) as

$$
\sigma(x)=\frac1{1+x^2},\qquad b(x)=-\frac1{2(1+x^2)^2}.
$$

Both are continuously differentiable, with

$$
\sigma'(x)=-\frac{2x}{(1+x^2)^2},\qquad
b'(x)=\frac{2x}{(1+x^2)^3}.
$$

These derivatives are bounded. For example $2|x|\leq1+x^2$ bounds both absolute values by one. The [mean value theorem](../../../../../mean-value-theorem.md) therefore makes both coefficients [globally Lipschitz](../../../../../globally-lipschitz-function.md). They are also bounded, so satisfy the [linear growth condition for an SDE](../../../../../linear-growth-condition-for-an-sde.md).

The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) consequently gives

$$
\boxed{\text{a global strong solution, unique up to indistinguishability}.}
$$

In particular, there is no finite explosion time. The solution has continuous paths, so all subsequent level-hitting and stopping arguments apply.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
