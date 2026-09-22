<h1 id="9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For explicit sketches take a symmetric, 50% [duty cycle](../../../../duty-cycle.md) square wave with levels $\pm V_0$. The source does not specify levels or duty cycle; a unipolar 50% wave follows by adding its mean and rescaling. Let $\tau=RC$ and $M$ be the positive output extremum in the periodic steady state. The [square-wave response of an RC low-pass filter](../../../../square-wave-response-of-an-rc-low-pass-filter.md) has

$$
M=V_0\tanh\frac{T}{4\tau},\qquad
V_{\mathrm{out}}(t)=\begin{cases}
V_0-(V_0+M)e^{-t/\tau},&0\leq t<T/2,\\
-V_0+(V_0+M)e^{-(t-T/2)/\tau},&T/2\leq t<T,
\end{cases}
$$

extended periodically. The extremum formula follows by imposing $V_{\mathrm{out}}(0)=-M$ and $V_{\mathrm{out}}(T/2)=M$. It makes the three regimes below quantitative, including their finite amplitudes.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [9](../../9.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
