<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) convention stated above, and lower indices with the [Minkowski metric](../../../../minkowski-metric.md) $g=\operatorname{diag}(-1,1,1,1)$. Lowering a single time index changes its sign. Summing both orders of each antisymmetric index pair gives the [Lorentz scalar](../../../../lorentz-scalar.md)

$$
F_{\kappa\lambda}F^{\kappa\lambda}
=2\sum_iF_{0i}F^{0i}+\sum_{i,j}F_{ij}F^{ij}
=2(B^2-E^2/c^2).
$$

For $T^{00}$, $F_j{}^0=F^{j0}=-E_j/c$ and $g^{00}=-1$. Direct substitution in the printed [electromagnetic stress-energy tensor](../../../../electromagnetic-stress-energy-tensor.md) yields

$$
\begin{aligned}
T^{00}&=\epsilon_0c^2\left[-\sum_j(E_j/c)(-E_j/c)
+\frac14\,2(B^2-E^2/c^2)\right]\\
&=\frac{\epsilon_0}{2}(E^2+c^2B^2).
\end{aligned}
$$

For a spatial index $i$, $g^{0i}=0$ and $F_j{}^i=F^{ji}=-\epsilon_{ijk}B_k$. Hence

$$
T^{0i}=-\epsilon_0c^2\sum_jF^{0j}F_j{}^i
=\epsilon_0c\epsilon_{ijk}E_jB_k.
$$

Thus the full top row is

$$
\boxed{T^{0\nu}=\left(u_{\rm EM},\frac{S_x}c,\frac{S_y}c,\frac{S_z}c\right),\qquad
u_{\rm EM}=\frac12\left(\epsilon_0E^2+\frac{B^2}{\mu_0}\right),\quad
\mathbf S=\frac1{\mu_0}\mathbf E\times\mathbf B.}
$$

Here $u_{\rm EM}$ is the [electromagnetic energy density](../../../../electromagnetic-energy-density.md) and $\mathbf S$ the [Poynting vector](../../../../poynting-vector.md), using $\epsilon_0\mu_0c^2=1$. By the symmetry $T^{0i}=T^{i0}$, these components describe both [energy](../../../../energy-split.md) flux divided by $c$ and $c$ times the [electromagnetic momentum density](../../../../electromagnetic-momentum-density.md) $\mathbf g=\mathbf S/c^2$. Keeping the factor $c$ is essential because the time coordinate is $ct$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
