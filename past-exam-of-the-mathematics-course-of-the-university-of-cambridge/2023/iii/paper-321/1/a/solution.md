<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the [razor-thin disk approximation](../../../../../../razor-thin-disk-approximation.md), the three-dimensional [Poisson equation](../../../../../../poisson-equation.md) is

$$
\nabla^2\Phi_d=4\pi G\Sigma(x,y)\delta(z).
$$

For a horizontal [Fourier mode](../../../../../../fourier-mode.md) with [wavevector](../../../../../../wavevector.md) $\mathbf k$ and $k=|\mathbf k|>0$, the [Fourier transform](../../../../../../fourier-transform.md) of this equation is

$$
\left(\frac{d^2}{dz^2}-k^2\right)\widehat\Phi_d
=4\pi G\widehat\Sigma\,\delta(z).
$$

The solution that decays away from the disk is

$$
\widehat\Phi_d(\mathbf k,z)
=-\frac{2\pi G}{k}\widehat\Sigma(\mathbf k)e^{-k|z|}.
$$

Consequently the required [razor-thin disk Poisson kernel](../../../../../../razor-thin-disk-poisson-kernel.md) in the midplane is

$$
\boxed{\widehat\Phi_{d,m}(\mathbf k)
=-\frac{2\pi G}{k}\widehat\Sigma(\mathbf k)}.
$$

The spatially uniform $k=0$ background is excluded from this local perturbation formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
