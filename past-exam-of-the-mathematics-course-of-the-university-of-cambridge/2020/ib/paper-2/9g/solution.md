<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

[Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md) states that the product of two [primitive polynomials](../../../../../primitive-polynomial.md) over a [unique factorization domain](../../../../../unique-factorization-domain.md) is primitive. In particular, a primitive polynomial in $\mathbb Z[X]$ is reducible over $\mathbb Q$ exactly when it is reducible over $\mathbb Z$.

[Eisenstein criterion](../../../../../eisenstein-criterion.md) says that a primitive polynomial

$$
F(X)=a_nX^n+\cdots+a_0\in\mathbb Z[X]
$$

is irreducible over $\mathbb Q$ if there is a prime $p$ such that $p\nmid a_n$, $p\mid a_j$ for every $j<n$, and $p^2\nmid a_0$. To prove it, suppose $F=GH$ with both factors of positive degree. After removing contents, Gauss's lemma lets us take $G,H\in\mathbb Z[X]$ primitive. Reduction modulo $p$ gives

$$
\overline F=a_nX^n=\overline G\,\overline H,
$$

so both reduced factors are monomials of positive degree. Their constant terms are therefore divisible by $p$, making $p^2$ divide $a_0=G(0)H(0)$, a contradiction.

An [algebraic integer](../../../../../algebraic-integer.md) is a complex number satisfying a monic polynomial in $\mathbb Z[X]$. Let $\alpha$ be one and let $m_\alpha\in\mathbb Q[X]$ be its monic [minimal polynomial](../../../../../minimal-polynomial.md). The usual proof using polynomial content shows that $m_\alpha\in\mathbb Z[X]$. The set

$$
I_\alpha=\{f\in\mathbb Z[X]:f(\alpha)=0\}
$$

is the kernel of the polynomial-evaluation [ring homomorphism](../../../../../ring-homomorphism.md), hence an ideal. Every $f\in I_\alpha$ is divisible by $m_\alpha$ in $\mathbb Q[X]$. Because $m_\alpha$ is monic, polynomial division of $f$ by $m_\alpha$ takes place in $\mathbb Z[X]$, and the remainder must vanish by minimality. Therefore

$$
\boxed{I_\alpha=(m_\alpha)},
$$

where $m_\alpha$ is monic and irreducible.

For

$$
f(X)=X^4+2X^3-3X^2-4X-11,
$$

translation gives

$$
f(X+1)=X^4+6X^3+9X^2-15.
$$

This is Eisenstein at $p=3$, so $f(X+1)$ and therefore $f(X)$ are irreducible over $\mathbb Q$. Hence

$$
\boxed{\mathbb Q[X]/(f)\text{ is a field}}.
$$

Irreducibility and Gauss's lemma also show that $(f)$ is a [prime ideal](../../../../../prime-ideal.md) of $\mathbb Z[X]$, so

$$
\boxed{\mathbb Z[X]/(f)\text{ is an integral domain}}.
$$

It is not a field. The class of $2$ is nonzero but not a unit: reducing further modulo $2$ gives a nonzero quotient

$$
\mathbb F_2[X]/(\overline f),
$$

in which the image of $2$ is zero, whereas a unit must remain a unit under every unital quotient map. Thus

$$
\boxed{\mathbb Z[X]/(f)\text{ is not a field}}.
$$

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
