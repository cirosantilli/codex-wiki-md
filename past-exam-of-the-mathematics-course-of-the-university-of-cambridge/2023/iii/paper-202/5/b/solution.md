<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $V'=v$, the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
\psi'(x)=e^{-V(x)},
\qquad
\psi''(x)=-v(x)e^{-V(x)}.
$$

Applying the [Itô formula](../../../../../../ito-s-lemma.md) before the lifetime, the two drift terms cancel:

$$
d\psi(X_t)
=\frac12v(X_t)\psi'(X_t)dt
+\psi'(X_t)dB_t
+\frac12\psi''(X_t)dt
=e^{-V(X_t)}dB_t.
$$

**Thus $\psi(X)$ is a continuous local martingale. The increasing function $\psi$ is the [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
