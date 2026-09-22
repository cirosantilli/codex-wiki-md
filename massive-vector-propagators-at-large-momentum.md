# Massive-vector propagators at large momentum

↑ **Parent:** [Renormalization of spontaneously broken gauge theories](renormalization-of-spontaneously-broken-gauge-theories.md)

Consider one massive [gauge field](gauge-field.md) with $m>0$ after [Higgs mechanism](higgs-mechanism.md). For this comparison perform a [Wick rotation](wick-rotation.md) and take a real nonzero [momentum](momentum-split.md) in [Euclidean space](euclidean-norm.md) $k_E$. The transverse and longitudinal [orthogonal projectors](orthogonal-projection.md) are

$$
P^L_{\mu\nu}=\frac{k_{E\mu}k_{E\nu}}{k_E^2},\qquad P^T_{\mu\nu}=\delta_{\mu\nu}-P^L_{\mu\nu}.
$$

Here “longitudinal” means parallel to the off-shell four-[momentum](momentum-split.md), not the physical longitudinal polarization of an on-shell massive [gauge boson](gauge-boson.md). The [R-xi gauge](r-xi-gauge.md) quadratic vector operator and its inverse are

$$
K_\xi=(k_E^2+m^2)P^T+(k_E^2/\xi+m^2)P^L,\qquad
D_\xi=\frac{P^T}{k_E^2+m^2}+\frac{\xi P^L}{k_E^2+\xi m^2},\quad \xi>0.
$$

Multiplication verifies $K_\xi D_\xi=P^T+P^L=I$, since $P^TP^L=0$ and $(P^{T,L})^2=P^{T,L}$. The [unitary gauge](unitary-gauge.md) vector operator lacks the [gauge fixing](gauge-fixing.md) derivative term in the longitudinal sector, giving

$$
K_U=(k_E^2+m^2)P^T+m^2P^L,\qquad
D_U=\frac{P^T}{k_E^2+m^2}+\frac{P^L}{m^2}
=\frac{\delta_{\mu\nu}+k_{E\mu}k_{E\nu}/m^2}{k_E^2+m^2}.
$$

Thus every eigenvalue of $D_\xi$ falls as $1/k_E^2$ at fixed finite positive $\xi$, whereas $D_U$ has the constant longitudinal eigenvalue $1/m^2$. [Unitary gauge](unitary-gauge.md) consequently obscures ordinary [power counting](power-counting-in-quantum-field-theory.md); this is not a failure of the physical theory.

<a id="image-large-momentum-eigenvalues-of-massive-vector-propagators-in-unitary-gauge-and-r-xi-gauge"></a>
![](massive-vector-propagator-scaling.png)

**[Figure 1](#image-large-momentum-eigenvalues-of-massive-vector-propagators-in-unitary-gauge-and-r-xi-gauge). Large-momentum eigenvalues of massive-vector propagators in unitary gauge and R-xi gauge**. Original curves from the displayed quadratic operators. The common transverse eigenvalue equals the blue curve. The plotted longitudinal sector is off shell and is not a physical polarization probability.

For a worked comparison choose $|k_E|=10m$. The dimensionless longitudinal eigenvalue $m^2D_L$ is $1$ in [unitary gauge](unitary-gauge.md), $1/101$ at $\xi=1$, and $1/11$ at $\xi=10$. Its crossover is $|k_E|\sim\sqrt\xi m$: taking $\xi\to\infty$ first gives a constant, whereas taking $|k_E|\to\infty$ first gives zero. The two limits do not commute. Contracting the [propagator](propagator.md) between conserved external [conserved currents](conserved-current.md) projects away $P^L$, but one cannot impose that simplification separately on every internal line of an interacting [Non-Abelian gauge theory](yang-mills-theory.md).

## ↑ Ancestors (7)

1. [Renormalization of spontaneously broken gauge theories](renormalization-of-spontaneously-broken-gauge-theories.md)
2. [Renormalization](renormalization.md)
3. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
4. [Quantum field theory](quantum-field-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
