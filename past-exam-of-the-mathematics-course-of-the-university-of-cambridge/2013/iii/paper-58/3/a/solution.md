<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

This is the [Deutsch-Jozsa test with an arbitrary uniform-state unitary](../../../../../../deutsch-jozsa-test-with-an-arbitrary-uniform-state-unitary.md), and does not require $N$ to be a power of two. Choose a known [unitary operator](../../../../../../unitary-operator.md) $F$ such that $F|0\rangle=|s\rangle=N^{-1/2}\sum_i|i\rangle$. Prepare the target [qubit](../../../../../../qubit.md) in $|{-}\rangle=(|0\rangle-|1\rangle)/\sqrt2$. One Boolean-oracle call gives [quantum phase kickback](../../../../../../phase-kickback.md):

$$
O_{\mathbf x}|i\rangle|{-}\rangle=(-1)^{x_i}|i\rangle|{-}\rangle.
$$

Apply $F^\dagger$ to the index register. The amplitude on $|0\rangle$ is

$$
\frac1N\sum_i(-1)^{x_i}.
$$

It equals $+1$ or $-1$ for the two constant strings, and equals zero for a balanced string. Consequently **a single query decides the promised problem exactly:** measure the index register and report constant for outcome zero, balanced for any other outcome. This is the [Deutsch-Jozsa algorithm](../../../../../../deutsch-jozsa-algorithm.md) with the available exact state-preparation operation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
