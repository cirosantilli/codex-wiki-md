<h1 id="33c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Contract the two Levi-Civita symbols:

$$
\begin{aligned}
L_iL_i
&=\varepsilon_{ijk}\varepsilon_{i\ell m}
X_jP_kX_\ell P_m\\
&=(\delta_{j\ell}\delta_{km}-\delta_{jm}\delta_{k\ell})
X_jP_kX_\ell P_m.
\end{aligned}
$$

Moving momenta past positions with  
$P_kX_\ell=X_\ell P_k-i\hbar\delta_{k\ell}$ gives the [squared orbital angular momentum in position and momentum operators](../../../../../../squared-orbital-angular-momentum-in-position-and-momentum-operators.md):

$$
\boxed{
L^2=X^2P^2-(X\cdot P)^2+i\hbar X\cdot P}.
$$

Therefore

$$
\boxed{c_1=i\hbar,\qquad c_2=1,\qquad c_3=-1}.
$$

In position representation,

$$
P=-i\hbar\nabla,
\qquad
X\cdot P=-i\hbar r\partial_r,
$$

and

$$
\nabla^2=\partial_r^2+\frac2r\partial_r+\frac1{r^2}\nabla_{S^2}^2.
$$

Also $(r\partial_r)^2=r^2\partial_r^2+r\partial_r$. Substitution into the Cartesian identity gives

$$
\begin{aligned}
L^2
&=-\hbar^2r^2\nabla^2
+\hbar^2(r\partial_r)^2
+\hbar^2r\partial_r\\
&=-\hbar^2\nabla_{S^2}^2,
\end{aligned}
$$

because every radial derivative cancels. Hence

$$
\boxed{L^2=-\hbar^2\nabla_{S^2}^2},
$$

the [spherical Laplacian from orbital angular momentum](../../../../../../spherical-laplacian-from-orbital-angular-momentum.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [33C](../../33c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
