# Continuity bounds for the square function

↑ **Parent:** [Epsilon-delta definition of continuity](epsilon-delta-definition-of-continuity.md)

For $f(x)=x^2$ at any real $a$, [polynomial factorization](factorization-of-polynomials.md) gives

$$
|f(x)-f(a)|=|x-a|\,|x+a|.
$$

If $|x-a|<1$, the [triangle inequality](triangle-inequality.md) yields $|x+a|\leq|x-a|+2|a|<2|a|+1$. Therefore the displayed choice of $\delta$ makes $|x-a|<\delta$ imply $|f(x)-f(a)|<\varepsilon$. This proves [continuity](continuous-function.md) and gives an explicit local error bound, rather than an inference from a drawing.

At $a=1$ and $\varepsilon=0.6$, this sufficient choice is $\delta=0.2$. The permitted [function inputs](function-input.md) satisfy $0.8<x<1.2$; their actual [function outputs](function-output.md) lie in $(0.64,1.44)$, inside the requested band $(0.4,1.6)$. A sufficient input window need not be the largest possible one.

<a id="image-an-input-window-that-guarantees-the-requested-output-tolerance-for-the-square-function"></a>
![](square-continuity-input-output-tolerances.png)

**[Figure 17](#image-an-input-window-that-guarantees-the-requested-output-tolerance-for-the-square-function). An input window that guarantees the requested output tolerance for the square function**. For the [polynomial function](polynomial-function.md) $f(x)=x^2$ at $a=1$, the blue input window has $\delta=0.2$ and the orange output band has $\varepsilon=0.6$. The highlighted [function graph](graph-of-a-function.md) segment lies inside their overlap. The illustration shows an exact mathematical example, rather than measured values.

## ↑ Ancestors (9)

1. [Epsilon-delta definition of continuity](epsilon-delta-definition-of-continuity.md)
2. [Continuous function](continuous-function.md)
3. [Limit of a function](limit-of-a-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Continuous function](continuous-function.md)
- [Uniformly continuous function](uniformly-continuous-function.md)
