<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

All [principal ideals](../../../../../principal-ideal.md) in this part are taken inside the [subring](../../../../../subring.md) $T$, rather than inside $\mathbb R[X]$. First, $T$ is a [subring](../../../../../subring.md): sums and [additive inverses](../../../../../additive-inverse.md) retain zero [coefficient](../../../../../coefficient.md) of $X$, and the [coefficient](../../../../../coefficient.md) of $X$ in a product $uv$ is $u(0)[X]v+v(0)[X]u=0$. It contains $1$.

The [principal ideal](../../../../../principal-ideal.md) $I=(X^3)_T=X^3T$ is precisely

$$
I=\left\{a_3X^3+\sum_{j\geq5}a_jX^j:\text{only finitely many }a_j\ne0\right\}.
$$

Indeed, multiplying an element of $T$ by $X^3$ gives a possible term of [polynomial degree](../../../../../degree-of-a-polynomial.md) $3$ and terms of [polynomial degrees](../../../../../degree-of-a-polynomial.md) at least $5$, with no $X^4$ term. Conversely, dividing any displayed [polynomial](../../../../../polynomial-split.md) by $X^3$ gives a [polynomial](../../../../../polynomial-split.md) with no $X$ term, hence an element of $T$.

Given $p\in T$, let $a,b,c$ be its [coefficients](../../../../../coefficient.md) of $1,X^2,X^4$, respectively. Subtracting these terms leaves an element of $I$, so

$$
\boxed{p+I=a+bX^2+cX^4+I}.
$$

For uniqueness, if two such representatives differ by an element of $I$, their difference has possible [monomials](../../../../../monomial.md) only $1,X^2,X^4$, whereas every element of $I$ has zero [coefficients](../../../../../coefficient.md) at all three. Comparing [coefficients](../../../../../coefficient.md) gives $a=a'$, $b=b'$, $c=c'$.

In particular, $X^4\notin I$. Treating $I$ as the [principal ideal](../../../../../principal-ideal.md) of $\mathbb R[X]$ instead would incorrectly discard this surviving term.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
