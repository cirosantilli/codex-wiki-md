<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [computational basis](../../../../../../computational-basis.md) ordered as $|000\rangle,|001\rangle,|010\rangle,|011\rangle,|100\rangle,|101\rangle,|110\rangle,|111\rangle$. Since $Z|0\rangle=|0\rangle$ and $Z|1\rangle=-|1\rangle$,

$$
\boxed{S\big|_{N=3}=\operatorname{diag}(3,1,1,-1,1,-1,-1,-3)}.
$$

For arbitrary $N$, a computational basis vector with $q$ ones has $N-q$ contributions $+1$ and $q$ contributions $-1$, giving eigenvalue $N-2q$. All $q=0,\ldots,N$ occur, so

$$
\boxed{\operatorname{spec}S=\{N,N-2,\ldots,-N\},\qquad\dim\ker(S-(N-2q)I)=\binom Nq}.
$$

The [binomial coefficient](../../../../../../binomial-coefficient.md) counts which $q$ sites are excited. Thus there are exactly $N+1$ distinct [magnetization sectors of a spin chain](../../../../../../magnetization-sectors-of-a-spin-chain.md), and their dimensions sum to $\sum_q\binom Nq=2^N$, the full Hilbert-space dimension.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
