<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $g\in K$, [convexity](../../../../../../convex-function.md) gives $h+t(g-h)\in K$ for $0\leq t\leq1$. Thus $F(t)=\|h-f+t(g-h)\|_p^p$ has a right minimum at $t=0$ and $F'(0)\geq0$. The [derivative of a power of the Lp norm](../../../../../../derivative-of-a-power-of-the-lp-norm.md) is

$$
F'(0)=p\,\operatorname{Re}\int_{\mathbb R^n}|h-f|^{p-2}\overline{(h-f)}(g-h)\,dx.
$$

Consequently

$$
\boxed{\operatorname{Re}\int_{\mathbb R^n}|h-f|^{p-2}\overline{(h-f)}(h-g)\,dx\leq0.}
$$

The printed hint has coefficient $2$ where the general coefficient is $p$. This does not affect the desired sign, since $p>0$. The complex conjugation is important for complex-valued functions; for real functions it can be omitted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
