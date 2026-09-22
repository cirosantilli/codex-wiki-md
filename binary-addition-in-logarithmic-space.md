# Binary addition in logarithmic space

↑ **Parent:** [Logarithmic space](logarithmic-space.md)

For canonical positive [binary numeral system](binary-numeral-system.md) inputs, a [logspace transducer](logspace-transducer.md) can emit the canonical representation of their [sum](sum.md) most significant digit first. Count the operand lengths, compute the final [arithmetic carry](carry-arithmetic.md) to determine output length, and then compute each requested result digit by restarting the least-significant-first column recurrence. Each pass uses only a fixed number of $O(\log n)$-[bit](bit.md) indices and one [arithmetic carry](carry-arithmetic.md). The [binary-addition carry invariant](binary-addition-carry-invariant.md) proves correctness. [Logspace composition by recomputation](logspace-composition-by-recomputation.md) consequently permits any [L](l-complexity.md) property of the resulting digit [string](string.md), including being a [binary palindrome](binary-palindrome.md), to be tested without storing the sum.

## ↑ Ancestors (7)

1. [Logarithmic space](logarithmic-space.md)
2. [Space complexity](space-complexity.md)
3. [Complexity class](complexity-class.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)
