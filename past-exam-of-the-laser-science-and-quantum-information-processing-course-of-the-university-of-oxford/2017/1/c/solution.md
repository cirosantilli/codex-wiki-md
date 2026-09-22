<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $N_2=N_{\mathrm{th}}+u$ and $n=n_{\mathrm{ss}}+w$. Keeping terms linear in the perturbations gives

$$
\frac d{dt}\begin{pmatrix}u\\w\end{pmatrix}
=\begin{pmatrix}-r/\tau_2&-1/(f\tau_c)\\f(r-1)/\tau_2&0\end{pmatrix}
\begin{pmatrix}u\\w\end{pmatrix}.
$$

Equivalently,

$$
\ddot w+\frac r{\tau_2}\dot w+\frac{r-1}{\tau_c\tau_2}w=0.
$$

The characteristic exponents are

$$
s_\pm=-\frac r{2\tau_2}\pm i\sqrt{\frac{r-1}{\tau_c\tau_2}-\frac{r^2}{4\tau_2^2}}.
$$

Consequently the above-threshold [steady state](../../../../steady-state.md) has damped [oscillations](../../../../oscillation.md) precisely when

$$
\boxed{\tau_2>\frac{r^2}{4(r-1)}\tau_c,\qquad r>1.}
$$

Their ordinary [frequency](../../../../frequency.md) is

$$
\boxed{f_{\mathrm{ro}}=\frac1{2\pi}\sqrt{\frac{r-1}{\tau_c\tau_2}-\frac{r^2}{4\tau_2^2}}
\simeq\frac1{2\pi}\sqrt{\frac{r-1}{\tau_c\tau_2}}.}
$$

The approximation neglects the damping correction when $r^2\tau_c\ll4(r-1)\tau_2$. The exponential envelope decays on time $2\tau_2/r$. The doped-volume fraction cancels out of this linear [frequency](../../../../frequency.md) once the pump is expressed through $r$. [MIT 6.974, Chapter 7, [laser](../../../../laser-split.md) dynamics and relaxation [oscillations](../../../../oscillation.md)](https://ocw.mit.edu/courses/6-974-fundamentals-of-photonics-quantum-electronics-spring-2006/18f30fad63a62ef4dd894d3752b55a60_chapter7.pdf)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
