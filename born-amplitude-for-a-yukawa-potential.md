# Born amplitude for a Yukawa potential

↑ **Parent:** [Born approximation](born-approximation.md)

For $V(r)=Ae^{-\kappa r}/r$, with real $A$ and $\kappa>0$, the [first Born approximation](born-approximation.md) gives the [scattering amplitude](scattering-amplitude.md)

$$
f_B(q)=-\frac{m}{2\pi\hbar^2}\int_{\mathbb R^3}e^{-i\mathbf q\cdot\mathbf r}V(r)\,d^3r
=-\frac{2mA}{\hbar^2(q^2+\kappa^2)}.
$$

Indeed, orienting the polar axis along the [momentum transfer](momentum-transfer.md) gives the angular integral $4\pi\sin(qr)/(qr)$, and the remaining integral is $\int_0^\infty e^{-\kappa r}\sin(qr)\,dr=q/(q^2+\kappa^2)$. The [differential scattering cross-section](differential-scattering-cross-section.md) is $|f_B(q)|^2$.

The limit $\kappa\to0^+$ at fixed nonzero $q$ produces the [Rutherford differential cross-section](rutherford-differential-cross-section.md) for a [Coulomb potential](coulomb-potential-energy.md). The unscreened interaction has long range, so this limiting calculation by itself does not establish the validity of a naive [Born approximation](born-approximation.md) to the full [Rutherford scattering](rutherford-scattering.md) state. The exact [Rutherford scattering](rutherford-scattering.md) amplitude has an additional phase, while its modulus agrees with the [Rutherford differential cross-section](rutherford-differential-cross-section.md).

## ↑ Ancestors (5)

1. [Born approximation](born-approximation.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2017/4/solution.md)
