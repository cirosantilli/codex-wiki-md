# Total correctness

↑ **Parent:** [Algorithm correctness](algorithm-correctness.md)

[Total correctness](total-correctness.md) requires [partial correctness](partial-correctness.md) and [algorithm termination](algorithm-termination.md) for every [program state](program-state.md) allowed by the [precondition](precondition.md). For a deterministic sequential program, every permitted start must reach a final [program state](program-state.md) satisfying the [postcondition](postcondition.md) after finitely many steps. Thus an infinite execution can satisfy [partial correctness](partial-correctness.md), but refutes [total correctness](total-correctness.md) for a permitted start.

In the [summation loop verification](summation-loop-verification.md), the [loop invariant](loop-invariant.md) establishes the answer conditional on exit, and the [loop variant](loop-variant.md) establishes exit. Both parts matter: replacing the body by a step that never returns would defeat [total correctness](total-correctness.md) even if every completed iteration preserved the [loop invariant](loop-invariant.md). Likewise, a terminating loop with the wrong [sum](sum.md) fails [partial correctness](partial-correctness.md) and therefore fails [total correctness](total-correctness.md).

These obligations depend on the [formal specification](formal-specification.md). A program that rejects every [input](input-computer-science.md) might correctly implement a rejection service, but does not meet a contract promising a [sum](sum.md) for every nonnegative [integer](integer-split.md). A proof of [total correctness](total-correctness.md) also gives no particular physical response-time guarantee: [time complexity](time-complexity.md) and the execution environment require their own assumptions.

**Table of contents**

- [Algorithm termination](algorithm-termination.md)

## ↑ Ancestors (4)

1. [Algorithm correctness](algorithm-correctness.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Algorithm correctness](algorithm-correctness.md)
- [Formal specification](formal-specification.md)
- [Hoare triple](hoare-triple.md)
- [Loop variant](loop-variant.md)
- [Partial correctness](partial-correctness.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Summation loop verification](summation-loop-verification.md)
- [Total correctness](total-correctness.md)
- [Well-founded progress in recursion](well-founded-progress-in-recursion.md)
