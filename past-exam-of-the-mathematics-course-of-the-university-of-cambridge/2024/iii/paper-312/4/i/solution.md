<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\widehat{\mathbf n}$ point from the observer toward the emission point, so the photon propagation direction is $\widehat{\mathbf p}=-\widehat{\mathbf n}$ and

$$
\mathbf x(\eta)=\mathbf x_0+(\eta_0-\eta)\widehat{\mathbf n}.
$$

Along this path $D=d/d\eta=\partial_\eta-\widehat{\mathbf n}\cdot\nabla$. Substituting $\widehat{\mathbf p}=-\widehat{\mathbf n}$ into the [Photon Boltzmann equation with Thomson scattering](../../../../../../photon-boltzmann-equation-with-thomson-scattering.md) gives

$$
D(\Theta+\Psi)+\Gamma(\Theta+\Psi)
=\Phi'+\Psi'+\Gamma(\Theta_0+\Psi-\widehat{\mathbf n}\cdot\mathbf v_e).
$$

Because $\partial_\eta e^{-\tau}=\Gamma e^{-\tau}$, multiplication by the integrating factor gives

$$
D[e^{-\tau}(\Theta+\Psi)]=\widehat S,
$$

where

$$
\boxed{\widehat S=e^{-\tau}(\Phi'+\Psi')
+g(\Theta_0+\Psi-\widehat{\mathbf n}\cdot\mathbf v_e)}.
$$

Integrating along the ray and using $e^{-\tau}\to0$ at sufficiently early time yields the [Cosmic microwave background line-of-sight solution](../../../../../../cosmic-microwave-background-line-of-sight-solution.md)

$$
\boxed{(\Theta+\Psi)(\eta_0,\mathbf x_0,\widehat{\mathbf n})
=\int_0^{\eta_0}d\eta',
\widehat S(\eta',\mathbf x_0+(\eta_0-\eta')\widehat{\mathbf n},
\widehat{\mathbf n})}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
