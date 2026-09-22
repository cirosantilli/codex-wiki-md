<h1 id="a1/a/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Project the expansion onto one normalized basis function. [Orthogonality](../../../../../../orthogonal-vectors.md) removes every other coefficient:

$$
\begin{aligned}
\int_0^a\Psi_m(x)^*f(x)\,\mathrm dx
&=\sum_{n=1}^{\infty}a_n\int_0^a\Psi_m(x)^*\Psi_n(x)\,\mathrm dx\\
&=\sum_{n=1}^{\infty}a_n\delta_{mn}=a_m.
\end{aligned}
$$

Consequently,

$$
\boxed{a_n=\langle\Psi_n|f\rangle
=\sqrt{\frac2a}\int_0^a f(x)\sin\frac{n\pi x}{a}\,\mathrm dx.}
$$

This is a [Fourier sine series](../../../../../../fourier-sine-series.md) in normalized form. For a square-integrable $f$, completeness gives convergence in the norm of the function space; pointwise convergence requires the usual additional regularity. If $f$ is a normalized [wavefunction](../../../../../../wave-function-split.md), the [Born rule](../../../../../../born-rule.md) gives probabilities $|a_n|^2$ and $\sum_n|a_n|^2=1$.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [A](../../a.md)
3. [A1](../../../a1.md)
4. [Paper 1](../../../../paper-1-split.md)
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
