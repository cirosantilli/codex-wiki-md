# Formal specification

↑ **Parent:** [Formal verification](formal-verification.md)

A mathematically precise description of permitted behaviour. A [formal specification](formal-specification.md) for the [microkernel file-read example](microkernel-file-read-example.md)'s service could relate an authorized request to the exact returned [bytes](byte.md); a [formal specification](formal-specification.md) of its [microkernel](microkernel.md)'s [IPC](inter-process-communication.md) need only describe the protected transport operation. They state different obligations.

For the [summation loop verification](summation-loop-verification.md), require a nonnegative [integer](integer-split.md) [input](input-computer-science.md) $n$ and a returned value $s$ satisfying $2s=n(n+1)$. The [formal specification](formal-specification.md) describes what answer is acceptable without requiring this particular loop: another implementation may satisfy the same contract. State separately whether [partial correctness](partial-correctness.md) or [total correctness](total-correctness.md) is required. A [Hoare triple](hoare-triple.md) packages the [precondition](precondition.md), the program and the [postcondition](postcondition.md); [Hoare logic](hoare-logic.md) supplies rules for establishing such claims.

Precision alone does not ensure a useful requirement. The [postcondition](postcondition.md) $s\geq0$ permits returning zero for every nonnegative [integer](integer-split.md) [input](input-computer-science.md); it does not specify the intended [triangular number](triangular-number.md). Conversely, an impossible [precondition](precondition.md) permits no starts, making a universal correctness claim vacuous. Check both that intended [inputs](input-computer-science.md) are admitted and that admitted [outputs](output-computing.md) express the intended task.

**Table of contents**

- [Precondition](precondition.md)
- [Postcondition](postcondition.md)

## ↑ Ancestors (5)

1. [Formal verification](formal-verification.md)
2. [Algorithm correctness](algorithm-correctness.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Abstraction function](abstraction-function.md)
- [Algorithm correctness](algorithm-correctness.md)
- [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)
- [Formal specification](formal-specification.md)
- [Formal verification](formal-verification.md)
- [Functional correctness](functional-correctness.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [seL4 verification scope](sel4-verification-scope.md)
- [Total correctness](total-correctness.md)
