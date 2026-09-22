<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For one-column [Gram matrices](../../../../../../gram-matrix.md), unit [Euclidean norm](../../../../../../euclidean-norm.md) of the columns gives $A_S^*A_S=1$. The [restricted isometry constant](../../../../../../restricted-isometry-constant.md) formula therefore gives $\delta_1=0$. For a two-column [Gram matrix](../../../../../../gram-matrix.md), put $c=\langle a_i,a_j\rangle$. The difference from the [identity matrix](../../../../../../identity-matrix.md) has the form

$$
\begin{pmatrix}0&c\\\overline c&0\end{pmatrix},
$$

up to the convention for the complex [inner product](../../../../../../inner-product.md). Its characteristic polynomial is $\lambda^2-|c|^2$, so the [eigenvalues](../../../../../../eigenvalue.md) are $\pm|c|$ and its [matrix 2-norm](../../../../../../matrix-2-norm.md) is $|c|$. Maximizing over pairs gives $\delta_2=\mu$, where $\mu$ is the [mutual coherence](../../../../../../coherence-of-a-normalized-matrix.md).

Part (b), together with the minimality defining the [restricted isometry constant](../../../../../../restricted-isometry-constant.md), gives $\delta_s\le\mu_1(s-1)$. Every summand defining [cumulative coherence](../../../../../../cumulative-coherence.md) is at most the [mutual coherence](../../../../../../coherence-of-a-normalized-matrix.md), so $\mu_1(s-1)\le(s-1)\mu$. **Thus, for normalized columns and $N\ge2$,**

$$
\boxed{\delta_1=0,\qquad\delta_2=\mu,\qquad\delta_s\le\mu_1(s-1)\le(s-1)\mu\quad(2\le s\le N).}
$$

The upper range $s\le N$ matters because the printed definition of [cumulative coherence](../../../../../../cumulative-coherence.md) stops at $N-1$. For $N=1$, only $\delta_1=0$ is needed; the maximum over pairs defining [mutual coherence](../../../../../../coherence-of-a-normalized-matrix.md) is otherwise empty.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
