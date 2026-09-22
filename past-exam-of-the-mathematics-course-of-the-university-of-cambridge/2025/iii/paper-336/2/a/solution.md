<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the fast time $t$ and slow time $T=\epsilon^2t$, and write

$$
u=u_0+\epsilon u_1+\epsilon^2u_2+\cdots,
\qquad
u_0=A(T)e^{it}+\overline A(T)e^{-it}.
$$

There is no $O(\epsilon)$ resonant forcing. Solving

$$
(\partial_t^2+1)u_1=-\sin t\,u_0
$$

gives a convenient particular solution

$$
u_1=-\frac{iA}{6}e^{2it}
+\frac{i\overline A}{6}e^{-2it}
+\frac i2(\overline A-A).
$$

At $O(\epsilon^2)$, the coefficient of $e^{it}$ in the forcing must vanish by the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md). This gives

$$
-2iA_T-fA+\frac16A-\frac14\overline A=0,
$$

or

$$
A_T=-\frac i2\left(\frac16-f\right)A
+\frac i8\overline A.
$$

The two slow exponents satisfy

$$
s^2=\frac1{64}-\frac14\left(\frac16-f\right)^2.
$$

The [second instability tongue of a weak Mathieu oscillator](../../../../../../second-instability-tongue-of-a-weak-mathieu-oscillator.md) has real $s$ when $-1/12<f<5/12$. At either endpoint the repeated zero exponent permits a linearly growing slow solution, so boundedness for every initial condition requires the strict stable ranges

$$
\boxed{f<-\frac1{12}\quad\hbox{or}\quad f>\frac5{12}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
