<h1 id="34c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By part (a), each $A\varphi_\pm+\partial_t\varphi_\pm$ lies in the same two-dimensional eigenspace. Reality and conjugacy again force the coefficient [matrix](../../../../../../../matrix.md) to have the form

$$
\Lambda=\begin{pmatrix}\lambda&\mu\\\bar\mu&\bar\lambda\end{pmatrix},
\qquad
(\partial_t+A)\Psi=\Lambda\Psi.
$$

Because $u$ and hence $A$ are periodic, $\partial_t+A$ commutes with translation by $2\pi$. Applying it to  
$\Psi(x+2\pi)=\widehat T\Psi(x)$ gives

$$
\Lambda\widehat T\Psi
=(\partial_t\widehat T)\Psi+\widehat T\Lambda\Psi.
$$

The [basis](../../../../../../../basis.md) $\Psi$ is independent, so the [periodic KdV transfer matrix](../../../../../../../periodic-kdv-transfer-matrix.md) obeys

$$
\boxed{\partial_t\widehat T=[\Lambda,\widehat T]}.
$$

Taking traces,

$$
\frac d{dt}(a+\bar a)=\operatorname{tr}[\Lambda,\widehat T]=0.
$$

Hence $\boxed{\operatorname{Re}a}$ is independent of time.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [34C](../../../34c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
