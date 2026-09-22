<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Bernstein polynomial](../../../../../../bernstein-polynomial.md) is

$$
B_n(f,x)=\sum_{j=0}^n f(j/n)\binom nj x^j(1-x)^{n-j}.
$$

It has degree at most $n$, since cancellation can lower the degree. For $0\le x\le1$, the [Bernstein basis](../../../../../../bernstein-basis.md) weights are nonnegative and their sum is $(x+(1-x))^n=1$ by the [binomial theorem](../../../../../../binomial-theorem.md). Consequently

$$
|B_n(f,x)|\le\sum_{j=0}^n |f(j/n)|\binom nj x^j(1-x)^{n-j}\le\|f\|_\infty.
$$

Thus the [Bernstein polynomial](../../../../../../bernstein-polynomial.md) defines a [positive linear operator on continuous functions](../../../../../../positive-linear-operator-on-continuous-functions.md) satisfying **$\|B_n f\|_\infty\le\|f\|_\infty$**. Since $B_n1=1$, its [operator norm](../../../../../../operator-norm.md) in the [supremum norm](../../../../../../supremum-norm.md) is exactly one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
