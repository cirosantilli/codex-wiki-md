<h1 id="a8/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiation of the restricted free energy gives the [magnetization](../../../../../../magnetization.md)

$$
\begin{aligned}
M_{\mathrm{restricted}}
&=-\frac1V\left(\frac{\partial A_{\mathrm{mag}}}{\partial B}\right)_{T,V}\\
&=\boxed{\frac{N\mu}{V}\tanh\frac{\mu B}{k_{\mathrm B}T}}.
\end{aligned}
$$

In the weak-field limit $|\mu B|\ll k_{\mathrm B}T$, $\tanh x\simeq x$, so

$$
\boxed{M_{\mathrm{restricted}}\simeq\frac{N\mu^2B}{Vk_{\mathrm B}T}
=\frac{4N\mu_{\mathrm B}^2B}{Vk_{\mathrm B}T}.}
$$

**The printed coefficient is inconsistent with the stated moment $\mu=2\mu_{\mathrm B}$.** The requested expression without the factor four would follow from $\mu=\mu_{\mathrm B}$ in this restricted model. This discrepancy is present in the original PDF, rather than introduced by its transcription.

For completeness, differentiating the full thermal free energy gives

$$
\boxed{M_{\mathrm{full}}=\frac{N\mu}{V}
\frac{e^{-\beta\Delta}\sinh x}{1+e^{-\beta\Delta}\cosh x}.}
$$

Its weak-field form is

$$
\boxed{M_{\mathrm{full}}\simeq\frac{N\mu^2B}{Vk_{\mathrm B}T}
\frac1{1+e^{\theta/T}}
=\frac{4N\mu_{\mathrm B}^2B}{Vk_{\mathrm B}T(1+e^{\theta/T})}.}
$$

At $k_{\mathrm B}T\gg\Delta$ this approaches $2N\mu_{\mathrm B}^2B/(Vk_{\mathrm B}T)$, so restoring the two nonmagnetic ground states does not recover the printed coefficient either. The inverse-temperature [Curie law](../../../../../../curie-s-law.md) form is valid, but the population factor and moment squared must be retained consistently.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [A8](../../../a8.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
