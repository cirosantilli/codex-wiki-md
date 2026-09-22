<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are $m=\binom n2$ independent edge indicators. Conditional on all indicators except one, changing that edge changes the [maximum matching number](../../../../../../matching-number.md) by at most one. The conditional range is therefore at most one, so [Popoviciu inequality on variances](../../../../../../popoviciu-s-inequality-on-variances.md) bounds each conditional variance by $1/4$. The tensorized conditional-variance inequality gives

$$
\boxed{\operatorname{Var}(f(G))
\leq\sum_{e=1}^m\mathbb E\operatorname{Var}(f(G)\mid X_{-e})
\leq\frac m4=\frac1{4}\binom n2.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
