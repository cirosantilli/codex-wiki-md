<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $x\in\mathbb R^n$ and a coordinate direction $e_i$. The [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives

$$
\frac{g(t,x+he_i)-g(t,x)}h
=\int_0^1D_i g(t,x+she_i)\,ds.
$$

For sufficiently small $h$, the points $(t,x+she_i)$ lie in a fixed compact set. The continuity of $D_i g$ makes it [uniformly continuous](../../../../../../uniform-continuity.md) there, so the right-hand side converges to $D_i g(t,x)$ uniformly in $t$. We may consequently pass the limit through the finite [integral](../../../../../../integral.md):

$$
\begin{aligned}
D_iG(x)
&=\lim_{h\to0}\int_0^1
\frac{g(t,x+he_i)-g(t,x)}h\,dt\\
&=\boxed{\int_0^1D_i g(t,x)\,dt}.
\end{aligned}
$$

To prove continuity, if $x_k\to x$, joint continuity makes $D_i g(t,x_k)\to D_i g(t,x)$ uniformly for $t\in[0,1]$ once the $x_k$ lie in a compact neighbourhood of $x$. Hence $D_iG(x_k)\to D_iG(x)$. This proves the stated [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) result and the continuity of every partial derivative.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
