<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use normalized instantaneous modes $\varphi_p(x,t)=\sqrt{2/L}\sin(p\pi x/L)$ and expand $\Psi=\sum_p a_pe^{-i\vartheta_p}\varphi_p$. Differentiating at fixed $x$ gives

$$
\partial_t\varphi_p=-\frac{\dot L}{2L}\varphi_p-\sqrt{\frac2L}\frac{p\pi x\dot L}{L^2}\cos(p\pi x/L).
$$

For $n\ne p$, [integration](../../../../../integral-split.md) uses

$$
\int_0^1 u\sin(n\pi u)\cos(p\pi u)\,du
=-\frac{(-1)^{n+p}n}{\pi(n^2-p^2)},
$$

so the [moving-wall derivative coupling](../../../../../moving-wall-derivative-coupling.md) is

$$
\langle\varphi_n|\dot\varphi_p\rangle
=\frac{\dot L}{L}(-1)^{n+p}\frac{2np}{n^2-p^2}.
$$

For $n=p$ the normalization [derivative](../../../../../derivative.md) and the remaining [integral](../../../../../integral-split.md) cancel exactly, giving zero. The moving [integration](../../../../../integral-split.md) endpoint contributes no boundary term because every mode vanishes there. Therefore

$$
\boxed{\dot a_n=\frac{\dot L}{L}\sum_{p\ne n}(-1)^{n+p}\frac{2np}{p^2-n^2}\,a_p e^{i(\vartheta_n-\vartheta_p)}}.
$$

The real coupling [matrix](../../../../../matrix.md) is antisymmetric, as required by conservation of total [probability](../../../../../probability.md).

## ↑ Ancestors (15)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
