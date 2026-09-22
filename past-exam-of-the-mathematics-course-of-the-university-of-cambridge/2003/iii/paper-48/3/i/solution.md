<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $p$ be the total external Euclidean [momentum](../../../../../../momentum.md) crossing one four-point channel. The two internal [scalar propagators](../../../../../../scalar-propagator.md) produce the [scalar bubble integral](../../../../../../scalar-bubble-integral.md)

$$
B_d(p)=\int\frac{d^dk}{(2\pi)^d}\frac1{(k^2+m^2)((k+p)^2+m^2)}.
$$

Using the [Feynman parameter](../../../../../../feynman-parameter.md) identity $1/(ab)=\int_0^1 dx\,[xa+(1-x)b]^{-2}$ and shifting the loop [momentum](../../../../../../momentum.md) yields

$$
\boxed{B_d(p)=\int_0^1dx\,I_d\big(m^2+x(1-x)p^2\big).}
$$

In [phi-fourth theory](../../../../../../quartic-interaction.md) the [bubble diagram](../../../../../../bubble-diagram.md) has two quartic vertices and a [symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md) $1/2$ from exchanging its two identical internal lines. There are three partitions of four labelled external legs into two pairs, the $s,t,u$ channels. The connected amputated loop diagram has positive coefficient $\lambda^2 B/2$, whereas the Euclidean [one-particle-irreducible vertex](../../../../../../one-particle-irreducible-vertex.md) in the effective [action](../../../../../../action.md) has the opposite sign. Thus

$$
\Gamma_E^{(4)}(p_1,p_2,p_3,p_4)=\mu^\epsilon(\lambda+\delta\lambda)-\frac{\mu^{2\epsilon}\lambda^2}{2}\big[B_d(p_1+p_2)+B_d(p_1+p_3)+B_d(p_1+p_4)\big]+O(\lambda^3).
$$

One can check this sign without external-line conventions by expanding the one-loop [quantum effective action](../../../../../../effective-action.md) $\tfrac12\operatorname{Tr}\log(K+\mu^\epsilon\lambda\phi^2/2)$. Its second logarithmic term is $-\mu^{2\epsilon}\lambda^2\operatorname{Tr}(K^{-1}\phi^2K^{-1}\phi^2)/16$; four field derivatives give precisely the three negative bubble terms above.

The four-dimensional pole of $I_d$ is independent of its mass argument, so each channel contributes $2/[(4\pi)^2\epsilon]$. The divergence of the proper four-point vertex is $-3\lambda^2/[(4\pi)^2\epsilon]$. The [minimal subtraction scheme](../../../../../../minimal-subtraction-scheme.md) therefore requires

$$
\boxed{\delta\lambda=\frac{3\lambda^2}{(4\pi)^2\epsilon},\qquad \mathcal L_{E,\mathrm{ct}}^{(4)}=\frac{\mu^\epsilon\delta\lambda}{4!}\phi^4.}
$$

For a Minkowski interaction $-\mu^\epsilon\lambda\phi^4/4!$, the corresponding local interaction [counterterm](../../../../../../counterterm.md) is $-\mu^\epsilon\delta\lambda\phi^4/4!$. No momentum-dependent four-point [counterterm](../../../../../../counterterm.md) is needed for these logarithmic poles. This calculation concerns the requested four-point bubble contributions; a massive two-point tadpole and vacuum diagrams require their own mass and vacuum-energy subtractions if those functions are also renormalized.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
