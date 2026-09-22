# Partial correctness

↑ **Parent:** [Algorithm correctness](algorithm-correctness.md)

[Partial correctness](partial-correctness.md) means that every terminating execution begun in a [program state](program-state.md) satisfying the [precondition](precondition.md) $P$ finishes in a [program state](program-state.md) satisfying the [postcondition](postcondition.md) $Q$. For a sequential program $C$, the usual [Hoare triple](hoare-triple.md) notation is

$$
\{P\}\ C\ \{Q\}.
$$

Here the notation expresses [partial correctness](partial-correctness.md); it makes no promise that $C$ finishes. The [precondition](precondition.md) and [postcondition](postcondition.md) describe permitted starting circumstances and required final circumstances, rather than tests performed automatically by the program.[Hoare, 1969, §3 Program Execution, p. 577, and §4 General Reservations, pp. 578–579; the paper instead labels the precondition P, program Q and result R](an-axiomatic-basis-for-computer-programming-by-tony-hoare.md)

For a sharp example, take the [precondition](precondition.md) $n=4$ and the following sequential program over mathematical [integers](integer-split.md):
```
i = 0
s = 0
while i < n:
    i = i
```
The condition remains true, so execution never reaches the instruction after the loop. Consequently its [partial correctness](partial-correctness.md) claim holds for the [postcondition](postcondition.md) $2s=n(n+1)$, and even for the impossible [postcondition](postcondition.md) $0=1$: there is no terminating execution with a wrong final result. This is [vacuous truth](vacuous-truth.md), not evidence that the loop computes a [sum](sum.md). The same program fails [total correctness](total-correctness.md) for this permitted [input](input-computer-science.md).

The distinction is useful in a proof: first show that an answer, whenever produced, is right; then establish [algorithm termination](algorithm-termination.md). The [summation loop verification](summation-loop-verification.md) supplies both arguments for a loop that actually progresses. Its finite trace illustrates one execution, while its [loop invariant](loop-invariant.md) covers every permitted [input](input-computer-science.md).

## ↑ Ancestors (4)

1. [Algorithm correctness](algorithm-correctness.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Algorithm correctness](algorithm-correctness.md)
- [Algorithm termination](algorithm-termination.md)
- [Formal specification](formal-specification.md)
- [Hoare triple](hoare-triple.md)
- [Loop variant](loop-variant.md)
- [Partial correctness](partial-correctness.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Summation loop verification](summation-loop-verification.md)
- [Total correctness](total-correctness.md)
- [Vacuous truth](vacuous-truth.md)
