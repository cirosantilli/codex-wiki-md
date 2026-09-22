<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $(u-p,q)=0$ for all $q\in A$, then for any $a\in A$ the difference $p-a$ lies in $A$ and [Pythagorean theorem](../../../../../pythagorean-theorem.md) gives

$$
\|u-a\|_2^2=\|(u-p)+(p-a)\|_2^2
=\|u-p\|_2^2+\|p-a\|_2^2\geq\|u-p\|_2^2.
$$

Thus $p$ is best.

Conversely, if $p$ is best, then for every $q\in A$ the real quadratic

$$
\|u-p-tq\|_2^2
=\|u-p\|_2^2-2t(u-p,q)+t^2\|q\|_2^2
$$

has its [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) at $t=0$. Its linear coefficient must vanish, giving $(u-p,q)=0$. Hence **[best approximation](../../../../../best-approximation-in-a-normed-space.md) is equivalent to [orthogonality](../../../../../orthogonal-vectors.md) of the residual to the approximation space**. The weight is positive almost everywhere, so this is a genuine positive-definite [inner product](../../../../../inner-product-split.md) on continuous functions.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
