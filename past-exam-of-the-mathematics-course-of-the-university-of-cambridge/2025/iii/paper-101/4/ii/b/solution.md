<h1 id="4/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\overline A=A/(x)$ and $\overline{\mathfrak m}=\mathfrak m/(x)$. Applying the dimension theorem to $A$ and $\overline A$ gives

$$
d(G_{\overline{\mathfrak m}}(\overline A))
=\dim\overline A,
\qquad
d(G_{\mathfrak m}(A))=\dim A.
$$

Since $x$ is a non-zero-divisor, it belongs to no minimal prime of the Noetherian ring $A$. Any chain of primes in $A/(x)$ lifts to a chain

$$
\mathfrak p_0\subsetneq\cdots\subsetneq\mathfrak p_r
$$

of primes of $A$ containing $x$. A minimal prime $\mathfrak q\subseteq\mathfrak p_0$ cannot contain $x$, so the inclusion is strict. Prepending $\mathfrak q$ gives a chain of length $r+1$ in $A$. Thus the [dimension drop by a non-zero-divisor](../../../../../../../dimension-drop-by-a-non-zero-divisor.md) gives

$$
\dim(A/(x))\leq\dim A-1.
$$

Combining these equalities proves

$$
\boxed{d(G_{\mathfrak m/(x)}(A/(x)))
\leq d(G_{\mathfrak m}(A))-1}.
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [4](../../../4.md)
4. [Paper 101](../../../../paper-101-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
