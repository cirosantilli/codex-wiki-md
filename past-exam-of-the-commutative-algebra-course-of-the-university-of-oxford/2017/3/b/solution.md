<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $P$ be a [prime ideal](../../../../prime-ideal.md) of $R$ disjoint from the [multiplicatively closed set](../../../../multiplicatively-closed-set.md) $Y$. In the [localization](../../../../localization-of-a-ring.md) $S=Y^{-1}R$, its [extension of an ideal](../../../../extension-of-an-ideal.md) is

$$
SP=\{p/y:p\in P,\ y\in Y\}.
$$

Indeed, finite sums of such fractions have a common denominator in $Y$ and numerator in $P$, and every generator $p/1$ has this form.

We show that its [contraction of an ideal](../../../../contraction-of-an-ideal.md) recovers $P$:

$$
\boxed{\{r\in R:r/1\in SP\}=P.}
$$

One inclusion is immediate. Conversely, if $r/1=p/y$ with $p\in P$ and $y\in Y$, equality of fractions in the [field of fractions](../../../../field-of-fractions.md) of the [integral domain](../../../../integral-domain.md) $R$ gives $yr=p\in P$. Since $y\notin P$ and $P$ is a [prime ideal](../../../../prime-ideal.md), $r\in P$.

If $SP_1=SP_2$, contracting would therefore give $P_1=P_2$, contrary to the hypothesis. Hence

$$
\boxed{SP_1\ne SP_2.}
$$

We will also need the fact that $SP$ is a [prime ideal](../../../../prime-ideal.md), part of the [prime ideal correspondence for localization](../../../../prime-ideal-correspondence-for-localization.md). It is proper by the contraction identity, since otherwise $1\in P$. If $(a/u)(b/v)\in SP$, multiplication by the denominator gives $ab/1\in SP$, and contraction gives $ab\in P$. Thus $a\in P$ or $b\in P$, so one of the two fractions belongs to $SP$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
