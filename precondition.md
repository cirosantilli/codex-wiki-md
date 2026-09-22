# Precondition

↑ **Parent:** [Formal specification](formal-specification.md)

The condition required of a starting [program state](program-state.md) for a stated correctness guarantee. In the [summation loop verification](summation-loop-verification.md), $n\in\mathbb Z$ and $n\geq0$ admit $n=0$ and $n=4$, but exclude $n=-1$. The accompanying model assumes exact [integer arithmetic](integer-arithmetic.md) and terminating elementary operations. The initial values of $i,s$ need no restriction because initialization overwrites them before use.

A [precondition](precondition.md) is a logical assumption, not automatically an executable check. Writing `require` in a procedure states its contract; an implementation that checks or rejects invalid [inputs](input-computer-science.md) needs that behavior specified too. Weakening a [precondition](precondition.md) admits more starts and therefore demands more proof: dropping $n\geq0$ here makes $n=-2$ a terminating [counterexample](counterexample.md) to $2s=n(n+1)$, since initialization returns zero while $n(n+1)=2$.

## ↑ Ancestors (6)

1. [Formal specification](formal-specification.md)
2. [Formal verification](formal-verification.md)
3. [Algorithm correctness](algorithm-correctness.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Algorithm correctness](algorithm-correctness.md)
- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Formal specification](formal-specification.md)
- [Hoare triple](hoare-triple.md)
- [Loop invariant](loop-invariant.md)
- [Partial correctness](partial-correctness.md)
- [Postcondition](postcondition.md)
- [Precondition](precondition.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Summation loop verification](summation-loop-verification.md)
- [Total correctness](total-correctness.md)
- [Well-founded progress in recursion](well-founded-progress-in-recursion.md)
