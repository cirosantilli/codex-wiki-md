<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) for $\theta$ is

$$
l\ddot\theta+\ddot x\cos\theta+g\sin\theta=0.
$$

For small [angles](../../../../angle.md), set $\cos\theta\simeq1$ and $\sin\theta\simeq\theta$. With $x=A\cos\omega t$ and $\omega_0^2=g/l$, the [harmonic forcing of a horizontally driven pendulum](../../../../harmonic-forcing-of-a-horizontally-driven-pendulum.md) obeys

$$
\ddot\theta+\omega_0^2\theta=\frac{A\omega^2}{l}\cos\omega t.
$$

For $\omega\ne\omega_0$, its general solution is

$$
\boxed{\theta(t)=C\cos\omega_0t+D\sin\omega_0t+\frac{A\omega^2}{l(\omega_0^2-\omega^2)}\cos\omega t.}
$$

The constants $C,D$ set the initial [angle](../../../../angle.md) and [angular velocity](../../../../angular-velocity.md). If the bob starts vertical with zero angular [velocity](../../../../velocity.md) at $t=0$, this reduces to

$$
\theta(t)=\frac{A\omega^2}{l(\omega_0^2-\omega^2)}\bigl(\cos\omega t-\cos\omega_0t\bigr).
$$

The solution remains an approximation only while the resulting [angle](../../../../angle.md) is small.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
