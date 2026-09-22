<h1 id="section-b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\omega_z=\gamma B_z$ and use the ordered [spin](../../../../../spin.md) basis $(|\uparrow\rangle,|\downarrow\rangle)$. The free [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is $H_0=-\hbar\omega_z\sigma_z/2$, so

$$
V_I(t)=-\frac{\gamma\hbar B_x}{2}\cos(\omega t)
\begin{pmatrix}0&e^{-i\omega_zt}\\e^{i\omega_zt}&0\end{pmatrix}.
$$

Resolving the cosine into its two complex exponentials gives the exact upper off-diagonal factor

$$
\cos(\omega t)e^{-i\omega_zt}
=\frac12\left[e^{i(\omega-\omega_z)t}+e^{-i(\omega+\omega_z)t}\right],
$$

with the complex conjugate in the lower entry. Choose the field orientation with $\omega_z>0$, as implicit in the printed near-resonance condition, and put $\delta=\omega-\omega_z$. The [rotating-wave approximation](../../../../../rotating-wave-approximation.md) discards the terms at $\omega+\omega_z$, retaining the slow terms at $\delta$. The resulting [interaction picture](../../../../../interaction-picture.md) equations are

$$
\boxed{\frac d{dt}\begin{pmatrix}c_1\\c_2\end{pmatrix}
=\frac{i\gamma B_x}{4}
\begin{pmatrix}0&e^{i\delta t}\\e^{-i\delta t}&0\end{pmatrix}
\begin{pmatrix}c_1\\c_2\end{pmatrix}.}
$$

The factor $1/4$ contains $1/2$ from $S_x=\hbar\sigma_x/2$ and $1/2$ from the cosine decomposition. This is a [Driven two-level Rabi model](../../../../../driven-two-level-rabi-model.md), with signed on-resonance coupling $\Omega=\gamma B_x/2$ and generalized [Rabi angular frequency](../../../../../rabi-angular-frequency.md) $\omega_R=\sqrt{\delta^2+\Omega^2}$. Here the [Rabi detuning](../../../../../rabi-detuning.md) uses the paper's convention, drive minus free frequency.

Small detuning alone is insufficient to derive the printed equations. One also requires $|\gamma B_x|,|\delta|\ll\omega+\omega_z$, and an evolution time over which neglected terms stay small. At resonance this is the weak transverse-field regime $|B_x|\ll|B_z|$. The supplied solution is thus an approximate solution for the linearly oscillating field, not an exact one at arbitrary drive strength. If $\gamma B_z<0$, the other exponential is resonant and the physical positive resonance frequency is $|\gamma B_z|$.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
