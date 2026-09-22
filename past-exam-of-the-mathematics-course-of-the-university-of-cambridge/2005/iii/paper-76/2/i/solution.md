<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In [mean-field electrodynamics](../../../../../../mean-field-electrodynamics.md), use [Reynolds averaging](../../../../../../reynolds-averaging.md) to write $\mathbf U_{\mathrm{tot}}=\overline{\mathbf U}+\mathbf u$ and $\mathbf B_{\mathrm{tot}}=\overline{\mathbf B}+\mathbf b$, with zero-mean fluctuations. Assume the averaging operation commutes with the [derivatives](../../../../../../derivative.md) and that resolved quantities vary little across an averaging region. Averaging the induction equation then gives

$$
\partial_t\overline{\mathbf B}=\nabla\times(\overline{\mathbf U}\times\overline{\mathbf B}+\boldsymbol{\mathcal E})+\eta\nabla^2\overline{\mathbf B},\qquad\boldsymbol{\mathcal E}=\langle\mathbf u\times\mathbf b\rangle.
$$

This is the [mean-field electromotive force](../../../../../../mean-field-electromotive-force.md), a vector correlation with units of velocity times [magnetic field](../../../../../../magnetic-field.md). The closure problem is to express this correlation in terms of the resolved field.

In the kinematic regime the flow statistics are prescribed, so the response is linear in the mean [magnetic field](../../../../../../magnetic-field.md), after independently excited fluctuation transients have decayed. If the mean-field scale $L$ is much greater than the turbulent scale $\ell$, and its evolution is slow compared with the response memory, expand that response in the local mean [magnetic field](../../../../../../magnetic-field.md) and its gradients:

$$
\mathcal E_i=\alpha_{ij}\overline B_j+c_{ijk}\partial_k\overline B_j+\cdots.
$$

Without scale separation one generally has a spatially nonlocal and temporally retarded response rather than constant local coefficients.

For [homogeneous turbulence](../../../../../../homogeneous-turbulence.md) the coefficients are independent of position. Invariance under proper rotations makes the rank-two response proportional to $\delta_{ij}$, and the isotropic rank-three gradient response proportional to the alternating tensor. Choosing the [diffusivity](../../../../../../diffusion-coefficient.md) sign convention gives

$$
\boxed{\boldsymbol{\mathcal E}=\alpha\overline{\mathbf B}-\beta\nabla\times\overline{\mathbf B}+\cdots.}
$$

The [alpha effect](../../../../../../alpha-effect.md) can regenerate a mean [magnetic field](../../../../../../magnetic-field.md), while $\beta$ supplies [turbulent magnetic diffusivity](../../../../../../turbulent-magnetic-diffusivity.md). For constant positive $\beta$, $\nabla\times(-\beta\nabla\times\overline{\mathbf B})=\beta\nabla^2\overline{\mathbf B}$ because the [magnetic field](../../../../../../magnetic-field.md) is [solenoidal](../../../../../../solenoidal-vector-field.md). Thus the total [diffusivity](../../../../../../diffusion-coefficient.md) is $\eta+\beta$.

The electromotive vector is a [polar vector](../../../../../../polar-vector.md), whereas the [magnetic field](../../../../../../magnetic-field.md) is an [axial vector](../../../../../../pseudovector.md). Therefore $\alpha$ is a [pseudoscalar](../../../../../../pseudoscalar.md) and changes sign under reflection; $\beta$ is an ordinary scalar. A nonzero isotropic [alpha effect](../../../../../../alpha-effect.md) requires broken reflection symmetry, such as nonzero [kinetic helicity](../../../../../../hydrodynamical-helicity.md). If “isotropic” includes reflection symmetry as well as rotations, $\alpha$ must vanish. The dimensions are $[\alpha]=L/T$ and $[\beta]=L^2/T$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
