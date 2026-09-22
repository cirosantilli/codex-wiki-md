<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [register machine](../../../../../../register-machine.md) has finitely many natural-number registers, a finite set of labelled states, and instructions that increment a register, conditionally decrement and branch according to whether a register is zero, or halt. A program is a finite sequence of such labelled instructions, and a configuration records the current instruction together with every current register value.

Given $k$ inputs, place them in designated input registers and initialize the remaining registers to zero. The machine computes a [partial computable function](../../../../../../computable-function.md) $f:\mathbb N^k\rightharpoonup\mathbb N$ when it halts with output $f(\mathbf x)$ in the output register exactly for $\mathbf x\in\operatorname{dom}f$ and runs forever otherwise.

To encode a machine, encode every instruction by a [natural number](../../../../../../natural-number.md) using effective encodings of its opcode, register number, and target labels. Encode the resulting finite sequence by a [Gödel numbering](../../../../../../godel-numbering.md), for example through iterated pairing or prime powers. Effective decoding gives an enumeration $(P_n)$ of machine programs, so the unary function computed by program code $n$ may be denoted $f_{n,1}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
