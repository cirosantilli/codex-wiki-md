<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $m=\min_r|u(x_r)-q(x_r)|$ and $M=\max_r|u(x_r)-q(x_r)|$. If the [best uniform approximation](../../../../../best-uniform-approximation.md) had error below $m$, the values of $p_n^*-q$ would strictly alternate in sign at all $n+2$ reference points. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) would give at least $n+1$ distinct [roots of a polynomial](../../../../../root-of-a-polynomial.md) of degree at most $n$, a contradiction. If $m=0$ the lower bound is immediate.

At least one reference point attains the global error maximum of $q$, so $M=\|u-q\|_\infty$. Optimality of $p_n^*$ gives the upper bound, and therefore

$$
\boxed{\min_r|u(x_r)-q(x_r)|\leq\|u-p_n^*\|_\infty\leq\max_r|u(x_r)-q(x_r)|.}
$$

This is the unequal-height version of the [alternating-reference error bound](../../../../../alternating-reference-error-bound.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
