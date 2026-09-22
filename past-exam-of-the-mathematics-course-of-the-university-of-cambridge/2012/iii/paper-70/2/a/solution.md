<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Bernstein polynomial](../../../../../../bernstein-polynomial.md) is the positive weighted average

$$
B_n(f,x)=\sum_{k=0}^n f(k/n)b_{n,k}(x),\qquad b_{n,k}(x)=\binom nkx^k(1-x)^{n-k}.
$$

For $0\le x\le1$, the [Bernstein basis](../../../../../../bernstein-basis.md) weights are nonnegative and the [binomial theorem](../../../../../../binomial-theorem.md) gives $\sum_{k=0}^nb_{n,k}(x)=1$. Hence $|B_n(f,x)|\le\sum_k\|f\|_\infty b_{n,k}(x)=\|f\|_\infty$. In particular,

$$
\boxed{\|B_n(f)\|_\infty\le\|f\|_\infty.}
$$

This is the contraction property of the [positive linear operator on continuous functions](../../../../../../positive-linear-operator-on-continuous-functions.md) defined by the [Bernstein polynomial](../../../../../../bernstein-polynomial.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
