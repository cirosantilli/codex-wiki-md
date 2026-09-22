<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take integer $n\geq3$ and positive integer $d$, so the interaction is genuinely non-Gaussian. For a connected two-point [Feynman diagram](../../../../../../feynman-diagram.md) with $V$ [interaction vertices](../../../../../../interaction-vertex.md) and $I$ internal lines, counting half-edges and using the [loop order](../../../../../../loop-order.md) gives

$$
nV=2I+2,\qquad L=I-V+1.
$$

At one loop $I=V$, hence $(n-2)V=2$. There are only two possibilities: a two-[interaction vertex](../../../../../../interaction-vertex.md) [bubble diagram](../../../../../../bubble-diagram.md) for $n=3$, or a one-[interaction vertex](../../../../../../interaction-vertex.md) [tadpole diagram](../../../../../../tadpole-diagram.md) for $n=4$. The latter is independent of external momentum and changes the mass, not the [kinetic term](../../../../../../kinetic-term.md).

For [cubic scalar field theory](../../../../../../phi-cubed-theory.md), introduce a positive auxiliary mass $\mu$ if needed to separate [infrared divergences](../../../../../../infrared-divergence.md) from [ultraviolet divergences](../../../../../../ultraviolet-divergence.md). The one-loop [self-energy](../../../../../../self-energy.md) in the [quantum effective action](../../../../../../effective-action.md) is $-\lambda^2 B_d(p)/2$, with

$$
B_d(p)=\int_0^1du\int\frac{d^dq}{(2\pi)^d}\frac{1}{[q^2+\mu^2+u(1-u)p^2]^2}.
$$

This [Feynman parameter](../../../../../../feynman-parameter.md) representation follows by shifting the [loop momentum](../../../../../../loop-momentum.md); it is directly valid for a translation-invariant regulator, or for the convergent subtracted integral. Differentiating at $p^2=0$ gives

$$
\left.\frac{d B_d}{dp^2}\right|_0=-\frac13\int\frac{d^dq}{(2\pi)^d}\frac{1}{(q^2+\mu^2)^3}.
$$

Thus the coefficient of the [kinetic term](../../../../../../kinetic-term.md) changes by $\lambda^2\int d^dq/[(2\pi)^d(q^2+\mu^2)^3]/6$.

**Only the cubic interaction has a momentum-dependent one-loop two-point correction.**

$$
\boxed{n=3\quad\text{for every }d\geq1.}
$$

There is a terminology qualification: if “[wave-function renormalization](../../../../../../wave-function-renormalization.md)” means a required ultraviolet [counterterm](../../../../../../counterterm.md), rather than a finite correction to the field normalization, the large-$q$ radial integral behaves as $\int dq\,q^{d-7}$, and the answer is

$$
\boxed{n=3,\ d\geq6\quad\text{for an ultraviolet-divergent kinetic correction}.}
$$

It is logarithmically divergent at $d=6$ and power divergent above $6$ with a momentum cutoff. Among interactions with a [relevant coupling](../../../../../../relevant-coupling.md) or [marginal coupling](../../../../../../marginal-coupling.md), the divergent case is uniquely $(n,d)=(3,6)$. The massless low-dimensional amplitude needs an [infrared divergence](../../../../../../infrared-divergence.md) prescription; one cannot take a local expansion at zero momentum without one. The $n=1,2$ cases, if admitted, are a source and a Gaussian mass term and have no interaction-induced [wave-function renormalization](../../../../../../wave-function-renormalization.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
