<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $I_a=\bar I_{aa}$ and use the right-handed rotation

$$
L(t)=\begin{pmatrix}\cos\Omega t&-\sin\Omega t&0\\
\sin\Omega t&\cos\Omega t&0\\0&0&1\end{pmatrix}.
$$

In the integral defining the [second mass moment tensor](../../../../../../../second-mass-moment-tensor.md), change variables to $\mathbf y=L^{-1}\mathbf x$. The [determinant](../../../../../../../determinant.md) is one and $x_i=L_{ik}y_k$, giving

$$
I_{ij}(t)=\int\rho(\mathbf y)L_{ik}y_kL_{jl}y_l\,d^3y
=L_{ik}L_{jl}\bar I_{kl},\qquad \boxed{I(t)=L(t)\bar I L(t)^T.}
$$

Set $C=(I_1+I_2)/2$ and $\Delta=I_1-I_2$. Multiplication gives

$$
\boxed{\begin{aligned}
I_{11}(t)&=C+\frac\Delta2\cos(2\Omega t),\\
I_{22}(t)&=C-\frac\Delta2\cos(2\Omega t),\\
I_{12}(t)=I_{21}(t)&=\frac\Delta2\sin(2\Omega t),\\
I_{33}(t)&=I_3,\qquad I_{13}(t)=I_{23}(t)=0.
\end{aligned}}
$$

In particular, $I_{kk}=I_1+I_2+I_3$ is constant. These expressions also show how the rotating anisotropy enters the [mass quadrupole moment](../../../../../../../mass-quadrupole-moment.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 309](../../../../paper-309-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
