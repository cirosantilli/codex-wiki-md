<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep the mostly-plus [Minkowski metric](../../../../../../minkowski-metric.md) and the [Fourier transform](../../../../../../fourier-transform.md) $e^{ip\cdot x}$. Write $\not p=\gamma^ap_a$, with $\{\gamma^a,\gamma^b\}=2\eta^{ab}$. To fix the otherwise unspecified phase of $\gamma^5$ and the [Dirac adjoint](../../../../../../dirac-adjoint.md), take

$$
\gamma^a=-i\Gamma^a,\qquad
\bar\psi=-i\psi^\dagger\gamma^0,\qquad
\gamma^5=\gamma^0\gamma^1\gamma^2\gamma^3,
$$

where $\Gamma^a$ are ordinary mostly-minus [gamma matrices](../../../../../../gamma-matrices.md). Then $(\gamma^5)^2=-1$, $\{\gamma^5,\gamma^a\}=0$, and the fermionic time-derivative term is $i\psi^\dagger\partial_t\psi$. In these conventions the interaction with real $g$ is Hermitian: in mostly-minus notation it is $ig\bar\psi_{\rm std}\Gamma^5\psi\phi$. If one instead calls $i\gamma^5$ the square-one [chirality](../../../../../../chirality-physics.md) matrix, its coefficient must be $-ig$ to represent the same interaction. These phase choices leave physical [relativistic scattering cross-sections](../../../../../../relativistic-scattering-cross-section.md) unchanged.

Expanding $e^{iS_{\rm int}}$ yields the following [Feynman rules](../../../../../../feynman-rule.md) with relativistically normalized external states:

- A [real scalar field](../../../../../../real-scalar-field.md) line carrying [four-momentum](../../../../../../four-momentum.md) $r$ contributes $-i/(r^2+m^2-i0)$.
- An oriented [Dirac field](../../../../../../dirac-field.md) line contributes the [Dirac propagator](../../../../../../dirac-propagator.md)$$
  S_F(r)=\frac{i(M-i\not r)}{r^2+M^2-i0}.
  $$

  This follows from $(i\not r+M)(M-i\not r)=(r^2+M^2)I$.
- Each [pseudoscalar Yukawa interaction](../../../../../../pseudoscalar-yukawa-interaction.md) vertex has one scalar leg, one incoming fermion arrow and one outgoing fermion arrow, and contributes $ig\gamma^5$. It also contributes $(2\pi)^4\delta^{(4)}(\sum r)$ with all vertex momenta counted incoming.
- External incoming particles contribute $u(p,s)$ and outgoing particles $\bar u(p,s)$. External incoming [antiparticles](../../../../../../antiparticle.md) contribute $\bar v(p,s)$ and outgoing [antiparticles](../../../../../../antiparticle.md) $v(p,s)$, with the corresponding fermion arrows. External scalar factors are one. Choose $u^\dagger u=v^\dagger v=2E$, $(i\not p+M)u=0$, and $(-i\not p+M)v=0$; all external momenta are on the appropriate [mass shell](../../../../../../mass-shell.md).
- Integrate each independent loop [four-momentum](../../../../../../four-momentum.md) with $d^4r/(2\pi)^4$. Keep matrix factors in their order along a fermion line, take a trace around a closed fermion loop, and include a minus sign for each closed fermion loop. Permuting external identical [fermions](../../../../../../fermion.md) contributes the corresponding [fermionic sign](../../../../../../fermionic-sign.md); the [Wick theorem](../../../../../../wick-s-theorem.md) determines the [Feynman-diagram symmetry factors](../../../../../../feynman-diagram-symmetry-factor.md).

Strip the overall [four-momentum conservation](../../../../../../four-momentum-conservation.md) delta function when defining the [scattering amplitude](../../../../../../scattering-amplitude.md). There are no further bare interaction vertices, no [gauge fixing](../../../../../../gauge-fixing.md) and no [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md) in this theory. Renormalized higher-order calculations add the required [counterterms](../../../../../../counterterm.md); these are additional to the rules of the displayed classical [Lagrangian density](../../../../../../lagrangian-density.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
