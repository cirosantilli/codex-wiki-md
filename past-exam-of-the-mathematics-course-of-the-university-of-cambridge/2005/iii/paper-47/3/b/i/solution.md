<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [ratio-of-uniforms method](../../../../../../../ratio-of-uniforms-method.md) on

$$
\mathcal R=\{(u,v):0<u\leq1,\ u^2\leq h(v/u)\}.
$$

Writing $x=v/u$ gives $u\leq e^{-x^2/(4\sigma^2)}$ and $v=ux$. Consequently

$$
|v|\leq\max_{x\geq0}x e^{-x^2/(4\sigma^2)}
=\sigma\sqrt{2/e},
$$

because the derivative vanishes at $x=\sigma\sqrt2$. Thus the [normal ratio-of-uniforms envelope](../../../../../../../normal-ratio-of-uniforms-envelope.md) is the rectangle $0<u<1$, $|v|<\sigma\sqrt{2/e}$.

Generate [independent](../../../../../../../independent-random-variables.md) $U_1,U_2$ with [uniform distribution](../../../../../../../continuous-uniform-distribution.md) on $(0,1)$, set $u=U_1$ and $v=(2U_2-1)\sigma\sqrt{2/e}$, and accept precisely when

$$
u^2\leq\exp\!\left[-\frac{(v/u)^2}{2\sigma^2}\right].
$$

Reject and repeat otherwise. **On acceptance return $X=v/u$.** One can compare logarithms instead of exponentials to avoid underflow.

For a proof, the change of variables $(u,x)\mapsto(u,v=ux)$ has [Jacobian determinant](../../../../../../../jacobian-determinant.md) $u$. A uniform point in $\mathcal R$ therefore gives an $x$-density proportional to

$$
\int_0^{\sqrt{h(x)}}u\,du=\frac{h(x)}2.
$$

Normalizing yields the required [normal distribution](../../../../../../../normal-distribution.md) with [mean](../../../../../../../expected-value.md) zero and [variance](../../../../../../../variance-split.md) $\sigma^2$. The region area is $\frac12\int h(x)\,dx=\sigma\sqrt{\pi/2}$; dividing it by the rectangle area $2\sigma\sqrt{2/e}$ gives acceptance [probability](../../../../../../../probability.md) $\sqrt{\pi e}/4$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
