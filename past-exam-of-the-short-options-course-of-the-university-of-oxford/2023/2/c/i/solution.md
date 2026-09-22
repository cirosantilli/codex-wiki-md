<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

After the reduction in part (b), multiply by $S$. The new bottom-left entry is $r$, whose absolute value is strictly smaller than the previous $|c|$:

$$
S T^nX=\begin{pmatrix}-c&-d\\r&b+nd\end{pmatrix}.
$$

Repeated [Euclidean division](../../../../../euclidean-division.md) must terminate because the nonnegative integers $|c|$ decrease strictly until zero. Thus a word $W$ in $S,T$ and their inverses gives a [matrix](../../../../../matrix.md) with bottom-left entry zero. Its determinant is one, so the diagonal entries are equal and are either both $1$ or both $-1$:

$$
WX=\begin{pmatrix}\varepsilon&b_0\\0&\varepsilon\end{pmatrix}=\varepsilon I\,T^{\varepsilon b_0},\qquad\varepsilon\in\{1,-1\}.
$$

Since $S^2=-I$, this final [matrix](../../../../../matrix.md) belongs to $\langle S,T\rangle$. So does $W^{-1}$, proving

$$
\boxed{SL(2,\mathbb Z)=\langle S,T\rangle}.
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
