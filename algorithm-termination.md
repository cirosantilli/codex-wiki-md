# Algorithm termination

↑ **Parent:** [Total correctness](total-correctness.md)

[Algorithm termination](algorithm-termination.md) means that execution finishes after finitely many steps on the [inputs](input-computer-science.md) under consideration. Specify that domain: the stalled loop in [partial correctness](partial-correctness.md) terminates for $n=0$ but runs forever for $n=4$. A successful run on one [input](input-computer-science.md) does not establish termination on another.

A useful method is a [loop variant](loop-variant.md) $V$ that is a nonnegative [integer](integer-split.md) at every condition check and strictly decreases whenever the condition is true and the body completes. Also prove that condition evaluation and each body execution terminate. An infinite run would then give an infinite strictly decreasing [sequence](sequence.md) of nonnegative [integers](integer-split.md), contradicting their [well-founded relation](well-founded-relation.md). This establishes [algorithm termination](algorithm-termination.md) without enumerating all executions.

For the [summation loop verification](summation-loop-verification.md), $V=n-i$ begins at $n$ and decreases by exactly one per iteration. The body executes exactly $n$ times, including zero times for $n=0$. Merely bounding a decreasing measure below is insufficient for [real numbers](real-number.md): $1,1/2,1/4,\ldots$ decreases forever while staying positive. The choice of a [well-founded relation](well-founded-relation.md) supplies the essential progress argument; [well-founded progress in recursion](well-founded-progress-in-recursion.md) applies the same idea to [recursive calls](recursive-call.md).

## ↑ Ancestors (5)

1. [Total correctness](total-correctness.md)
2. [Algorithm correctness](algorithm-correctness.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Algorithm correctness](algorithm-correctness.md)
- [Algorithm termination](algorithm-termination.md)
- [Base case](base-case.md)
- [Binary array sum by recursion](binary-array-sum-by-recursion.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Linear probing](linear-probing.md)
- [Loop variant](loop-variant.md)
- [Matrix-chain split reconstruction](matrix-chain-split-reconstruction.md)
- [Partial correctness](partial-correctness.md)
- [Postcondition](postcondition.md)
- [Prefix maximum correctness example](prefix-maximum-correctness-example.md)
- [Recursion (computer science)](recursion-computer-science.md)
- [Summation loop verification](summation-loop-verification.md)
- [Total correctness](total-correctness.md)
