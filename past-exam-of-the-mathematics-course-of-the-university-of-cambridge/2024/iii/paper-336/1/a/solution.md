<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Factor out the elementary exponential and write

$$
I(\lambda)=\lambda^{-1/2}e^{2\lambda}J(\lambda),
\qquad
J(\lambda)=\int_0^\infty
e^{-s-\lambda^2/s}\,ds.
$$

Use a [matched asymptotic expansion](../../../../../../matched-asymptotic-expansion.md) with $0<\lambda\ll\delta\ll1$. In the outer part,

$$
J_{\rm out}
=\int_{\delta^2}^\infty e^{-s}
\left(1-\frac{\lambda^2}{s}+\cdots\right)ds.
$$

The given identity for the [Euler--Mascheroni constant](../../../../../../euler-s-constant.md), integrated by parts, implies

$$
\int_{\delta^2}^\infty\frac{e^{-s}}s\,ds
=-\gamma_e-2\log\delta+O(\delta^2).
$$

Hence

$$
J_{\rm out}
=1-\delta^2
+\lambda^2(\gamma_e+2\log\delta)
+o(\lambda^2),
$$

apart from pure higher matching powers in $\delta$.

In the inner part, use $t=\lambda^2/s$:

$$
J_{\rm in}
=\lambda^2
\int_{\lambda^2/\delta^2}^\infty
t^{-2}e^{-t}e^{-\lambda^2/t}\,dt.
$$

Since $s=\lambda^2/t\leq\delta^2$, expand the last exponential. At the required order,

$$
\int_a^\infty t^{-2}e^{-t}\,dt
=\frac{e^{-a}}a-int_a^\infty\frac{e^{-t}}t\,dt
=\frac1a-1+\gamma_e+\log a+O(a).
$$

With $a=\lambda^2/\delta^2$, this gives

$$
J_{\rm in}
=\delta^2
+\lambda^2
\left[-1+\gamma_e
+2\log\lambda-2\log\delta\right]
+o(\lambda^2).
$$

The overlap terms $\delta^2$ and $\log\delta$ cancel, leaving the logarithmic [switchback term](../../../../../../switchback-term.md)

$$
J(\lambda)
=1+\lambda^2
\left(2\log\lambda+2\gamma_e-1\right)
+o(\lambda^2).
$$

Finally,

$$
e^{2\lambda}=1+2\lambda+2\lambda^2+O(\lambda^3),
$$

so

$$
\boxed{
I(\lambda)
\sim\lambda^{-1/2}
+2\lambda^{1/2}
+\lambda^{3/2}
\left(1+2\log\lambda+2\gamma_e\right)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
