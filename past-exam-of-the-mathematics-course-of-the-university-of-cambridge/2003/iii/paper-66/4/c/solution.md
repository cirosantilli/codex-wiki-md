<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Follow a conserved mass element from its [Lagrangian coordinate](../../../../../../lagrangian-coordinate.md) $\mathbf q$ to its [Eulerian coordinate](../../../../../../eulerian-coordinate.md) $\mathbf x=\mathbf q+b\mathbf p$. The integrated [continuity equation](../../../../../../continuity-equation.md) gives

$$
\rho(\mathbf r,t)a^3\,d^3x=\rho_0\,d^3q,
\qquad
1+\delta=\frac{\rho}{\bar\rho}=
\frac1{J},\qquad J=\det\left(\delta_{ij}+b\frac{\partial p_i}{\partial q_j}\right),
$$

where $\bar\rho=\rho_0/a^3$ and the Lagrangian labels are chosen with uniform reference mass per $d^3q$. These equations hold before [shell crossing](../../../../../../shell-crossing.md), when the oriented determinant is positive. If $\mu_i$ are the eigenvalues of $\partial p_i/\partial q_j$, then

$$
\boxed{1+\delta=\prod_{i=1}^3(1+b\mu_i)^{-1}.}
$$

For an irrotational displacement the deformation matrix is symmetric, so these eigenvalues are real. Using the conventional positive collapse eigenvalues $\lambda_i=-\mu_i$, equivalently the eigenvalues of $-\partial p_i/\partial q_j$, gives

$$
\boxed{1+\delta=\prod_{i=1}^3(1-b\lambda_i)^{-1}.}
$$

There is a sign mismatch in the printed pairing of this last expression with eigenvalues of $+\partial p_i/\partial q_j$: for the displayed plus-sign displacement map, those eigenvalues give plus signs in the determinant. For example, $p_1=cq_1$, $p_2=p_3=0$ makes $x_1=(1+bc)q_1$, so mass conservation gives $1+\delta=(1+bc)^{-1}$, not $(1-bc)^{-1}$. The corrected eigenvalue convention restores the intended formula without changing the map.

Now take $\mathbf p=(p(q_1),0,0)$ and $J=1+bp'$. The physical trajectory is $\mathbf r=a\mathbf x$. Differentiating at fixed $\mathbf q$ gives

$$
\ddot{\mathbf r}=\frac{\ddot a}{a}\mathbf r+
 a(\ddot b+2H\dot b)\mathbf p
=\frac{\ddot a}{a}\mathbf r+4\pi Ga\bar\rho b\mathbf p.
$$

The physical derivative in the perturbed direction is $\partial/\partial r_1=[a(1+bp')]^{-1}\partial/\partial q_1$. The two transverse directions still have the background acceleration. Therefore

$$
\nabla_r\cdot\ddot{\mathbf r}
=3\frac{\ddot a}{a}+4\pi G\bar\rho\frac{bp'}{1+bp'}.
$$

Use the pressureless, $\Lambda=0$ background acceleration equation $3\ddot a/a=-4\pi G\bar\rho$ to obtain

$$
\boxed{\nabla_r\cdot\ddot{\mathbf r}
=-\frac{4\pi G\bar\rho}{1+bp'}=-4\pi G\rho(\mathbf r,t).}
$$

This proves the [planar exactness of the Zeldovich approximation](../../../../../../planar-exactness-of-the-zeldovich-approximation.md) for the requested full force-divergence equation. The displacement depends on only one coordinate, but the divergence includes all three physical directions; discarding the transverse background terms would give the wrong result. The proof is valid until [shell crossing](../../../../../../shell-crossing.md). With the planar gravitational boundary condition fixing the possible spatially uniform force, it is the exact single-stream dust evolution; it does not describe the multistream density by a single invertible map after crossing.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
