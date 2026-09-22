<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let the motor's constant [power](../../../power.md) be $P>0$ and put $\omega=\dot\theta$. The braking coefficient in the proposed formula must describe a retarding [torque](../../../torque.md) $k\omega$. This [constant-power rotational acceleration](../../../constant-power-rotational-acceleration.md) obeys the [energy balance](../../../energy-balance.md):

$$
\frac d{dt}\left(\frac I2\omega^2\right)=P-k\omega^2.
$$

Consequently the steady [angular velocity](../../../angular-velocity.md) is $\omega_0=\sqrt{P/k}$, and the ordinary rotational [frequency](../../../frequency.md) is $\omega_0/(2\pi)$. Solving the linear equation for $\omega^2$ from rest gives

$$
\omega^2(t)=\omega_0^2\left(1-e^{-2kt/I}\right),\qquad
\boxed{t=-\frac I{2k}\ln\left(1-\frac{\omega^2}{\omega_0^2}\right).}
$$

**The printed time formula is missing a minus sign.** Its logarithm is negative for $0<\omega<\omega_0$, whereas elapsed time must be positive. The terminal speed is approached only as $t\to\infty$.

A constant-power motor starting exactly from rest is an idealization: its driving [torque](../../../torque.md) $P/\omega$ would diverge. The energy equation has a regular solution for $\omega^2$, although the initial angular acceleration is singular. If $k\omega$ were literally a tangential force, a lever arm would also be needed; the dimensions of the requested expression identify $k$ as a rotational damping coefficient.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2016 resit](../../2016-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
