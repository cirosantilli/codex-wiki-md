<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $A_n$ denote the given [tridiagonal matrix](../../../../../../tridiagonal-matrix.md) and put $D_n=\det A_n$, including $D_0=1$ for the empty [determinant](../../../../../../determinant.md). The starting values are

$$
D_0=1,\qquad D_1=1,\qquad D_2=\det\begin{pmatrix}1&1\\1&1\end{pmatrix}=0.
$$

For $n\ge3$, apply the following [elementary row operations](../../../../../../elementary-row-operation.md) in the indicated order, always using the updated rows:

$$
R_2\leftarrow R_2-R_1,\qquad R_3\leftarrow R_3-R_2,\qquad R_2\leftrightarrow R_3.
$$

The first three rows now begin

$$
\begin{pmatrix}
1&1&0&0&\cdots\\
0&1&0&1&\cdots\\
0&0&1&0&\cdots
\end{pmatrix},
$$

with the fourth column omitted if $n=3$. When $n\ge4$, also use $R_4\leftarrow R_4-R_3$. The resulting [block upper triangular matrix](../../../../../../block-upper-triangular-matrix.md) has a $3\times3$ [upper triangular matrix](../../../../../../upper-triangular-matrix.md) with diagonal entries all one in its top left corner, and $A_{n-3}$ in its bottom right corner. All [elementary row operations](../../../../../../elementary-row-operation.md) preserved the [determinant](../../../../../../determinant.md) except the single row interchange. Therefore

$$
\boxed{D_n=-D_{n-3}\quad(n\ge3).}
$$

Applying this [recurrence relation](../../../../../../recurrence-relation.md) to the three starting values proves by [mathematical induction](../../../../../../mathematical-induction.md) that

$$
\boxed{D_n=\begin{cases}
(-1)^k,&n=3k,\\
(-1)^k,&n=3k+1,\\
0,&n=3k+2.
\end{cases}}
$$

Equivalently, the sequence is periodic with period six, with values $1,1,0,-1,-1,0$ starting at $n=0$. A compact closed form is $D_n=\sin((n+1)\pi/3)/\sin(\pi/3)$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
