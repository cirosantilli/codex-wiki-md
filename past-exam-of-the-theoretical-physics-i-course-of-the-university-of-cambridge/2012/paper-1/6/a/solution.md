<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the forward spatial transform $\hat f(k)=\int e^{-ikx}f(x)\,dx$ and inverse $f(x)=\int e^{ikx}\hat f(k)\,dk/(2\pi)$. The retarded transformed [Green function](../../../../../green-s-function-split.md) obeys

$$
\left[\frac1{c^2}\frac{d^2}{d\tau^2}+2\alpha\frac d{d\tau}+k^2\right]G_k(\tau)=\delta(\tau),\qquad \tau=t-t'.
$$

It vanishes for negative $\tau$. Continuity at zero excludes an unwanted $\delta'$ term; integrating across zero then fixes $G_k'(0^+)=c^2$. Define $\gamma=\alpha c^2$ and $d_k=\sqrt{\gamma^2-c^2k^2}$. The two homogeneous exponents are $-\gamma\pm d_k$. Imposing the two matching conditions gives the [Fourier-mode Green function of the telegraph equation](../../../../../fourier-mode-green-function-of-the-telegraph-equation.md),

$$
\boxed{G_k(\tau)=\Theta(\tau)\frac{c^2}{d_k}e^{-\gamma\tau}\sinh(d_k\tau)
=\Theta(\tau)\frac{e^{-\alpha c^2\tau}}{\sqrt{\alpha^2-k^2/c^2}}
\sinh\!\left(\sqrt{\alpha^2c^4-k^2c^2}\,\tau\right).}
$$

For an explicit time-Fourier route, use $G_k(\tau)=\int e^{-i\omega\tau}\mathcal G_k(\omega)\,d\omega/(2\pi)$. Then

$$
\mathcal G_k(\omega)=\frac1{k^2-2i\alpha\omega-\omega^2/c^2},\qquad
\omega_\pm=-i\gamma\pm\sqrt{c^2k^2-\gamma^2}.
$$

For $k\ne0$, both [poles](../../../../../pole.md) lie below the real axis. Closing above for $\tau<0$ gives zero; closing below for $\tau>0$ is clockwise, giving $-i$ times the [residue](../../../../../residue.md) sum. Since $\mathcal G_k=-c^2/[(\omega-\omega_+)(\omega-\omega_-)]$, this is

$$
G_k(\tau)=ic^2\frac{e^{-i\omega_+\tau}-e^{-i\omega_-\tau}}{\omega_+-\omega_-}
\quad(\tau>0),
$$

which reduces to the same damped sine or hyperbolic sine above. The $k=0$ [pole](../../../../../pole.md) on the real axis is interpreted by the retarded limiting prescription, or directly by the initial-value matching above.

For $|k|<\alpha c$ the response is overdamped and nonoscillatory. For $|k|>\alpha c$, put $\Omega_k=\sqrt{c^2k^2-\gamma^2}$; analytic continuation gives $G_k=\Theta(\tau)c^2e^{-\gamma\tau}\sin(\Omega_k\tau)/\Omega_k$, a real damped [oscillation](../../../../../oscillation.md). At equality the finite limit is $\Theta(\tau)c^2\tau e^{-\gamma\tau}$.

All nonzero [Fourier modes](../../../../../fourier-mode.md) decay. The uniform mode instead has $G_0=(1-e^{-2\gamma\tau})/(2\alpha)$ for positive time, leaving a constant [temperature](../../../../../temperature-split.md) increment. At small wavenumber the slow decay exponent is $-k^2/(2\alpha)+O(k^4)$, so the [diffusion limit of the damped heat-transmission equation](../../../../../diffusion-limit-of-the-damped-heat-transmission-equation.md) has [diffusivity](../../../../../diffusion-coefficient.md) $1/(2\alpha)$. The full hyperbolic equation has [finite propagation speed](../../../../../finite-propagation-speed.md) $c$, unlike the limiting parabolic [heat equation](../../../../../heat-equation.md).

## ↑ Ancestors (15)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
