<h1 id="4i/solution">Solution</h1>

↑ **Parent:** [4I](../4i.md)

A [context-free grammar](../../../../../context-free-grammar.md) is in [Chomsky normal form](../../../../../chomsky-normal-form.md) when every production has one of the forms

$$
A\to BC,
\qquad
A\to a,
$$

where $A,B,C$ are nonterminals and $a$ is a terminal. One may additionally allow $S\to\epsilon$ when the empty word belongs to the language, usually with the restriction that the start symbol does not occur on a right-hand side.

An $\epsilon$-production has the form $A\to\epsilon$. A [unit production](../../../../../unit-production.md) has the form $A\to B$ for nonterminals $A,B$.

In $G_1$, the productions for $T$ give

$$
L_{G_1}(T)=\{c\}\{a,b\}^*.
$$

Consequently

$$
L(G_1)
=\{\epsilon\}
\cup
\{a,b\}c\{a,b\}^*a.
$$

In $G_2$, $X$ and $Y$ generate $a$ and $b$, while $T\to TX\mid TY\mid c$ again gives

$$
L_{G_2}(T)=\{c\}\{a,b\}^*.
$$

Since $Z\to TX$, the two start productions $S\to XZ\mid YZ$ generate exactly

$$
L(G_2)=\{a,b\}c\{a,b\}^*a.
$$

Thus

$$
\boxed{L(G_2)=L(G_1)\setminus\{\epsilon\}}.
$$

Every production of $G_2$ has the required binary-nonterminal or single-terminal form, so $G_2$ is the Chomsky-normal-form grammar for the nonempty part of $L(G_1)$.

## ↑ Ancestors (10)

1. [4I](../4i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
