<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Bernstein polynomial](../../../../../../bernstein-polynomial.md) in its partition-normalized [Bernstein basis](../../../../../../bernstein-basis.md):

$$
\boxed{B_n(f,x)=\sum_{k=0}^nf(k/n)\binom nkx^k(1-x)^{n-k}.}
$$

For $0\le x\le1$, every weight is nonnegative, and the [binomial theorem](../../../../../../binomial-theorem.md) gives their sum as $(x+1-x)^n=1$. Consequently

$$
|B_n(f,x)|\le\sum_{k=0}^n|f(k/n)|\binom nkx^k(1-x)^{n-k}\le\|f\|_\infty.
$$

Taking the [supremum norm](../../../../../../supremum-norm.md) proves **$\|B_n(f)\|_\infty\le\|f\|_\infty$**. The construction yields degree at most $n$, possibly lower for special functions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
