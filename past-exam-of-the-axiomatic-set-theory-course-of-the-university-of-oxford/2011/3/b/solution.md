<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an infinite [cardinal number](../../../../cardinal-number-split.md) $\kappa$, its [cofinality](../../../../cofinality.md) is

$$
\operatorname{cf}(\kappa)=\min\{|A|:A\subseteq\kappa,\ \sup A=\kappa\},
$$

viewing $\kappa$ as an [initial ordinal](../../../../initial-ordinal.md). Equivalently it is the smallest [cardinal number](../../../../cardinal-number-split.md) which is the domain size of a [cofinal map](../../../../cofinal-map.md) into $\kappa$.

Put $\lambda=2^\kappa$ and $\mu=\operatorname{cf}(\lambda)$. Suppose $\mu\leq\kappa$, and choose cofinal [ordinals](../../../../ordinal-split.md) $\alpha_i<\lambda$ for $i<\mu$. Put $a_i=|\alpha_i|<\lambda$. Their union is $\lambda$, so [infinite cardinal arithmetic](../../../../infinite-cardinal-arithmetic.md) gives

$$
\lambda\leq\sum_{i<\mu}a_i\leq\lambda\mu=\lambda.
$$

Apply the [König theorem for cardinal numbers](../../../../konig-s-theorem-set-theory.md) to $a_i<a_i^+$. Each [successor cardinal](../../../../successor-cardinal.md) $a_i^+$ is at most $\lambda$, whence

$$
\lambda=\sum_{i<\mu}a_i<\prod_{i<\mu}a_i^+\leq\lambda^\mu\leq(2^\kappa)^\kappa=2^{\kappa\cdot\kappa}=2^\kappa=\lambda.
$$

Here the last equalities use the [currying law for cardinal exponentiation](../../../../currying-law-for-cardinal-exponentiation.md) and [square of an infinite cardinal](../../../../square-of-an-infinite-cardinal.md). This contradiction proves the [cofinality of a power-set cardinal](../../../../cofinality-of-a-power-set-cardinal.md) bound

$$
\boxed{\operatorname{cf}(2^\kappa)>\kappa.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the axiomatic set theory course of the University of Oxford](../../../split.md)
5. [Axiomatic set theory course of the University of Oxford](../../../../axiomatic-set-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
