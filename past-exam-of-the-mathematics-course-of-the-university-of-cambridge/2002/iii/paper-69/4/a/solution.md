<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the interaction [matrix](../../../../../../matrix.md) as $\mathsf J$ to distinguish it from its scalar strength. The printed pair sum contains both orientations and has no factor $1/2$. For a [positive-definite matrix](../../../../../../positive-definite-matrix.md) $\mathsf J$, completion of the square gives the [Hubbard–Stratonovich transformation](../../../../../../hubbard-stratonovich-transformation.md)

$$
\int_{\mathbb R^N}d^Nm\,e^{-m^T\mathsf J^{-1}m+2m^T\sigma}
=\pi^{N/2}\sqrt{\det\mathsf J}\,e^{\sigma^T\mathsf J\sigma},
$$

since $m^T\mathsf J^{-1}m-2m^T\sigma=(m-\mathsf J\sigma)^T\mathsf J^{-1}(m-\mathsf J\sigma)-\sigma^T\mathsf J\sigma$. For the exponential kernel with $J>0$ and $\kappa>0$, positivity follows from the positive Fourier symbol derived in part (b), or from its finite open-chain [covariance](../../../../../../covariance.md) [matrix](../../../../../../matrix.md).

Insert this identity into the [Ising model](../../../../../../ising-model.md) partition sum and interchange the finite spin sum with the convergent [Gaussian integral](../../../../../../gaussian-integral.md). The spin variables now factor independently:

$$
\sum_{\sigma_i=\pm1}e^{(2m_i+h)\sigma_i}=2\cosh(2m_i+h).
$$

It follows that

$$
\boxed{\mathcal Z=C\int_{\mathbb R^N}\prod_i dm_i\,
\exp\left[-\sum_{ij}m_i[\mathsf J^{-1}]_{ij}m_j+\sum_i\log(2\cosh(2m_i+h))\right],}
$$

with $C=(\pi^N\det\mathsf J)^{-1/2}$ for the measure used here. The factor two in the spin-field coupling is required by the double pair sum; replacing it by one would decouple a [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) with a different normalization. The diagonal $J_{ii}\sigma_i^2=J$ is a spin-independent energy. Including it as printed makes the positive Gaussian identity directly applicable; if diagonal self-couplings are removed they should first be restored as an irrelevant constant before this real auxiliary-field decoupling.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
