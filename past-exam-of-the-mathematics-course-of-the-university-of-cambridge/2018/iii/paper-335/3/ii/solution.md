<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To first order in $n_\epsilon$, replace $q$ by $2n_\epsilon$ and use the known incident field in the outgoing integral. The [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md) gives

$$
\boxed{\psi_s(\mathbf r)\simeq2k_0^2\int_BG_{k_0}(\mathbf r,\mathbf r')\psi_{inc}(\mathbf r')n_\epsilon(\mathbf r')\,d\mathbf r'.}
$$

Both the $n_\epsilon^2$ contrast term and the internal-field correction are second order for fixed geometry in the perturbative regime established in part i.

Specify the data space before taking an [adjoint operator](../../../../../../adjoint-operator.md). For example, let $X=L^2(B)$ and $Y=L^2(\Gamma)$, where $\Gamma$ is a bounded measurement surface separated from $B$. Define the [linear operator](../../../../../../linear-operator.md)

$$
(Af)(\mathbf r)=2k_0^2\int_BG_{k_0}(\mathbf r,\mathbf r')\psi_{inc}(\mathbf r')f(\mathbf r')\,d\mathbf r',\qquad\mathbf r\in\Gamma.
$$

For bounded incident field this is a [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md), hence a [compact operator](../../../../../../compact-operator-split.md). The equation is $An_\epsilon=y$, with $y=\psi_s|_\Gamma$. Other sampling geometries give corresponding data spaces and weights; the paper does not specify one. Using the usual complex $L^2$ inner products, its [adjoint operator](../../../../../../adjoint-operator.md) is

$$
(A^*y)(\mathbf r')=2k_0^2\overline{\psi_{inc}(\mathbf r')}\int_\Gamma\overline{G_{k_0}(\mathbf r,\mathbf r')}y(\mathbf r)\,dS(\mathbf r).
$$

The complex conjugations are required by the [adjoint operator](../../../../../../adjoint-operator.md) identity, not by [wave reciprocity](../../../../../../wave-reciprocity.md) alone.

The [Landweber iteration](../../../../../../landweber-iteration.md) starts from $f_0=0$ and applies [gradient descent](../../../../../../gradient-descent.md) to $\frac12\|Af-y\|^2$:

$$
\boxed{f_{m+1}=f_m+\tau A^*(y-Af_m),\qquad0<\tau<\frac2{\|A\|^2}.}
$$

Each step back-propagates the data residual. The [Landweber relaxation parameter](../../../../../../landweber-relaxation-parameter.md) controls stability, and [early stopping of Landweber iteration](../../../../../../early-stopping-of-landweber-iteration.md) prevents small [singular values](../../../../../../singular-value.md) from amplifying [measurement errors](../../../../../../measurement-error.md). For an explicitly real-valued index contrast, use the real [Hilbert space](../../../../../../hilbert-space-split.md) structure and replace $A^*$ by $\operatorname{Re}A^*$ in this update. Additional sign or support constraints require corresponding projections; none are assumed here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
