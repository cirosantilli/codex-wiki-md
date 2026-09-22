<h1 id="4h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat the fixed letters $a_1,\ldots,a_n$, the empty-language and empty-word symbols, and the punctuation of expressions as a finite token alphabet. In the usual syntax allowing parentheses, union, concatenation, and star, the following [context-free grammar](../../../../../../context-free-grammar.md) generates exactly the syntactically valid [regular expressions](../../../../../../regular-expression.md):

$$
E\to\varnothing\mid\varepsilon\mid a_1\mid\cdots\mid a_n
\mid(E)\mid E+E\mid EE\mid E^*.
$$

Structural induction proves that every generated string is an expression and that every expression has a derivation. Grammar ambiguity does not affect the [context-free language](../../../../../../context-free-language.md) assertion.

If the language of these expressions were a [regular language](../../../../../../regular-language.md), its intersection with the regular token language consisting of some opening parentheses, then $a_1$, then some closing parentheses would be regular. That intersection is exactly

$$
\{\mathtt{(}^{\,r}a_1\mathtt{)}^{\,r}:r\ge0\}.
$$

The [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md) contradicts regularity: a sufficiently long opening-parenthesis prefix forces a pumpable segment wholly within that prefix, and pumping it changes the two parenthesis counts unequally. Hence **the expression syntax is context-free but not regular**. This conclusion concerns the strings describing expressions, not the languages those expressions denote; it uses the usual concrete syntax with arbitrary nested parentheses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4H](../../4h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
