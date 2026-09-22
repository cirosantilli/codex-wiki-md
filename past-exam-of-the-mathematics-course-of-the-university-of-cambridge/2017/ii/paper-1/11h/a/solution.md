<h1 id="11h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) is described by finite state and alphabet label lists, one initial state label, an accepting-state bit mask, and a finite transition table. Keep each label in increasing order and list transitions lexicographically by the actual state and alphabet labels. This retains arbitrary finite subsets of the permitted labels, rather than assuming they are consecutive.

The [prime-exponent encoding of a finite list](../../../../../../prime-exponent-encoding-of-a-finite-list.md) gives an explicit [Gödel encoding](../../../../../../godel-numbering.md) for a list $(a_0,\ldots,a_{r-1})$ of [nonnegative integers](../../../../../../natural-number.md):

$$
\operatorname{code}(a_0,\ldots,a_{r-1})
=2^r\prod_{j=0}^{r-1}p_{j+2}^{a_j+1},
$$

where $p_i$ is the $i$th [prime number](../../../../../../prime-number.md). Encode the descriptor as a list beginning with the numbers of states and alphabet symbols, followed by their sorted labels, the start label, the accepting mask, and all transition destinations. The lengths are then known during decoding.

[Unique prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) recovers the list and hence the automaton. Reject an integer if the prescribed prime exponents are missing, additional primes occur, the list lengths disagree, state or alphabet labels repeat, the initial state or a transition target is absent, or the mask is out of range. These are effective finite checks. Thus every automaton has an integer code, valid codes are decidable, and the transition system of a coded automaton is computable. Invalid integers may be excluded explicitly or assigned a fixed empty-language automaton.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11H](../../11h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
