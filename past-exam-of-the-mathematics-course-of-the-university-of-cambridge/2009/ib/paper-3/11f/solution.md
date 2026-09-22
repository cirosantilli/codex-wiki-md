<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Use the standard commutative-ring convention with identity and a nonempty multiplicative subset. An [ideal](../../../../../ideal.md) disjoint from that subset is proper. Suppose $ab\in I$ but $a,b\notin I$. Maximality among disjoint [ideals](../../../../../ideal.md) means that both $I+(a)$ and $I+(b)$ meet $S$. Thus $s=i+ra\in S$ and $t=j+ub\in S$ for some $i,j\in I$, $r,u\in R$. Their product belongs to $S$ by multiplicative closure, but

$$
st=ij+iub+jra+ruab\in I,
$$

a contradiction. Consequently **$I$ is prime**. This is [prime ideal avoiding a multiplicative subset](../../../../../prime-ideal-avoiding-a-multiplicative-subset.md).

For an [integral domain](../../../../../integral-domain.md), form its [field of fractions](../../../../../field-of-fractions.md) from pairs $(a,b)$ with $b\ne0$, identifying $(a,b)$ and $(c,d)$ when $ad=bc$. Write the class as $a/b$ and define addition and multiplication by

$$
\frac ab+\frac cd=\frac{ad+bc}{bd},\qquad
\frac ab\frac cd=\frac{ac}{bd}.
$$

The domain condition makes the equivalence relation and these operations well-defined. Every nonzero $a/b$ has inverse $b/a$. The map $a\mapsto a/1$ is an injective [ring homomorphism](../../../../../ring-homomorphism.md) because $a/1=0/1$ implies $a=0$.

For the final assertion, pass to $R/I$. The image $\overline S$ is multiplicatively closed and does not contain zero, because $S\cap I=\varnothing$. Apply the allowed existence result to obtain an [ideal](../../../../../ideal.md) $J$ of $R/I$ maximal among those disjoint from $\overline S$. The first proof makes $J$ prime. Its inverse image $P$ in $R$ is therefore prime, contains $I$ and avoids $S$. The quotient $R/P$ is an [integral domain](../../../../../integral-domain.md); compose

$$
\boxed{R\longrightarrow R/P\longrightarrow\operatorname{Frac}(R/P).}
$$

This homomorphism kills every element of $I$. No element of $S$ maps to zero, because the first map kills precisely $P$ and the second is injective. Thus it has both required properties. Commutativity is essential to the general statement; it is the ring convention under which the printed prime-ideal argument is used.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
