<h1 id="4h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Context-free languages](../../../../../../context-free-language.md) are closed under [union](../../../../../../set-union.md): use a new start symbol with alternatives for two renamed [context-free grammars](../../../../../../context-free-grammar.md). If they were closed under [complement](../../../../../../complement-of-a-set.md) in $\Sigma^*$, [De Morgan's laws](../../../../../../de-morgan-s-laws.md) would give

$$
 L_1\cap L_2=\Sigma^*\setminus\bigl((\Sigma^*\setminus L_1)\cup(\Sigma^*\setminus L_2)\bigr),
$$

contradicting the preceding [intersection](../../../../../../set-intersection.md) example. Therefore **some CFL has a non-context-free [complement](../../../../../../complement-of-a-set.md)**. This is an existence argument; it does not assert that both [complements](../../../../../../complement-of-a-set.md) of the particular $L_1,L_2$ are non-context-free.

A concrete choice is $L=\{a,b,c\}^*\setminus\{a^n b^n c^n:n\geq0\}$. Words outside $a^*b^*c^*$ form a [regular language](../../../../../../regular-language.md). Among words inside it, membership in $L$ means the first two counts or the last two counts differ. Each unequal-count comparison has a [context-free grammar](../../../../../../context-free-grammar.md): for $a^i b^j$ with $i>j$, use $T\to aTb\mid A$, $A\to aA\mid a$; for $i<j$, replace $A$ by $B\to bB\mid b$. Append any number of $c$'s, or prefix any number of $a$'s for the analogous $b,c$ comparison. Taking these [unions](../../../../../../set-union.md) gives a [context-free language](../../../../../../context-free-language.md) whose [complement](../../../../../../complement-of-a-set.md) is the non-context-free equal-three-count language. These productions are definitions of the example, not a restriction to strict [Chomsky normal form](../../../../../../chomsky-normal-form.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4H](../../4h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
