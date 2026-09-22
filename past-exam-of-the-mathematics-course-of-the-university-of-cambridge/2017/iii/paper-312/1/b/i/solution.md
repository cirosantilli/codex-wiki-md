<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $h_{ij}={}^{(3)}g_{ij}$, and retain only first-order [scalar cosmological perturbations](../../../../../../../scalar-cosmological-perturbation.md). The inverse [induced metric](../../../../../../../induced-metric.md) and inverse [lapse function](../../../../../../../lapse-function.md) are

$$
h^{ij}=a^{-2}\bigl[(1+2\Phi)\delta^{ij}-2\delta^{ik}\delta^{j\ell}E_{,k\ell}\bigr],\qquad N^{-1}=\bar N^{-1}(1-\Psi).
$$

The flat background spatial connection vanishes, and $N_i=-a^2B_{,i}$ is already first order. Consequently

$$
N_{i|j}=-a^2B_{,ij}+O(\text{perturbation}^2).
$$

The comma on $B_{,i}$ matters: this is the [gradient](../../../../../../../gradient.md) of the scalar [shift vector](../../../../../../../shift-vector.md) potential, not an unrelated vector field. Substituting the time [derivative](../../../../../../../derivative.md) of $h_{ij}$ into the negative [extrinsic curvature](../../../../../../../extrinsic-curvature.md) convention gives

$$
K_{ij}=-\frac{a^2}{\bar N}\left[\frac{\dot a}{a}\bigl((1-2\Phi-\Psi)\delta_{ij}+2E_{,ij}\bigr)-\dot\Phi\delta_{ij}+\dot E_{,ij}-B_{,ij}\right].
$$

Raising the first index with the perturbed inverse [induced metric](../../../../../../../induced-metric.md) is essential. Its $\Phi$ and $E$ terms cancel the corresponding terms multiplying the background [Hubble parameter](../../../../../../../hubble-parameter.md), leaving

$$
K^i{}_j=-H\delta^i_j+\left(\frac{\dot\Phi}{\bar N}+H\Psi\right)\delta^i_j+\frac1{\bar N}\delta^{ik}(B-\dot E)_{,kj}.
$$

For the [scalar shear potential](../../../../../../../scalar-shear-potential.md) $\chi=a^2(\dot E-B)/\bar N$, raised spatial derivatives mean $\partial^i=a^{-2}\delta^{ij}\partial_j$ to the required order. Thus the final term is $-\partial^i\partial_j\chi$. Taking the [trace](../../../../../../../matrix-trace.md) identifies the [scalar expansion perturbation](../../../../../../../scalar-expansion-perturbation.md):

$$
K=-3H+\kappa,\qquad \kappa=3\left(\frac{\dot\Phi}{\bar N}+H\Psi\right)-\Delta\chi,\qquad \Delta=a^{-2}\nabla^2.
$$

Separating the [trace](../../../../../../../matrix-trace.md) and trace-free parts now yields

$$
\boxed{K^i{}_j=-H\delta^i_j+\frac\kappa3\delta^i_j-\left(\partial^i\partial_j-\frac\Delta3\delta^i_j\right)\chi.}
$$

All signs follow from the source's $dx^i-N^i dt$ [shift vector](../../../../../../../shift-vector.md) convention and negative [extrinsic curvature](../../../../../../../extrinsic-curvature.md) definition.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
