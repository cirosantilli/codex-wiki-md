<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [normalized](../../../../normalization.md) state the position [probability density](../../../../probability-density.md) is $\boxed{f=|\psi|^2}$. With a real potential, the [Time-dependent Schrödinger equation](../../../../time-dependent-schrodinger-equation.md) and its conjugate give

$$
f_t=\frac{i\hbar}{2m}(\overline\psi\psi_{xx}-\psi\overline{\psi_{xx}})=-\partial_x\left[\frac{\hbar}{2mi}(\overline\psi\psi_x-\psi\overline{\psi_x})\right].
$$

This is the [continuity equation](../../../../continuity-equation.md) $\boxed{f_t+j_x=0}$. Integrating over the line yields $d\|\psi\|^2/dt=-j(\infty)+j(-\infty)=0$ under the stated decay. A real-valued [wave function](../../../../wave-function-split.md) gives $\overline\psi\psi_x-\psi\overline{\psi_x}=0$, so its instantaneous current vanishes; the same is true up to a spatially constant [phase](../../../../phase-waves.md).

Put $\alpha=m\omega/\hbar$. [Complete](../../../../completeness.md) the square in the overlap:

$$
\overline{G(u,x)}G(s,x)=|N|^2\overline{\sqrt u}\sqrt s\,e^{-\alpha[(x+\overline u+s)^2-2\overline u s]}.
$$

The [Gaussian integral](../../../../gaussian-integral.md) is $\sqrt{\pi/\alpha}$, also for complex displacement by [analytic continuation](../../../../analytic-continuation.md). Hence

$$
\boxed{\langle G(u),G(s)\rangle=|N|^2\overline{\sqrt u}\sqrt s\sqrt{\pi/\alpha}\,e^{2\alpha\overline u s}.}
$$

The product of square roots fixes the branch convention implicit in the printed square root of $\overline u s$. At $u=s\ne0$ the [norm](../../../../norm.md) squared is $|N|^2|s|\sqrt{\pi/\alpha}\,e^{2\alpha|s|^2}$, which becomes one for the stated $N$. In particular

$$
\boxed{|G(s,x)|^2=\sqrt{\alpha/\pi}\,e^{-\alpha(x+2\operatorname{Re}s)^2}.}
$$

The centre is $-2\operatorname{Re}s$ and its position [variance](../../../../variance-split.md) is $1/(2\alpha)$.

When differentiating in $s$, keep $N$ fixed on the chosen constant-radius orbit. Then

$$
G_x=-\alpha(x+2s)G,\quad G_{xx}=[\alpha^2(x+2s)^2-\alpha]G,\quad sG_s=(\tfrac12-2\alpha sx-2\alpha s^2)G.
$$

Substitution gives $HG=\hbar\omega sG_s$. Since $\dot s=-i\omega s$, the [chain rule](../../../../chain-rule.md) gives $\boxed{i\hbar G_t=HG}$. Continue $\sqrt{s(t)}$ continuously along the time orbit; its sign after a full orbit supplies the usual oscillator zero-point [phase](../../../../phase-waves.md). The case of zero displacement is obtained as a limit, since the separate printed $N$ and $\sqrt s$ expressions are singular at $s=0$.

Finally $j=(\hbar/m)\operatorname{Im}(\overline G G_x)=-2\omega\operatorname{Im}s\,|G|^2$. For real nonzero $a$ this is

$$
\boxed{j(x,t)=2a\omega\sin(\omega t)\sqrt{\frac{m\omega}{\pi\hbar}}\exp\!\left[-\frac{m\omega}{\hbar}(x+2a\cos\omega t)^2\right].}
$$

**The printed final current omits the Gaussian [normalization](../../../../normalization.md) factor** $\sqrt{m\omega/(\pi\hbar)}$. Retaining that factor is required both by the [normalized](../../../../normalization.md) state and by the [continuity equation](../../../../continuity-equation.md). This current is the [Gaussian probability density](../../../../normal-distribution.md) times the velocity of its moving centre, $2a\omega\sin\omega t$.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
