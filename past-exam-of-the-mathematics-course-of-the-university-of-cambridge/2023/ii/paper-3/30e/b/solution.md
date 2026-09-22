<h1 id="30e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the evenness of $V$, the [semiclassical action integral](../../../../../../semiclassical-action-integral.md) is twice its integral over the positive half-axis. If $0\leq E\leq1$, then

$$
\begin{aligned}
f(E)
&=2\int_0^{4E}\sqrt{E-\frac x4}\,dx\\
&=8\int_0^E u^{1/2}\,du
=\boxed{\frac{16}{3}E^{3/2}}.
\end{aligned}
$$

If $E\geq1$, split the integral at $x=4$:

$$
f(E)=2\left[
\int_0^4\sqrt{E-\frac x4}\,dx
+\int_4^{(E+1)^2}\sqrt{E+1-\sqrt x}\,dx
\right].
$$

The first integral is

$$
\frac83\left(E^{3/2}-(E-1)^{3/2}\right).
$$

In the second, put $r=\sqrt x$ and then $u=E+1-r$. It becomes

$$
\frac43(E+1)(E-1)^{3/2}
-\frac45(E-1)^{5/2}.
$$

After simplification,

$$
\boxed{
f(E)=
\begin{cases}
\dfrac{16}{3}E^{3/2},&0\leq E\leq1,\\[5pt]
\dfrac{16}{3}E^{3/2}
+\dfrac{16}{15}(E-1)^{5/2},&E\geq1.
\end{cases}}
$$

This is the [action integral for a linear-to-square-root potential](../../../../../../action-integral-for-a-linear-to-square-root-potential.md).

The graph begins at the origin, is continuous and strictly increasing, passes through $(1,16/3)$, and tends to infinity. Therefore for every $n\geq0$ and $\varepsilon>0$, the equation

$$
f(E)=\pi\varepsilon\left(n+\frac12\right)
$$

has exactly one solution $E=E_n$ by the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) and strict monotonicity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30E](../../30e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
