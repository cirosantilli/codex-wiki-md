<h1 id="13d/solution">Solution</h1>

↑ **Parent:** [13D](../13d.md)

Let $F(z)=e^{az}/(1+e^z)$ and integrate counterclockwise around the rectangle with vertices $-R,R,R+2\pi i,-R+2\pi i$. It contains a single [simple pole](../../../../../simple-pole.md) at $z=\pi i$, with [residue](../../../../../residue.md)

$$
\operatorname{Res}_{z=\pi i}F=\frac{e^{a\pi i}}{e^{\pi i}}=-e^{a\pi i}.
$$

On the top edge $F(x+2\pi i)=e^{2\pi ia}F(x)$, and its orientation reverses that of the bottom edge. On the right edge $|F|\le e^{aR}/(e^R-1)$, so its [integral](../../../../../integral.md) tends to zero for $a<1$. On the left $|F|\le e^{-aR}/(1-e^{-R})$, which tends to zero for $a>0$. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
(1-e^{2\pi ia})\int_{-\infty}^{\infty}\frac{e^{ax}}{1+e^x}\,dx=-2\pi i e^{a\pi i}.
$$

Since $1-e^{2\pi ia}=-2ie^{\pi ia}\sin(\pi a)$,

$$
\boxed{\int_{-\infty}^{\infty}\frac{e^{ax}}{1+e^x}\,dx=\frac\pi{\sin(\pi a)}.}
$$

The restriction is also necessary for ordinary convergence: at $-\infty$ the integrand behaves as $e^{ax}$, requiring $a>0$, while at $+\infty$ it behaves as $e^{(a-1)x}$, requiring $a<1$. At either endpoint one tail approaches a nonzero constant; outside this range one tail grows. There is no cancellation because the real integrand is positive.

## ↑ Ancestors (10)

1. [13D](../13d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
