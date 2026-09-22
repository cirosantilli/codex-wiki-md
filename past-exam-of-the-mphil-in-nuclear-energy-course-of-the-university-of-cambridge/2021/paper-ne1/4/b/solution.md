<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first equation is a prescribed first-order removal law. For a constant absorption coefficient,

$$
\frac{dN_{\rm Th}}{N_{\rm Th}}=-\sigma_{a\rm Th}\phi(t)\,dt.
$$

Integrating from the initial condition gives

$$
\ln\frac{N_{\rm Th}(t)}{N_{\rm Th0}}=-\sigma_{a\rm Th}\int_0^t\phi(t')\,dt',
$$

and hence

$$
\boxed{N_{\rm Th}(t)=N_{\rm Th0}e^{-\sigma_{a\rm Th}\Phi(t)}.}
$$

The [neutron fluence](../../../../../neutron-fluence.md) $\Phi$ is the time integral of scalar [neutron flux](../../../../../neutron-flux.md); it has inverse-area units, making $\sigma\Phi$ dimensionless. Constant flux is not needed for this integration, but a constant effective coefficient is.

## ↑ Ancestors (10)

1. [B](../b.md)
2. [4](../../4.md)
3. [Module NE1](../../../paper-ne1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
