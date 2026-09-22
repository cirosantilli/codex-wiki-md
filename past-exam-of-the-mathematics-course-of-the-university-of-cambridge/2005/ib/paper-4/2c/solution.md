<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

The [Eisenstein criterion](../../../../../eisenstein-criterion.md) says that a primitive integer [polynomial](../../../../../polynomial-split.md) $P(x)=a_mx^m+\cdots+a_0$ is irreducible over $\mathbb Q$ if some [prime number](../../../../../prime-number.md) $p$ divides every $a_j$ for $j<m$, does not divide $a_m$, and $p^2$ does not divide $a_0$. By [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md), this gives irreducibility in $\mathbb Z[x]$ as well.

For prime $n=p$, translate the variable in $P_p(x)=(x^p-1)/(x-1)$:

$$
P_p(x+1)=\frac{(x+1)^p-1}{x}=\sum_{j=1}^p\binom pj x^{j-1}.
$$

Its leading coefficient is one, all other coefficients are divisible by $p$, and its constant coefficient is exactly $p$. The [Eisenstein criterion](../../../../../eisenstein-criterion.md) proves this translated [polynomial](../../../../../polynomial-split.md) irreducible. Since $x\mapsto x+1$ is an invertible substitution in $\mathbb Z[x]$, $P_p$ is irreducible too.

If $n=ab$ with $a,b>1$, then

$$
P_n(x)=(1+x+\cdots+x^{a-1})(1+x^a+\cdots+x^{(b-1)a}).
$$

Both factors have positive degree and integer coefficients, proving reducibility. Consequently $\boxed{1+x+\cdots+x^{n-1}\text{ is irreducible exactly when }n\text{ is prime}.}$

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
