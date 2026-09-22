<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put

$$
a=2\cos\left(\frac{\pi}{m_{ij}}\right).
$$

After ordering $I_1$ before $I_2$, the only nonzero off-diagonal entries between the two blocks occur at $(i,j)$ and $(j,i)$, where they equal $-a$. Thus

$$
G(W)=
\begin{pmatrix}
G(W_1)&-a,e_ie_j^T\\
-a,e_je_i^T&G(W_2)
\end{pmatrix},
$$

where the coordinate vectors in the two blocks are understood. Expanding the [determinant](../../../../../../determinant.md) according to whether neither or both cross-block entries are selected gives

$$
\det G(W)
=\det G(W_1)\det G(W_2)
-a^2\det G(W_1')\det G(W_2').
$$

The minus sign is the sign of the transposition pairing the two cross-block entries. This formula remains valid when either diagonal block is singular, so no inverse or [Schur complement](../../../../../../schur-complement.md) is needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
