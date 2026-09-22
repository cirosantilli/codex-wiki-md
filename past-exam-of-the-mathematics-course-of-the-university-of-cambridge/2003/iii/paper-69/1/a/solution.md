<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [continuous function](../../../../../../continuous-function.md) $f$ on $[0,1]$, its [Bernstein polynomial](../../../../../../bernstein-polynomial.md) is

$$
B_n(f,x)=\sum_{j=0}^n f(j/n)\binom njx^j(1-x)^{n-j}.
$$

The weights are nonnegative and, by the [binomial theorem](../../../../../../binomial-theorem.md), sum to $(x+1-x)^n=1$. Thus $|B_n(f,x)|\le\sum_j|f(j/n)|\binom njx^j(1-x)^{n-j}\le\|f\|_\infty$ at every $x\in[0,1]$, including the endpoints. Taking the [supremum norm](../../../../../../supremum-norm.md) gives

$$
\boxed{\|B_nf\|_\infty\le\|f\|_\infty.}
$$

In particular, $B_n$ is a [linear operator](../../../../../../linear-operator.md) of norm one, since it preserves the constant function one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
