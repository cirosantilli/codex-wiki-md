<h1 id="16a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The dyed particle satisfies the [Lagrangian trajectory](../../../../../../lagrangian-trajectory.md) equations

$$
\dot x=\varepsilon y\cos(x-t),
\qquad
\dot y=\varepsilon\sin(x-t),
\qquad
x(0)=y(0)=0.
$$

For the proposed approximation, $x=O(\varepsilon^2)$ and

$$
\dot y=-\varepsilon\sin t
=\varepsilon\sin(x-t)+O(\varepsilon^3).
$$

Also

$$
\dot x
=\varepsilon^2(\cos^2t-\cos t)
=\varepsilon y\cos(x-t)+O(\varepsilon^3).
$$

The initial conditions hold, verifying

$$
x=\varepsilon^2\left(\frac14\sin2t+\frac t2-\sin t\right),
\qquad
y=\varepsilon(\cos t-1)
$$

through order $\varepsilon^2$.

Over one period, the periodic terms return to their initial values while the secular term changes $x$ by $\varepsilon^2\pi$. Hence the dyed particle has [Stokes drift](../../../../../../stokes-drift.md)

$$
\boxed{\overline v_{\rm particle}
=\left(\frac{\varepsilon^2}{2},0\right)}
$$

to this order, despite the zero Eulerian mean velocity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16A](../../16a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
