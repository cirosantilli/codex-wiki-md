<h1 id="11c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A nonzero [primitive polynomial](../../../../../../primitive-polynomial.md) in $\mathbb Z[x]$ has greatest common divisor of its coefficients equal to one. Suppose primitive polynomials $f,g$ had a product whose coefficients were all divisible by some prime $p$. Their reductions in $\mathbb F_p[x]$ are both nonzero, because neither polynomial has every coefficient divisible by $p$. A polynomial ring over a field is an [integral domain](../../../../../../integral-domain.md), so their product is nonzero modulo $p$, a contradiction. Hence **the product of primitive polynomials is primitive**.

To deduce unique factorization, write any nonzero integer polynomial as its positive [polynomial content](../../../../../../polynomial-content.md) times a primitive polynomial, with its sign treated as a unit. The preceding result gives multiplicativity of content. Factor the primitive part over the Euclidean polynomial ring $\mathbb Q[x]$, and rescale every irreducible rational factor to a primitive integer polynomial. If $f=q\prod_if_i$ with all polynomials primitive and $q=a/b$ in lowest terms, the equality $bf=a\prod_if_i$ has contents $b$ and $|a|$. Thus $b=|a|$, forcing $q=\pm1$. The rational factorization therefore lifts to an integer factorization.

A primitive integer polynomial is irreducible over $\mathbb Z$ exactly when it is irreducible over $\mathbb Q$: an integer factorization gives a rational one, and a rational factorization lifts by the same primitive-content argument. Factor the content into integer primes. Existence and uniqueness over the integers and over $\mathbb Q[x]$ now give existence and uniqueness of the resulting factorization into constant prime factors and primitive irreducible polynomial factors, up to order and signs. Therefore $\boxed{\mathbb Z[x]\text{ is a unique factorization domain}}$. This is the full lifting step in [Gauss lemma for polynomials](../../../../../../gauss-lemma-for-polynomials.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
