<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $\boxed{v_4=e^t(1-t)}$, and denote the new ordered [basis](../../../../../basis.md) by $\mathcal C=(b_1,b_2,b_3,b_4)$. The [change of basis](../../../../../change-of-basis.md) [matrix](../../../../../matrix.md), with columns expressed in $\mathcal B$, is

$$
P=\begin{pmatrix}
1&1&0&0\\
-1&1&0&0\\
0&0&1&1\\
0&0&1&-1
\end{pmatrix},\qquad\det P=-4\ne0.
$$

This nonzero [determinant](../../../../../determinant.md) proves that the proposed fourth function completes a [basis](../../../../../basis.md). Express the derivatives in that [basis](../../../../../basis.md):

$$
\begin{aligned}
F(b_1)&=-1=-\tfrac12b_1-\tfrac12b_2,\\
F(b_2)&=1=\tfrac12b_1+\tfrac12b_2,\\
F(b_3)&=e^t(2+t)=\tfrac32b_3+\tfrac12b_4,\\
F(b_4)&=-te^t=-\tfrac12b_3+\tfrac12b_4.
\end{aligned}
$$

Reading off columns therefore gives

$$
\boxed{[F]_{\mathcal C}=P^{-1}MP=
\begin{pmatrix}
-\tfrac12&\tfrac12&0&0\\
-\tfrac12&\tfrac12&0&0\\
0&0&\tfrac32&-\tfrac12\\
0&0&\tfrac12&\tfrac12
\end{pmatrix}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [2021 resit](../../../../2021-resit-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
