<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Insert a complete set of [momentum eigenstates](../../../../../../../momentum-eigenstate.md) into the [quantum-mechanical propagator](../../../../../../../quantum-mechanical-propagator.md):

$$
\begin{aligned}
K(x_f,T;x_i,0)
&=\langle x_f|e^{-i\widehat p^2T/(2m\hbar)}|x_i\rangle\\
&=\int_{-\infty}^{\infty}\frac{dp}{2\pi\hbar}
\exp\!\left[\frac{i}{\hbar}p(x_f-x_i)-\frac{iT}{2m\hbar}p^2\right].
\end{aligned}
$$

Completing the square and evaluating the resulting [Gaussian integral](../../../../../../../gaussian-integral.md), with the usual [i-epsilon prescription](../../../../../../../feynman-i-epsilon-prescription.md), gives the [free-particle propagator](../../../../../../../free-particle-propagator.md)

$$
\boxed{K(x_f,T;x_i,0)=
\sqrt{\frac{m}{2\pi i\hbar T}}
\exp\!\left[\frac{im(x_f-x_i)^2}{2\hbar T}\right]}.
$$

The square-root branch is fixed by requiring $K(x_f,T;x_i,0)\to\delta(x_f-x_i)$ as $T\downarrow0$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 304](../../../../paper-304-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
