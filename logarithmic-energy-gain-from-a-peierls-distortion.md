# Logarithmic energy gain from a Peierls distortion

↑ **Parent:** [Dimerized tight-binding chain](dimerized-tight-binding-chain.md)

Fill the lower [energy band](energy-band.md) of the [dimerized tight-binding chain](dimerized-tight-binding-chain.md) with both [spin](spin.md) states. Take zero on-site [energy](energy-split.md) and measure [ground-state energy](ground-state-energy.md) per doubled [primitive unit cell](primitive-unit-cell.md). [State counting in a Bloch band](state-counting-in-a-bloch-band.md) and $q=ka$ give

$$
\mathcal E(\delta)=-\frac8\pi\int_0^{\pi/2}\sqrt{t^2\cos^2q+\delta^2\sin^2q}\,dq,\qquad \mathcal E(0)=-\frac{8t}\pi.
$$

Equivalently, for $|\delta|\leq t$, $\mathcal E(\delta)=-(8t/\pi)E(\sqrt{1-\delta^2/t^2})$, where $E(k)$ is the [complete elliptic integral of the second kind](complete-elliptic-integral-of-the-second-kind.md) in the modulus convention.

For fixed $t>0$ and $|\delta|/t\to0$, the change is

$$
\boxed{\mathcal E(\delta)-\mathcal E(0)=-\frac{4\delta^2}{\pi t}\log\frac{t}{|\delta|}+O(\delta^2/t).}
$$

The [logarithm](logarithm.md) comes from states near the edge of the [Brillouin zone](brillouin-zone.md). Put $u=\pi/2-q$. To leading order the square root there is $\sqrt{t^2u^2+\delta^2}$. For a fixed small cutoff $\eta>0$, direct integration gives

$$
\int_0^\eta\left[\sqrt{t^2u^2+\delta^2}-tu\right]du=\frac{\delta^2}{2t}\log\frac{t}{|\delta|}+O(\delta^2/t).
$$

The rest of the band, and the higher-order corrections near its edge, contribute only $O(\delta^2/t)$; multiplying by $-8/\pi$ gives the displayed [asymptotic expansion](asymptotic-expansion-split.md). Here the remainder uses [Big O notation](big-o-notation.md). The negative logarithmic term exceeds any fixed quadratic elastic cost $K\delta^2$, $K>0$, for sufficiently small nonzero $\delta$. This explains the zero-[temperature](temperature-split.md) instability to a [Peierls distortion](peierls-distortion.md) in the ideal chain model.

## ↑ Ancestors (12)

1. [Dimerized tight-binding chain](dimerized-tight-binding-chain.md)
2. [Peierls distortion](peierls-distortion.md)
3. [Peierls transition](peierls-transition.md)
4. [Electron-phonon interaction](electron-phonon-interaction.md)
5. [Phonon](phonon.md)
6. [Bose-Einstein distribution](bose-einstein-distribution.md)
7. [Bose-Einstein statistics](bose-einstein-statistics.md)
8. [Quantum ideal-gas statistics](quantum-ideal-gas-statistics-split.md)
9. [Statistical physics](statistical-physics-split.md)
10. [Branches of physics](branches-of-physics.md)
11. [Physics](physics-split.md)
12. [Codex Wiki](split.md)
