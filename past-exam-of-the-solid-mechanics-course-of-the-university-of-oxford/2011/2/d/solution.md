<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Green-Lagrange strain tensor](../../../../green-lagrange-strain-tensor.md) has [eigenvalues](../../../../eigenvalue.md) $(\lambda_j^2-1)/2$. Its [Frobenius norm](../../../../frobenius-norm.md) and trace are invariant under the orthogonal principal-axis change, so

$$
\boxed{W(F)=\frac\mu4\sum_{j=1}^3(\lambda_j^2-1)^2+\frac\lambda8\left(\sum_{j=1}^3\lambda_j^2-3\right)^2.}
$$

For the homogeneous dilation $F=\rho I$, put $K=\mu+3\lambda/2$. Then $E=(\rho^2-1)I/2$. Differentiating the energy through $E$ gives the [second Piola-Kirchhoff stress tensor](../../../../second-piola-kirchhoff-stress-tensor.md) $2\mu E+\lambda\operatorname{tr}(E)I=K(\rho^2-1)I$, and multiplication by $F$ gives the [first Piola-Kirchhoff stress tensor](../../../../first-piola-kirchhoff-stress-tensor.md). Thus

$$
\boxed{T=\rho K(\rho^2-1)I,\qquad S=J^{-1}TF^T=\frac{K(\rho^2-1)}\rho I.}
$$

The normals of the reference and deformed spheres point in the same radial direction. As $\rho\downarrow0$, the reference [traction](../../../../traction.md) magnitude $|T N|$ tends to zero, while the current [traction](../../../../traction.md) magnitude $|S n|$ tends to infinity, provided $K>0$, as for physically stable [Lamé parameters](../../../../lame-parameter.md). The negative signs of the [stress](../../../../stress.md) coefficients for $0<\rho<1$ indicate compression.

There is no contradiction: the current [area](../../../../surface-area.md) is $\rho^2$ times the reference [area](../../../../surface-area.md), so the same [force](../../../../force-split.md) divided by the vanishing current [area](../../../../surface-area.md) has the larger [stress](../../../../stress.md). Indeed $T N=\rho^2S n$. The limiting map at $\rho=0$ is not itself an admissible [deformation in continuum mechanics](../../../../deformation-mechanics.md); the statement concerns the approach through positive $\rho$. A degenerate choice $K=0$ would not have the asserted growth without bound.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
