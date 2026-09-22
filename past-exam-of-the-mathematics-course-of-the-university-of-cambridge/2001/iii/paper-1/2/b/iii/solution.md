<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $N$ be the [normal closure](../../../../../../../normal-closure.md) of the upper unipotents $U(t)=A(t)$. Conjugation by $J=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ gives

$$
JU(t)J^{-1}=\begin{pmatrix}1&0\\-t&1\end{pmatrix}.
$$

Thus $N$ also contains every lower unipotent $L(s)=\begin{pmatrix}1&0\\s&1\end{pmatrix}$. We prove explicitly that these [elementary unipotent generators of SL2R](../../../../../../../elementary-unipotent-generators-of-sl2r.md) generate the full [group](../../../../../../../group-split.md).

For $a\ne0$, multiplication gives

$$
w(a)=U(a)L(-a^{-1})U(a)
=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix},
\qquad
w(a)w(-1)=\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}.
$$

So all determinant-one diagonal [matrices](../../../../../../../matrix.md) lie in $N$. If $g=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ has $a\ne0$ and $ad-bc=1$, then

$$
g=L(c/a)\begin{pmatrix}a&0\\0&a^{-1}\end{pmatrix}U(b/a),
$$

because its lower-right entry is $(1+bc)/a=d$. If $a=0$, then $c\ne0$ and left multiplication by $U(1)$ makes the upper-left entry equal to $c$. The resulting [matrix](../../../../../../../matrix.md) lies in $N$ by the preceding factorization, and $U(1)^{-1}\in N$ restores $g$. Therefore

$$
\boxed{N=SL_2(\mathbb R).}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
