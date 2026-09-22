# Finite-state path expression

↑ **Parent:** [State elimination for finite automata](state-elimination-for-finite-automata.md)

For numbered states of a [finite-state automaton](finite-state-machine.md), $R_{ij}^{(k)}$ is a [regular expression](regular-expression.md) describing paths from $i$ to $j$ whose internal states have numbers at most $k$. Splitting a path at its visits to state $k$ gives $R_{ij}^{(k)}=R_{ij}^{(k-1)}+R_{ik}^{(k-1)}(R_{kk}^{(k-1)})^*R_{kj}^{(k-1)}$. At stage zero use individual edge labels and an empty-word option when the endpoints coincide. This proves the automaton-to-expression direction of [Kleene theorem](kleene-theorem.md).

## ↑ Ancestors (8)

1. [State elimination for finite automata](state-elimination-for-finite-automata.md)
2. [Generalized finite automaton](generalized-finite-automaton.md)
3. [Finite-state machine](finite-state-machine.md)
4. [Formal language theory](formal-language-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/1/solution.md)
