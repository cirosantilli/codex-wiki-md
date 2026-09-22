<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [polynomial](../../../../polynomial-split.md) $X^n-2$ is irreducible over $\mathbb Q$ by [Eisenstein's criterion](../../../../eisenstein-criterion.md) with prime two: all [coefficients](../../../../coefficient.md) except the leading one are divisible by two, while the constant [coefficient](../../../../coefficient.md) is not divisible by four. Together with [Gauss's lemma](../../../../gauss-s-lemma-riemannian-geometry.md), this establishes irreducibility in $\mathbb Q[X]$. Part (b) shows that its [principal ideal](../../../../principal-ideal.md) is a [maximal ideal](../../../../maximal-ideal.md), so

$$
\boxed{K_n=\mathbb Q[X]/(X^n-2)\text{ is a field}.}
$$

Let $\alpha$ denote the residue class of $X$. The [polynomial division algorithm](../../../../polynomial-division.md) gives every residue class a representative of degree less than $n$, so $1,\alpha,\ldots,\alpha^{n-1}$ span $K_n$ over $\mathbb Q$. If a [linear combination](../../../../linear-combination.md) of them vanished, its degree-less-than-$n$ representative would be a multiple of the degree-$n$ [polynomial](../../../../polynomial-split.md) $X^n-2$, and hence would be zero. They are therefore a [basis](../../../../basis.md), giving

$$
\boxed{\dim_{\mathbb Q}K_n=n.}
$$

The [quadratic polynomial](../../../../quadratic-polynomial.md) $X^2+1$ has no rational root, so it is irreducible over $\mathbb Q$. The same maximal-ideal argument proves **$L=\mathbb Q[X]/(X^2+1)$ is a [field](../../../../field.md)**.

These two quadratic fields are **not isomorphic**. In $L$, the class of $X$ squares to $-1$. But $K_2$ embeds in $\mathbb R$ by sending its class of $X$ to $\sqrt2$: evaluation at $\sqrt2$ has kernel $(X^2-2)$, by irreducibility and [polynomial](../../../../polynomial-split.md) division. No [real number](../../../../real-number.md) squares to $-1$, so no element of $K_2$ does. A [field isomorphism](../../../../field-isomorphism.md) preserves one, minus one and squaring, so it cannot carry $L$ to $K_2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
