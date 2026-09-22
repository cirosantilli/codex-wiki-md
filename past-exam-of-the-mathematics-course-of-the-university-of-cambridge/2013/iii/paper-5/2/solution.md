<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an integer tuple $\ell=(\ell_1,\ldots,\ell_m)$, the [monomial alternant](../../../../../monomial-alternant.md) is

$$
A_\ell(x)=|x^{\ell_1},\ldots,x^{\ell_m}|=\det(x_i^{\ell_j})_{1\le i,j\le m}.
$$

Negative exponents require nonzero coordinates; all exponents in the [character](../../../../../character-of-a-representation.md) expansion below are nonnegative. The [power-sum symmetric polynomial](../../../../../power-sum-symmetric-polynomial.md) is $s_k(x)=\sum_{i=1}^m x_i^k$. Put $\delta=(m-1,m-2,\ldots,0)$, so $A_\delta(x)=\prod_{i<j}(x_i-x_j)$ is the [Vandermonde determinant](../../../../../vandermonde-determinant.md).

Let a [conjugacy class](../../../../../conjugacy-class.md) of $S_n$ have $\alpha_k$ cycles of length $k$, with $\sum k\alpha_k=n$, and put $p_\alpha(x)=\prod_k s_k(x)^{\alpha_k}$. The product $p_\alpha A_\delta$ is an [alternating polynomial](../../../../../alternating-polynomial.md) homogeneous of degree $n+\binom m2$. In an alternating [polynomial](../../../../../polynomial-split.md), a monomial with two equal exponents has zero coefficient, since interchanging those variables fixes the monomial and reverses its sign. Grouping the remaining monomials by their permutation orbits gives a unique expansion in alternants $A_\ell$ with $\ell_1>\cdots>\ell_m\ge0$.

Such tuples of the indicated total degree are exactly $\ell_i=\lambda_i+m-i$ for [partitions of an integer](../../../../../partition-of-an-integer.md) $\lambda$ of $n$ with at most $m$ parts. Define the [class function](../../../../../class-function.md)

$$
\boxed{\omega_\lambda(\alpha)=[x_1^{\lambda_1+m-1}\cdots x_m^{\lambda_m}]\,p_\alpha(x)A_\delta(x).}
$$

The displayed monomial occurs with coefficient $1$ in $A_{\lambda+\delta}$ and in no other ordered alternant, so

$$
p_\alpha(x)A_\delta(x)=\sum_{\lambda\vdash n,\ \ell(\lambda)\le m}\omega_\lambda(\alpha)A_{\lambda+\delta}(x).
$$

This proves the expansion and explicitly defines its coefficients. They depend only on the cycle counts and hence are [class functions](../../../../../class-function.md). Identifying these coefficients with [Specht module](../../../../../specht-module.md) [characters](../../../../../character-of-a-representation.md) is the [Frobenius alternant character formula](../../../../../frobenius-alternant-character-formula.md), which the remaining parts allow us to assume.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
