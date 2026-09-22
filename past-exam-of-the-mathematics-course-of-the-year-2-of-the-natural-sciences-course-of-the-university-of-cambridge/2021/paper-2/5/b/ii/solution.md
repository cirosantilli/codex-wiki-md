<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiply the transformed equation by $\sin(k_nx)$ and integrate from zero to $L$. Two [integrations by parts](../../../../../../integration-by-parts.md), using the zero endpoint values of both $\widetilde y$ and the sine, give

$$
\int_0^L\widetilde y_{xx}\sin(k_nx)dx=-k_n^2\int_0^L\widetilde y\sin(k_nx)dx.
$$

The delta source contributes $\widetilde F(\omega)\sin(k_nx_0)$. Multiplying by $2/L$ and using the coefficient definition therefore yields

$$
(k_n^2-\omega^2)b_n(\omega)=\frac2L\sin(k_nx_0)\widetilde F(\omega).
$$

Away from the resonant frequencies this gives

$$
\boxed{b_n(\omega)=\alpha_n\frac{\widetilde F(\omega)}{k_n^2-\omega^2},\qquad\alpha_n=\frac2L\sin(k_nx_0).}
$$

At $\omega=\pm k_n$ the quotient must be interpreted with a [pole](../../../../../../pole.md) prescription if the source excites that mode. In distributional form, arbitrary delta terms at those frequencies may also be added; they are the free homogeneous oscillations. This is the frequency-space issue addressed explicitly in part (iii).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
