<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The tangent matrices are

$$
X=H'(0)=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad Y=g'(0)=\begin{pmatrix}0&1\\-1&0\end{pmatrix}.
$$

Use the derivative of conjugation from part (i), rather than assuming antisymmetry. Since $H(s)^{-1}=\begin{pmatrix}1&-s\\0&1\end{pmatrix}$, direct multiplication gives

$$
\operatorname{Ad}_{H(s)}Y=H(s)YH(s)^{-1}=\begin{pmatrix}-s&1+s^2\\-1&s\end{pmatrix}.
$$

Differentiating at zero yields

$$
\boxed{[X,Y]=\begin{pmatrix}-1&0\\0&1\end{pmatrix}.}
$$

For the reverse order put $c=\cos t$, $s=\sin t$. The other conjugation is

$$
\operatorname{Ad}_{g(t)}X=\begin{pmatrix}cs&c^2\\-s^2&-sc\end{pmatrix}.
$$

Its derivative at zero is

$$
\boxed{[Y,X]=\begin{pmatrix}1&0\\0&-1\end{pmatrix}=-[X,Y].}
$$

Both computations use actual curves in the [special linear group](../../../../../../special-linear-group.md); the opposite off-diagonal signs in $g(t)$ ensure its determinant is one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
