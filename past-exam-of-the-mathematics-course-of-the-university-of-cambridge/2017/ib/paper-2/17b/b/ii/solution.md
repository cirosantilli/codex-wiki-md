<h1 id="17b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [sudden approximation](../../../../../../../sudden-approximation.md) keeps the wavefunction unchanged at the instant of switching: a finite step of potential creates no delta-function impulse in the [Schrödinger equation](../../../../../../../schrodinger-equation.md). Just before switching the old [ground state](../../../../../../../ground-state.md) differs from the printed real wavefunction only by an overall phase, which does not affect probabilities.

Let $\widetilde\psi_0(x)=(\pi\hbar)^{-1/4}e^{-(x-d)^2/(2\hbar)}$, $d=qE$, be the new ground state. Its overlap with the initial state is, up to that phase,

$$
A_0=(\pi\hbar)^{-1/2}\int_{-\infty}^\infty
e^{-[x^2+(x-d)^2]/(2\hbar)}\,dx.
$$

Since $x^2+(x-d)^2=2(x-d/2)^2+d^2/2$, the [Gaussian integral](../../../../../../../gaussian-integral.md) gives $A_0=e^{-d^2/(4\hbar)}$. The [Born rule](../../../../../../../born-rule.md) and the [ground-state overlap after sudden oscillator displacement](../../../../../../../ground-state-overlap-after-sudden-oscillator-displacement.md) thus give

$$
\boxed{P_0=|A_0|^2=e^{-q^2E^2/(2\hbar)}.}
$$

This is an overlap probability, not a claim that the original wavefunction instantaneously relaxes to the new ground state. It becomes one when $qE=0$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [17B](../../../17b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
