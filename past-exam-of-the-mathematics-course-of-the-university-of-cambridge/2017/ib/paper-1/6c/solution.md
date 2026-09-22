<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

The [Lagrange cardinal polynomials](../../../../../lagrange-cardinal-polynomial.md) are

$$
\ell_i(x)=\prod_{\substack{0\le j\le n\\j\ne i}}\frac{x-x_j}{x_i-x_j},\qquad \ell_i(x_j)=\delta_{ij}.
$$

Thus the [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) is

$$
\boxed{p(x)=\sum_{i=0}^n f_i\ell_i(x)}.
$$

It has degree at most $n$ and takes the required values. Uniqueness follows because the difference of two such [polynomials](../../../../../polynomial-split.md) has $n+1$ distinct roots and degree at most $n$, so is zero. The source's phrase “degree $n$” must allow a smaller degree, for example when $f$ is constant.

Define the [divided difference](../../../../../divided-difference.md) recursively by $f[x_i]=f_i$ and

$$
f[x_0,\ldots,x_n]=\frac{f[x_1,\ldots,x_n]-f[x_0,\ldots,x_{n-1}]}{x_n-x_0}.
$$

Induction on this recursion, or comparison of the leading coefficient in the [Newton interpolation polynomial](../../../../../newton-polynomial.md), gives

$$
\boxed{f[x_0,\ldots,x_n]=\sum_{i=0}^n\frac{f_i}{\prod_{j\ne i}(x_i-x_j)}}.
$$

For completeness the induction works term by term: an interior term gets the coefficient $(1/(x_i-x_n)-1/(x_i-x_0))/(x_n-x_0)=1/((x_i-x_n)(x_i-x_0))$, multiplying the product over the other interior nodes; the two endpoint terms give the same formula. This is also the leading coefficient of $p$ directly from the cardinal formula, so $p^{(n)}=n!f[x_0,\ldots,x_n]$.

The function $f-p\in C^n[x_0,x_n]$ has $n+1$ distinct zeros. Repeated application of [Rolle theorem](../../../../../rolle-theorem.md) gives $\xi\in(x_0,x_n)$ with $(f-p)^{(n)}(\xi)=0$ when $n\ge1$. Hence

$$
\boxed{f[x_0,\ldots,x_n]=\frac{f^{(n)}(\xi)}{n!}}.
$$

For $n=0$, this is simply $f[x_0]=f(x_0)$ and we take $\xi=x_0$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
