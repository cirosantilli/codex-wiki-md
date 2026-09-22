<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\alpha>0$, variation of constants gives the stationary [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md)

$$
f(t)=c\int_{-\infty}^t
\Lambda_f(s)e^{-\alpha(t-s)}\,ds.
$$

For $t\geq t'$ its covariance is

$$
\begin{aligned}
\langle f(t)f(t')\rangle
&=c^2\int_{-\infty}^{t'}
e^{-\alpha(t-s)}e^{-\alpha(t'-s)}\,ds\\
&=\frac{c^2}{2\alpha}e^{-\alpha(t-t')}.
\end{aligned}
$$

Symmetry in $t,t'$ therefore gives

$$
\boxed{
\langle f(t)f(t')\rangle
=f_0^2e^{-\alpha|t-t'|},
\qquad
f_0^2=\frac{c^2}{2\alpha}
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
