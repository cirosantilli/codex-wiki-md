<h1 id="hardy-s-integral-inequality-for-an-interval-indicator">Hardy's integral inequality for an interval indicator</h1>

↑ **Parent:** [Hardy's integral inequality](hardy-s-integral-inequality.md)

Take the [indicator function](indicator-function.md) $f=\mathbf1_{(0,1)}$. Direct [integration](integral-split.md) gives

$$
Hf(x)=\begin{cases}1,&0<x\leq1,\\1/x,&x>1.\end{cases}
$$

Although the [function](function-split.md) vanishes beyond one, its average remembers the unit area accumulated before one. Squaring and integrating both portions gives

$$
\|f\|_2^2=1,\qquad \|Hf\|_2^2=\int_0^1 1\,dx+\int_1^\infty x^{-2}\,dx=1+1=2\leq4\|f\|_2^2=4.
$$

Thus the tail accounts for half of the squared [L2 norm](l2-norm.md). Averaging does not always decrease the [L2 norm](l2-norm.md) with this [Lebesgue measure](lebesgue-measure.md) on the half-line. The same [indicator function](indicator-function.md) also explains the restriction $p>1$: $\int_1^\infty x^{-1}\,dx=\infty$, so its average is not in [L1 space](l1-space.md).

<a id="image-an-indicator-function-its-hardy-operator-average-and-the-tail-s-squared-l2-norm"></a>
![](hardy-interval-indicator-average-tail.png)

**[Figure 1](#image-an-indicator-function-its-hardy-operator-average-and-the-tail-s-squared-l2-norm). An indicator function, its Hardy operator average, and the tail's squared L2 norm**. The upper panel shows the input and its running average. The lower panel splits the squared average at one: each portion has [integral](integral-split.md) one, including the tail beyond the plotted range.

## ↑ Ancestors (7)

1. [Hardy's integral inequality](hardy-s-integral-inequality.md)
2. [Hardy's inequality](hardy-s-inequality.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
