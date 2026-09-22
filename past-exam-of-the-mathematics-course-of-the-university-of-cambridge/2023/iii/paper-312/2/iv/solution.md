<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Applying the scalar transformation from part i to both fields gives

$$
\langle\Delta O\rangle
=\omega_{ij}\sum_{a=1}^2k_{a i}\frac{\partial}{\partial k_{a j}}
\left[(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2)P_\varphi(k_1)\right].
$$

The derivative of the [Dirac delta distribution](../../../../../../dirac-delta-function.md) is proportional to $\delta_{ij}$ and vanishes after contraction with traceless $\omega_{ij}$. Removing that delta function leaves

$$
\langle\Delta O\rangle'
=\omega_{ij}k_i\frac{\partial}{\partial k_j}P_\varphi(k).
$$

Equating the two sides of the [Ward-Takahashi identity](../../../../../../ward-identity.md) and resolving the soft graviton into a polarization $s$ yields the [cosmological soft-graviton consistency relation](../../../../../../cosmological-soft-graviton-consistency-relation.md)

$$
\boxed{
\lim_{q\to0}
\frac{\langle\gamma^s(\mathbf q)
\varphi(\mathbf k)\varphi(-\mathbf k-\mathbf q)\rangle'}{P_\gamma(q)}
=-\frac12\epsilon_{ij}^s(\mathbf q)
k_i\frac{\partial}{\partial k_j}P_\varphi(k)}.
$$

For an isotropic power spectrum this is equivalently

$$
-\epsilon_{ij}^s k_i k_j\frac{\partial P_\varphi}{\partial k^2}.
$$

The long-wavelength [adiabatic tensor mode](../../../../../../adiabatic-tensor-mode.md) acts on the short two-point function as an anisotropic rescaling of its momentum.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
