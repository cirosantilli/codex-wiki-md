<h1 id="39b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The five-point stencil on the forcing satisfies

$$
\Gamma_5f=h^2\Delta f+\frac{h^4}{12}(f_{xxxx}+f_{yyyy})+O(h^6).
$$

Thus the correction $h^2\Gamma_5f/12$ cancels exactly the $h^4\Delta f/12$ residual in part (i), leaving

$$
\Gamma_9u-h^2f-\frac{h^2}{12}\Gamma_5f
=h^6\left[-\frac{u_{xxxxxx}+u_{yyyyyy}}{240}+\frac{u_{xxxxyy}+u_{xxyyyy}}{144}\right]+O(h^8).
$$

The modified scheme therefore has **fourth-order normalized local accuracy**, the same improved order as the harmonic-forcing case, now without assuming $\Delta f=0$. It need not have the same leading error constant.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [39B](../../39b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
