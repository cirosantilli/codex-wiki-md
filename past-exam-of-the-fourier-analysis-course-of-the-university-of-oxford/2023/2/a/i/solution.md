<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $R\phi(x)=\phi(-x)$, and define reflection of a [tempered distribution](../../../../../tempered-distribution.md) by $\langle Ru,\phi\rangle=\langle u,R\phi\rangle$. The [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) on the [Schwartz space](../../../../../schwartz-space.md) says $\widehat{\widehat\phi}=2\pi R\phi$. Thus

$$
\langle\widehat{\widehat u},\phi\rangle
=\langle u,\widehat{\widehat\phi}\rangle
=2\pi\langle u,R\phi\rangle
=2\pi\langle Ru,\phi\rangle.
$$

Reflection commutes with the [Fourier transform](../../../../../fourier-transform-split.md), since $\widehat{R\phi}=R\widehat\phi$ and the same relation follows by duality for [tempered distributions](../../../../../tempered-distribution.md). Define the [inverse Fourier transform](../../../../../inverse-fourier-transform.md) on [tempered distributions](../../../../../tempered-distribution.md) by

$$
\mathcal F^{-1}v=\frac1{2\pi}R\widehat v,
\qquad
\langle\mathcal F^{-1}v,\phi\rangle=\langle v,\mathcal F^{-1}\phi\rangle.
$$

It follows that

$$
\boxed{\mathcal F^{-1}\mathcal Fu=u=\mathcal F\mathcal F^{-1}u\quad(u\in\mathcal S'(\mathbb R)).}
$$

In particular $u=(2\pi)^{-1}R\widehat{\widehat u}$ is the general [Fourier inversion](../../../../../fourier-inversion-theorem.md) formula. When $\widehat u$ is an [integrable function](../../../../../lebesgue-integrable-function.md), this is the [regular distribution](../../../../../regular-distribution.md) of $(2\pi)^{-1}\int\widehat u(\xi)e^{ix\xi}\,d\xi$; an arbitrary [tempered distribution](../../../../../tempered-distribution.md) need not have an ordinary integral representation.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
