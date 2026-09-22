# Bounded-difference automaton

↑ **Parent:** [Group multiplier automaton](group-multiplier-automaton.md)

For a fixed finite generating alphabet and integer $K$, use the elements of the word-metric ball $B_K(1)$ as states, together with a reject state and padding-status flags. Starting at the identity, a padded letter pair $(u,v)$ changes the state to $u^{-1}dv$ if it stays in the ball. A padding letter acts as the identity. Final state $a$ recognizes endpoint difference $a$ among pairs whose prefixes remain within $K$. On a regular synchronous [combing](combing-of-a-group.md), intersecting with the two word acceptors gives the full [group multiplier automaton](group-multiplier-automaton.md). It does not recognize unrestricted endpoint relations for all input words.

## ↑ Ancestors (8)

1. [Group multiplier automaton](group-multiplier-automaton.md)
2. [Automatic structure for a group](automatic-structure-for-a-group.md)
3. [Automatic group](automatic-group.md)
4. [Geometric group theory](geometric-group-theory-split.md)
5. [Geometry and topology](geometry-and-topology-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5/4/iii/solution.md)
