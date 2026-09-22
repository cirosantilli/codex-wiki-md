<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $\lambda>0$, define $\widetilde g_t(z)=\lambda^{-1/2}g_{\lambda t}(\sqrt\lambda z)$. Differentiating the [Chordal Loewner equation](../../../../../../../chordal-loewner-equation.md) gives

$$
\partial_t\widetilde g_t(z)=\frac2{\widetilde g_t(z)-\widetilde W_t},
\qquad \widetilde W_t=\lambda^{-1/2}W_{\lambda t}.
$$

[Brownian scaling](../../../../../../../brownian-scaling.md) makes $\widetilde W$ have the original driver law. The corresponding hull is $\lambda^{-1/2}K_{\lambda t}$, so

$$
\boxed{(K_{\lambda t})_{t\geq0}\overset d=(\sqrt\lambda K_t)_{t\geq0}.}
$$

The time scaling applies to the whole coupled hull process. In particular, the joint law of swallowing times satisfies $(T(cx),T(cy))\overset d=c^2(T(x),T(y))$.

Thus $F(cx,cy)=F(x,y)$. A pair $0<x<y$ is determined up to dilation by $z=y/(y-x)>1$: dilating by $(y-x)^{-1}$ turns it into $(z-1,z)$. Define $f(z)=F(z-1,z)$. Then

$$
\boxed{F(x,y)=f\!\left(\frac{y}{y-x}\right).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
