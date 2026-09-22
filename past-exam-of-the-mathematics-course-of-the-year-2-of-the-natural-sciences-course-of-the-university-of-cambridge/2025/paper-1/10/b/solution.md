<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the trial function, $y_T'=-ax\,y_T$. The required [Gaussian integrals](../../../../../gaussian-integral.md) are

$$
G[y_T]=\int_{\mathbb R}e^{-ax^2}\,dx=\sqrt{\frac\pi a},\qquad\int_{\mathbb R}x^2e^{-ax^2}\,dx=\frac{\sqrt\pi}{2a^{3/2}}.
$$

The second formula follows by differentiating the first with respect to $a$. Therefore

$$
F[y_T]=a^2\frac{\sqrt\pi}{2a^{3/2}}-V_0\sqrt{\frac\pi{1+a}},
$$

and division by $G[y_T]$ gives the [Gaussian variational bound for an attractive Gaussian well](../../../../../gaussian-variational-bound-for-an-attractive-gaussian-well.md):

$$
\boxed{E(a)=\frac a2-V_0\sqrt{\frac a{1+a}},\qquad a>0.}
$$

This is a good trial family because it consists of smooth, positive, [square-integrable functions](../../../../../square-integrable-function.md) decaying at both infinities. Each is an [even function](../../../../../even-function.md), matching the symmetry of the lowest [bound state](../../../../../bound-state.md) in this even potential, and the parameter varies its width. It also permits exact [Gaussian integrals](../../../../../gaussian-integral.md). Its Gaussian tail need not equal the exact exponential tail of a negative-energy [bound state](../../../../../bound-state.md) for the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md) to give a valid bound.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
