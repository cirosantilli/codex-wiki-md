<h1 id="4f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The set

$$
\mathbb K=\{n:f_{n,1}(n)\text{ halts}\}
$$

is the [diagonal halting set](../../../../../../diagonal-halting-set.md). It is recursively enumerable by simulating the coded machine, but it is not recursive by the [halting problem](../../../../../../halting-problem.md) diagonal argument.

By contrast, $\mathbb K_{100}$ is recursive: decode $n$, reject it if it is not a program code, otherwise simulate the program on input $n$ for exactly $100$ steps and accept precisely if it has halted. This bounded computation always terminates. Thus

$$
\boxed{\mathbb K\text{ is not recursive},\qquad
\mathbb K_{100}\text{ is recursive}}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
