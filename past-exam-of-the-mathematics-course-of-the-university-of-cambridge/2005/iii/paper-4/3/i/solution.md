<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $u(t)=\begin{pmatrix}1&t\\0&1\end{pmatrix}$ and $l(s)=\begin{pmatrix}1&0\\s&1\end{pmatrix}$. These [elementary matrices](../../../../../../elementary-matrix.md) belong to the [special linear group](../../../../../../special-linear-group.md). Let $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ have determinant one. If $a\ne0$, elementary row elimination gives

$$
l(-c/a)g=\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}
=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}u(b/a).
$$

The remaining diagonal matrix is also a product of the given generators. Indeed, for $a\ne0$, direct multiplication gives

$$
w(a):=u(a)l(-a^{-1})u(a)=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix},\qquad
w(a)w(-1)=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}.
$$

Hence $g=l(c/a)w(a)w(-1)u(b/a)$. If $a=0$, its [determinant](../../../../../../determinant.md) forces $c\ne0$, and $u(1)g$ has upper-left entry $c$. The established case applies to it, and $g=u(-1)(u(1)g)$ is again generated. No division by two was used, so the proof works over every [field](../../../../../../field.md). **The upper and lower elementary unipotent matrices generate $SL_2(K)$.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
