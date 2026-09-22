<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Using the assumed [square-free polynomial](../../../../../square-free-polynomial.md) property, factor

$$
X^p-1=f_1\cdots f_r
$$

into distinct [monic polynomials](../../../../../monic-polynomial.md) that are [irreducible polynomials](../../../../../irreducible-polynomial.md), with $n_j=\deg f_j$. Part (b)(iii) identifies $T=\mathbb F_2[X]/(X^p-1)$ with $\prod_jK_j$, where $|K_j|=2^{n_j}$.

By the [first isomorphism theorem for rings](../../../../../first-isomorphism-theorem-for-rings.md), the image $S$ from part (c)(i) is $T/J$, where $J$ is the [kernel of a ring homomorphism](../../../../../kernel-of-a-ring-homomorphism.md). By part (a)(ii), $J=\prod_jJ_j$ for [ideals](../../../../../ideal.md) $J_j\subseteq K_j$. A [field](../../../../../field.md) has only the zero [ideal](../../../../../ideal.md) and the whole [field](../../../../../field.md) as [ideals](../../../../../ideal.md), so each $K_j/J_j$ is either $K_j$ or the [zero ring](../../../../../zero-ring.md). Consequently, for a subset $D\subseteq\{1,\ldots,r\}$,

$$
S\cong\prod_{j\in D}K_j.
$$

This is the [quotient of a finite product of fields](../../../../../quotient-of-a-finite-product-of-fields.md) principle. The subset is nonempty because $|U(S)|=p>2$, whereas the [zero ring](../../../../../zero-ring.md) has only one [unit](../../../../../unit-in-a-ring.md). By part (a)(i),

$$
\boxed{p=|U(S)|=\prod_{j\in D}(2^{n_j}-1)}.
$$

Each factor is a positive [integer](../../../../../integer-split.md). Since $p$ is a [prime number](../../../../../prime-number-split.md), exactly one factor is $p$ and all remaining factors are one. Thus

$$
\boxed{p=2^n-1\text{ for some }n\geq2},
$$

so $p$ is a [Mersenne prime](../../../../../mersenne-prime.md). If $n=ab$ with $a,b>1$, then $2^a-1$ would be a proper divisor of $2^{ab}-1$; thus $n$ is itself a [prime number](../../../../../prime-number-split.md), although only the displayed form is needed.

The assumed [square-free polynomial](../../../../../square-free-polynomial.md) property can also be checked directly: in [characteristic of a ring](../../../../../characteristic-of-a-ring.md) two, the [formal derivative](../../../../../formal-derivative.md) of $X^p-1$ is $X^{p-1}$ because $p$ is odd. These two [polynomials](../../../../../polynomial-split.md) have [greatest common divisor](../../../../../greatest-common-divisor.md) one, since $X$ does not divide $X^p-1$, so no repeated [irreducible polynomial](../../../../../irreducible-polynomial.md) factor occurs.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
