<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For an unpolarized initial [fermion](../../../../../../fermion.md), average over its two [spin](../../../../../../spin.md) states and sum over the unobserved final [spin](../../../../../../spin.md):

$$
\overline{|T|^2}=\frac12\sum_{s,s'}|T_{s's}|^2.
$$

The initial scalar has only one [spin](../../../../../../spin.md) state. One can evaluate this sum directly from normalized [Dirac spinors](../../../../../../dirac-spinor.md), or use consistent [fermion spin sums](../../../../../../fermion-spin-sum.md) to express it as a trace. It is the squared sum of both tree [scattering amplitudes](../../../../../../scattering-amplitude.md), not the sum of their separate squares.

The [relativistic scattering cross-section](../../../../../../relativistic-scattering-cross-section.md) is obtained by integrating the [Lorentz-invariant phase-space measure](../../../../../../lorentz-invariant-phase-space-measure.md) and dividing by the [invariant flux factor](../../../../../../invariant-flux-factor.md):

$$
\boxed{\sigma=\frac{1}{4\sqrt{(p\cdot k)^2-M^2m^2}}
\int\frac{d^3\boldsymbol q}{(2\pi)^3 2E_q}
\frac{d^3\boldsymbol l}{(2\pi)^3 2E_l}
(2\pi)^4\delta^{(4)}(p+k-q-l)\,\overline{|T|^2}}.
$$

There is no identical-final-particle factor, because the outgoing scalar and [fermion](../../../../../../fermion.md) are distinct. All [energies](../../../../../../energy.md) are positive, with $E_q^2=|\boldsymbol q|^2+M^2$ and $E_l^2=|\boldsymbol l|^2+m^2$.

Equivalently, in the [centre-of-momentum frame](../../../../../../center-of-momentum-frame.md) set $s=-(p+k)^2$. Integrating the energy delta function in the [relativistic two-body phase space](../../../../../../relativistic-two-body-phase-space.md) gives

$$
\frac{d\sigma}{d\Omega}=\frac{1}{64\pi^2s}\frac{k_f}{k_i}\overline{|T|^2}.
$$

For this elastic process $k_f=k_i$, so integrate $\overline{|T|^2}/(64\pi^2s)$ over the full solid angle. This supplies the requested prescription without evaluating the angular integral.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
