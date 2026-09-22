<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

Use the weighted [inner product](../../../../../inner-product.md)

$$
\langle f,g\rangle=\int_a^bf(x)g(x)w(x)\,dx,\qquad h_n=\langle Q_n,Q_n\rangle>0.
$$

Here the interval is nondegenerate and the indicated integrals are finite, as required for the given [orthogonal polynomials](../../../../../orthogonal-polynomial.md). Strict positivity follows because $w>0$ and a nonzero polynomial cannot vanish on an interval. Since each $Q_j$ is [monic](../../../../../monic-polynomial.md) of degree $j$, $Q_0,\ldots,Q_{n+1}$ form a [basis](../../../../../basis.md) of the polynomials of degree at most $n+1$. Comparing leading coefficients, expand

$$
xQ_n=Q_{n+1}+\sum_{j=0}^nc_jQ_j.
$$

By [orthogonality](../../../../../orthogonal-vectors.md), $c_j=\langle xQ_n,Q_j\rangle/h_j$. For $j\leq n-2$, symmetry of multiplication by $x$ gives

$$
\langle xQ_n,Q_j\rangle=\langle Q_n,xQ_j\rangle=0,
$$

because $xQ_j$ has degree at most $n-1$ and is a [linear combination](../../../../../linear-combination.md) of $Q_0,\ldots,Q_{n-1}$. Only the last two terms remain. Their coefficients are

$$
\boxed{a_n=\frac{\int_a^bxQ_n(x)^2w(x)\,dx}{\int_a^bQ_n(x)^2w(x)\,dx},\qquad
b_n=\frac{\int_a^bQ_n(x)Q_{n-1}(x)xw(x)\,dx}{h_{n-1}}=\frac{h_n}{h_{n-1}}>0\quad(n\geq1).}
$$

For the second equality, $xQ_{n-1}-Q_n$ has degree at most $n-1$, so its [inner product](../../../../../inner-product.md) with $Q_n$ vanishes. Rearranging proves the [three-term recurrence for monic orthogonal polynomials](../../../../../three-term-recurrence-for-monic-orthogonal-polynomials.md):

$$
\boxed{Q_{n+1}=(x-a_n)Q_n-b_nQ_{n-1}.}
$$

For $n=0$ this reads $Q_1=x-a_0$ because $Q_{-1}=0$ and $Q_0=1$. The coefficient $b_0$ is therefore immaterial and is not determined by the polynomials. The usual convention is $b_0=0$; if a positive $b_0$ is desired, any positive value gives the identical recurrence. The strictly positive norm-ratio formula is the assertion for **$n\geq1$**, not a division by the norm of $Q_{-1}$.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
