<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Divide the [external force](../../../../external-force.md) by $m$. Away from resonance a particular solution has the forcing frequency, so the general [forced harmonic oscillator](../../../../forced-harmonic-oscillator.md) solution is

$$
\boxed{x(t)=A\cos\omega_0t+B\sin\omega_0t+
\frac{F_0}{m(\omega_0^2-\omega^2)}\cos(\omega t-\phi),\qquad\omega\ne\omega_0.}
$$

The two homogeneous terms cannot be discarded in an undamped system: they do not decay. If the same initial conditions are imposed, then $A=x_0-C\cos\phi$, $B=-C(\omega/\omega_0)\sin\phi$, where $C=F_0/[m(\omega_0^2-\omega^2)]$.

For $\omega\gg\omega_0$, the forced displacement approaches $-F_0\cos(\omega t-\phi)/(m\omega^2)$: its amplitude decreases quadratically and it is in antiphase with the force. This statement concerns the forced component; a freely excited component at $\omega_0$ can remain.

At [resonance](../../../../resonance.md) the preceding denominator is zero and the appropriate solution is

$$
\boxed{x(t)=A\cos\omega_0t+B\sin\omega_0t+
\frac{F_0t}{2m\omega_0}\sin(\omega_0t-\phi).}
$$

Its amplitude grows linearly because the external force supplies energy coherently. For $x(0)=x_0$, $\dot x(0)=0$, choose $A=x_0$ and $B=F_0\sin\phi/(2m\omega_0^2)$. Physical damping or nonlinear response ultimately limits the ideal resonant growth.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [2017 resit](../../../2017-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
