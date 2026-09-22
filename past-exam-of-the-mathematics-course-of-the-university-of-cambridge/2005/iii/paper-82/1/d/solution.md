<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At a sharp interface, continuity of [velocity](../../../../../../velocity.md) and [traction](../../../../../../traction.md) gives, for unit incident [velocity](../../../../../../velocity.md) from the left,

$$
1+r_v=t_v,\qquad Z_a(1-r_v)=Z_bt_v.
$$

Thus $r_v=(Z_a-Z_b)/(Z_a+Z_b)$ and $t_v=2Z_a/(Z_a+Z_b)$. Normalizing the transmitted [velocity](../../../../../../velocity.md) by its [elastic-wave energy flux](../../../../../../elastic-wave-energy-flux.md) gives $T_{ba}=\sqrt{Z_b/Z_a}\,t_v$, exactly the result above. Right incidence gives the reversed reflection sign and the same flux-normalized transmission. A [stress](../../../../../../stress.md) [reflection coefficient](../../../../../../reflection-coefficient.md) has the opposite sign to the [velocity](../../../../../../velocity.md) [reflection coefficient](../../../../../../reflection-coefficient.md); the convention matters.

Put $r=R_{aa}$ and $t=T_{ab}$. The incoming-to-outgoing [matrix](../../../../../../matrix.md) is $S_0=\begin{pmatrix}r&t\\t&-r\end{pmatrix}$, with $r^2+t^2=1$. Therefore **$S_0^\dagger S_0=I$**, proving equality of incoming and outgoing time-averaged flux for arbitrary coherent incident [wave amplitudes](../../../../../../wave-amplitude.md), not just incidence from one side.

For all real [frequencies](../../../../../../frequency.md) the harmonic equations instead give

$$
\frac{d|\phi_+|^2}{dx}=2g\operatorname{Re}(\phi_+^*\phi_-),\qquad \frac{d|\phi_-|^2}{dx}=2g\operatorname{Re}(\phi_-^*\phi_+).
$$

Their right sides are equal; the diagonal terms $\pm i\omega/\beta$ have zero real contribution. Consequently

$$
\boxed{\frac{d}{dx}\left(|\phi_+|^2-|\phi_-|^2\right)=0.}
$$

The mean flux for real-part phasors is $(|\phi_+|^2-|\phi_-|^2)/2$. Evaluating it at the two endpoints proves exactly that total outgoing flux equals total incoming flux at every real [frequency](../../../../../../frequency.md). This relies on real lossless moduli and [mass density](../../../../../../density.md); absorption would change the identity.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
