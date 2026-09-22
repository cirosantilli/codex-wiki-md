<h1 id="2b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The coefficient [matrix](../../../../../../matrix.md) has [determinant](../../../../../../determinant.md)

$$
\det\begin{pmatrix}p&1&1\\1&2&4\\1&4&10\end{pmatrix}
=4p-6+2=4(p-1).
$$

A square [linear system](../../../../../../system-of-linear-equations.md) has a unique solution for every right-hand side precisely when its coefficient [matrix](../../../../../../matrix.md) is an [invertible matrix](../../../../../../invertible-matrix.md). Here **a unique solution exists exactly when $p\ne1$, for every real $t$**.

For an explicit [Gaussian elimination](../../../../../../gaussian-elimination.md), subtract twice the second equation from the third, then use the second equation, obtaining $x=2z+2t-t^2$ and $y=(t^2-t)/2-3z$. The first equation determines

$$
z=\frac{2+(2p-1)t^2+(1-4p)t}{4(p-1)},
$$

and the preceding formulas determine $x,y$. When $p=1$ this last coefficient vanishes; the next parts determine compatibility rather than dividing by zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2B](../../2b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
