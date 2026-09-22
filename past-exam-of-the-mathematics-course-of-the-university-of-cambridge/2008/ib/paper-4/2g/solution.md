<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Write $q_n(X)=1+X+\cdots+X^{n-1}$, a monic [primitive polynomial](../../../../../primitive-polynomial.md). If $n=ab$ with $a,b>1$, grouping terms gives a factorization in the [polynomial ring](../../../../../polynomial-ring.md) $\mathbb Z[X]$:

$$
q_n(X)=(1+X+\cdots+X^{a-1})(1+X^a+\cdots+X^{(b-1)a}).
$$

Both factors have positive degree, so $q_n$ is not an [irreducible polynomial](../../../../../irreducible-polynomial.md).

Conversely, if $n=p$ is a [prime number](../../../../../prime-number.md), change variables by $X=Y+1$. The [binomial theorem](../../../../../binomial-theorem.md) gives

$$
q_p(Y+1)=\frac{(Y+1)^p-1}{Y}=p+\binom p2Y+\cdots+\binom p{p-1}Y^{p-2}+Y^{p-1}.
$$

Every coefficient except the leading one is divisible by $p$, because $p\mid\binom pk$ for $1\leq k<p$, whereas the constant coefficient $p$ is not divisible by $p^2$. The [Eisenstein criterion](../../../../../eisenstein-criterion.md) makes this [polynomial](../../../../../polynomial-split.md) irreducible over $\mathbb Q$. The substitution $X\mapsto Y+1$ is an invertible [ring homomorphism](../../../../../ring-homomorphism.md), so $q_p$ is also irreducible over $\mathbb Q$; the [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md) transfers this to $\mathbb Z[X]$. Hence

$$
\boxed{q_n\text{ is irreducible over }\mathbb Z\iff n\text{ is prime}.}
$$

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
