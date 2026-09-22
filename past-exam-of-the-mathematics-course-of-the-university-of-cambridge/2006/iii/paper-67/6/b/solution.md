<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The order-$k$ [divided difference](../../../../../../divided-difference.md) defining $M_i$ is a finite linear combination of values at its knots. Hence integration can be interchanged with it directly. For a knot value $u\in[a,b]$,

$$
\int_a^b(u-t)_+^{k-1}\,dt=\frac{(u-a)^k}{k}.
$$

It follows that

$$
\begin{aligned}
\int_a^bM_i(t)\,dt
&=k[t_i,\ldots,t_{i+k}]\left(u\mapsto\int_a^b(u-t)_+^{k-1}\,dt\right)\\
&=[t_i,\ldots,t_{i+k}](u-a)^k=1.
\end{aligned}
$$

The final equality holds because the order-$k$ [divided difference](../../../../../../divided-difference.md) of a degree-$k$ monic [polynomial](../../../../../../polynomial-split.md) is its [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md), one. Thus

$$
\boxed{\int_a^bM_i(t)\,dt=1.}
$$

This proves the [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md). Its [support](../../../../../../support.md) is contained in $[t_i,t_{i+k}]$: below all its knots, the sampled truncated power agrees with a degree-$k-1$ [polynomial](../../../../../../polynomial-split.md), annihilated by the order-$k$ divided difference; above all its knots, every sample is zero. No mass is omitted by integration over $[a,b]$.

Since $N_i=(t_{i+k}-t_i)M_i/k$, the corresponding partition-normalized [B-spline](../../../../../../b-spline.md) has integral $(t_{i+k}-t_i)/k$. Its normalization is different from that of $M_i$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
