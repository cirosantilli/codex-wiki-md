<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

Insert the transform definitions and use Fubini:

$$
\frac1{2\pi}\int\tilde f(k)\tilde g(k)e^{ikx}dk
=\int f(u)\left[\frac1{2\pi}\int\tilde g(k)e^{ik(x-u)}dk\right]du
=\int f(u)g(x-u)du.
$$

For the indicator of $(-1,1)$,

$$
\tilde f(k)=\int_{-1}^1e^{-ikx}dx=\frac{2\sin k}{k}.
$$

Putting $g=f$ and $x=0$ in the [convolution theorem](../../../../../convolution-theorem.md) gives

$$
2=\frac1{2\pi}\int_{-\infty}^{\infty}\frac{4\sin^2k}{k^2}dk,
$$

and hence

$$
\boxed{\int_{-\infty}^{\infty}\frac{\sin^2k}{k^2}dk=\pi.}
$$

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
