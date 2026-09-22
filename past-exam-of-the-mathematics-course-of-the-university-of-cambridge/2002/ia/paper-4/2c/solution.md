<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

The base case $n=1$ is the [product rule](../../../../../product-rule.md). Suppose the [Leibniz rule](../../../../../leibniz-rule.md) holds at order $n$. Taking one more [derivative](../../../../../derivative.md) of each term and collecting the coefficient of $f^{(n+1-r)}g^{(r)}$ gives

$$
(fg)^{(n+1)}=\sum_{r=0}^{n+1}\left[\binom nr+\binom n{r-1}\right]f^{(n+1-r)}g^{(r)}.
$$

Here [binomial coefficients](../../../../../binomial-coefficient.md) outside $0\le r\le n$ are zero. For $1\le r\le n$, the factorial definition proves [Pascal's identity](../../../../../pascal-s-rule.md) directly:

$$
\binom nr+\binom n{r-1}=\frac{n!}{r!(n-r)!}+\frac{n!}{(r-1)!(n-r+1)!}=\frac{(n+1)!}{r!(n+1-r)!}=\binom{n+1}r.
$$

At $r=0,n+1$, the identity is $1+0=1$. Substitution gives the required order-$n+1$ formula, completing the [induction](../../../../../mathematical-induction.md).

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
