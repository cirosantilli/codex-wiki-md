<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E_{12}=\begin{pmatrix}0&1\\0&0\end{pmatrix}$, so $A(t)=I+tE_{12}$ and $E_{12}^2=0$. Multiplication gives

$$
\begin{pmatrix}m&0\\0&m^{-1}\end{pmatrix}
A(t)
\begin{pmatrix}m^{-1}&0\\0&m\end{pmatrix}
=\begin{pmatrix}1&m^2t\\0&1\end{pmatrix}.
$$

The nilpotence also gives $(I+tE_{12})^k=I+ktE_{12}$ for every nonnegative integer $k$, since all higher binomial terms vanish. Hence, for each positive integer $m$,

$$
\boxed{\operatorname{diag}(m,m^{-1})A(t)\operatorname{diag}(m,m^{-1})^{-1}
=A(m^2t)=A(t)^{m^2}.}
$$

These are [unipotent matrices](../../../../../../../unipotent-matrix.md) in [SL2R](../../../../../../../real-special-linear-group-of-degree-two.md). The integer is positive, since the displayed diagonal [matrix](../../../../../../../matrix.md) is undefined at $m=0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Iii](../../../../split.md)
6. [2001](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
