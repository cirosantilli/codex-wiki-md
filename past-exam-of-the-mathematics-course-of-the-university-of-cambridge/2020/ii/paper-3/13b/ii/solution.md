<h1 id="13b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because $e(x,0)=0$, the egg density is the accumulated deposition

$$
e(x,t)=\lambda\int_0^t n(x,s)\,ds.
$$

It is convenient to use the [Fourier transform](../../../../../../fourier-transform.md). The larval equation gives

$$
\widehat n(k,t)=N e^{-(Dk^2+\mu)t},
\qquad
\widehat e(k,\infty)=\frac{N\lambda}{Dk^2+\mu}.
$$

Applying the stated inverse-transform integral with $\alpha=\sqrt{\mu/D}$ gives the [remnant density from diffusion with mortality and deposition](../../../../../../remnant-density-from-diffusion-with-mortality-and-deposition.md)

$$
\boxed{e(x,\infty)=\frac{N\lambda}{2\sqrt{D\mu}}
\exp\left(-|x|\sqrt{\frac\mu D}\right).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13B](../../13b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
