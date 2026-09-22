<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $w$ constant and $w\ne-1$, with a barotropic perturbation $\delta P=w\delta\rho$. Define the [density contrast](../../../../../../density-contrast.md) $\delta=\delta\rho/\bar\rho$ and use the scalar [velocity potential](../../../../../../velocity-potential.md) convention $v_i(\mathbf k)=ik_i\theta(\mathbf k)$, so $\partial_iv^i=-k^2\theta$. This $\theta$ is a potential, not the sometimes-used velocity-divergence variable. In [synchronous gauge in cosmology](../../../../../../synchronous-gauge-in-cosmology.md), the inverse metric is $g^{00}=-a^{-2}$ and $g^{ij}=a^{-2}(\delta^{ij}-h^{ij})$ to first order. Discarding products of perturbations in the [perfect fluid in general relativity](../../../../../../perfect-fluid-in-general-relativity.md) gives

$$
\boxed{T^{00}=a^{-2}\bar\rho(1+\delta),\quad T^{0i}=a^{-2}(1+w)\bar\rho\,ik_i\theta,\quad T^{ij}=a^{-2}w\bar\rho[(1+\delta)\delta^{ij}-h^{ij}].}
$$

For the linearization, each $h_{ij}$ must be small: the PDF's determinant condition alone is insufficient, since $h=\operatorname{diag}(L,0,0)$ has zero determinant even for large $L$.

Write $\mathcal H=a'/a$. The time component of [covariant conservation of stress-energy](../../../../../../stress-energy-conservation.md) is

$$
\partial_\mu T^{0\mu}+\Gamma^0_{\mu\nu}T^{\mu\nu}+\Gamma^\mu_{\mu\nu}T^{0\nu}=0.
$$

Here $\Gamma^\mu_{\mu0}=4\mathcal H+h'/2$. To first order, $\Gamma^0_{ij}T^{ij}=a^{-2}w\bar\rho[3\mathcal H(1+\delta)+h'/2]$: the two metric-$h$ contributions cancel. Multiplying the conservation equation by $a^2$, including $\Gamma^0_{00}T^{00}$, gives

$$
\bar\rho'(1+\delta)+\bar\rho\delta'+3\mathcal H(1+w)\bar\rho(1+\delta)-(1+w)\bar\rho k^2\theta+\tfrac12(1+w)\bar\rho h'=0.
$$

The background [cosmological perfect-fluid continuity equation](../../../../../../cosmological-perfect-fluid-continuity-equation.md), $\bar\rho'=-3\mathcal H(1+w)\bar\rho$, cancels the first and third terms. Thus

$$
\boxed{\delta'-(1+w)k^2\theta+\tfrac12(1+w)h'=0.}
$$

The $h'$ term accounts for perturbation of the spatial volume expansion in [synchronous gauge in cosmology](../../../../../../synchronous-gauge-in-cosmology.md). The PDF's correct connection $\Gamma^i_{0j}=\mathcal H\delta^i_j+h'^i{}_j/2$ is garbled in the TeX aid.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
