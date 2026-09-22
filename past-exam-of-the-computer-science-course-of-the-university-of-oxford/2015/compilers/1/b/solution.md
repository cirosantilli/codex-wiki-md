<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [lexical tokens](../../../../../lexical-token.md) `ID`, `ASSIGN`, `SEMI`, `BEGIN`, `END`, `CASE`, `OF`, `COLON`, and `BAR`, corresponding to identifiers and the displayed punctuation or keywords. Let `E` be the already defined [context-free grammar](../../../../../context-free-grammar.md) category for a [program expression](../../../../../program-expression.md), with attribute `E.tree`; expressions do not consume statement delimiters except inside their own explicitly delimited constructs. `ID.name` is the recognized [program identifier](../../../../../program-identifier.md). The following [context-free grammar](../../../../../context-free-grammar.md) uses `S` for a statement, `C` for a closed elementary statement, `D` for a nonempty sequence of closed statements, and `A` for a nonempty arm list. The braces in this display are [semantic actions](../../../../../semantic-action.md), not input [lexical tokens](../../../../../lexical-token.md).

```
S -> C                       { S.tree = C.tree }
S -> C SEMI S1               { S.tree = Seq(C.tree, S1.tree) }
S -> CASE E OF A             { S.tree = Case(E.tree, A.arms) }

C -> ID ASSIGN E             { C.tree = Assign(ID.name, E.tree) }
C -> BEGIN S END             { C.tree = S.tree }

D -> C                       { D.tree = C.tree }
D -> C SEMI D1               { D.tree = Seq(C.tree, D1.tree) }

A -> E COLON S               { A.arms = [(E.tree, S.tree)] }
A -> E COLON D BAR A1        { A.arms = [(E.tree, D.tree)] ++ A1.arms }
```

Here `++` is [list concatenation](../../../../../list-concatenation.md), and distinct suffixes distinguish occurrences of the same [nonterminal symbol](../../../../../nonterminal-symbol.md). Every statement and arm body is nonempty; no empty statement or optional trailing semicolon is needed for the supplied language.

The distinction between `D` and `S` resolves both possible sources of [grammar ambiguity](../../../../../ambiguous-grammar.md). First, an unbracketed `CASE` can occur only at the right end of an `S`: there is no production `S -> S SEMI S`. Consequently all semicolon-separated statements after such a `CASE` enter its last arm. Enclosing that whole `CASE` in `BEGIN ... END` turns it into a `C`, which can be followed by another statement outside the `CASE`.

Second, an arm followed by another arm at the same level must have a `D` body. Such a body contains no unbracketed `CASE`. If an arm body does contain an unbracketed `CASE`, only the final-arm production `A -> E COLON S` can apply, and every following `BAR` before the enclosing `END` or end of input must be consumed by the inner `CASE`. Thus each bar belongs to the nearest preceding `CASE` whose block has not ended. A `CASE` inside `BEGIN ... END` is hidden from that rule outside its block.

For uniqueness, at any statement level an initial `ID` or `BEGIN` determines a `C`; an immediately following `SEMI` determines the recursive sequence production. An initial `CASE` determines the third `S` production. In an arm, a bar at the current block level either follows an entirely closed body, forcing the second `A` production, or follows an unbracketed nested `CASE`, forcing it into that inner arm list. With an unambiguous expression sublanguage these choices leave a unique [parse tree](../../../../../parse-tree.md). **Closed bodies before an outer bar, and a possibly open body only in the final arm, enforce the required interpretation.** Thus the [context-free grammar](../../../../../context-free-grammar.md) implements

$$
\boxed{\text{nearest open case for each bar; following statements enter its last arm}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
