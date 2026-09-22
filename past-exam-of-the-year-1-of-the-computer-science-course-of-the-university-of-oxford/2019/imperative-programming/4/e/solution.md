<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Give each solving session a shared visited [set](../../../../../set-split.md) keyed by immutable snapshots of [permutation](../../../../../permutation.md) contents, for example `game.toList`, and insert the initial snapshot immediately. Have all successor objects refer to that same session's set. The refined `flip` first constructs the candidate state; if its key is present, return `None`. Otherwise add the key immediately and return `Some(candidate)`. The search enqueues only `Some` results. Keys must compare contents rather than [array](../../../../../array-data-structure.md) identities, and a fresh solving session must start with a fresh visited set.

Marking at generation time prevents the same state from being queued repeatedly, including the immediate cycle made by applying the same reversal twice. **First discovery in [breadth-first search](../../../../../breadth-first-search.md) already has minimum depth**, so discarding later discoveries cannot remove a shorter solution. The graph now has at most $n!$ admitted states. If only cycles along one path were to be rejected, a path-local set would suffice, but it would still repeat states reached by different paths; the shared session-wide set avoids both kinds of repetition. Public game fields must not be externally mutated while their states are being searched.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
