<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Schrödinger equation](../../../../../../schrodinger-equation.md) and its complex conjugate are

$$
i\hbar\frac{\partial\psi}{\partial t}
=-\frac{\hbar^2}{2m}\nabla^2\psi+U\psi,
\qquad
-i\hbar\frac{\partial\psi^*}{\partial t}
=-\frac{\hbar^2}{2m}\nabla^2\psi^*+U\psi^*.
$$

Because the potential $U$ is real, its two contributions cancel when differentiating the [probability density](../../../../../../probability-density.md) $\rho=\psi^*\psi$. Therefore

$$
\begin{aligned}
\frac{\partial\rho}{\partial t}
&=\psi^*\frac{\partial\psi}{\partial t}
+\psi\frac{\partial\psi^*}{\partial t}\\
&=\frac{i\hbar}{2m}
\left(\psi^*\nabla^2\psi-\psi\nabla^2\psi^*\right)\\
&=-\nabla\cdot
\left[
-\frac{i\hbar}{2m}
\left(\psi^*\nabla\psi-\psi\nabla\psi^*\right)
\right].
\end{aligned}
$$

The expression in square brackets is the [probability current](../../../../../../probability-current.md) $J$, so

$$
\boxed{\frac{\partial\rho}{\partial t}+\nabla\cdot J=0}.
$$

This [probability continuity equation](../../../../../../probability-continuity-equation.md) says that probability can leave a region only through the current across its boundary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
