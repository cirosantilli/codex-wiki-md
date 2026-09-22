<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Every generated [word](../../../../../../string.md) satisfies

$$
\#_b(w)\geq\#_a(w),
$$

where $\#_a,\#_b$ count occurrences of the indicated [terminal symbols](../../../../../../terminal-symbol.md). To see this, follow the unique chain of $S$ occurrences in a [parse tree](../../../../../../parse-tree.md). Each use of $S\to UST$ introduces one $a$ from $U$, at least one $b$ from its rightmost $T$, and possibly one further $b$ from $U\to aT$. Each use of $S\to ST$ adds one $b$ and no $a$. The terminating $S\to\varepsilon$ contributes neither. Hence no generated [word](../../../../../../string.md) has more $a$ symbols than $b$ symbols.

Also, for every $n\geq0$, the [word](../../../../../../string.md) $a^nb^n$ is generated: apply $S\to UST$ exactly $n$ times, choose $U\to a$ each time, then use $S\to\varepsilon$ and all remaining $T\to b$.

Suppose $L(G)$ were a [regular language](../../../../../../regular-language.md), and let $p\geq1$ be a [pumping length](../../../../../../pumping-length.md) from the [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md). Apply it to $w=a^pb^p$. Every allowed decomposition $w=xyz$ with $|xy|\leq p$ and $|y|>0$ has $y=a^r$ for some $r\geq1$. Pumping twice gives

$$
xy^2z=a^{p+r}b^p,
$$

which violates the proved counting inequality and hence is not generated. This contradicts the [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md). **Therefore $L(G)$ is not a [regular language](../../../../../../regular-language.md).** Ambiguity was not used: the obstruction is the unbounded constraint on symbol counts.

$$
\boxed{L(G)\text{ is not regular}.}
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
