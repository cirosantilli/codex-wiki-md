<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) says that if $p$ is prime, $L\subseteq\mathbb F_p$ has $s\leq\min\{r,n-r\}$ elements, and $\mathcal F\subseteq[n]^{(r)}$ satisfies

$$
|A\cap B|\bmod p\in L\quad(A\ne B),
\qquad
r\bmod p\notin L,
$$

then $|\mathcal F|\leq\binom ns$.

For each $A\in\mathcal F$, form the multilinearization on the Boolean cube of

$$
P_A(x)=\prod_{\ell\in L}
\left(\sum_{i\in A}x_i-\ell\right).
$$

At the [characteristic vector of a set](../../../../../characteristic-vector-of-a-set.md) $\mathbf1_B$, this polynomial vanishes for $B\ne A$ and is nonzero for $B=A$. Hence the restricted functions $P_A$ are linearly independent. On the $r$-slice, every square-free monomial of degree below $s$ can be raised to degree $s$ using the relation $\sum_i x_i=r$, so the degree-at-most-$s$ function space is spanned by the $\binom ns$ square-free degree-$s$ monomials. Linear independence gives the theorem.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
