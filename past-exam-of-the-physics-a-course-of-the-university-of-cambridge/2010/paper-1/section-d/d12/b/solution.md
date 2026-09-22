<h1 id="section-d/d12/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The transient is the homogeneous part of a [damped harmonic oscillator](../../../../../../damped-harmonic-oscillator.md), $m\ddot x+b\dot x+kx=0$. Define $\alpha=b/(2m)$ and $\omega_0=\sqrt{k/m}$. Its characteristic roots are $-\alpha\pm\sqrt{\alpha^2-\omega_0^2}$.

- For $\alpha<\omega_0$, the [underdamped](../../../../../../underdamping.md) response is $x=e^{-\alpha t}(A\cos\omega_dt+B\sin\omega_dt)$, with $\omega_d=\sqrt{\omega_0^2-\alpha^2}$. The displacement oscillates with a decaying envelope.
- At critical damping, $x=(A+Bt)e^{-\omega_0t}$. It has a repeated root, so two identical exponentials are not an independent pair of solutions.
- For $\alpha>\omega_0$, two real negative exponentials produce an [overdamped](../../../../../../overdamping.md) return without sustained oscillation. In the strong-damping limit the slow decay rate is approximately $k/b$, not $b/m$.

Initial position and velocity determine A,B. For an imposed force or support motion, the full solution is a particular response plus this transient, which decays for b\>0 and k\>0. The mechanical energy obeys $d(K+U)/dt=-b\dot x^2$. In light damping its cycle-averaged envelope decays as $e^{-2\alpha t}$, with $Q\simeq\omega_0/(2\alpha)$. Initial conditions can still produce an overshoot in a nonoscillatory regime; the damping category describes the roots rather than every possible trajectory.

<a id="section-d/d12/b/image-oscillator-transients"></a>
![](../../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2010/paper-1-pa2010-oscillator-transients.png)

**[Figure 8](#section-d/d12/b/image-oscillator-transients). Oscillator transients**. [Source](paper-1-pa2010-oscillator-transients.py). Dimensionless release from unit displacement and zero velocity for three damping regimes.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
