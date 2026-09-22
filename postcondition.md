# Postcondition

↑ **Parent:** [Formal specification](formal-specification.md)

The condition required of a final [program state](program-state.md) when a program finishes under its [precondition](precondition.md). The [summation loop verification](summation-loop-verification.md) requires returned value $s$ to satisfy $2s=n(n+1)$ and preserves the [input](input-computer-science.md) $n$. Relating the answer to the original [input](input-computer-science.md) matters: allowing the program to replace $n$ by zero would change the intended contract.

A [postcondition](postcondition.md) alone gives no promise of [algorithm termination](algorithm-termination.md). It also need not specify a unique [output](output-computing.md): $s\geq0$ allows many answers, while the exact [triangular number](triangular-number.md) equation determines one [integer](integer-split.md) answer for each permitted $n$. Stronger [postconditions](postcondition.md) express more obligations; proving only a weaker consequence cannot justify the stronger requirement.

## ↑ Ancestors (6)

1. [Formal specification](formal-specification.md)
2. [Formal verification](formal-verification.md)
3. [Algorithm correctness](algorithm-correctness.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Algorithm correctness](algorithm-correctness.md)
- [Formal specification](formal-specification.md)
- [Formal verification](formal-verification.md)
- [Hoare triple](hoare-triple.md)
- [Loop invariant](loop-invariant.md)
- [Partial correctness](partial-correctness.md)
- [Postcondition](postcondition.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Summation loop verification](summation-loop-verification.md)
- [Total correctness](total-correctness.md)
- [Vacuous truth](vacuous-truth.md)
- [Well-founded progress in recursion](well-founded-progress-in-recursion.md)
