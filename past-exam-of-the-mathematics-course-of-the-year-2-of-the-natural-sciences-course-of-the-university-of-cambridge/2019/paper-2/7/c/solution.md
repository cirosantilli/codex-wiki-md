<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [mode shapes](../../../../../mode-shape.md) from part (b), and put $\omega=\sqrt{2k/m}$. The initial [velocity](../../../../../velocity.md) decomposes as

$$
(0,0,\Omega)=\frac\Omega2(1,1,1)-\frac\Omega2(1,1,-1).
$$

There is no antisymmetric component because the initial state treats the equal [masses](../../../../../mass.md) identically. Initial displacements are zero, so the [zero mode](../../../../../zero-mode.md) contributes a linear drift and the nonzero [normal mode](../../../../../normal-mode.md) contributes a sine:

$$
\mathbf q(t)=\frac{\Omega t}{2}(1,1,1)
-\frac{\Omega}{2\omega}\sin(\omega t)(1,1,-1).
$$

In terms of actual angular positions,

$$
\boxed{\begin{aligned}
\theta_1(t)&=\frac\Omega2\left(t-\frac{\sin\omega t}{\omega}\right),\\
\theta_2(t)&=\frac{2\pi}{3}+\frac\Omega2\left(t-\frac{\sin\omega t}{\omega}\right),\\
\theta_3(t)&=\frac{4\pi}{3}+\frac\Omega2\left(t+\frac{\sin\omega t}{\omega}\right),\qquad
\omega=\sqrt{\frac{2k}{m}}.
\end{aligned}}
$$

The conserved [angular momentum](../../../../../angular-momentum.md) is initially $2m\Omega$ and the total [moment of inertia](../../../../../moment-of-inertia.md) is $4m$, so the common [angular velocity](../../../../../angular-velocity.md) must be $\Omega/2$, agreeing with the drift. The relative displacements remain of order $\Omega/\omega$, even when the common angle becomes large. Hence small $\Omega/\omega$ preserves the cyclic ordering and small spring extensions at arbitrarily late times. In the ideal arc-spring model the displayed energies are exactly quadratic in the relative angles, so this motion remains exact while that ordering persists.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
