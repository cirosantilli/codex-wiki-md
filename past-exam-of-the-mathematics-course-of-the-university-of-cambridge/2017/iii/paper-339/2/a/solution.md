<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Split the sign [vector](../../../../../../vector.md) as $x=(p^T,q^T)^T$. Multiplication of the two off-diagonal blocks gives

$$
x^TAx=\frac12(p^TSq+q^TS^Tp)=p^TSq,
$$

because the two terms are the same real [scalar](../../../../../../scalar.md). The map $(p,q)\mapsto x$ is a bijection between the feasible sign choices. Therefore

$$
\boxed{\max_{p,q}p^TSq=\max_x x^TAx}.
$$

This is the symmetric lifting of [bipartite binary quadratic optimization](../../../../../../bipartite-binary-quadratic-optimization.md) to [binary quadratic optimization](../../../../../../binary-quadratic-optimization.md). The factor $1/2$ is necessary: otherwise the two blocks would double the objective. No [positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md) of $A$ is assumed; generally its off-diagonal structure makes its [quadratic form](../../../../../../quadratic-form.md) indefinite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
