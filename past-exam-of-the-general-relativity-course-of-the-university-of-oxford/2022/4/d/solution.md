<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $u=Br/A$, retaining $r_0$ in $B$. Replacing only the lower integration limit by zero gives

$$
\tau\simeq\frac{A}{B^{3/2}}\int_0^1\sqrt{\frac u{1-u}}\,du
=\frac{\pi A}{2B^{3/2}}.
$$

Substitution of the constants yields

$$
\boxed{\tau\simeq\frac{\pi GM}{(2G\delta M/r_0)^{3/2}}
=\frac{\pi M r_0^{3/2}}{2\sqrt{2G}\,(\delta M)^{3/2}}.}
$$

To quantify the approximation, write $\epsilon=\delta M/M\ll1$. The true lower limit is $u_0=Br_0/A=\epsilon$, and an elementary [integration by substitution](../../../../integration-by-substitution.md), $u=\sin^2\chi$, gives

$$
\tau_{\rm exact}=\frac{A}{B^{3/2}}
\left[\frac\pi2-\arcsin\sqrt\epsilon+\sqrt{\epsilon(1-\epsilon)}\right].
$$

Since $\arcsin\sqrt\epsilon-\sqrt{\epsilon(1-\epsilon)}=\tfrac23\epsilon^{3/2}+O(\epsilon^{5/2})$, the approximate time is too large by a relative fraction $\tfrac4{3\pi}\epsilon^{3/2}+O(\epsilon^{5/2})$. This explains why changing the lower limit introduces little error for a small excess mass. The [cosmological turnaround](../../../../cosmological-turnaround.md) time diverges as $\delta M\to0^+$, consistently with the absence of finite [cosmological turnaround](../../../../cosmological-turnaround.md) in an exactly critical [Einstein-de Sitter universe](../../../../einstein-de-sitter-universe.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
