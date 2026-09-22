<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The Maxwell quadratic action has a null longitudinal direction: its momentum-space kinetic operator annihilates $k_\mu$, reflecting [gauge invariance](../../../../../../gauge-invariance.md) under addition of a gradient to the potential. It cannot be inverted on all four vector components before [gauge fixing](../../../../../../gauge-fixing.md).

Add the [covariant gauge](../../../../../../covariant-gauge.md) density $\mathcal L_{\rm gf}=-(\partial_\mu A^\mu)^2/(2\xi)$. Away from the pole, introduce the [transverse and longitudinal momentum projectors](../../../../../../transverse-and-longitudinal-momentum-projectors.md)

$$
P^{\rm L}_{\mu\nu}=\frac{k_\mu k_\nu}{k^2},\qquad
P^{\rm T}_{\mu\nu}=\eta_{\mu\nu}-P^{\rm L}_{\mu\nu}.
$$

With one index raised they obey $P^{\rm T}+P^{\rm L}=I$, $(P^{\rm T})^2=P^{\rm T}$, $(P^{\rm L})^2=P^{\rm L}$ and $P^{\rm T}P^{\rm L}=0$. The gauge-fixed kinetic operator is $K=-k^2(P^{\rm T}+\xi^{-1}P^{\rm L})$. Its inverse times $i$ gives the [photon propagator](../../../../../../photon-propagator.md)

$$
\boxed{D^{(\xi)}_{\mu\nu}(k)=\frac{-i}{k^2+i0}\left(\eta_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2}\right)}.
$$

The pole factors are interpreted with the Feynman boundary prescription; the algebraic projector inversion is performed off the pole. The choice $\xi=1$ is [Feynman gauge](../../../../../../feynman-gauge.md).

Changing $\xi$ changes only a longitudinal term proportional to $k_\mu k_\nu$. Between conserved currents it vanishes because $k_\mu J^\mu=0$. In full QED amplitudes, the [Ward-Takahashi identity](../../../../../../ward-identity.md) supplies the corresponding cancellations when all diagrams at an order are combined. Thus physical on-shell scattering is gauge-parameter independent, whereas off-shell Green functions and the propagator itself can depend on the gauge choice. For the charged scalar, derivative vertices and contact terms must likewise be included for this cancellation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
