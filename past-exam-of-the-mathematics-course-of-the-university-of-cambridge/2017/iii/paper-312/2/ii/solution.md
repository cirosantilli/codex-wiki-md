<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The collisionless [Boltzmann equation](../../../../../../boltzmann-equation.md) is conservation of $f$ along the [photon](../../../../../../photon.md) trajectory. To linear order, use the unperturbed trajectory $d\mathbf x/d\eta=\mathbf e$ when differentiating $\Theta$. Deflection of $\mathbf e$ is first order and multiplies the first-order angular dependence of $\delta f$, while the background has no angular dependence; it therefore contributes only at second order. Similarly, the energy derivative of $\delta f$ times the perturbed energy change is second order. Thus

$$
0=\frac{df}{d\eta}=\bar f'(\epsilon)\frac{d\epsilon}{d\eta}-\epsilon\bar f'(\epsilon)\left(\frac{\partial\Theta}{\partial\eta}+\mathbf e\cdot\nabla\Theta\right).
$$

For a nontrivial spectrum this identifies the linear [Free-streaming photon Boltzmann equation](../../../../../../free-streaming-photon-boltzmann-equation.md):

$$
\boxed{\frac{\partial\Theta}{\partial\eta}+\mathbf e\cdot\nabla\Theta-\frac{d\ln\epsilon}{d\eta}=0.}
$$

In [Newtonian gauge in cosmology](../../../../../../newtonian-gauge.md), substitute the specified scalar gravitational-redshift source to write

$$
\dot\Theta+e^j\partial_j\Theta=\dot\phi-e^j\partial_j\psi.
$$

Multiply its [angular average](../../../../../../angular-average.md) by four. Since $\langle e^j\rangle_\Omega=0$, the [photon angular temperature moments](../../../../../../photon-angular-temperature-moments.md) imply the [photon continuity equation](../../../../../../photon-continuity-equation.md)

$$
\boxed{\dot\delta+\frac43\nabla\cdot\mathbf v-4\dot\phi=0.}
$$

For the [photon Euler equation](../../../../../../photon-euler-equation.md), multiply by $3e^i$ and average. The source is $-3\langle e^ie^j\rangle_\Omega\partial_j\psi=-\partial^i\psi$, while the second angular moment is

$$
\langle\Theta e^ie^j\rangle_\Omega=\frac{\delta\,\delta^{ij}}{12}-\frac{\Pi^{ij}}{4\bar\rho}.
$$

It follows that

$$
\boxed{\dot v^i+\frac14\delta^{ij}\partial_j\delta-\frac3{4\bar\rho}\partial_j\Pi^{ij}+\delta^{ij}\partial_j\psi=0.}
$$

The background [energy density](../../../../../../energy-density.md) is spatially homogeneous, so no spatial derivative acts on $\bar\rho$. The minus sign of its [anisotropic stress](../../../../../../anisotropic-stress.md) term follows from the PDF's $\Pi=-\pi$ convention. Switching to the conventional trace-free stress $\pi$ changes that term to a plus sign.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
