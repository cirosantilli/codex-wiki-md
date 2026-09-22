<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For any [prime number](../../../../prime-number-split.md) $p$, there is a [prime chain](../../../../prime-chain.md)

$$
(0)\subsetneq(p)\subsetneq(p,t)
$$

in $\mathbb Z[t]$. These are [prime ideals](../../../../prime-ideal.md) because the respective [quotient rings](../../../../quotient-ring.md) are $\mathbb Z[t]$, $\mathbb F_p[t]$, and $\mathbb F_p$, all [integral domains](../../../../integral-domain.md). The inclusions are strict because $p\ne0$ and $t\notin(p)$. Hence $\dim\mathbb Z[t]\geq2$.

To prove the upper bound, suppose there were a [prime chain](../../../../prime-chain.md) of length at least three. Since $\mathbb Z[t]$ is an [integral domain](../../../../integral-domain.md), we could insert $(0)$ at its beginning if necessary and select a chain

$$
(0)\subsetneq P_1\subsetneq P_2\subsetneq P_3.
$$

By [c](../c.md), $P_2\cap\mathbb Z\ne(0)$. This intersection is a proper [prime ideal](../../../../prime-ideal.md) of $\mathbb Z$: if a product of integers lies in it, primality of $P_2$ puts one factor in it. Therefore $P_2\cap\mathbb Z=(p)$ for a [prime number](../../../../prime-number-split.md) $p$, and $(p)\subseteq P_2$.

We need to check that $P_2\ne(p)$. Here [prime ideals below a principal prime](../../../../prime-ideals-below-a-principal-prime.md) give the necessary restriction: no nonzero [prime ideal](../../../../prime-ideal.md) can lie strictly below $(p)$. If $0\ne P\subsetneq(p)$, then $p\notin P$. Choose $0\ne f\in P$ and factor out the largest common power of $p$ from its integer coefficients:

$$
f=p^kg,\qquad g\notin(p).
$$

Such a finite $k$ exists because $f$ has at least one nonzero integer coefficient. Since $p\notin P$ and $P$ is a [prime ideal](../../../../prime-ideal.md), repeated primality gives $g\in P\subseteq(p)$, a contradiction. Applied to $P_1\subsetneq P_2$, this rules out $P_2=(p)$.

It follows that $P_2/(p)$ is a nonzero [prime ideal](../../../../prime-ideal.md) of

$$
\mathbb Z[t]/(p)\cong\mathbb F_p[t].
$$

As in [c](../c.md), the [polynomial division algorithm](../../../../polynomial-division.md) makes $\mathbb F_p[t]$ a [principal ideal domain](../../../../principal-ideal-domain.md), so its nonzero [prime ideals](../../../../prime-ideal.md) are maximal by [a](../a.md). Thus $P_2/(p)$ is maximal. The [ideal correspondence theorem](../../../../correspondence-theorem-for-ideals.md) makes $P_2$ a [maximal ideal](../../../../maximal-ideal.md) of $\mathbb Z[t]$, contradicting $P_2\subsetneq P_3$. Consequently

$$
\boxed{\dim\mathbb Z[t]=2.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
