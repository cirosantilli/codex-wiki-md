<h1 id="7e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the positive real axis, whose path does not cross the left-displaced cut,

$$
F_B(x)=\int_0^x\frac{dt}{1+t^2}=\arctan x
=\frac\pi2+O(x^{-1}).
$$

Since $F_B'(z)=1/(1+z^2)=O(|z|^{-2})$ near infinity, integrating this [derivative](../../../../../../derivative.md) along large arcs extends the same expansion uniformly there:

$$
F_B(z)=\frac\pi2+O(|z|^{-1}).
$$

Therefore

$$
\oint_{\gamma_R}\frac{F_B(t)}t\,dt
=\frac\pi2\oint_{\gamma_R}\frac{dt}{t}+O(R^{-1})
=i\pi^2+O(R^{-1}),
$$

and hence

$$
\boxed{\lim_{R\to\infty}\oint_{\gamma_R}\frac{F_B(t)}t\,dt=i\pi^2.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7E](../../7e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
