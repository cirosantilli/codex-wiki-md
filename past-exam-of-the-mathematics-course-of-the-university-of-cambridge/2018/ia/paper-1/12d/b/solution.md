<h1 id="12d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) says first that if $h$ is continuous on $[a,b]$ and $H(x)=\int_a^xh(t)\,dt$, then $H'(x)=h(x)$. Indeed,

$$
\frac{H(x+s)-H(x)}s-h(x)=\frac1s\int_x^{x+s}(h(t)-h(x))\,dt,
$$

whose absolute value tends to zero by continuity. Consequently, if $F$ is differentiable with continuous derivative, applying the first part to $h=F'$ shows that $F(x)-\int_a^xF'(t)\,dt$ has zero derivative and is constant. Hence

$$
\boxed{\int_a^bF'(t)\,dt=F(b)-F(a).}
$$

A derivative need not be [Riemann integrable](../../../../../../riemann-integrable-function.md). Define $f(0)=0$ and $f(x)=x^2\sin(x^{-2})$ for $x\ne0$. Then $f$ is differentiable at zero with $f'(0)=0$, while for $x\ne0$,

$$
f'(x)=2x\sin(x^{-2})-\frac2x\cos(x^{-2}),
$$

which is unbounded near zero. Since every Riemann-integrable function on a compact interval is bounded, **$g=f'|_{[0,1]}$ need not be Riemann integrable**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12D](../../12d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
