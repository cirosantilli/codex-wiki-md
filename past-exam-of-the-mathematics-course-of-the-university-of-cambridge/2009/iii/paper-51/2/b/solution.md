<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $N>1$, use the [orthonormal basis](../../../../../../orthonormal-basis.md) $(|a\rangle,|\omega\rangle)$ from the preceding part. Both [reflection operators](../../../../../../reflection-operator.md) preserve $\mathcal V$, because their reflected vectors belong to it. With $s=\sin\theta$ and $c=\cos\theta$, their restricted [matrices](../../../../../../matrix.md) are

$$
V_{|a\rangle}=\begin{pmatrix}-1&0\\0&1\end{pmatrix},\qquad
V_{|\psi_A\rangle}=I-2\begin{pmatrix}s^2&sc\\sc&c^2\end{pmatrix}
=\begin{pmatrix}\cos2\theta&-\sin2\theta\\-\sin2\theta&-\cos2\theta\end{pmatrix}.
$$

Multiplying in the specified order, including the overall minus sign, gives

$$
\boxed{G\big|_{\mathcal V}=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}.}
$$

Equivalently,

$$
G\big|_{\mathcal V}=\cos2\theta\bigl(|a\rangle\langle a|+|\omega\rangle\langle\omega|\bigr)
+\sin2\theta\bigl(|a\rangle\langle\omega|-|\omega\rangle\langle a|\bigr).
$$

In particular, $G$ sends $\sin t|a\rangle+\cos t|\omega\rangle$ to $\sin(t+2\theta)|a\rangle+\cos(t+2\theta)|\omega\rangle$. This proves the [Grover rotation angle](../../../../../../grover-rotation-angle.md) description with the signs appropriate to these [reflection operators](../../../../../../reflection-operator.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
