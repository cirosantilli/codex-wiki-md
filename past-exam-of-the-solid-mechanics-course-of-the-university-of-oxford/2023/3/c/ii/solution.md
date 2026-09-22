<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this [homogeneous motion](../../../../../homogeneous-elastic-deformation.md), suppose the [matrix](../../../../../matrix.md) $\mathbf A=\ddot{\mathbf F}\mathbf F^{-1}$ is symmetric. Put $\mathbf y=\mathbf x-\mathbf c(t)$. The [acceleration potential of a homogeneous motion](../../../../../acceleration-potential-of-a-homogeneous-motion.md) is

$$
\boxed{\xi(\mathbf x,t)
=-\frac12\mathbf y^T\mathbf A(t)\mathbf y
-\ddot{\mathbf c}(t)\cdot\mathbf y+g(t),}
$$

where $g(t)$ is arbitrary. When taking the spatial [gradient](../../../../../gradient.md), $t$, $\mathbf c$, $\ddot{\mathbf c}$, and $\mathbf A$ are fixed. Symmetry gives

$$
\nabla\xi=-\frac12(\mathbf A+\mathbf A^T)\mathbf y-\ddot{\mathbf c}
=-\mathbf A\mathbf y-\ddot{\mathbf c}
=-\ddot{\mathbf x}.
$$

This verifies the potential directly and also proves sufficiency of the [symmetric matrix](../../../../../symmetric-matrix.md) condition within the static-family setting. Its dimension is $\mathsf L^2\mathsf T^{-2}$, so the [pressure](../../../../../pressure-split.md) correction $-\rho\xi$ has the dimension of [stress](../../../../../stress.md). Combining with part (b)(ii), the corresponding dynamic [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) is

$$
\mathbf T=\mathbf T_0(t)+
\left[\frac\rho2\mathbf y^T\mathbf A\mathbf y
+\rho\ddot{\mathbf c}\cdot\mathbf y+\widetilde C(t)\right]\mathbf1,
$$

where $\widetilde C(t)=C(t)-\rho g(t)$. Substituting its [divergence](../../../../../divergence.md) into the [Cauchy momentum equation](../../../../../cauchy-momentum-equation.md) reproduces $\rho[\mathbf A\mathbf y+\ddot{\mathbf c}]$, as required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
