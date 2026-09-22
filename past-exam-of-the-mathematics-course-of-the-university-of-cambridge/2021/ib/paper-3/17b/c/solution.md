<h1 id="17b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [monic orthogonal polynomials](../../../../../../monic-orthogonal-polynomial.md), taking the inner product of the recurrence with $p_{n-1}$ gives

$$
\beta_n
=\frac{\langle xp_n,p_{n-1}\rangle}
{\langle p_{n-1},p_{n-1}\rangle}
=\frac{\langle p_n,xp_{n-1}\rangle}
{\langle p_{n-1},p_{n-1}\rangle}
=\frac{\langle p_n,p_n\rangle}
{\langle p_{n-1},p_{n-1}\rangle}.
$$

Using part (b) and the [Gamma function recurrence](../../../../../../gamma-function-recurrence.md),

$$
\boxed{\beta_n=n\left(n+\frac12\right)}.
$$

The Rodrigues expansion also shows that the coefficient of $x^{n-1}$ in $p_n$ is

$$
-n\left(n+\frac12\right).
$$

Comparing the coefficients of $x^n$ in

$$
p_{n+1}=(x-\alpha_n)p_n-\beta_np_{n-1}
$$

therefore gives

$$
-(n+1)\left(n+\frac32\right)
=-n\left(n+\frac12\right)-\alpha_n,
$$

and hence

$$
\boxed{\alpha_n=2n+\frac32}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
