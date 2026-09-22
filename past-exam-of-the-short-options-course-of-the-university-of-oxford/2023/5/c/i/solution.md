<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../fourier-transform-split.md) convention $\hat f(s)=\int_{\mathbb R}e^{-isx}f(x)\,dx$. First observe that $f(x)=(2\pi)^{-1/2}e^{-x^2/2}$ satisfies the differential equation, decay, and normalization, using the [Gaussian integral](../../../../../gaussian-integral.md). The uniqueness allowed in the question identifies it with $f$. In particular it is a [Schwartz function](../../../../../schwartz-function.md), so the derivative and multiplication rules below are justified.

Taking the [Fourier transform](../../../../../fourier-transform-split.md) of the differential equation gives

$$
-s^2\hat f+\hat f+\hat f''=0.
$$

The [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md) gives decay of $\hat f$. Every decaying solution $h$ of this equation is proportional to $e^{-s^2/2}$: setting $w=h'+sh$ gives $w'=sw$, and integration yields

$$
h(s)=e^{-s^2/2}\left(D+C\int_0^se^{t^2}\,dt\right).
$$

The term with $C\ne0$ grows like $Ce^{s^2/2}/(2s)$ as $s\to+\infty$, so decay forces $C=0$. Thus $\hat f=\lambda f$ for a scalar $\lambda$. This establishes proportionality before using [Fourier inversion](../../../../../fourier-inversion-theorem.md) to calculate the scalar.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
