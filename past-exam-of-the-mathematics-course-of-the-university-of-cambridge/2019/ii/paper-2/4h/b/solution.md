<h1 id="4h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Encode each $k$-tuple of nonnegative integers by one nonnegative integer using a computable [pairing function](../../../../../../pairing-function.md). Define a unary partial procedure $P$ on input $m$ as follows: use [dovetailing](../../../../../../dovetailing.md) on the computations of $f_{n,k}$ over all encoded $k$-tuples, and halt as soon as one of them halts with output $m$. Then

$$
P(m)\downarrow
\quad\Longleftrightarrow\quad
\exists(m_1,\ldots,m_k)\in\mathbb N_0^k:
f_{n,k}(m_1,\ldots,m_k)=m.
$$

By the [Church–Turing thesis](../../../../../../church-turing-thesis.md), this effective procedure is implemented by a register machine with some fixed code $j$, so

$$
E=\{m\in\mathbb N_0:f_{j,1}(m)\downarrow\}.
$$

**Thus $E$ is the domain of a [partial computable function](../../../../../../computable-function.md) and is recursively enumerable.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4H](../../4h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
