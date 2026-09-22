<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Twice applying the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
f(x+h)-2f(x)+f(x-h)=\int_0^h\int_{-s}^{s}f''(x+u)\,du\,ds,
$$

hence $\boxed{\omega_2(f,t)\leq t^2\lVert f''\rVert_\infty}$. Part (b) gives $\lVert\sigma_n(f)-f\rVert_\infty=O(n^{-1})$. This cannot be little-$o$ for every $C^2$ function: for $f_0(x)=\cos x$,

$$
\sigma_n(f_0)=(1-n^{-1})\cos x,\qquad
\boxed{\lVert\sigma_n(f_0)-f_0\rVert_\infty=n^{-1}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
