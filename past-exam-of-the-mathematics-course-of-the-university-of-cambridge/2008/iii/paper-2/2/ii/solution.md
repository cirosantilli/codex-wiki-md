<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [recursive function](../../../../../../total-computable-function.md) $f:\mathbb N^k\to\mathbb N$ is a [total computable function](../../../../../../total-computable-function.md): an algorithm halts on every input and returns the specified value. Equivalently it is an everywhere-defined member of the [partial recursive functions](../../../../../../computable-function.md), obtained from the initial zero, successor and projection functions by composition, [primitive recursion](../../../../../../primitive-recursion.md) and [unbounded minimization](../../../../../../mu-operator.md). In minimization $\mu y\,[g(\mathbf x,y)=0]$, the sequential search must find a zero after all earlier tests have been defined; otherwise the result is undefined. The [Church–Turing thesis](../../../../../../church-turing-thesis.md) allows the algorithmic formulation here.

A [recursively enumerable set](../../../../../../recursively-enumerable-set.md) $E\subseteq\mathbb N^k$ is the domain of a [partial computable function](../../../../../../computable-function.md). Thus an algorithm halts and accepts exactly on members of $E$, and may run forever on nonmembers. Equivalently an algorithm lists exactly its elements, allowing repetition and allowing an empty output for the empty set. To pass from a listing to a membership semidecision, wait for the input to appear. To pass back, use [dovetailing](../../../../../../dovetailing.md) on all inputs and list each whose recognizing computation halts. This differs from a [recursive set](../../../../../../computable-set.md), whose zero-one characteristic function is total recursive and decides both membership and nonmembership.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
