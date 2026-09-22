<h1 id="a2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The density $|\Psi_0|^2=\sqrt{\alpha/\pi}\,e^{-\alpha x^2}$ is even. Hence $\langle x\rangle=0$; also $\Psi_0'=-\alpha x\Psi_0$ gives $\langle p_x\rangle=i\hbar\alpha\langle x\rangle=0$.

To evaluate the second position moment, differentiate the [Gaussian integral](../../../../../gaussian-integral.md) with respect to its positive parameter:

$$
\begin{aligned}
G(\alpha)&=\int_{-\infty}^{\infty}e^{-\alpha x^2}\,\mathrm dx=\sqrt\pi\,\alpha^{-1/2},\\
\int_{-\infty}^{\infty}x^2e^{-\alpha x^2}\,\mathrm dx
&=-G'(\alpha)=\frac{\sqrt\pi}{2\alpha^{3/2}},\\
\langle x^2\rangle&=\sqrt{\frac\alpha\pi}\frac{\sqrt\pi}{2\alpha^{3/2}}
=\frac1{2\alpha}=\frac{\hbar}{2m\omega}.
\end{aligned}
$$

For the momentum second moment, apply the [momentum operator](../../../../../momentum-operator.md) twice:

$$
\langle p_x^2\rangle=-\hbar^2\int\Psi_0^*\Psi_0''\,\mathrm dx
=\hbar^2\left(\alpha-\alpha^2\langle x^2\rangle\right)
=\frac{\hbar^2\alpha}{2}=\frac{m\hbar\omega}{2}.
$$

Both means vanish, so

$$
\boxed{\Delta x=\sqrt{\frac{\hbar}{2m\omega}},\qquad
\Delta p_x=\sqrt{\frac{m\hbar\omega}{2}},\qquad
\Delta x\,\Delta p_x=\frac\hbar2.}
$$

The [ground state](../../../../../ground-state.md) attains the bound proved above and is therefore a [minimum uncertainty state](../../../../../minimum-uncertainty-state.md). A wider Gaussian reduces momentum spread while increasing position spread: the product remains at this lower limit. Other states, including excited oscillator eigenstates, generally give a larger product.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [A2](../../a2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the chemistry A course of the University of Cambridge](../../../../split.md)
6. [Chemistry A course of the University of Cambridge](../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
