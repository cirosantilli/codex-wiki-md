<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

Subtract the [identity matrix](../../../../identity-matrix.md) and put

$$
N=A_{\lambda,\mu}-I=
\begin{pmatrix}
\lambda&\lambda&0\\
\mu-\lambda&\mu-\lambda&\mu\\
-\mu&-\mu&-\mu
\end{pmatrix}.
$$

Direct [matrix multiplication](../../../../matrix-multiplication.md) gives

$$
N^2=\lambda\mu
\begin{pmatrix}1&1&1\\-1&-1&-1\\0&0&0\end{pmatrix},\qquad N^3=0.
$$

For the last equality, each column of $N^2$ is a multiple of $(1,-1,0)^T$, and $N(1,-1,0)^T=0$. Thus $N$ is a [nilpotent matrix](../../../../nilpotent-matrix.md). The [minimal polynomial](../../../../minimal-polynomial.md) of $A_{\lambda,\mu}$ divides $(t-1)^3$ and equals $(t-1)^s$, where $s$ is the [nilpotency index](../../../../nilpotency-index.md) of $N$.

The first row of $N$ forces $\lambda=0$ if $N=0$, and its third row then forces $\mu=0$. Conversely $\lambda=\mu=0$ gives $N=0$. If exactly one parameter is nonzero, then $N\ne0$ but $N^2=0$. If both are nonzero, then $N^2\ne0$ while $N^3=0$. Consequently the complete answer is

$$
\boxed{
m_{A_{\lambda,\mu}}(t)=
\begin{cases}
t-1,&\lambda=\mu=0,\\
(t-1)^2,&\lambda\mu=0\text{ and }(\lambda,\mu)\ne(0,0),\\
(t-1)^3,&\lambda\mu\ne0.
\end{cases}}
$$

No lower power can annihilate the [matrix](../../../../matrix.md) in any of these cases, as the displayed nonvanishing [matrix powers](../../../../matrix-power.md) show.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
