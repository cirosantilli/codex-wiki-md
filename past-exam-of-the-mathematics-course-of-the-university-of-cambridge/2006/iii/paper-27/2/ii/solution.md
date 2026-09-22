<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $c_n$ be the [Mahler coefficients](../../../../../../mahler-coefficient.md) of $f$. Define its [discrete antiderivative](../../../../../../discrete-antiderivative.md) by

$$
\boxed{g(x)=\sum_{n\ge0}c_n\binom{x}{n+1}.}
$$

Because $c_n\to0$ and the [binomial polynomials](../../../../../../binomial-polynomial.md) have [field absolute value](../../../../../../absolute-value-algebra.md) at most one on $\mathbb Z_p$, this series converges uniformly to a continuous $\mathbb Z_p$-valued function. Every summand vanishes at zero. [Pascal's identity](../../../../../../pascal-s-rule.md) gives $\binom{x+1}{n+1}-\binom{x}{n+1}=\binom xn$, so taking differences through the uniformly convergent series proves $g(x+1)-g(x)=f(x)$. For nonnegative integers, induction from $g(0)=0$ gives precisely $g(m)=\sum_{j=0}^{m-1}f(j)$. Thus this is the required continuous extension, unique because the nonnegative integers are dense in $\mathbb Z_p$.

The [Mahler expansion](../../../../../../mahler-s-theorem.md) of $g$ has coefficient zero in degree zero and coefficient $c_{m-1}$ in degree $m\ge1$. This [discrete antidifferentiation on the p-adic integers](../../../../../../discrete-antidifferentiation-on-the-p-adic-integers.md) is the mechanism behind the next part.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
