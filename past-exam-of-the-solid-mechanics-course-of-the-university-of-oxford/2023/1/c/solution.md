<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiplying the [deformation gradient](../../../../deformation-gradient.md) by its [matrix transpose](../../../../transpose.md) gives the [left Cauchy-Green deformation tensor](../../../../left-cauchy-green-deformation-tensor.md) and its [trace](../../../../matrix-trace.md):

$$
\mathbf B=\begin{pmatrix}
1&0&0\\
0&1+\tau^2r^2&\tau r\\
0&\tau r&1
\end{pmatrix},\qquad I_1=3+\tau^2r^2.
$$

The derivative of the [strain energy density](../../../../strain-energy-density.md) is

$$
\hat w'(I_1)=\mu_1+\mu_2 I_1^n.
$$

For brevity put $g(r)=\mu_1+\mu_2(3+\tau^2r^2)^n$. Part (a) gives the [Cauchy stress tensor](../../../../cauchy-stress-tensor.md), in the current [cylindrical coordinate system](../../../../cylindrical-coordinate-system.md) [orthonormal basis](../../../../orthonormal-basis.md), as

$$
\boxed{\mathbf T=\begin{pmatrix}
2g-p&0&0\\
0&2g(1+\tau^2r^2)-p&2g\tau r\\
0&2g\tau r&2g-p
\end{pmatrix}.}
$$

In particular, the end-face [shear stress](../../../../shear-stress.md) is $T_{\theta z}=2g\tau r$. The undetermined [pressure](../../../../pressure-split.md) $p$ affects the normal [stresses](../../../../stress.md) but does not affect this [shear stress](../../../../shear-stress.md). No normal [traction](../../../../traction.md) conditions have been specified to determine $p$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
