<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The [formal language](../../../../../../formal-language.md) is a [context-free language](../../../../../../context-free-language.md).** A [context-free grammar](../../../../../../context-free-grammar.md) with start [nonterminal symbol](../../../../../../nonterminal-symbol.md) $S$ is

$$
\boxed{S\to AB,\qquad A\to aAb\mid\varepsilon,\qquad B\to bBc\mid\varepsilon.}
$$

The [production rule](../../../../../../production-rule.md) for $A$ nests one $a$ on the left and one $b$ on the right on each recursive use, so $A$ generates exactly $a^mb^m$ for $m\geq0$. Similarly, $B$ generates exactly $b^nc^n$ for $n\geq0$. The start [production rule](../../../../../../production-rule.md) concatenates these [words](../../../../../../string.md), yielding

$$
a^mb^m b^nc^n=a^mb^{m+n}c^n.
$$

Conversely, every choice of nonnegative [integers](../../../../../../integer-split.md) $m,n$ is achieved by using the recursive [production rules](../../../../../../production-rule.md) exactly $m,n$ times before their [epsilon productions](../../../../../../epsilon-production.md). Hence this [context-free grammar](../../../../../../context-free-grammar.md) generates precisely the required [formal language](../../../../../../formal-language.md), including all cases where either count is zero.

## ↑ Ancestors (12)

1. [I](../i.md)
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
