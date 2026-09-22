<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The interaction contains no time derivatives, so $\pi=\dot\phi$. The [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md) gives

$$
\mathcal H=\pi\dot\phi-\mathcal L
=\frac12\pi^2+\frac12(\nabla\phi)^2+\frac12m^2\phi^2+\frac{\lambda}{4!}\phi^4.
$$

Thus

$$
\boxed{\mathcal H_0=\tfrac12\pi^2+\tfrac12(\nabla\phi)^2+\tfrac12m^2\phi^2,
\qquad\mathcal H_I=\frac{\lambda}{4!}\phi^4,\qquad H=H_0+H_I.}
$$

Here $H_0=\int\mathcal H_0$ is the free [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) of mass $m$, and $H_I=\int\mathcal H_I$ is the [interaction Hamiltonian](../../../../../interaction-hamiltonian.md).

In the [interaction picture](../../../../../interaction-picture.md), operators evolve with $H_0$ and the states with $H_I(t)=e^{iH_0t}H_Ie^{-iH_0t}$. With $U_I(t_0,t_0)=I$, the state evolution satisfies $i\partial_tU_I(t,t_0)=H_I(t)U_I(t,t_0)$. Integrating once and iterating gives the [Dyson series](../../../../../dyson-series.md)

$$
U_I(t,t_0)=I+\sum_{r\ge1}(-i)^r\int_{t_0<t_r<\cdots<t_1<t}dt_1\cdots dt_r\,
H_I(t_1)\cdots H_I(t_r).
$$

Equivalently it is the [time ordering](../../../../../time-ordering.md) of the exponential. Taking the infinite-time scattering limit, with adiabatic switching understood, gives the [scattering matrix](../../../../../s-matrix.md)

$$
\boxed{S=T\exp\!\left[-i\int d^4x\,\mathcal H_I(\phi_I(x))\right].}
$$

The field in the interaction is the free interaction-picture field, which is essential for applying the free-field contractions.

Use [relativistic normalization of a one-particle state](../../../../../relativistic-normalization-of-a-one-particle-state.md), $|\mathbf p\rangle=\sqrt{2E_{\mathbf p}}a^\dagger(\mathbf p)|0\rangle$, so each external scalar contraction contributes its plane-wave phase without an extra $1/\sqrt{2E}$ factor. For the connected on-shell two-to-two [scattering amplitude](../../../../../scattering-amplitude.md), the first [Dyson series](../../../../../dyson-series.md) term is $-i\lambda\int d^4x\,\phi_I(x)^4/4!$. The [Wick theorem](../../../../../wick-s-theorem.md) gives $4!$ ways to attach the two incoming and two outgoing external particles to the four fields, canceling the denominator. Consequently

$$
\langle p_3,p_4|(S-I)|p_1,p_2\rangle_{\mathrm{connected}}
=-i\lambda\int d^4x\,e^{i(p_3+p_4-p_1-p_2)\cdot x}+O(\lambda^2)
=i(2\pi)^4\delta^4(p_3+p_4-p_1-p_2)\mathcal A,
$$

where

$$
\boxed{\mathcal A=-\lambda+O(\lambda^2).}
$$

The delta function expresses [four-momentum conservation](../../../../../four-momentum-conservation.md). The connected scattering convention removes spectator, vacuum and external self-energy contributions; equivalently at this order one can normal-order the interaction and keep the physical external mass fixed. These contributions should not be mistaken for additional connected four-point diagrams.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
