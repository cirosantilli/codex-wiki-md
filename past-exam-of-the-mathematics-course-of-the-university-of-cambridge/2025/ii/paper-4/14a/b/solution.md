<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $D=1$, both species have the same diffusion coefficient. For a perturbation proportional to $e^{\sigma t+ikx}$, diffusion replaces $J$ by $J-k^2I$, shifting both reaction eigenvalues to the left by $k^2$. Since the homogeneous equilibrium is already stable, every spatial mode remains stable.

For general $D$, put $q=k^2$. The mode matrix is

$$
A(q)=J-q\begin{pmatrix}D&0\\0&1\end{pmatrix}
=\begin{pmatrix}
\beta-1-Dq&\alpha^2\\
-\beta&-\alpha^2-q
\end{pmatrix}.
$$

Its trace is

$$
\operatorname{tr}A(q)=\beta-1-\alpha^2-(D+1)q<0,
$$

while its determinant is

$$
\Delta(q)=Dq^2+\bigl(D\alpha^2-(\beta-1)\bigr)q+\alpha^2.
$$

With negative trace, instability occurs exactly when $\Delta(q)<0$ for some $q>0$. The [two-species diffusion-driven instability criterion](../../../../../../two-species-diffusion-driven-instability-criterion.md) says that this upward-opening quadratic has a negative minimum precisely when

$$
\beta-1-D\alpha^2>2\alpha\sqrt D.
$$

Equivalently, the condition is

$$
\boxed{\beta>(1+\alpha\sqrt D)^2}.
$$

This is the [Turing instability](../../../../../../turing-instability.md) region.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
