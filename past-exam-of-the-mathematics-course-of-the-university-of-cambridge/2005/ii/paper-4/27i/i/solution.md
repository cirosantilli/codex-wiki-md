<h1 id="27i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Complete the square in the independent normal prior and [likelihood](../../../../../../likelihood-function.md):

$$
\tau\theta_i^2+\tau_\varepsilon(X_i-\theta_i)^2
=(\tau+\tau_\varepsilon)\left(\theta_i-\frac{\tau_\varepsilon X_i}{\tau+\tau_\varepsilon}\right)^2
+\frac{\tau\tau_\varepsilon}{\tau+\tau_\varepsilon}X_i^2.
$$

Thus, conditional on the full observations, the hospital parameters remain independent and

$$
\boxed{\theta_i\mid X\sim
N\!\left(\frac{\tau_\varepsilon}{\tau+\tau_\varepsilon}X_i,\
\frac1{\tau+\tau_\varepsilon}\right)}.
$$

If $j$ is the observed minimum index and $X_j=x$, its conditional distribution is exactly this formula with $X_j=x$. No extra truncation is introduced because the selection index is already a function of the conditioned data. Its posterior mean is shrunk toward zero, so the worst measured performance is not simply identified with the worst true performance.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [27I](../../27i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
