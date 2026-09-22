<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the [permanent of a matrix](../../../../../../permanent-mathematics.md) as the total weight of the [cycle covers](../../../../../../cycle-cover-of-a-directed-graph.md) of its weighted directed graph. Valiant's reduction builds a graph from three constant-size components.

- A [Variable gadget in Valiant's permanent reduction](../../../../../../variable-gadget-in-valiant-s-permanent-reduction.md) has exactly two relevant cycle-cover states, representing true and false, and exposes occurrence ports consistent with the selected state.
- A [Clause gadget in Valiant's permanent reduction](../../../../../../clause-gadget-in-valiant-s-permanent-reduction.md) has external ports for its three literals and contributes a fixed total weight exactly when at least one selected literal satisfies the clause.
- An [Exclusive-or gadget in Valiant's permanent reduction](../../../../../../exclusive-or-gadget-in-valiant-s-permanent-reduction.md) joins occurrence ports while allowing exactly one of two corresponding external edges. Its edges have weights in $\{-1,0,1\}$; unwanted cycle covers occur in sign-reversing pairs and cancel.

Wire one variable port to every literal occurrence and one clause port to each literal. The balanced-occurrence hypothesis lets the true and false tracks of each variable be paired without extra weighting. A routine gadget case analysis shows that cycle covers surviving cancellation correspond to satisfying assignments, each with the same fixed multiplicity and sign. A small normalization gadget removes that fixed factor, or it can be tracked explicitly. The construction has constant size per variable, clause, and occurrence, so it is a polynomial-time counting reduction from [Balanced number 3-SAT](../../../../../../balanced-number-3-sat.md) to the permanent of a $\{-1,0,1\}$ matrix.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
