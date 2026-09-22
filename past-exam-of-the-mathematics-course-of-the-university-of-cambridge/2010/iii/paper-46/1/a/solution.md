<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [quantum rotor](../../../../../../quantum-rotor.md), the transition kernel is the [path integral](../../../../../../path-integral.md)

$$
K(\theta_f,\theta_i;T)=\int_{\theta(0)=\theta_i}^{\theta(T)=\theta_f\ ({\rm mod}\ 2\pi)}\mathcal D\theta\,e^{iS[\theta]/\hbar},\qquad S[\theta]=\frac\Lambda2\int_0^T\dot\theta^2\,dt.
$$

The integral includes all paths on the circle, not just paths whose chosen real lifts have the same endpoint difference. Operator evolution and the stated energy-state normalization give

$$
\boxed{K(\theta_f,\theta_i;T)=\langle\theta_f|e^{-iHT/\hbar}|\theta_i\rangle=\frac1{2\pi}\sum_{n\in\mathbb Z}e^{in(\theta_f-\theta_i)}e^{-i\hbar n^2T/(2\Lambda)}.}
$$

The factor $1/(2\pi)$ comes from the completeness relation; it makes the zero-time limit the periodic [Dirac delta distribution](../../../../../../dirac-delta-function.md). For real time the oscillatory sum is understood through $T\to T-i0$, or as a distributional limit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
