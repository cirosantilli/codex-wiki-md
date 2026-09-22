<h1 id="3g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First suppose each $g_j$ is [differentiable](../../../../../../differentiable-function.md) at $x_j$. Write $g_j(x_j+t)=g_j(x_j)+v_jt+r_j(t)$, where $v_j\in\mathbb R^m$ and $r_j(t)=o(|t|)$. Define the [linear map](../../../../../../linear-map.md) $Lh=\sum_jv_jh_j$. Given $\varepsilon>0$, choose a common sufficiently small neighbourhood so that $\|r_j(h_j)\|\le\varepsilon|h_j|$ for all $j$, with $r_j(0)=0$. Then

$$
\left\|f(x+h)-f(x)-Lh\right\|\le\varepsilon\sum_j|h_j|\le\varepsilon\sqrt n\,\|h\|.
$$

This proves [differentiability](../../../../../../differentiability.md), with

$$
\boxed{Df(x)h=\sum_{j=1}^n g_j'(x_j)h_j.}
$$

Conversely, suppose $f$ is [differentiable](../../../../../../differentiable-function.md) with [Fréchet derivative](../../../../../../frechet-derivative.md) $L$. Along the $j$th coordinate direction $e_j$, the other summands cancel exactly:

$$
g_j(x_j+t)-g_j(x_j)=f(x+te_j)-f(x)=tLe_j+o(|t|).
$$

Thus $g_j$ is [differentiable](../../../../../../differentiable-function.md) at $x_j$, with $g_j'(x_j)=Le_j$. **The equivalence works because each summand varies in only one coordinate; it is stronger than merely having partial derivatives.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3G](../../3g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
