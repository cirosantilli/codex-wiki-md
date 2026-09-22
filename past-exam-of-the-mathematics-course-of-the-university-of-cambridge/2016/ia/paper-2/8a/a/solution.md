<h1 id="8a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the system as $\mathbf x'=M\mathbf x$, with $M=\begin{pmatrix}2&5\\-1&-2\end{pmatrix}$. Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $\lambda^2+1$, so its [eigenvalues](../../../../../../eigenvalue.md) are $i$ and $-i$. An [eigenvector](../../../../../../eigenvector.md) for $i$ is $v=(5,-2+i)^{\mathsf T}$. Thus $e^{it}v$ is a complex solution, and its [real part](../../../../../../real-part.md) and [imaginary part](../../../../../../imaginary-part.md) give real solutions:

$$
u(t)=\begin{pmatrix}5\cos t\\-2\cos t-\sin t\end{pmatrix},\qquad w(t)=\begin{pmatrix}5\sin t\\\cos t-2\sin t\end{pmatrix}.
$$

Their initial vectors are $(5,-2)^{\mathsf T}$ and $(0,1)^{\mathsf T}$, with determinant $5\ne0$. Consequently they are [linearly independent](../../../../../../linear-independence.md) and span the two-dimensional solution space.

**The general real solution is**

$$
\boxed{\begin{pmatrix}x(t)\\y(t)\end{pmatrix}=\alpha\begin{pmatrix}5\cos t\\-2\cos t-\sin t\end{pmatrix}+\beta\begin{pmatrix}5\sin t\\\cos t-2\sin t\end{pmatrix}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
