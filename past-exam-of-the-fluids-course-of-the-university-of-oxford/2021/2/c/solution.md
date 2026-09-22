<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [plane wave](../../../../plane-wave.md) proportional to $e^{i(kx-\omega t)}$. Substitution into the [convected acoustic wave equation](../../../../convected-acoustic-wave-equation.md) gives the [dispersion relation](../../../../dispersion-relation-split.md)

$$
\boxed{(\omega-U_0k)^2=c_0^2k^2,\qquad \omega=(U_0\pm c_0)k.}
$$

The two branches have signed [phase velocities](../../../../phase-velocity.md) and [group velocities](../../../../group-velocity.md) $U_0\pm c_0$. On a branch with $\omega-U_0k=s c_0k$, $s=\pm1$, the linearized [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) gives

$$
p_1=c_0^2\rho_1,\qquad v_1=s\frac{c_0}{\rho_0}\rho_1.
$$

In [subsonic flow](../../../../subsonic-flow.md) with $0\leq U_0<c_0$, the absence of [wave reflection](../../../../wave-reflection.md) selects the outgoing branch on each side:

$$
\rho_1(x,t)=\rho_0\operatorname{Re}\left[Ae^{i(k_\pm x-\omega t)}\right],\qquad
k_+=\frac{\omega}{U_0+c_0}\ (x>0),\quad
k_-=\frac{\omega}{U_0-c_0}\ (x<0).
$$

For $U_0=0$, take $A$ real and positive by choosing the source [phase](../../../../phase-waves.md), and put $k_0=\omega/c_0$. At $\omega t=2n\pi$, the requested spatial profiles are

$$
\boxed{\rho_1=\rho_0A\cos(k_0x),\qquad
p_1=\rho_0c_0^2A\cos(k_0x),\qquad
v_1=c_0A\operatorname{sgn}(x)\cos(k_0x)\quad(x\ne0).}
$$

For complex $A$, retain $\operatorname{Re}[Ae^{ik_0|x|}]$ instead. The normalized [sound pressure](../../../../sound-pressure.md) and [acoustic density perturbation](../../../../acoustic-density-perturbation.md) lie on the same even cosine curve. The [acoustic particle velocity](../../../../acoustic-particle-velocity.md) follows that curve on the right and its negative on the left, as in the figure in part 2(a). Compressed fluid moves away from the source on both sides. These are two outgoing [travelling waves](../../../../travelling-wave.md), not a [standing wave](../../../../standing-wave.md). The ideal point [loudspeaker](../../../../loudspeaker.md) supplies the discontinuity of [velocity](../../../../velocity.md) at $x=0$; the source-free equations apply on either side of it.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
