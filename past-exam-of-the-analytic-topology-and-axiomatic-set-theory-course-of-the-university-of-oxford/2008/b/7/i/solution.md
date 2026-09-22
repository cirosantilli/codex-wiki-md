<h1 id="b/7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[König theorem for cardinal numbers](../../../../../konig-s-theorem-set-theory.md) states that if $\kappa_i<\lambda_i$ for each index $i\in I$, then

$$
\boxed{\sum_{i\in I}\kappa_i<\prod_{i\in I}\lambda_i.}
$$

Represent each [cardinal](../../../../../cardinal-number-split.md) by its [initial ordinal](../../../../../initial-ordinal.md), let $A=\{(i,\alpha):i\in I,\alpha<\kappa_i\}$, and let $B=\prod_{i\in I}\lambda_i$.

First there is an [injection](../../../../../injective-function.md) $A\to B$: encode $(i,\alpha)$ by the [function](../../../../../function-split.md) which is zero away from $i$ and takes value $\alpha+1$ at $i$. The nonzero coordinate identifies $i$, and its value identifies $\alpha$. It is valid because $\alpha+1\le\kappa_i<\lambda_i$; an index with $\kappa_i=0$ contributes no domain points.

For strictness suppose a surjection $F:A\to B$ existed. At coordinate $i$, the values $F(i,\alpha)(i)$ for $\alpha<\kappa_i$ occupy fewer than $\lambda_i$ possibilities. Choose $b_i$ as the least [ordinal](../../../../../ordinal-split.md) below $\lambda_i$ absent from that [set](../../../../../set-split.md). The resulting $b=(b_i)\in B$ differs from $F(i,\alpha)$ at coordinate $i$ for every $(i,\alpha)\in A$, contradicting [surjectivity](../../../../../surjective-function.md).

An [injection](../../../../../injective-function.md) $B\to A$ would produce a surjection $A\to B$ by inverting on its image and assigning the zero [function](../../../../../function-split.md) elsewhere. It is therefore impossible. The [injection](../../../../../injective-function.md) in the first direction and impossibility of the reverse give the strict [cardinal](../../../../../cardinal-number-split.md) inequality. This diagonal argument uses the canonical well-orders of the specified [cardinals](../../../../../cardinal-number-split.md) to choose missing coordinate values, rather than an unexplained arbitrary choice at that step.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
