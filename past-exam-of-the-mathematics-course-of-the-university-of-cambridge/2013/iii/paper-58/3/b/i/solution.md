<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $|u_i\rangle$ denote the specified image of $|i\rangle|0\rangle$. Its components comprise $N-1$ distinct ordered-pair basis states, each with coefficient $\pm N^{-1/2}$, together with $|0,0\rangle$ with coefficient $N^{-1/2}$. Hence $\langle u_i|u_i\rangle=1$.

For distinct indices $i<j$, only two output basis states occur in both images. Their common $|0,0\rangle$ contributions have product $1/N$, while the $|i,j\rangle$ contributions have product $-1/N$. Thus

$$
\boxed{\langle u_i|u_j\rangle=\delta_{ij}.}
$$

The specified map is therefore a [linear isometry](../../../../../../../linear-isometry-of-hilbert-spaces.md) on the $N$-dimensional input subspace. Complete the input vectors $|i,0\rangle$ to an [orthonormal basis](../../../../../../../orthonormal-basis.md) of the $N^2$-dimensional space, and independently complete their images $|u_i\rangle$ to another [orthonormal basis](../../../../../../../orthonormal-basis.md). Map the first full basis to the second. This is a [unitary extension of a finite-dimensional isometry](../../../../../../../unitary-extension-of-a-finite-dimensional-isometry.md), giving the required $\widetilde U$. **The prescribed columns are orthonormal, so a full [unitary extension](../../../../../../../unitary-extension-of-a-finite-dimensional-isometry.md) exists.** Its construction depends only on $N$, not on the unknown string, and is permitted by the question's exact-unitary assumption.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 58](../../../../paper-58-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
