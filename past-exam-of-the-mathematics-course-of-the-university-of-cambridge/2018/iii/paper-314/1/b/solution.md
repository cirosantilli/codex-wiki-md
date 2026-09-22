<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $q=\mathbf u\cdot\boldsymbol\omega$ for the [kinetic helicity density](../../../../../../kinetic-helicity-density.md), and retain $\mathcal B=w+u^2/2$. Since $\boldsymbol\omega$ is a [curl](../../../../../../curl.md), $\nabla\cdot\boldsymbol\omega=0$. Differentiating the density and using the equations from the preceding part gives

$$
\partial_tq=-\boldsymbol\omega\cdot\nabla\mathcal B+\mathbf u\cdot\nabla\times(\mathbf u\times\boldsymbol\omega).
$$

The [divergence of a cross product](../../../../../../divergence-of-a-cross-product.md) gives

$$
\nabla\cdot\{\mathbf u\times(\mathbf u\times\boldsymbol\omega)\}=(\mathbf u\times\boldsymbol\omega)\cdot\boldsymbol\omega-\mathbf u\cdot\nabla\times(\mathbf u\times\boldsymbol\omega).
$$

The first term on the right is zero, while $\boldsymbol\omega\cdot\nabla\mathcal B=\nabla\cdot(\mathcal B\boldsymbol\omega)$. Thus the [kinetic helicity conservation law](../../../../../../kinetic-helicity-conservation-law.md) has flux

$$
\boxed{\mathbf F_{H_k}=\mathcal B\boldsymbol\omega+\mathbf u\times(\mathbf u\times\boldsymbol\omega)=q\mathbf u+\left(w-\frac{u^2}{2}\right)\boldsymbol\omega,\qquad\partial_tq+\nabla\cdot\mathbf F_{H_k}=0.}
$$

The last equality for the flux uses the [vector triple product identity](../../../../../../vector-triple-product.md). Integrating and applying the [divergence theorem](../../../../../../divergence-theorem.md) gives $d\int_Vq\,dV/dt=-\int_{\partial V}\mathbf F_{H_k}\cdot\mathbf n\,dS$ for a fixed volume. Hence its total [kinetic helicity](../../../../../../hydrodynamical-helicity.md) is conserved when the boundary flux vanishes; for example, tangency of both [velocity field](../../../../../../velocity-field.md) and [vorticity](../../../../../../vorticity.md) to the boundary is sufficient. The local [conservation law](../../../../../../conservation-law.md) does not by itself imply that its density follows each fluid particle unchanged.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
