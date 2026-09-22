<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce the [slow time](../../../../../../slow-time.md) $T=\varepsilon t$ and treat $t,T$ independently in the [method of multiple scales](../../../../../../method-of-multiple-scales.md). Write

$$
y=y_0(t,T)+\varepsilon y_1(t,T)+\cdots,\qquad
y_0=R(T)\cos\phi,\quad \phi=t+\theta(T).
$$

At the next order,

$$
(\partial_t^2+1)y_1=
 f(R\cos\phi,-R\sin\phi)+2R_T\sin\phi+2R\theta_T\cos\phi.
$$

For fixed $R$ define the [period average](../../../../../../period-average.md) by

$$
\langle h\rangle=\frac1{2\pi}\int_0^{2\pi}
 h(\phi;R)\,d\phi.
$$

Here $f$ inside the averages is evaluated at the leading [position](../../../../../../position.md) and [velocity](../../../../../../velocity.md) $R\cos\phi,-R\sin\phi$. [Orthogonality](../../../../../../orthogonal-vectors.md) to both fundamental harmonics is the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md): it removes the resonant forcing that would otherwise generate a [secular term](../../../../../../secular-term.md). Since the squared sine and cosine averages are $1/2$, the [amplitude-phase equations](../../../../../../amplitude-phase-equations-for-a-weakly-perturbed-oscillator.md) are

$$
\boxed{R_T=-\langle f\sin\phi\rangle,\qquad
\theta_T=-\frac1R\langle f\cos\phi\rangle}.
$$

Equivalently $\dot R=-\varepsilon\langle f\sin(t+\theta)\rangle$ and $\dot\theta=-\varepsilon\langle f\cos(t+\theta)\rangle/R$ at first order. These equations describe a bounded, weakly perturbed oscillation over $t=O(\varepsilon^{-1})$ while the [amplitude](../../../../../../wave-amplitude.md) remains in a range where the expansion is ordered. At zero [amplitude](../../../../../../wave-amplitude.md) the [oscillation phase](../../../../../../phase-waves.md) coordinate is singular; Cartesian harmonic coefficients or an equilibrium analysis should replace it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
