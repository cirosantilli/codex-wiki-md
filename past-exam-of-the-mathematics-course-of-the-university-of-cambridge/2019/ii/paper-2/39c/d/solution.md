<h1 id="39c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Each coordinate of the transformed vectors evolves independently because $D$ and $E$ are [diagonal matrices](../../../../../../diagonal-matrix.md). Reorder the unknowns by collecting the $k$th components across all grid columns:

$$
\widehat v_k=((v_1)_k,\ldots,(v_m)_k)^T,
\qquad
\widehat c_k=((c_1)_k,\ldots,(c_m)_k)^T.
$$

Then system (3) splits into the $m$ uncoupled systems

$$
\boxed{\Lambda_k\widehat v_k=\widehat c_k,
\qquad k=1,\ldots,m,}
$$

where

$$
\boxed{\Lambda_k=[e_k,d_k,e_k]
=\begin{pmatrix}
d_k&e_k&&\\
e_k&d_k&\ddots&\\
&\ddots&\ddots&e_k\\
&&e_k&d_k
\end{pmatrix}.}
$$

**Thus the original $m^2\times m^2$ problem reduces to one [discrete sine transform](../../../../../../discrete-sine-transform.md) followed by $m$ independent tridiagonal solves and an inverse sine transform.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [39C](../../39c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
