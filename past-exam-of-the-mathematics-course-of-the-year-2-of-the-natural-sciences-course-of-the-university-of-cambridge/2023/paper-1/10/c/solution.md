<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\gamma>0$ and set $A=\pi/2$. The [Rayleigh quotient](../../../../../rayleigh-quotient.md) of the trial for the [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md) is

$$
R(\gamma)=\frac{\int_{-A/\gamma}^{A/\gamma}[\gamma^2\sin^2(\gamma x)+x^2\cos^2(\gamma x)]dx}{\int_{-A/\gamma}^{A/\gamma}\cos^2(\gamma x)dx}.
$$

Its denominator is $\pi/(2\gamma)$. The kinetic numerator is $\gamma^2$ times that denominator. For the remaining [integral](../../../../../integral-split.md), put $t=\gamma x$ and use

$$
\int_{-\pi/2}^{\pi/2}t^2\cos^2t\,dt=\frac{\pi^3}{24}-\frac\pi4=\frac{\pi(\pi^2-6)}{24},
$$

obtained from $\cos^2t=(1+\cos2t)/2$ and [integration by parts](../../../../../integration-by-parts.md). Thus the [compact cosine trial bound for the quantum harmonic oscillator](../../../../../compact-cosine-trial-bound-for-the-quantum-harmonic-oscillator.md) is

$$
\boxed{R(\gamma)=\gamma^2+\frac{\pi^2-6}{12\gamma^2}.}
$$

Differentiation gives $R'=2\gamma-(\pi^2-6)/(6\gamma^3)$, so the minimizing parameter satisfies

$$
\boxed{\gamma_{\mathrm{opt}}^4=\frac{\pi^2-6}{12}.}
$$

The quotient tends to infinity at either end of $\gamma>0$, and the two positive terms are equal at this stationary point, proving it is the global minimum. Therefore

$$
\boxed{\lambda_0\leq\sqrt{\frac{\pi^2-6}{3}}\approx1.13572.}
$$

For comparison, the exact [ground state](../../../../../ground-state.md) has value $1$. The trial is admissible for the energy [quadratic form](../../../../../quadratic-form-split.md): it is continuous, has compact support, and its [weak derivative](../../../../../weak-derivative.md) is square-integrable. Its first [derivative](../../../../../derivative.md) jumps at the support endpoints, so it need not belong to the smaller twice-differentiable [operator domain](../../../../../operator-domain.md); this does not invalidate the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) bound.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
