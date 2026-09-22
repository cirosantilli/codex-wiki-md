<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because the [Fejér kernel](../../../../../../fejer-kernel.md) has normalized integral one,

$$
\sigma_n(f,x)-f(x)
=\frac1\pi\int_{\mathbb T}F_n(t)
[f(x-t)-f(x)]\,dt.
$$

For $f\in\operatorname{Lip}\alpha$ this implies

$$
|\sigma_n(f,x)-f(x)|
\leq\frac{2M}{\pi}\int_0^\pi F_n(t)t^\alpha\,dt.
$$

On $0\leq t\leq\pi$, the inequalities $\sin(t/2)\geq t/\pi$ and $|\sin(nt/2)|\leq n|\sin(t/2)|$ give

$$
F_n(t)\leq\min\left(\frac n2,\frac{\pi^2}{2nt^2}\right).
$$

Splitting the integral at $1/n$ gives

$$
\int_0^\pi F_n(t)t^\alpha\,dt
\leq\frac n2\int_0^{1/n}t^\alpha\,dt
+\frac{\pi^2}{2n}\int_{1/n}^{\pi}t^{\alpha-2}\,dt.
$$

For $0\lt\alpha\lt1$, both terms are $O(n^{-\alpha})$. For $\alpha=1$, the second is $O((\log n)/n)$. Uniformly in $x$,

$$
\boxed{
\|\sigma_n(f)-f\|_\infty\leq
\begin{cases}
c_\alpha n^{-\alpha},&0\lt\alpha\lt1,\\
c_1(\log n)/n,&\alpha=1,
\end{cases}}
$$

where the constants absorb the [Lipschitz continuity](../../../../../../lipschitz-continuity.md) constant $M$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
