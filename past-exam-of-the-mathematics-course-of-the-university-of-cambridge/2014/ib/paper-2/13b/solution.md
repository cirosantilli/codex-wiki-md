<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

Use the [rectangular contour for an exponential beta integral](../../../../../rectangular-contour-for-an-exponential-beta-integral.md). For $F(z)=e^{az}/(1+e^z)$, integrate counterclockwise around the rectangle with vertices $-R,R,R+2\pi i,-R+2\pi i$. Its only pole is at $z=\pi i$, with

$$
\operatorname{Res}_{z=\pi i}F(z)=-e^{\pi ia}.
$$

The right vertical side is bounded in modulus by $2\pi e^{aR}/(e^R-1)$, and the left by $2\pi e^{-aR}/(1-e^{-R})$. Both tend to zero because $0<a<1$. On the top edge $F(x+2\pi i)=e^{2\pi ia}F(x)$, and that edge is traversed right to left. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
(1-e^{2\pi ia})\int_{-\infty}^{\infty}\frac{e^{ax}}{1+e^x}\,dx
=-2\pi i e^{\pi ia}.
$$

Since $1-e^{2\pi ia}=-2i e^{\pi ia}\sin(\pi a)$,

$$
\boxed{\int_{-\infty}^{\infty}\frac{e^{ax}}{1+e^x}\,dx=\frac{\pi}{\sin(\pi a)}.}
$$

The same inequalities establish convergence at both real infinities. With $t=e^x$, this integral becomes $\int_0^\infty t^{a-1}/(1+t)\,dt$. Taking $a=1/6$ gives

$$
\boxed{\int_0^\infty\frac{dt}{t^{5/6}(1+t)}=2\pi.}
$$

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
