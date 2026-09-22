<h1 id="6b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For this two-dimensional [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md), the covariance matrix

$$
C(t)=\mathbb E[x(t)x(t)^T]
$$

satisfies

$$
\frac{dC}{dt}=aC+Ca^T+b.
$$

Thus the stationary covariance solves the continuous [Lyapunov equation](../../../../../../continuous-lyapunov-equation.md)

$$
\boxed{aC+Ca^T+b=0}.
$$

Write

$$
C=
\begin{pmatrix}
u&v\\
v&w
\end{pmatrix}.
$$

Substitution gives

$$
-2u+2v+1=0,
\qquad
w-2u-2v=0,
\qquad
-4v-2w+1=0.
$$

Solving,

$$
u=\frac5{12},
\qquad
v=-\frac1{12},
\qquad
w=\frac23.
$$

Therefore

$$
\boxed{
C=
\begin{pmatrix}
5/12&-1/12\\
-1/12&2/3
\end{pmatrix}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6B](../../6b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
