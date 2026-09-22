# Local subtraction with a sharp momentum cutoff

↑ **Parent:** [Renormalization of spontaneously broken gauge theories](renormalization-of-spontaneously-broken-gauge-theories.md)

The following scalar toy isolates one step in [renormalization](renormalization.md): removing a local divergence while retaining a finite dependence on a physical [mass](mass.md). For $M,\mu>0$ and a sharp [cutoff regularization](cutoff-regularization.md) in [Euclidean space](euclidean-norm.md) with momentum bound $\Lambda$, define the dimensionless [Feynman integral](feynman-integral.md)

$$
I_\Lambda(M)=\int_{|k_E|<\Lambda}\frac{d^4k_E}{(2\pi)^4}\frac1{(k_E^2+M^2)^2}.
$$

This is a zero-external-[momentum](momentum-split.md) [scalar bubble integral](scalar-bubble-integral.md) stripped of coupling and combinatorial factors. Using the three-sphere area $2\pi^2$ and $t=k_E^2$ reduces the [integral](integral-split.md) to

$$
I_\Lambda(M)=\frac1{16\pi^2}\int_0^{\Lambda^2}\frac{t\,dt}{(t+M^2)^2}
=\frac1{16\pi^2}\left[\log\left(1+\frac{\Lambda^2}{M^2}\right)-\frac{\Lambda^2}{\Lambda^2+M^2}\right].
$$

The [antiderivative](antiderivative.md) follows by writing $t=(t+M^2)-M^2$. At large $\Lambda$ the divergent part is $\log\Lambda^2/(16\pi^2)$, with the logarithm's dimensionful argument understood only within the displayed ratios. It has no external-[momentum](momentum-split.md) dependence. In a four-[scalar](scalar.md)-field vertex this structure can therefore be removed by a [local operator](lawvere-tierney-topology.md) proportional to $\phi^4$, rather than a momentum-dependent nonlocal interaction.

Choose the fixed reference [mass](mass.md) $\mu$ and subtract $I_\Lambda(\mu)$. If the loop contribution to a chosen four-point vertex coefficient is $c\lambda^2 I_\Lambda(M)$, choose the additive [counterterm](counterterm.md) in that same coefficient as $\delta\lambda_\Lambda=-c\lambda^2I_\Lambda(\mu)$, where $c$ includes its stated diagram factors. This defines a finite subtraction prescription:

$$
I_R(M;\mu)=\lim_{\Lambda\to\infty}\left[I_\Lambda(M)-I_\Lambda(\mu)\right]
=\frac1{16\pi^2}\log\frac{\mu^2}{M^2}.
$$

The [renormalization condition](renormalization-condition.md) for this toy loop contribution is $I_R(\mu;\mu)=0$. The reference [mass](mass.md) stays fixed when $M$ is varied; finite dependence on $M$ survives. A different finite subtraction changes the [renormalization scheme](renormalization-scheme.md), and the defined [renormalized coupling](renormalized-coupling.md) must change consistently.

<a id="image-a-local-counterterm-cancels-a-logarithmic-cutoff-regularization-divergence"></a>
![](cutoff-subtraction-local-counterterm.png)

**[Figure 2](#image-a-local-counterterm-cancels-a-logarithmic-cutoff-regularization-divergence). A local counterterm cancels a logarithmic cutoff regularization divergence**. Original scalar toy with $M=2\mu$: the two separately growing terms leave $16\pi^2I_R=-\log4$. The subtraction is constant in external momentum; it does not remove all mass dependence.

For $M=2\mu$, the limiting result is $16\pi^2I_R=-\log4\approx-1.38629436$. At $\Lambda=10\mu$, the exact regulated difference is about $-1.32846343$; at $\Lambda=100\mu$, it is about $-1.38569459$. Expanding the exact expression gives the leading residual $2(M^2-\mu^2)/\Lambda^2$ in $16\pi^2[I_\Lambda(M)-I_\Lambda(\mu)]$. This explicitly separates finite-cutoff error from the chosen finite [renormalization condition](renormalization-condition.md).

A sharp [cutoff regularization](cutoff-regularization.md) is convenient for this scalar demonstration, but shifts of a divergent [loop momentum](loop-momentum.md) can change its integration domain. A [gauge theory](gauge-theory.md) calculation cannot assume that it preserves the [Ward identities](ward-identity.md). The toy contains no interacting [gauge bosons](gauge-boson.md), [ghost loops](ghost-loop.md) or overlapping [ultraviolet subdivergences](ultraviolet-subdivergence.md), so its successful subtraction does not prove [Non-Abelian gauge theory](yang-mills-theory.md) [renormalizability](renormalizable-quantum-field-theory.md).

## ↑ Ancestors (7)

1. [Renormalization of spontaneously broken gauge theories](renormalization-of-spontaneously-broken-gauge-theories.md)
2. [Renormalization](renormalization.md)
3. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
4. [Quantum field theory](quantum-field-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
