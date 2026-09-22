<h1 id="6c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At time $t$ the state is

$$
\chi(t)=\frac12e^{-iE_1t/\hbar}\chi_1
+\frac{\sqrt3}{2}e^{-iE_2t/\hbar}\chi_2.
$$

Direct evaluation of the radial [integral](../../../../../../integral.md) gives the [matrix elements](../../../../../../matrix-element.md)

$$
\langle\chi_1|r|\chi_1\rangle=\frac{3a}{2},
\qquad
\langle\chi_2|r|\chi_2\rangle=6a,
$$

and

$$
\begin{aligned}
\langle\chi_1|r|\chi_2\rangle
&=4\pi\int_0^\infty r^3\chi_1(r)\chi_2(r)\,dr\\
&=-\frac{64a}{81\sqrt2}.
\end{aligned}
$$

It follows that

$$
\boxed{
R(t)=\frac{39a}{8}
-\frac{32a}{81}\sqrt{\frac32}
\cos\!\left(\frac{E_2-E_1}{\hbar}t\right)
}.
$$

Thus $R(t)$ oscillates sinusoidally about $39a/8$. Its [angular frequency](../../../../../../angular-frequency.md) is

$$
\boxed{\omega=\frac{E_2-E_1}{\hbar}
=\frac{3mK^2}{8\hbar^3}
=\frac{3K}{8a\hbar}}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6C](../../6c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
