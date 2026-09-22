<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $u=t-t'$ and $\Omega=\sqrt{\omega_0^2-\gamma^2/4}$. With the printed [Fourier transform](../../../../../fourier-transform-split.md) convention, a time [derivative](../../../../../derivative.md) transforms to $i\omega$. The [retarded Green function](../../../../../retarded-green-function.md) is

$$
G(u)=\int_{-\infty}^\infty\frac{d\omega}{2\pi}
\frac{e^{i\omega u}}{\omega_0^2-\omega^2+i\gamma\omega}.
$$

Its [poles](../../../../../pole.md) are $\omega=\pm\Omega+i\gamma/2$, both in the upper half-plane. For $u>0$ close the contour above; for $u<0$ close below, where there are no [poles](../../../../../pole.md). [Residues](../../../../../residue.md) give

$$
\boxed{G(t-t')=\Theta(t-t')e^{-\gamma(t-t')/2}
\frac{\sin[\Omega(t-t')]}{\Omega}.}
$$

It is continuous at $u=0$ and has [derivative](../../../../../derivative.md) jump $G'(0^+)-G'(0^-)=1$, reproducing the [Dirac delta function](../../../../../dirac-delta-function.md) source. Thus the solution initially at rest is

$$
\eta(t)=A\int_0^t G(t-s)e^{-\alpha s}\,ds\quad(t\geq0),
$$

and vanishes for $t<0$. Set $D=\alpha^2-\gamma\alpha+\omega_0^2=(\alpha-\gamma/2)^2+\Omega^2>0$. Evaluating the integral gives

$$
\boxed{\eta(t)=\frac A D\left[e^{-\alpha t}
-e^{-\gamma t/2}\cos(\Omega t)
+\frac{\alpha-\gamma/2}{\Omega}e^{-\gamma t/2}\sin(\Omega t)\right],\quad t\geq0.}
$$

The [homogeneous solution](../../../../../homogeneous-solution.md) constants are $C_1=-A/D$ and $C_2=A(\alpha-\gamma/2)/(D\Omega)$. Substitution at zero gives $\eta(0)=\dot\eta(0)=0$. [Causality](../../../../../causality.md) selects this response; an arbitrarily excited prehistory would add a [homogeneous solution](../../../../../homogeneous-solution.md).

<a id="1/d/image-illustrative-retarded-impulse-response-and-initially-resting-response-to-a-decaying-drive"></a>
![](../../../../../past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2013/paper-1-tp1-causal-response.png)

**[Figure 1](#1/d/image-illustrative-retarded-impulse-response-and-initially-resting-response-to-a-decaying-drive). Illustrative retarded impulse response and initially resting response to a decaying drive**.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
