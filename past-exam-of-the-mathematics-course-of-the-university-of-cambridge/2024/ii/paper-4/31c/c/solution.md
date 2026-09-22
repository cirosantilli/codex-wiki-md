<h1 id="31c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\lambda=1+\delta$, where $\delta\downarrow0$, and put $x=\lambda(1-u)$. The integration range is $0\leq u\leq1-1/\lambda=\delta+O(\delta^2)$, and

$$
\left((1-u)^{-2}-1\right)^{1/2}
=(2u)^{1/2}+O(u^{3/2}).
$$

Consequently

$$
\int_1^\lambda\left(\frac{\lambda^2}{x^2}-1\right)^{1/2}dx
=\frac{2\sqrt2}{3}\delta^{3/2}+O(\delta^{5/2}).
$$

Substitution into the quantization condition gives

$$
\boxed{\lambda=1+\alpha_n\epsilon^{2/3}+O(\epsilon^{4/3}),
\qquad
\alpha_n=\left[\frac{3\pi}{2\sqrt2}
\left(n+\frac34\right)\right]^{2/3}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31C](../../31c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
