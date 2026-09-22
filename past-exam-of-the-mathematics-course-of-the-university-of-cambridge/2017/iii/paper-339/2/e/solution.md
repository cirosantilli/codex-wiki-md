<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $t=\log(1+\sqrt2)=\operatorname{arsinh}(1)$, so $c_K=2t/\pi$. The [power series](../../../../../../power-series.md) [coefficients](../../../../../../coefficient.md) of the [hyperbolic sine](../../../../../../hyperbolic-sine.md) preprocessing are

$$
f_{2k}=g_{2k}=0,\qquad
f_{2k+1}=\frac{t^{2k+1}}{(2k+1)!},\qquad
g_{2k+1}=(-1)^kf_{2k+1}.
$$

Thus $f_j=|g_j|$ for every $j\geq0$, and the series converge on the full interval. Applying [coefficient-dominated entrywise positivity](../../../../../../coefficient-dominated-entrywise-positivity.md) gives $Y\succeq0$.

Every diagonal entry belongs to one of the diagonal blocks and equals $f(X_{ii})=f(1)=\sinh t$. Because $e^t=1+\sqrt2$ and $e^{-t}=\sqrt2-1$, this is $(e^t-e^{-t})/2=1$. Therefore

$$
\boxed{Y\succeq0,\qquad Y_{ii}=1}.
$$

The [matrix](../../../../../../matrix.md) lies in the [elliptope](../../../../../../elliptope.md) and admits a [Gram matrix](../../../../../../gram-matrix.md) representation by unit [vectors](../../../../../../vector.md). This preprocessing is the [Krivine rounding scheme](../../../../../../krivine-rounding-scheme.md); the equality of absolute [coefficients](../../../../../../coefficient.md) is what preserves [positive semidefiniteness](../../../../../../positive-semidefinite-matrix.md) even though the cross-block [sine](../../../../../../sine.md) [coefficients](../../../../../../coefficient.md) alternate in sign.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
