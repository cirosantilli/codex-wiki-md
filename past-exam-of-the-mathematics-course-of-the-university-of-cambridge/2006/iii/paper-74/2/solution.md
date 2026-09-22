<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\langle\cdot\rangle$ denote the spatial average. Assume periodicity, or an equivalent homogeneous averaging limit in which total derivatives average to zero and [integration by parts](../../../../../integration-by-parts.md) is valid. Fix the induced field to have zero mean. Expand the solution of the [resistive induction equation](../../../../../resistive-induction-equation.md) in small [magnetic Reynolds number](../../../../../magnetic-reynolds-number.md):

$$
\mathbf b=R_m\mathbf b_1+R_m^2\mathbf b_2+\cdots,\qquad
\Delta\mathbf b_1=-(\mathbf B\cdot\nabla)\mathbf u,\qquad
\Delta\mathbf b_2=-\nabla\times(\mathbf u\times\mathbf b_1).
$$

The uniform test [magnetic field](../../../../../magnetic-field.md) commutes with differentiation. Since $\Delta\mathbf u=-\mathbf u$, the first equation has solution $\mathbf b_1=(\mathbf B\cdot\nabla)\mathbf u$.

The quadratic second-order forcing need not be monochromatic, so one must not simply replace its inverse [Laplacian](../../../../../laplacian.md) by multiplication by $-1$. Instead use the [self-adjointness](../../../../../self-adjoint-operator.md) of the [Laplacian](../../../../../laplacian.md) under the average:

$$
\langle\mathbf u\times\mathbf b_2\rangle
=-\langle\Delta\mathbf u\times\mathbf b_2\rangle
=-\langle\mathbf u\times\Delta\mathbf b_2\rangle
=\langle\mathbf u\times\nabla\times(\mathbf u\times\mathbf b_1)\rangle.
$$

This proves the [monochromatic small-Reynolds-number mean electromotive force](../../../../../monochromatic-small-reynolds-number-mean-electromotive-force.md) expansion

$$
\boxed{\boldsymbol{\mathcal E}
=R_m\langle\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u\rangle
+R_m^2\langle\mathbf u\times\nabla\times[\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u]\rangle
+O(R_m^3).}
$$

For the [symmetry of the first-order monochromatic alpha tensor](../../../../../symmetry-of-the-first-order-monochromatic-alpha-tensor.md), write

$$
\alpha^{(1)}_{ij}=\epsilon_{ikl}\langle u_k\partial_j u_l\rangle.
$$

Its antisymmetric part is determined by contraction with the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). The contraction identity gives

$$
\epsilon_{pij}\alpha^{(1)}_{ij}
=\langle u_j\partial_j u_p-u_p\partial_j u_j\rangle.
$$

The second term vanishes by [incompressibility](../../../../../incompressible-flow.md); the first is $\langle\partial_j(u_ju_p)\rangle=0$. Since every three-dimensional [antisymmetric second-rank tensor](../../../../../antisymmetric-second-rank-tensor.md) is equivalent to its contracted axial vector, **$\alpha^{(1)}$ is symmetric**. No [Fourier series](../../../../../fourier-series-split.md) or [Fourier transform](../../../../../fourier-transform.md) is required.

To derive the next identity, set $\mathbf C=\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u$. Expanding the [curl](../../../../../curl.md) and [cross product](../../../../../cross-product.md) in components,

$$
(\mathbf u\times\nabla\times\mathbf C)_i
=u_j\partial_iC_j-u_j\partial_jC_i.
$$

The average of the second term is zero: [integration by parts](../../../../../integration-by-parts.md) makes it $-\langle C_i\partial_j u_j\rangle$. Integrating the first term by parts gives

$$
\boxed{\mathcal E_i^{(2)}=-\langle(\partial_i u_j)\,[\mathbf u\times(\mathbf B\cdot\nabla)\mathbf u]_j\rangle.}
$$

Extracting the coefficient of $B_j$ now yields

$$
\alpha^{(2)}_{ij}
=-\langle\partial_i\mathbf u\cdot(\mathbf u\times\partial_j\mathbf u)\rangle
=\langle\mathbf u\cdot(\partial_i\mathbf u\times\partial_j\mathbf u)\rangle.
$$

Interchanging $i$ and $j$ reverses the [cross product](../../../../../cross-product.md), proving the [antisymmetry of the second-order monochromatic alpha tensor](../../../../../antisymmetry-of-the-second-order-monochromatic-alpha-tensor.md):

$$
\boxed{\alpha^{(1)}_{ij}=\alpha^{(1)}_{ji},\qquad
\alpha^{(2)}_{ij}=-\alpha^{(2)}_{ji}.}
$$

The second coefficient of the [alpha tensor](../../../../../alpha-tensor.md) can therefore contribute [turbulent magnetic pumping](../../../../../turbulent-magnetic-pumping.md), while its symmetric part vanishes at this order.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
