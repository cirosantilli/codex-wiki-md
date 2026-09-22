<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

**Eisenstein's criterion.** Let $f(X)=a_nX^n+\cdots+a_0\in\mathbb Z[X]$ be a nonconstant [primitive polynomial](../../../../../primitive-polynomial.md). If a [prime number](../../../../../prime-number.md) $p$ satisfies $p\nmid a_n$, $p\mid a_j$ for $0\leq j<n$, and $p^2\nmid a_0$, then $f$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md) over $\mathbb Q$.

To prove the [Eisenstein criterion](../../../../../eisenstein-criterion.md), suppose a nontrivial factorization exists over $\mathbb Q$. [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md) gives $f=gh$ with $g,h\in\mathbb Z[X]$ of positive degree. Their leading coefficients are not divisible by $p$, because their product is $a_n$. Reduction modulo $p$ therefore preserves both degrees, and

$$
\overline g\,\overline h=\overline{a_n}X^n\quad\text{in }\mathbb F_p[X].
$$

Since the only irreducible factor of the right side is $X$, both reduced factors are nonzero monomials of positive degree. Their constant coefficients are consequently divisible by $p$. This would make $p^2\mid g(0)h(0)=a_0$, a contradiction.

For the requested [polynomial](../../../../../polynomial-split.md), shift the variable by one. The [binomial theorem](../../../../../binomial-theorem.md) gives

$$
\Phi_p(X+1)=\frac{(X+1)^p-1}{X}=\sum_{j=1}^p\binom pjX^{j-1}.
$$

It is monic, all coefficients below the leading one are divisible by $p$, and the constant coefficient is $p$, not divisible by $p^2$. The [Eisenstein criterion](../../../../../eisenstein-criterion.md) proves irreducibility of this shifted [polynomial](../../../../../polynomial-split.md). The substitution $X\mapsto X+1$ is an [automorphism](../../../../../automorphism.md) of $\mathbb Q[X]$, with inverse $X\mapsto X-1$, so it preserves nontrivial factorizations. Hence

$$
\boxed{X^{p-1}+X^{p-2}+\cdots+1\text{ is irreducible over }\mathbb Q.}
$$

This is the [cyclotomic polynomial](../../../../../cyclotomic-polynomial.md) for a prime index.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
