<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the quarter-turn [rotation matrix](../../../../../rotation-matrix.md)

$$
R=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix}.
$$

For a general second-order [tensor](../../../../../tensor.md), direct multiplication gives

$$
RTR^T=\begin{pmatrix}T_{22}&-T_{21}&-T_{23}\\-T_{12}&T_{11}&T_{13}\\-T_{32}&T_{31}&T_{33}\end{pmatrix}.
$$

Requiring $RTR^T=T$ gives $T_{11}=T_{22}$, $T_{12}=-T_{21}$, $T_{13}=-T_{23}$ together with $T_{23}=T_{13}$, and $T_{31}=-T_{32}$ together with $T_{32}=T_{31}$. Thus all mixed axial-transverse entries vanish and

$$
\boxed{T=\begin{pmatrix}\alpha&\omega&0\\-\omega&\alpha&0\\0&0&\beta\end{pmatrix}.}
$$

For an arbitrary rotation angle $\theta$, the transverse rotation is $Q_\theta=\cos\theta\,I+\sin\theta\,J$, where $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$. The transverse block of $T$ is $\alpha I-\omega J$, so it commutes with $Q_\theta$. Therefore $Q_\theta(\alpha I-\omega J)Q_\theta^T=\alpha I-\omega J$, while the axial component $\beta$ is unchanged.

Hence **invariance holds under every rotation about the axis**, not just the quarter-turn. This is the general [axisymmetric second-order tensor](../../../../../axisymmetric-second-order-tensor.md); a [symmetric tensor](../../../../../symmetric-tensor.md) would additionally require $\omega=0$, but that restriction was not assumed.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
