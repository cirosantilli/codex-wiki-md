<h1 id="17b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the [Leibniz rule](../../../../../../leibniz-rule.md),

$$
\frac{d^n}{dx^n}\left(x^{n+1/2}e^{-x}\right)
=e^{-x}\sum_{j=0}^n\binom nj(-1)^{n-j}
\frac{d^j}{dx^j}x^{n+1/2}.
$$

After multiplication by $(-1)^nx^{-1/2}e^x$, the term $j=0$ is $x^n$, and every other term has lower degree. Thus $p_n$ is a [monic polynomial](../../../../../../monic-polynomial.md) of degree $n$. Direct calculation gives

$$
\boxed{
p_0(x)=1,\qquad
p_1(x)=x-\frac32,\qquad
p_2(x)=x^2-5x+\frac{15}{4}
}.
$$

These are the monic normalization of the [generalized Laguerre polynomials](../../../../../../generalized-laguerre-polynomial.md) with parameter $1/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
