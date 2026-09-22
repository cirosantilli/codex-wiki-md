<h1 id="14e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Papperitz symbol](../../../../../../papperitz-symbol.md) by listing pairs of exponents at $0,1,\infty$. For $F(a,c-b;c;w)$ they are $(0,1-c)$, $(0,b-a)$, and $(a,c-b)$. Under $w=z/(z-1)$ the points $0,1,\infty$ in the $z$-plane correspond respectively to $0,\infty,1$ in the $w$-plane. Thus the pulled-back exponents are $(0,1-c)$ at zero, $(a,c-b)$ at one, and $(0,b-a)$ at infinity.

Multiplication by $(1-z)^{-a}$ shifts the exponents at one by $-a$ and those at infinity by $+a$, yielding

$$
P\left\{\begin{array}{ccc|c}0&1&\infty&z\\0&0&a&\\1-c&c-a-b&b&\end{array}\right\}.
$$

This is the original [Gauss hypergeometric equation](../../../../../../gauss-hypergeometric-equation.md). Both functions are analytic and normalized to one at zero, so uniqueness of that normalized local solution proves the [Pfaff transformation](../../../../../../pfaff-transformation.md)

$$
\boxed{F(a,b;c;z)=(1-z)^{-a}F\left(a,c-b;c;\frac z{z-1}\right).}
$$

Continue the identity using the branch $|\arg(1-z)|<\pi$. As usual, the parameters must admit the normalized hypergeometric solution; excluded singular parameter values are treated only when their limiting solution exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14E](../../14e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
