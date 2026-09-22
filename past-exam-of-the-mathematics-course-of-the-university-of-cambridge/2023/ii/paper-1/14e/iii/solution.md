<h1 id="14e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\lambda=-m$ with $m\in\mathbb N$. The amplitude is now the rational function

$$
f(t)=\frac{t^{m-1}}{(t-1)^m}.
$$

Choose $\gamma_1$ to be a small positively oriented circle around the pole $t=1$, and choose $\gamma_2$ from $t=0$ along the negative real axis to $-\infty$. At zero the endpoint factor behaves as $t^m$ and vanishes; at negative infinity the exponential decays.

By the [residue theorem](../../../../../../residue-theorem.md), the finite-contour solution is

$$
y_{\gamma_1}(z)
=\frac{2\pi i}{(m-1)!}
 \left.\frac{d^{m-1}}{dt^{m-1}}
 \left(e^{zt}t^{m-1}\right)\right|_{t=1}.
$$

Every derivative term contains $e^z$ times a power of $z$ of degree at most $m-1$, and the highest-degree term is nonzero. Hence

$$
\boxed{y_1(z)=e^zP_{m-1}(z)}
$$

up to a constant, where $P_{m-1}$ is a polynomial of degree $m-1$. This is the negative-integer case of the [Integer-parameter Laguerre contour residues](../../../../../../integer-parameter-laguerre-contour-residues.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
