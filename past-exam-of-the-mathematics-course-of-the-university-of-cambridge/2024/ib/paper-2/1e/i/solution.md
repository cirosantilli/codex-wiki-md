<h1 id="1e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
P_n(X)=1+X+\cdots+X^{n-1}.
$$

If $n=ab$ with $a,b>1$, then

$$
P_n(X)=\left(1+X+\cdots+X^{a-1}\right)
\left(1+X^a+\cdots+X^{a(b-1)}\right),
$$

so $P_n$ is reducible.

Conversely, let $n=p$ be prime. Translation by one is an automorphism of $\mathbb Z[X]$, and

$$
P_p(X+1)=\frac{(X+1)^p-1}{X}
=\sum_{k=1}^p\binom pkX^{k-1}.
$$

Its leading coefficient is one, every lower coefficient is divisible by $p$, and its constant coefficient is $p$, which is not divisible by $p^2$. The [Eisenstein criterion](../../../../../../eisenstein-criterion.md) proves that $P_p(X+1)$ is irreducible, hence so is $P_p(X)$. Therefore the [geometric-sum irreducibility criterion](../../../../../../geometric-sum-irreducibility-criterion.md) is

$$
\boxed{1+X+\cdots+X^{n-1}\text{ is irreducible in }\mathbb Z[X]
\Longleftrightarrow n\text{ is prime}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1E](../../1e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
