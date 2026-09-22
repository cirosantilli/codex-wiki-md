<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Choose orthonormal coordinates with origin $P$ and horizontal axis $l$. The [Euclidean reflection](../../../../../reflection-mathematics.md) and [planar rotation](../../../../../planar-rotation.md) have [matrices](../../../../../matrix.md)

$$
S=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad R_\alpha=\begin{pmatrix}\cos\alpha&-\sin\alpha\\\sin\alpha&\cos\alpha\end{pmatrix}.
$$

Their [function composition](../../../../../function-composition.md) therefore satisfies the [composition of a plane rotation and a reflection](../../../../../composition-of-a-plane-rotation-and-a-reflection.md) identity

$$
R_\alpha S=\begin{pmatrix}\cos\alpha&\sin\alpha\\\sin\alpha&-\cos\alpha\end{pmatrix}=R_{\alpha/2}S R_{-\alpha/2}.
$$

Conjugating by a [planar rotation](../../../../../planar-rotation.md) transports the horizontal reflection axis to the line at angle $\alpha/2$. Equivalently, the vector $e=(\cos(\alpha/2),\sin(\alpha/2))$ is fixed, whereas its perpendicular $e_\perp=(-\sin(\alpha/2),\cos(\alpha/2))$ is sent to $-e_\perp$. Consequently **the fixed line is the line through $P$ obtained by rotating $l$ through $\alpha/2$, and $\tau\rho$ is reflection in that line**. Angles of an unoriented line are understood modulo $\pi$, so this description is independent of the representative chosen for $\alpha$ modulo $2\pi$.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
