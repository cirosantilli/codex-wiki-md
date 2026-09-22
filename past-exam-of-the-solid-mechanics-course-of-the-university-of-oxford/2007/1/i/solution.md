<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We first derive the [stress](../../../../stress.md) and energy facts used in both parts. The Cauchy [traction](../../../../traction.md) $s=Tn$ is [force](../../../../force-split.md) per unit area in the deformed configuration. The first Piola-Kirchhoff [traction](../../../../traction.md) $s_R=T_RN$ is [force](../../../../force-split.md) per unit reference area. Their [force](../../../../force-split.md) vectors are measured in the same spatial coordinates, but the area measures and the normals used to specify the surface are different.

Parametrize a reference surface by $x=x(u,v)$. Its oriented area vector is $(x_u\times x_v)\,du\,dv$. Under deformation, the two tangents become $Fx_u,Fx_v$. The cross-product identity

$$
(Fa)\times(Fb)=(\operatorname{cof}F)(a\times b)=JF^{-T}(a\times b)
$$

therefore proves [Nanson's formula](../../../../nanson-s-formula.md) $n\,da=JF^{-T}N\,dA$. Equality of the physical [force](../../../../force-split.md) on corresponding surface patches now gives

$$
T_RN\,dA=Tn\,da=JT F^{-T}N\,dA.
$$

Since this holds for every reference [normal](../../../../normal-distribution.md),

$$
\boxed{T_R=JT F^{-T},\qquad T=J^{-1}T_RF^T.}
$$

The [first Piola-Kirchhoff stress tensor](../../../../first-piola-kirchhoff-stress-tensor.md) is generally not [symmetric](../../../../symmetric-relation.md), whereas the [Cauchy stress tensor](../../../../cauchy-stress-tensor.md) is [symmetric](../../../../symmetric-relation.md) in the absence of couple stresses.

For the stated energy on orientation-preserving gradients, [differentiation](../../../../differentiation.md) gives

$$
T_R=DW(F)=\mu\bigl(F-J^{-2}\operatorname{cof}F\bigr)
=\mu(F-J^{-1}F^{-T}).
$$

A stress-free state satisfies $FF^T=J^{-1}I$. Taking [determinants](../../../../determinant.md) yields $J^2=J^{-3}$, so $J=1$ and $FF^T=I$: precisely $F\in SO(3)$. These states are also the global energy [minimizers](../../../../global-minimizer.md). If $v_i>0$ are the [singular values](../../../../singular-value.md), the [arithmetic-geometric mean inequality](../../../../arithmetic-geometric-mean-inequality.md) gives $|F|^2\geq3J^{2/3}$, with equality only when the [singular values](../../../../singular-value.md) are equal. The function $3J^{2/3}/2+J^{-1}$ decreases up to $J=1$ and increases thereafter, with [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) $5/2$. Thus $W\geq5\mu/2$, with equality precisely at [rotations](../../../../rotation-mathematics.md). A constant shift of the energy can set this [minimum](../../../../minimum-of-a-subset-of-a-total-order.md) to zero without changing the [stress](../../../../stress.md).

For the given [simple shear](../../../../simple-shear.md),

$$
F=\begin{pmatrix}1&1&0\\0&1&0\\0&0&1\end{pmatrix},\qquad
F^{-T}=\begin{pmatrix}1&0&0\\-1&1&0\\0&0&1\end{pmatrix},\qquad
T_R=\mu\begin{pmatrix}0&1&0\\1&0&0\\0&0&0\end{pmatrix}.
$$

For a [unit normal](../../../../unit-normal.md) $N$, $|T_RN|^2=\mu^2(N_1^2+N_2^2)=\mu^2(1-N_3^2)$. Hence **every reference [plane](../../../../plane.md) whose [normal](../../../../normal-distribution.md) lies in the $e_1,e_2$ [plane](../../../../plane.md) is maximizing**:

$$
\boxed{N=(\cos\alpha,\sin\alpha,0),\quad
x_1\cos\alpha+x_2\sin\alpha=0,\qquad\max|s_R|=\mu.}
$$

There is a family of maximizing planes, rather than one distinguished [normal](../../../../normal-distribution.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [1](../../1.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
