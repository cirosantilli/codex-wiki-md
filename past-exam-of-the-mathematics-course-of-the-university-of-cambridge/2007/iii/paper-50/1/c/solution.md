<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For positive frequency take $p^0=E=\sqrt{|\mathbf p|^2+m^2}>0$, with $m\geq0$. Lowering the index in $p_\mu\sigma^\mu$ is important: put

$$
A=p\cdot\sigma=E I_2-\mathbf p\cdot\boldsymbol\sigma,\qquad
B=p\cdot\bar\sigma=E I_2+\mathbf p\cdot\boldsymbol\sigma.
$$

These are commuting [Hermitian matrices](../../../../../../hermitian-operator.md) with $AB=(E^2-|\mathbf p|^2)I_2=m^2I_2$. Their [eigenvalues](../../../../../../eigenvalue.md) are $E\pm|\mathbf p|$, so they are positive definite for $m>0$ and [positive semidefinite matrices](../../../../../../positive-semidefinite-matrix.md) for $m=0$. [Simultaneous diagonalization](../../../../../../simultaneous-diagonalization.md) defines their positive [square roots of a matrix](../../../../../../square-root-of-a-matrix.md) and gives $\sqrt A\sqrt B=mI_2$.

The plane-wave ansatz reduces the [Dirac equation](../../../../../../dirac-equation.md) to $(\not p-m)u=0$, where

$$
\not p=\begin{pmatrix}0&A\\B&0\end{pmatrix}.
$$

For $u_L=\sqrt A\xi$ and $u_R=\sqrt B\xi$, commutativity gives $Au_R=m u_L$ and $Bu_L=m u_R$. Therefore

$$
\boxed{\psi_+(x)=\begin{pmatrix}\sqrt A\xi\\\sqrt B\xi\end{pmatrix}e^{-ip\cdot x}.}
$$

This is the [Hermitian square-root construction of Dirac plane waves](../../../../../../hermitian-square-root-construction-of-dirac-plane-waves.md).

For negative frequency retain the future-directed momentum label $p$ and use $\psi_-(x)=v(\mathbf p)e^{+ip\cdot x}$. The equation is now $(\not p+m)v=0$. Its general solution is

$$
\boxed{v(\mathbf p)=\begin{pmatrix}\sqrt A\zeta\\-\sqrt B\zeta\end{pmatrix},\qquad\psi_-(x)=v(\mathbf p)e^{+ip\cdot x},}
$$

with arbitrary two-spinor $\zeta$. The minus between its two blocks gives $Av_R=-m v_L$ and $Bv_L=-m v_R$. For $m>0$ these parametrizations span the two-dimensional positive- and negative-frequency solution spaces. At nonzero null momentum the square roots have complementary rank-one supports and still give the full two-dimensional kernels. If $\xi^\dagger\xi=\zeta^\dagger\zeta=1$, both spinors have norm squared $2E$; the positive one also has $\bar uu=2m$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
