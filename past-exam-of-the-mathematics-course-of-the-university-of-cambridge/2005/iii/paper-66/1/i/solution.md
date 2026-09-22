<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $B_j^n(t)=\binom njt^j(1-t)^{n-j}$ for the [Bernstein basis](../../../../../../bernstein-basis.md), and set $B_j^n=0$ when $j$ is outside its index range. Differentiating and using $j\binom nj=n\binom{n-1}{j-1}$ and $(n-j)\binom nj=n\binom{n-1}j$ gives

$$
\frac{d}{dt}B_j^n(t)=nB_{j-1}^{n-1}(t)-nB_j^{n-1}(t).
$$

Hence, after shifting the first sum by one index,

$$
\begin{aligned}
P'(t)&=n\sum_{j=0}^nP_jB_{j-1}^{n-1}(t)-n\sum_{j=0}^nP_jB_j^{n-1}(t)\\
&=n\sum_{j=0}^{n-1}(P_{j+1}-P_j)B_j^{n-1}(t).
\end{aligned}
$$

Thus **the [derivative](../../../../../../derivative.md) is a degree-at-most-$(n-1)$ [Bézier curve](../../../../../../bezier-curve.md) whose [control points](../../../../../../control-point.md) are $n(P_{j+1}-P_j)$**. They are vectors rather than necessarily positions on the original [Bézier curve](../../../../../../bezier-curve.md). This is the [Bézier derivative control polygon](../../../../../../bezier-derivative-control-polygon.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
