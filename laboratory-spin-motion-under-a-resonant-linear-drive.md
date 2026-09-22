# Laboratory spin motion under a resonant linear drive

↑ **Parent:** [Rotating-wave approximation](rotating-wave-approximation.md)

For $H=-\gamma B_zS_z-\gamma B_xS_x\cos(\omega t)$, choose $\omega_z=\gamma B_z>0$ and nominal resonance $\omega=\omega_z$. Starting from up spin, the [rotating-wave approximation](rotating-wave-approximation.md) gives the normalized [Bloch vector](bloch-vector.md) in the title, with signed $\Omega=\gamma B_x/2$. It follows by transforming the spinor $(\cos(\Omega t/2),i\sin(\Omega t/2))^T$ from the [interaction picture](interaction-picture.md) back to the [Schrödinger picture](schrodinger-picture.md). Thus weak transverse driving combines slow meridional [Rabi oscillations](rabi-cycle.md) with fast [Larmor precession](larmor-precession.md).

This result requires $|B_x|\ll|B_z|$ and cannot be extrapolated as a controlled strong-drive formula. The exact equation is $\dot{\mathbf s}=\gamma\mathbf s\times(B_x\cos\omega t,0,B_z)$. For $|\gamma B_z|t\ll1$, neglecting the bias gives the controlled leading solution

$$
\mathbf s\simeq(0,\sin\Theta,\cos\Theta),\qquad
\Theta=\frac{\gamma B_x}{\omega}\sin\omega t.
$$

The fixed-axis driving generators commute at all times, making this solution exact when the bias is zero at any prescribed drive frequency. At nominal resonance in a strong-drive experiment, the initial rotation scale is $\Theta\simeq\gamma B_xt$, twice the incorrectly extrapolated rotating-wave rate. Bias effects must be retained on longer times.

## ↑ Ancestors (5)

1. [Rotating-wave approximation](rotating-wave-approximation.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
