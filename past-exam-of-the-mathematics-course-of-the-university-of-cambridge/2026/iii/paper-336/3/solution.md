<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Introduce the slow time $T=\epsilon t$ and write

$$
v_0=A(T)e^{i\omega t}+\overline{A(T)}e^{-i\omega t}.
$$

At leading order the relaxation equation gives

$$
Z_0=
2|A|^2
+\frac{A^2}{1+2i\omega\tau}e^{2i\omega t}
+\frac{\overline A^2}{1-2i\omega\tau}e^{-2i\omega t}
+K e^{-t/\tau}.
$$

The last term is the freely decaying initial transient; it does not alter the long-time solvability condition.

At order $\epsilon$, eliminating the resonant $e^{i\omega t}$ forcing is the [solvability condition in the method of multiple scales](../../../../../solvability-condition-in-the-method-of-multiple-scales.md). It gives

$$
\boxed{
\frac{dA}{dT}
=A\left[1-(\alpha+i\beta)|A|^2\right]},
\qquad
\alpha+i\beta
=\frac{3+4i\omega\tau}{1+2i\omega\tau}.
$$

Write $A=Re^{i\varphi}$ and let $R(0)=R_0$, $\varphi(0)=\varphi_0$. Then

$$
R'=R(1-\alpha R^2),
\qquad
\varphi'=-\beta R^2.
$$

With

$$
D(T)=1+\alpha R_0^2(e^{2T}-1),
$$

their explicit solutions are

$$
\boxed{
R(T)=\frac{R_0e^T}{\sqrt{D(T)}}},
\qquad
\boxed{
\varphi(T)=\varphi_0-\frac{\beta}{2\alpha}\log D(T)}.
$$

The complete real leading approximation, uniform for $t=O(\epsilon^{-1})$, is therefore

$$
\boxed{
v(t)\sim2R(\epsilon t)
\cos\!\left[\omega t+\varphi(\epsilon t)\right]},
$$



$$
\boxed{
\begin{aligned}
Z(t)\sim{}&
2R(\epsilon t)^2\\
&+\frac{2R(\epsilon t)^2}
{\sqrt{1+4\omega^2\tau^2}}
\cos\!\left[
2\omega t+2\varphi(\epsilon t)
-\tan^{-1}(2\omega\tau)
\right]
+K e^{-t/\tau}.
\end{aligned}}
$$

The constant $K$ is chosen from the initial value of $Z$ after subtracting the mean and second-harmonic pieces. If the initial transient is not required, set $K=0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 336](../../paper-336-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
