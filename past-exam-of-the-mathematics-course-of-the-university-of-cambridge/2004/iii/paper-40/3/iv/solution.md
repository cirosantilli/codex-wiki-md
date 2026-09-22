<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $\sigma>0$, use the unnormalized normal shape $h(x)=e^{-x^2/(2\sigma^2)}$. The [ratio-of-uniforms method](../../../../../../ratio-of-uniforms-method.md) samples uniformly from

$$
\mathcal A=\{(u,v):0<u<1,\ u^2\leq h(v/u)\}.
$$

Its boundary is $|v|\leq2\sigma u\sqrt{-\log u}$. The largest possible $|v|$ occurs at $u=e^{-1/2}$ and equals $b=\sigma\sqrt{2/e}$, giving the [normal ratio-of-uniforms envelope](../../../../../../normal-ratio-of-uniforms-envelope.md) $0<u<1$, $-b<v<b$.

Use [independent](../../../../../../independent-random-variables.md) uniform pairs to propose $u=U_{2j-1}$ and $v=b(2U_{2j}-1)$. Accept precisely when

$$
\boxed{v^2\leq-4\sigma^2u^2\log u,\qquad\text{then return }X=v/u.}
$$

To verify its distribution, change coordinates from $(u,v)$ to $(u,x)$, with $v=ux$ and [Jacobian determinant](../../../../../../jacobian-determinant.md) $u$. The accepted point is uniform on $\mathcal A$, and the marginal [probability density function](../../../../../../probability-density-function.md) of $x$ is proportional to

$$
\int_0^{\sqrt{h(x)}}u\,du=\frac12h(x).
$$

Thus the result is $N(0,\sigma^2)$. The region has positive finite area $\sigma\sqrt{\pi/2}$, and the acceptance [probability](../../../../../../probability.md) is $\sqrt{\pi e}/4$. The case $\sigma=0$ requires simply returning zero.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
