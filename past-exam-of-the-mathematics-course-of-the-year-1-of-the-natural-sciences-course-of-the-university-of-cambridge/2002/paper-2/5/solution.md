<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The required [matrix](../../../../matrix.md) form of the [linear system](../../../../system-of-linear-equations.md) is

$$
\boxed{A=\begin{pmatrix}1&1&2\\1&0&\lambda\\1&\lambda&2\end{pmatrix},\qquad\mathbf x=\begin{pmatrix}x\\y\\z\end{pmatrix},\qquad\mathbf b=\begin{pmatrix}1\\\mu\\2\end{pmatrix},\qquad A\mathbf x=\mathbf b.}
$$

Subtract the first row from the third and expand the [determinant](../../../../determinant.md) along the resulting row:

$$
\det A=-(\lambda-1)\det\begin{pmatrix}1&2\\1&\lambda\end{pmatrix}=(\lambda-1)(2-\lambda).
$$

Thus the [linear system](../../../../system-of-linear-equations.md) has a unique solution, for every real $\mu$, precisely when $\boxed{\lambda\ne1,2}$.

For $\lambda=0$, the second equation gives $x=\mu$. Subtracting the first equation from the third gives $-y=1$, and the first equation then determines $z$:

$$
\boxed{\lambda=0:\quad(x,y,z)=(\mu,-1,1-\mu/2),\qquad\mu\in\mathbb R.}
$$

For $\lambda=1$, the first and third left-hand sides are identical but their right-hand sides are $1$ and $2$. Hence

$$
\boxed{\lambda=1:\quad\text{no solution for any }\mu.}
$$

For $\lambda=2$, subtracting the first equation from the third gives $y=1$. The first equation now gives $x+2z=0$, while the second requires $x+2z=\mu$. Consequently

$$
\boxed{\lambda=2:\quad\begin{cases}(x,y,z)=(-2t,1,t),\quad t\in\mathbb R,&\mu=0,\\\text{no solution},&\mu\ne0.\end{cases}}
$$

The [free variable in a linear system](../../../../free-variable-in-a-linear-system.md) in the consistent singular case describes a [line](../../../../straight-line.md) of solutions. These direct reductions distinguish an inconsistent [linear system](../../../../system-of-linear-equations.md) from one with infinitely many solutions, which a zero [determinant](../../../../determinant.md) alone cannot do.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
