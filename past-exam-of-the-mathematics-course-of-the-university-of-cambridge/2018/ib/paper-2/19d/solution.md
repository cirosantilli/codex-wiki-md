<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

This is the [Gram-Schmidt process](../../../../../gram-schmidt-process.md) applied degree by degree. Inductively, subtracting projections onto $p_0,\ldots,p_n$ makes $p_{n+1}$ orthogonal to every earlier polynomial. Since every subtracted polynomial has degree at most $n$, the leading coefficient of the monic $q_{n+1}$ remains one, so $p_{n+1}$ is a real [monic orthogonal polynomial](../../../../../monic-orthogonal-polynomial.md) of degree exactly $n+1$.

Now take $q_{n+1}=xp_n$. For $k\leq n-2$, symmetry of the [inner product](../../../../../inner-product.md) gives

$$
\langle xp_n,p_k\rangle=\langle p_n,xp_k\rangle=0,
$$

because $xp_k$ has degree at most $n-1$. Only the $p_n$ and $p_{n-1}$ projections remain, yielding the [three-term recurrence for monic orthogonal polynomials](../../../../../three-term-recurrence-for-monic-orthogonal-polynomials.md)

$$
p_{n+1}=(x-\alpha_n)p_n-\beta_np_{n-1},
$$

where

$$
\boxed{\alpha_n=\frac{\langle xp_n,p_n\rangle}{\langle p_n,p_n\rangle},
\qquad
\beta_n=\frac{\langle p_n,p_n\rangle}{\langle p_{n-1},p_{n-1}\rangle}.}
$$

The second identity uses $xp_{n-1}=p_n$ plus lower-degree terms.

For the symmetric Legendre inner product, parity gives $\alpha_n=0$. Starting with $p_0=1$, one obtains $p_1=x$, then

$$
\beta_1=\frac{\int_{-1}^1x^2\,dx}{\int_{-1}^1 1\,dx}=\frac13,
\qquad
\beta_2=\frac{\int_{-1}^1(x^2-1/3)^2\,dx}{\int_{-1}^1x^2\,dx}=\frac4{15}.
$$

Thus the first four monic [Legendre polynomials](../../../../../legendre-polynomial.md) are

$$
\boxed{p_0=1,\qquad p_1=x,\qquad
p_2=x^2-\frac13,\qquad
p_3=x^3-\frac35x.}
$$

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
