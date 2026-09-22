<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

A [context-free grammar](../../../../../context-free-grammar.md) is in [Chomsky normal form](../../../../../chomsky-normal-form.md) when every production has the form $A\to BC$ or $A\to a$, where $A,B,C$ are [nonterminals](../../../../../nonterminal-symbol.md) and $a$ is a [terminal symbol](../../../../../terminal-symbol.md); one may additionally allow the new start production $S_0\to\epsilon$ when the language contains the [empty string](../../../../../empty-word.md), provided $S_0$ never appears on a right-hand side.

The standard conversion proceeds as follows.

- Introduce a fresh start symbol $S_0$ and $S_0\to S$. This changes $N$ only when the old start symbol occurs on a right-hand side or when a protected start symbol is needed to preserve $\epsilon$.
- Find all nullable nonterminals, add productions obtained by omitting nullable occurrences, and remove the original $\epsilon$-productions except the permitted $S_0\to\epsilon$. This leaves $N$ unchanged.
- Eliminate each [unit production](../../../../../unit-production.md) $A\to B$ by adding to $A$ the non-unit productions reachable through its transitive closure. This leaves $N$ unchanged.
- Delete non-generating symbols and then unreachable symbols. This is the only simplification stage that can shrink $N$.
- In every right-hand side of length at least two, replace a terminal $a$ by a fresh nonterminal $T_a$ with $T_a\to a$. New nonterminals are needed exactly for terminals that occur in such mixed or long productions.
- Break every right-hand side of length at least three into binary productions, introducing fresh nonterminals for successive suffixes. New nonterminals are needed exactly when such long productions remain.

The terminal alphabet $\Sigma$ may be kept unchanged throughout, although unused terminals may be discarded by convention. Every stage preserves the generated language, with the explicit protection of $\epsilon$ at the start-symbol stage. For example,

$$
S\to SS\mid a
$$

is already in [Chomsky normal form](../../../../../chomsky-normal-form.md) and generates the infinite language $\{a^n:n\geq1\}$, so its conversion may be the grammar itself.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
