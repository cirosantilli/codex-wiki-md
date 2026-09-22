<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\alpha=a+x$, $\beta=b+m-x$, and $S=\alpha+\beta=m+a+b$. Integrate the future [binomial distribution](../../../../../../binomial-distribution.md) against the current [Beta distribution](../../../../../../beta-distribution.md) [posterior density](../../../../../../posterior-density.md):

$$
p(y\mid x)=\binom ny\frac{\mathrm B(\alpha+y,\beta+n-y)}{\mathrm B(\alpha,\beta)},\qquad y=0,\ldots,n.
$$

This is the [beta-binomial distribution](../../../../../../beta-binomial-distribution.md). For positive integer $a,b$, the [gamma function](../../../../../../gamma-function.md) values reduce to factorials, giving

$$
p(y\mid x)=\frac{n!}{y!(n-y)!}
\frac{(\alpha+y-1)!(\beta+n-y-1)!(S-1)!}
{(\alpha-1)!(\beta-1)!(S+n-1)!}.
$$

Using $(S-1)!=(S-1)(S-2)!$ and $(S+n-1)!=(S+n-1)(S+n-2)!$ rewrites this as

$$
\boxed{p(y\mid x)=\frac{S-1}{S+n-1}
\frac{\binom{\alpha+y-1}{y}\binom{\beta+n-y-1}{n-y}}
{\binom{S+n-2}{n}}.}
$$

Substitution of $\alpha,\beta,S$ gives exactly the two required factors. The probability is zero outside $0\leq y\leq n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
