<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The [formal language](../../../../../../formal-language.md) is not a [context-free language](../../../../../../context-free-language.md).** Suppose otherwise, and let $p\geq1$ be a [pumping length](../../../../../../pumping-length.md) from the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md). Choose

$$
w=a^p b^{p^2}c^p.
$$

This [word](../../../../../../string.md) belongs to the [formal language](../../../../../../formal-language.md), since its middle exponent is the product of the two outer exponents. The [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md) would give

$$
w=uvxyz,\qquad |vxy|\leq p,\qquad |vy|>0,
$$

with $uv^ixy^iz$ in the [formal language](../../../../../../formal-language.md) for every [integer](../../../../../../integer-split.md) $i\geq0$.

Let $\alpha,\beta,\gamma$ be the respective numbers of $a,b,c$ symbols in the two pumped pieces $v,y$ together. The window $vxy$ cannot contain both an $a$ and a $c$: it would have to contain the entire middle block of length $p^2$, plus at least those two outer symbols, exceeding $p$. Hence

$$
\alpha\gamma=0,\qquad 1\leq\alpha+\beta+\gamma\leq p.
$$

Pump once extra, taking $i=2$. The resulting symbol counts are $p+\alpha$, $p^2+\beta$, and $p+\gamma$. A necessary condition for membership, regardless of whether the block order survives, is

$$
p^2+\beta=(p+\alpha)(p+\gamma),
\quad\text{or equivalently}\quad
\beta=p(\alpha+\gamma),
$$

where $\alpha\gamma=0$ was used.

If $\alpha+\gamma=0$, then $\beta>0$, contradicting that equality. If $\alpha+\gamma\geq1$, then

$$
\beta\leq p-(\alpha+\gamma)<p\leq p(\alpha+\gamma),
$$

again contradicting it. Thus every permissible decomposition fails at $i=2$. This contradicts the [pumping lemma for context-free languages](../../../../../../pumping-lemma-for-context-free-languages.md) and proves the claim. The obstruction is the [multiplicative block-count language](../../../../../../multiplicative-block-count-language.md): a bounded local change cannot preserve the product constraint.

$$
\boxed{\{a^m b^{mn}c^n:m,n\geq0\}\text{ is not context-free}.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
