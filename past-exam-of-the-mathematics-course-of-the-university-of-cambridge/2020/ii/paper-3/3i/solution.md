<h1 id="3i/solution">Solution</h1>

↑ **Parent:** [3I](../3i.md)

Use [Shamir's secret sharing](../../../../../shamir-s-secret-sharing.md) over the [finite field](../../../../../finite-field.md) $\mathbb F_p$. The Chair independently chooses $a_1,\ldots,a_{r-1}$ from the [uniform distribution on a finite set](../../../../../discrete-uniform-distribution.md) $\mathbb F_p$ and forms the random [polynomial](../../../../../polynomial-split.md)

$$
f(X)=N+a_1X+\cdots+a_{r-1}X^{r-1}\in\mathbb F_p[X].
$$

Choose distinct nonzero $x_1,\ldots,x_s\in\mathbb F_p$, with $s$ equal to the number of discs to be issued, and inscribe $(x_i,f(x_i))$ on disc $i$.

Any $r$ discs give $r$ distinct values of a polynomial of degree at most $r-1$. Their [Vandermonde determinant](../../../../../vandermonde-determinant.md) is nonzero, so [polynomial interpolation](../../../../../polynomial-interpolation.md) recovers $f$ uniquely and hence recovers the secret as $N=f(0)$.

Conversely, fix any $r-1$ observed discs and any candidate secret $n\in\mathbb F_p$. Interpolating through those $r-1$ points and $(0,n)$ gives exactly one polynomial of degree at most $r-1$. Thus every candidate $n$ is compatible with the observed discs in exactly the same number of ways. Because the coefficients were chosen [uniformly](../../../../../discrete-uniform-distribution.md), the [conditional distribution](../../../../../conditional-distribution.md) of the secret is unchanged after seeing any $r-1$ discs. This proves the [Perfect secrecy of Shamir's threshold scheme](../../../../../perfect-secrecy-of-shamir-s-threshold-scheme.md).

## ↑ Ancestors (10)

1. [3I](../3i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
