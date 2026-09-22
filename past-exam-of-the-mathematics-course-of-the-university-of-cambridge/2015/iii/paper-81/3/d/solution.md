<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $a=2mL^2/(\hbar^2\beta)$ and $C=\sqrt{m/(2\pi\hbar^2\beta)}$. For the reflected images, the intervals $rL-q$, $0\le q\le L$, tile the real line once. A [Gaussian integral](../../../../../../gaussian-integral.md) gives

$$
C\sum_r\int_0^Le^{-2m(rL-q)^2/(\hbar^2\beta)}dq=C\int_{-\infty}^\infty e^{-2mx^2/(\hbar^2\beta)}dx=\frac12.
$$

Consequently $Z=CL\sum_re^{-ar^2}-1/2$. The [Poisson summation formula](../../../../../../poisson-summation-formula.md) applied to the Gaussian yields

$$
\sum_{r\in\mathbb Z}e^{-ar^2}=\sqrt{\frac\pi a}\sum_{n\in\mathbb Z}e^{-\pi^2n^2/a},\qquad CL\sqrt{\frac\pi a}=\frac12.
$$

The zero dual mode cancels the reflected contribution, while the positive and negative modes pair:

$$
\boxed{Z=\frac12\sum_{n\in\mathbb Z}e^{-\beta\hbar^2\pi^2n^2/(2mL^2)}-\frac12=\sum_{n=1}^\infty e^{-\beta\hbar^2\pi^2n^2/(2mL^2)}}.
$$

This proves equality with the [energy eigenstate](../../../../../../energy-eigenstate.md) calculation. The image expansion converges rapidly at small $\beta$; the spectral expansion converges rapidly at large $\beta$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
