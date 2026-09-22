<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Insert the interaction-picture expansion into the Schrödinger equation. The [phases](../../../../phase-waves.md) multiplying the basis states already solve the unperturbed evolution, leaving

$$
i\hbar\dot c_r=\sum_s H'_{rs}\cos(\omega t)
\,e^{i(\omega_r-\omega_s)t}c_s.
$$

Hermiticity requires $H'_{21}=\hbar(\omega')^*$, not $\hbar\omega'$ unless the coupling is real. Since the diagonal [matrix elements](../../../../matrix-element.md) vanish and $\omega_0=\omega_2-\omega_1$, expanding the cosine gives

$$
\boxed{i\dot c_2=\frac{(\omega')^*}{2}c_1
[e^{i(\omega+\omega_0)t}+e^{-i(\omega-\omega_0)t}],}
$$



$$
\boxed{i\dot c_1=\frac{\omega'}{2}c_2
[e^{i(\omega-\omega_0)t}+e^{-i(\omega+\omega_0)t}].}
$$

The conjugate pair of couplings conserves $|c_1|^2+|c_2|^2$. Near resonance, the difference [frequency](../../../../frequency.md) is slow while the sum [frequency](../../../../frequency.md) is approximately $2\omega_0$. Rapid terms alternate sign before an appreciable slow transfer accumulates. The [rotating-wave approximation](../../../../rotating-wave-approximation.md) retains the slow terms when $|\omega'|,|\omega-\omega_0|\ll\omega+\omega_0$; resonance alone is insufficient for a strong drive. Counter-rotating corrections include small shifts of the resonance and need not remain negligible at arbitrary strength or arbitrarily long times.

For the [spin](../../../../spin.md) preparation, use $H=-\boldsymbol\mu\cdot\mathbf B=-\gamma\mathbf s\cdot\mathbf B$ and $\mathbf s=\hbar\boldsymbol\sigma/2$. Choose $B>0$ and $\gamma>0$ to fix helicity, with $|\uparrow\rangle=(1,0)^T$, $|\downarrow\rangle=(0,1)^T$ and $\omega_0=\gamma B$. The initial $|\uparrow\rangle$ is the lower state. For negative $\gamma$, reverse the RF rotation sense; [pulse areas](../../../../quantum-pulse-area.md) use $|\gamma|$, and signed [Larmor precession](../../../../larmor-precession.md) determines the corresponding [phase](../../../../phase-waves.md) adjustment.

A [circularly rotating magnetic drive](../../../../circularly-rotating-magnetic-drive.md) uses two transverse fields in quadrature during $0<t<\tau$:

$$
\mathbf B(t)=(B_1\cos(\omega_0t+\varphi),\,-B_1\sin(\omega_0t+\varphi),\,B),
\qquad \Omega=\gamma B_1>0.
$$

With $U_0(t)=e^{+i\omega_0t\sigma_z/2}$, their interaction [Hamiltonian](../../../../hamiltonian.md) is exactly constant,

$$
H_I=-\frac{\hbar\Omega}{2}(\cos\varphi\,\sigma_x-\sin\varphi\,\sigma_y).
$$

The minus sign in the second RF component selects co-rotation for the specified positive [gyromagnetic ratio](../../../../gyromagnetic-ratio.md). Exponentiating this Pauli matrix gives

$$
|\psi_I(t)\rangle=\cos\frac{\Omega t}{2}|\uparrow\rangle
+i e^{-i\varphi}\sin\frac{\Omega t}{2}|\downarrow\rangle.
$$

The [laboratory phase of a resonant spin pulse](../../../../laboratory-phase-of-a-resonant-spin-pulse.md) includes free precession. Returning to the laboratory frame and removing a common [phase](../../../../phase-waves.md),

$$
\boxed{|\psi(t)\rangle\sim
\cos\frac{\Omega t}{2}|\uparrow\rangle+
 i e^{-i(\varphi+\omega_0t)}\sin\frac{\Omega t}{2}|\downarrow\rangle.}
$$

Unlike a linearly polarized RF field, this exactly co-rotating field has no counter-rotating component. A single linearly polarized field $B_{x,\rm peak}\cos(\omega_0t+\varphi)$ gives the same slow rotation in the weak-drive [rotating-wave approximation](../../../../rotating-wave-approximation.md) with **$\Omega=|\gamma|B_{x,\rm peak}/2$**. For the circular field above, **$\Omega=|\gamma|B_1$**. Keeping these amplitude conventions distinct avoids a factor-of-two pulse-duration error.

<a id="4/image-resonant-rotations-in-rotating-axes-and-the-maximum-transfer-permitted-by-a-fixed-detuned-pulse"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2015/paper-1-spin-pulses.png)

**[Figure 5](#4/image-resonant-rotations-in-rotating-axes-and-the-maximum-transfer-permitted-by-a-fixed-detuned-pulse). Resonant rotations in rotating axes and the maximum transfer permitted by a fixed detuned pulse**.

For a single harmonic pulse detuned by $\Delta=\omega_0-\omega$, the effective rotating-frame field tilts out of the transverse plane. Its rotation rate becomes $\sqrt{\Omega^2+\Delta^2}$, and its maximum population transfer is $\Omega^2/(\Omega^2+\Delta^2)$. **Exact inversion to $-z$ is impossible with one fixed nonzero-detuning pulse**. Half transfer, needed for a transverse [eigenstate](../../../../eigenstate.md), gives the [equatorial reachability of a detuned spin pulse](../../../../equatorial-reachability-of-a-detuned-spin-pulse.md) criterion **$|\Delta|\leq\Omega$**. With that condition, changing the duration and RF [phase](../../../../phase-waves.md) can still prepare $+x$ or $+y$ at the chosen laboratory stopping time. The mere statement $\omega\approx\omega_0$ does not ensure this condition, because the drive can be much weaker than either [frequency](../../../../frequency.md). If $|\Delta|>\Omega$, neither transverse target is reached by that single pulse. These restrictions concern fixed-frequency, fixed-amplitude single-pulse control; retuning, chirping or phase-controlled composite pulses change the available controls and can remove the restriction. No dissipative [spin relaxation](../../../../spin-relaxation.md) is included in this coherent two-state model.

## ↑ Ancestors (13)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
