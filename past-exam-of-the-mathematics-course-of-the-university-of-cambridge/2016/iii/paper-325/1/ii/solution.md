<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $h=f\mathbin\square g$ for the [infimal convolution](../../../../../../infimal-convolution.md). It is proper by the permitted hypothesis. If $h(x_0)$ and $h(x_1)$ are finite, choose $y_0,y_1$ within $\varepsilon$ of their respective infima. For $0<t<1$, put $x_t=(1-t)x_0+tx_1$ and $y_t=(1-t)y_0+ty_1$. [Convexity](../../../../../../convex-function.md) of $f$ and $g$ gives

$$
\begin{aligned}
h(x_t)&\leq f(x_t-y_t)+g(y_t)\\
&\leq(1-t)[f(x_0-y_0)+g(y_0)]+t[f(x_1-y_1)+g(y_1)]\\
&\leq(1-t)h(x_0)+th(x_1)+\varepsilon.
\end{aligned}
$$

Let $\varepsilon\downarrow0$. If either endpoint value is infinite, the desired inequality is automatic. Thus **the [infimal convolution](../../../../../../infimal-convolution.md) is convex**, without assuming the infimum is attained.

For its [convex conjugate](../../../../../../convex-conjugate.md), replace a negative infimum by a supremum and then change variables $u=x-y$:

$$
\begin{aligned}
h^*(p)
&=\sup_x\left[\langle p,x\rangle-\inf_y\{f(x-y)+g(y)\}\right]\\
&=\sup_{x,y}\{\langle p,x\rangle-f(x-y)-g(y)\}\\
&=\sup_{u,y}\{\langle p,u\rangle-f(u)+\langle p,y\rangle-g(y)\}\\
&=f^*(p)+g^*(p).
\end{aligned}
$$

The two suprema separate because $u$ and $y$ are independent. Properness of $f$ and $g$ makes each supremum strictly greater than $-\infty$, so this separation remains valid when one or both are $+\infty$. Therefore **$(f\mathbin\square g)^*=f^*+g^*$**. This is the [conjugate of an infimal convolution](../../../../../../conjugate-of-an-infimal-convolution.md). The bounded-domain assumption is unnecessary for these two calculations; the assumed properness and [lower semicontinuity](../../../../../../lower-semicontinuity.md) of $h$ will be used when applying [subgradient inversion under convex conjugacy](../../../../../../subgradient-inversion-under-convex-conjugacy.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
