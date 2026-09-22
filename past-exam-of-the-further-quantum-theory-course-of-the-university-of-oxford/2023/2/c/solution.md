<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $a>0$ and put $\mu=mg/\hbar^2$, $q=k/\hbar$, and $\gamma=\mu/q$. At a [delta potential](../../../../delta-potential.md) located at $x_0$, integration of the [Schrödinger equation](../../../../schrodinger-equation.md) gives the matching conditions

$$
\psi(x_0^+)=\psi(x_0^-),\qquad \psi'(x_0^+)-\psi'(x_0^-)=2\mu\psi(x_0).
$$

Writing the adjacent [plane wave](../../../../plane-wave.md) coefficients as $(A_L,B_L)$ and $(A_R,B_R)$ gives

$$
(A_R-A_L)e^{iqx_0}+(B_R-B_L)e^{-iqx_0}=0,
$$



$$
iq\bigl[(A_R-A_L)e^{iqx_0}-(B_R-B_L)e^{-iqx_0}\bigr]=2\mu(A_Le^{iqx_0}+B_Le^{-iqx_0}).
$$

Solving these two linear equations yields the [transfer matrix of a delta potential](../../../../transfer-matrix-of-a-delta-potential.md):

$$
\begin{pmatrix}A_R\\B_R\end{pmatrix}=D(x_0)\begin{pmatrix}A_L\\B_L\end{pmatrix},\qquad D(x_0)=\begin{pmatrix}1-i\gamma&-i\gamma e^{-2iqx_0}\\i\gamma e^{2iqx_0}&1+i\gamma\end{pmatrix},\qquad\det D(x_0)=1.
$$

For the [symmetric double-delta potential](../../../../symmetric-double-delta-potential.md), use separate [plane wave](../../../../plane-wave.md) pairs in $x<-a$, $-a<x<a$, and $x>a$. Successive matching gives $M=D(a)D(-a)$ between the two exterior pairs. For real $q$, multiplication gives

$$
M=\begin{pmatrix}d^*&-iF\\iF&d\end{pmatrix},\qquad d=(1+i\gamma)^2+\gamma^2e^{4iqa},\qquad F=2\gamma\bigl[\cos(2qa)+\gamma\sin(2qa)\bigr].
$$

The [determinant](../../../../determinant.md) identity $\det M=1$ reads $|d|^2-F^2=1$. Left incidence means $(t,0)^T=M(1,r)^T$, whence

$$
\boxed{t=\frac1d=\frac{q^2}{(q+i\mu)^2+\mu^2e^{4iqa}},\qquad r=-\frac{iF}{d}.}
$$

Here the first relation also follows from $t=M_{11}-M_{12}M_{21}/M_{22}=\det M/M_{22}$. Therefore the requested [transmission probability](../../../../transmission-probability.md) and [quantum reflection probability](../../../../quantum-reflection-probability.md), as functions of the printed [momentum](../../../../momentum-split.md) $k$, are

$$
\boxed{T(k)=\frac{1}{1+F(k)^2},\qquad R(k)=\frac{F(k)^2}{1+F(k)^2},\quad F(k)=\frac{2\mu\hbar}{k}\left[\cos\frac{2ka}{\hbar}+\frac{\mu\hbar}{k}\sin\frac{2ka}{\hbar}\right].}
$$

They obey $R+T=1$. As checks, $g=0$ gives $T=1$, and the coincident limit $a\to0$ gives $T=q^2/(q^2+4\mu^2)$, the answer for a single [delta potential](../../../../delta-potential.md) of strength $2g$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
