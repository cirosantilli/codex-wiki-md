<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Repeatedly differentiating $f''=-f$ and using $f(0)=1$, $f'(0)=0$ gives

$$
f^{(2k)}(0)=(-1)^k,
\qquad
f^{(2k+1)}(0)=0.
$$

Also,

$$
\frac d{dx}\bigl(f(x)^2+f'(x)^2\bigr)
=2f'f+2f'f''=0,
$$

so $f^2+(f')^2=1$. Every derivative is one of $\pm f,\pm f'$, and hence has absolute value at most one.

Taylor's theorem at zero through degree $2N+1$ gives

$$
f(x)=\sum_{k=0}^N(-1)^k\frac{x^{2k}}{(2k)!}
+R_N(x),
$$

where

$$
|R_N(x)|
\leq\frac{|x|^{2N+2}}{(2N+2)!}\longrightarrow0
$$

for each fixed $x$. Therefore

$$
\boxed{
f(x)=\sum_{k=0}^{\infty}(-1)^k\frac{x^{2k}}{(2k)!}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
