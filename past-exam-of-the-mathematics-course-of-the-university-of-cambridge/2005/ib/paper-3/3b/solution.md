<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

A function is a [differentiable function](../../../../../differentiable-function.md) at $a_0=(a,b)$ if there is a [linear map](../../../../../linear-map.md) $L:\mathbb R^2\to\mathbb R$ with

$$
f(a_0+h)=f(a_0)+Lh+r(h),\qquad\frac{r(h)}{\|h\|}\longrightarrow0\quad(h\to0).
$$

The map $L=Df_{a_0}$ is its derivative; equivalently $L(h_1,h_2)=Ah_1+Bh_2$ for fixed constants. Since every such linear map is bounded, $|f(a_0+h)-f(a_0)|\leq\|L\|\|h\|+|r(h)|\to0$. This proves **[differentiability implies continuity](../../../../../differentiability-implies-continuity.md)**, not merely continuity along each coordinate axis.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
