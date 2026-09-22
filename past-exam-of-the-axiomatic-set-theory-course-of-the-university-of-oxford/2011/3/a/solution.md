<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual [cardinal arithmetic](../../../../cardinal-arithmetic.md) with the [axiom of choice](../../../../axiom-of-choice.md). The [König theorem for cardinal numbers](../../../../konig-s-theorem-set-theory.md) states that for any index set $I$ and [cardinal numbers](../../../../cardinal-number-split.md) $\kappa_i<\lambda_i$,

$$
\boxed{\sum_{i\in I}\kappa_i<\prod_{i\in I}\lambda_i.}
$$

Represent the [cardinal numbers](../../../../cardinal-number-split.md) as [initial ordinals](../../../../initial-ordinal.md). Let $A=\{(i,\alpha):i\in I,\alpha<\kappa_i\}$ and $B=\prod_{i\in I}\lambda_i$. There is an [injection](../../../../injective-function.md) $A\to B$: send $(i,\alpha)$ to the function whose $i$th coordinate is $\alpha+1$ and whose other coordinates are zero. The unique nonzero coordinate identifies $i$, and its value identifies $\alpha$. All values are allowed because $\alpha+1\leq\kappa_i<\lambda_i$.

For any proposed [surjection](../../../../surjective-function.md) $F:A\to B$, its $i$th row has at most $\kappa_i$ elements, so

$$
\{F(i,\alpha)(i):\alpha<\kappa_i\}\ne\lambda_i.
$$

Choose $b_i$ to be the least omitted [ordinal](../../../../ordinal-split.md). The function $b=(b_i)_{i\in I}$ belongs to $B$ and differs from $F(i,\alpha)$ at coordinate $i$, for every $(i,\alpha)\in A$. Thus $F$ is not surjective. Cardinal comparison now gives the strict inequality. If $I=\varnothing$, the conclusion is $0<1$, also valid.

## ↑ Ancestors (12)

1. [A](../a.md)
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
