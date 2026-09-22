<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We work in the usual real-valued setting of the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md). For $f\in C[-1,1]$ and an algebraic [polynomial](../../../../../../polynomial-split.md) $p$ of degree at most $n$, the theorem says that $p$ is a [best uniform approximation](../../../../../../best-uniform-approximation.md) if and only if its error has $n+2$ ordered points with alternating maximal values:

$$
-1\le x_0<\cdots<x_{n+1}\le1,\qquad
f(x_j)-p(x_j)=\varepsilon(-1)^j\|f-p\|_\infty,
\quad \varepsilon\in\{1,-1\}.
$$

If $f=p$, the zero-error case is included directly.

Existence follows, for example, by taking a minimizing sequence: its [supremum norms](../../../../../../supremum-norm.md) are bounded, all norms on the finite-dimensional [polynomial](../../../../../../polynomial-split.md) space are equivalent, and a convergent coefficient subsequence attains the infimum. To prove [uniqueness of best uniform polynomial approximation](../../../../../../uniqueness-of-best-uniform-polynomial-approximation.md), let $p,q$ both attain the minimum error $E$. Their average $r=(p+q)/2$ has error at most $E$ by the triangle inequality and therefore exactly $E$ by minimality.

If $E=0$, both [polynomials](../../../../../../polynomial-split.md) equal $f$ and are equal. Otherwise apply the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) to $r$. At every alternating extremal point, $f-r$ is either $E$ or $-E$. But it is the average of $f-p$ and $f-q$, each lying in $[-E,E]$. An average attains an endpoint of this interval only when both entries equal that endpoint. Hence $p(x_j)=q(x_j)$ at all $n+2$ points. The difference is a degree-at-most-$n$ [polynomial](../../../../../../polynomial-split.md) with more than $n$ distinct zeros, so it is identically zero. **The best approximating [polynomial](../../../../../../polynomial-split.md) is unique.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
