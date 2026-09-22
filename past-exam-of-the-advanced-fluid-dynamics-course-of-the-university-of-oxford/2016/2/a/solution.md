<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label a trajectory by $\mathbf a$ and write its [flow map](../../../../flow-map.md) as $\mathbf X(\mathbf a,t)$, with $\partial_t\mathbf X=\mathbf u(\mathbf X,t)$. An infinitesimal [material line](../../../../material-curve.md) joining neighboring labels has tangent $\ell_i=F_{ij}\,d a_j$, where $F_{ij}=\partial X_i/\partial a_j$ is the [deformation gradient](../../../../deformation-gradient.md). Differentiating at fixed labels gives

$$
\frac{D\ell_i}{Dt}=\partial_j u_i\,\ell_j,
\qquad
\boxed{\partial_t\boldsymbol\ell+\mathbf u\cdot\nabla\boldsymbol\ell=(\boldsymbol\ell\cdot\nabla)\mathbf u.}
$$

This identity holds for an unnormalized [material line](../../../../material-curve.md) tangent even in a compressible flow. [Incompressibility](../../../../incompressible-flow.md) also makes an advected [magnetic field](../../../../magnetic-field-split.md) obey the same stretching law. A unit tangent would instead require a projection removing its change of length.

Use the source's [velocity gradient](../../../../velocity-gradient.md) convention $G_{ij}=\partial_i u_j$. For a [outer product](../../../../outer-product.md) $A_{ij}=\ell_i\ell_j$, the [product rule](../../../../product-rule.md) yields

$$
\frac{DA_{ij}}{Dt}=(\partial_k u_i)A_{kj}+A_{ik}(\partial_k u_j)
=(G^T\mathsf A+\mathsf A G)_{ij}.
$$

The same law holds for a sum or locally transported average of such [outer products](../../../../outer-product.md). Thus the [dyadic transport of material line elements](../../../../dyadic-transport-of-material-line-elements.md) motivates

$$
\boxed{\overset{\triangledown}{\mathsf A}=\partial_t\mathsf A+\mathbf u\cdot\nabla\mathsf A-\mathsf A G-G^T\mathsf A.}
$$

This [upper-convected derivative](../../../../upper-convected-derivative.md) vanishes for a symmetric [tensor](../../../../tensor.md) transported solely by stretching of [material lines](../../../../material-curve.md). It subtracts both advection and geometric deformation, allowing a [constitutive equation](../../../../constitutive-equation.md) to isolate intrinsic relaxation or production. More generally $\mathsf A=F\mathsf A_{\rm ref}F^T$ gives $\overset{\triangledown}{\mathsf A}=F\dot{\mathsf A}_{\rm ref}F^T$. Under a time-dependent rigid rotation $Q$, its value transforms as $Q\overset{\triangledown}{\mathsf A}Q^T$, making it an [objective time derivative](../../../../objective-time-derivative.md). This is a suitable derivative for this transport type; symmetry alone does not make it the unique possible [objective time derivative](../../../../objective-time-derivative.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
