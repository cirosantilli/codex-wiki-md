<h1 id="39d/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $x$ upward, let $y$ measure distance from the wall, and work in the cylinder frame. The wall at $y=0$ moves upward with speed $V$. Choose the sign of $\Omega$ so that the near-cylinder surface at $y=h$ moves upward with speed $a\Omega$. Lubrication theory gives

$$
\mu\frac{\partial^2u}{\partial y^2}=\frac{dp}{dx},
\qquad u(0)=V,\qquad u(h)=a\Omega.
$$

Thus

$$
\boxed{
u(y)=V+\frac{a\Omega-V}{h}y
+\frac1{2\mu}\frac{dp}{dx}y(y-h).}
$$

The vertical volume flux per unit cylinder length is independent of $x$ and equals

$$
Q=\int_0^h u\,dy
=\frac h2(V+a\Omega)-\frac{h^3}{12\mu}\frac{dp}{dx}.
$$

Therefore

$$
\frac{dp}{dx}=\frac{6\mu(V+a\Omega)}{h^2}-\frac{12\mu Q}{h^3}.
$$

Because $p(+\infty)=p(-\infty)$, its [integral](../../../../../../../integral.md) over $x$ vanishes. With

$$
t=\frac{x}{\sqrt{2ah_0}},\qquad h=h_0(1+t^2),
$$

the quoted [integrals](../../../../../../../integral.md) give

$$
\frac{\int_{-\infty}^{\infty}h^{-2}\,dx}
{\int_{-\infty}^{\infty}h^{-3}\,dx}
=\frac{4h_0}{3}.
$$

It follows that

$$
\boxed{Q=\frac{2h_0}{3}(V+a\Omega).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [39D](../../../39d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
