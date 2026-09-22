<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In this [localization of a ring](../../../../localization-of-a-ring.md), a nonzero fraction $a/b$ with odd $b$ is a [unit](../../../../unit-in-a-ring.md) exactly when $a$ is odd: its reciprocal then has odd denominator; if $a$ is even, an inverse would equate an even integer with an odd one after clearing denominators. Consequently every nonzero element has a unique form

$$
x=2^r u,\qquad r\geq0,\quad u\in R^\times.
$$

Here $r$ is the exponent of $2$ in the numerator of the reduced fraction, its nonnegative [2-adic valuation](../../../../2-adic-valuation.md).

Every nonzero [ideal](../../../../ideal.md) has the form $dR$ by part (c). Write the nonzero integer $d=2^r v$ with $v$ odd; since $v$ is a [unit](../../../../unit-in-a-ring.md), $dR=2^rR$. Hence the nonzero proper [ideals](../../../../ideal.md) are exactly

$$
\boxed{2^rR=\{a/b\in R:2^r\mid a\},\qquad r=1,2,3,\ldots.}
$$

The [zero ideal](../../../../zero-ideal.md) and $R=2^0R$ complete the full list. These ideals are distinct: $2^r$ does not belong to $2^{r+1}R$, since $1/2\notin R$.

The reduction map $a/b\mapsto a\bmod2$ is a well-defined surjective [ring homomorphism](../../../../ring-homomorphism.md) $R\to\mathbb F_2$ with [kernel of a ring homomorphism](../../../../kernel-of-a-ring-homomorphism.md) $2R$; odd denominators reduce to $1$. Thus $R/2R\cong\mathbb F_2$ is a [field](../../../../field.md), so $2R$ is a [prime ideal](../../../../prime-ideal.md) and $2$ is a [prime element](../../../../prime-element.md). Every nonzero [nonunit](../../../../nonunit.md) is associated to $2^r$ with $r\geq1$. If $r\geq2$, the factorization $2^r=2\cdot2^{r-1}$ is into two [nonunits](../../../../nonunit.md), so it is not an [irreducible element](../../../../irreducible-element.md) and therefore not a [prime element](../../../../prime-element.md). We conclude

$$
\boxed{\text{The sole prime element up to units is }2.}
$$

The failed step in the argument of part (b) is the guarantee that the product plus one is a nonunit and hence has an irreducible factor. Here every [prime element](../../../../prime-element.md) is an even fraction, so a product of [prime elements](../../../../prime-element.md) plus $1$ is an odd fraction, therefore a [unit](../../../../unit-in-a-ring.md). Already $2+1=3$ has no prime divisor in this ring. In $k[t]$, positive degree prevented that failure.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
