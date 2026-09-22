<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Let $R(\theta)$ be the real rotation matrix with columns along the plate's fast and slow axes. Expressing the input in those axes, applying the principal retardance, then rotating back gives the rotated [half-wave plate](../../../../../half-wave-plate.md) matrix

$$
H(\theta)=R(\theta)\begin{pmatrix}1&0\\0&-1\end{pmatrix}R(-\theta)
=\begin{pmatrix}\cos2\theta&\sin2\theta\\\sin2\theta&-\cos2\theta\end{pmatrix}.
$$

Each fixed [quarter-wave plate](../../../../../quarter-wave-plate.md) has $Q=\operatorname{diag}(1,i)$ in the supplied convention. Propagation through the three plates therefore gives

$$
\boxed{J(\theta)=QH(\theta)Q
=\begin{pmatrix}\cos2\theta&i\sin2\theta\\i\sin2\theta&\cos2\theta\end{pmatrix}
=e^{i2\theta\sigma_x}.}
$$

The order matters: this is a product of three propagating plates, not a similarity transformation $QHQ^{-1}$. For input Jones vector $\mathbf e_+=(1,1)^T/\sqrt2$, the Pauli matrix has eigenvalue $+1$, so $J\mathbf e_+=e^{i2\theta}\mathbf e_+$. The final [polarization](../../../../../polarization-waves.md) remains at 45 degrees, but its phase depends on the rotating angle.

Take the physical field as the real part of $\mathbf E e^{-i\omega t}$ and let $\theta=\Omega t$. Then

$$
\mathbf E_{\rm out}(t)\propto\mathbf e_+ e^{i2\Omega t}e^{-i\omega t}
=\mathbf e_+e^{-i(\omega-2\Omega)t}.
$$

Thus the [rotating half-wave plate frequency shift](../../../../../rotating-half-wave-plate-frequency-shift.md) has

$$
\boxed{\omega_{\rm out}-\omega=-2\Omega,\qquad |\Delta\omega|=2|\Omega|.}
$$

The magnitude is the stated $2\Omega$ shift. Its sign follows the explicit time and rotation conventions above; reversing the physical rotation or using the orthogonal linear input reverses the shift. A time-phasor convention must be changed consistently with the plate matrices, rather than used alone to change a physical redshift into a blueshift.

The physical origin is a [rotational Doppler effect](../../../../../rotational-doppler-effect.md) and angular-momentum exchange. In the stated convention, the first fixed quarter-wave plate changes the 45-degree input into circular [polarization](../../../../../polarization-waves.md) of spin $+\hbar$ per [photon](../../../../../photon.md). The rotating half-wave plate flips it to spin $-\hbar$, transferring $2\hbar$ to the rotating plate. Maintaining its rotation takes mechanical [energy](../../../../../energy-split.md) $2\hbar\Omega$ from each [photon](../../../../../photon.md), agreeing with the redshift. The final fixed plate restores linear [polarization](../../../../../polarization-waves.md); fixed plates can exchange [angular momentum](../../../../../angular-momentum.md) with their supports without the rotating element's corresponding mechanical work. The instantaneous Jones treatment assumes slow rotation compared with optical and transit-time scales and ideal retardances over the small shifted bandwidth.

## ↑ Ancestors (13)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
