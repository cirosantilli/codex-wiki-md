<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $C=Q_1A$ and write its second column as $v$. For $n\geq3$, take

$$
\boxed{Q_2=J(2,n)J(2,n-1)\cdots J(2,3),}
$$

where each angle is computed from the current second column, in the right-to-left application order. These [Givens rotations](../../../../../givens-rotation.md) eliminate its entries in rows $3,\ldots,n$ by accumulating their [Euclidean norm](../../../../../euclidean-norm.md) in row two.

Each rotation acts only on rows with indices at least two. The first column of $C$ is $\|a\|_2e_1$, whose entries in all those rows are zero. Mixing two zeros leaves them zero, and row one is untouched. Thus the first column is unchanged. The resulting [matrix](../../../../../matrix.md) has the form

$$
\boxed{Q_2Q_1A=
\begin{pmatrix}
\|a\|_2&v_1\\
0&\sqrt{v_2^2+\cdots+v_n^2}\\
0&0\\
\vdots&\vdots\\
0&0
\end{pmatrix}\quad(n\geq3).}
$$

This verifies both required properties, including the case of zero second-column tail. When $n=2$ there are no rows to eliminate: take $Q_2=I_2$, the empty product. No sign change of $v_2$ is required in that case. Each [Givens row-pair update](../../../../../givens-row-pair-update.md) preserves previously eliminated columns, which is the central invariant of [QR decomposition by Givens rotations](../../../../../qr-decomposition-by-givens-rotations.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
