<h1 id="10b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $x>0$, $x\ne1$,

$$
\int_0^1x^y\,dy=\frac{x-1}{\log x},
$$

with limiting value one at $x=1$. Integrating over $0<x<1$ in the opposite order gives

$$
\int_0^1\int_0^1x^y\,dy\,dx
=\int_0^1\frac{dy}{y+1}
=\log2.
$$

On the other hand, after setting $x=e^{-u}$,

$$
\int_0^1\frac{x-1}{\log x}\,dx
=\int_0^\infty\frac{e^{-u}-e^{-2u}}u\,du.
$$

Consequently

$$
\boxed{
\int_0^\infty\frac{e^{-u}-e^{-2u}}u\,du=\log2}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10B](../../10b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
