<h1 id="6/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the four-dimensional real vector space of [Hermitian matrices](../../../../../../../hermitian-operator.md)

$$
X=tI+x\cdot\sigma=\begin{pmatrix}t+x_3&x_1-ix_2\\x_1+ix_2&t-x_3\end{pmatrix},
\qquad \det X=t^2-|x|^2.
$$

For $A\in SL(2,\mathbb C)$, $X\mapsto AXA^\dagger$ preserves determinant, hence defines a [Lorentz transformation](../../../../../../../lorentz-transformation.md). Positive definite $X$ stays positive definite, so future timelike vectors remain future timelike. Connectedness also fixes the orientation, giving an image in $SO_0(3,1)$.

If the action is trivial, $X=I$ makes $A$ unitary. The remaining condition says it commutes with every Hermitian matrix, forcing $A=\lambda I$ with $\lambda^2=1$. Infinitesimally $aX+Xa^\dagger=0$ first makes $a$ anti-Hermitian and then scalar; tracelessness forces $a=0$. Both real Lie-algebra dimensions are six, so the image is open. Polar decomposition shows $SL(2,\mathbb C)$ is connected, with connected unitary factor $SU(2)$ and a contractible positive Hermitian determinant-one factor. The image is therefore the full proper orthochronous [Lorentz group](../../../../../../../lorentz-group.md).

$$
\boxed{SL(2,\mathbb C)/\{\pm I\}\cong SO_0(3,1).}
$$

This is the [Hermitian-matrix double cover of SO0(3,1)](../../../../../../../hermitian-matrix-double-cover-of-so0-3-1.md). The full determinant-one [Lorentz group](../../../../../../../lorentz-group.md) also contains transformations reversing time orientation, so the identity-component qualification cannot be omitted.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
