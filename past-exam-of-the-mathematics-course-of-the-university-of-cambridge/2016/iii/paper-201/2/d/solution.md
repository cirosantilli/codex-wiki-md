<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $T>n$, either $T_R\leq n$, or both stopping times exceed $n$. Therefore the [maximal bound for a nonnegative martingale](../../../../../../maximal-bound-for-a-nonnegative-martingale.md) and the [Markov inequality](../../../../../../markov-inequality.md) give, for $R\geq1$,

$$
\mathbb P(T>n)
\leq\mathbb P(T_R<\infty)+\mathbb P(T\wedge T_R>n)
\leq\frac1R+\frac{\tau^2R}{\sigma^2n}.
$$

The right-hand side is minimized at $R=\sigma\sqrt n/\tau$. Whenever the claimed bound is nontrivial, $2\tau/(\sigma\sqrt n)<1$, this choice has $R>2$ and is allowed under the corrected overshoot hypothesis. Substituting gives the [square-root tail bound for martingale absorption](../../../../../../square-root-tail-bound-for-martingale-absorption.md):

$$
\boxed{\mathbb P(T>n)\leq\frac{2\tau}{\sigma\sqrt n}\qquad(n\geq1).}
$$

When the displayed upper bound is at least one, the inequality follows from $\mathbb P(T>n)\leq1$. **This handles every $n$ without using the impossible small-threshold hypothesis.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
