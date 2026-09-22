# Stability of a supremum under uniform perturbations

↑ **Parent:** [Supremum](supremum.md)

Suppose $f,g:X\to\mathbb R$ are [bounded functions](bounded-function.md) on the same nonempty [set](set-split.md), and the [supremum norm](supremum-norm.md) of their difference is at most $\delta$. Then their optimal values differ by at most the same amount:

$$
\boxed{\left|\sup_{x\in X}f(x)-\sup_{x\in X}g(x)\right|\leq\|f-g\|_\infty\leq\delta.}
$$

Indeed, $f(x)\leq g(x)+\delta\leq\sup_X g+\delta$ for every $x$, so $\sup_X f\leq\sup_X g+\delta$; exchange $f$ and $g$ for the other direction. Adding a constant shifts a [supremum](supremum.md) by that constant, a basic compatibility between [upper bounds](upper-bound-in-a-partially-ordered-set.md) and [addition](addition.md).[Basic Analysis: Introduction to Real Analysis, Volume I by Jiří Lebl; §1.2.3, Proposition 1.2.6(i): translating a nonempty bounded-above set translates its supremum](basic-analysis-introduction-to-real-analysis-volume-i-by-jiri-lebl/1-2-the-set-of-real-numbers.md)

For a chosen example on $[-1,1]$, take $f(x)=-x^2$ and $g(x)=-x^2+0.2x$. Their [supremum error](supremum-error.md) is $0.2$, since $|g(x)-f(x)|=0.2|x|$. [Completing the square](completing-the-square.md) gives

$$
g(x)=-(x-0.1)^2+0.01.
$$

Thus $f$ has [maximum](maximum-of-a-subset-of-a-total-order.md) zero at $x=0$, while $g$ has [maximum](maximum-of-a-subset-of-a-total-order.md) $0.01$ at $x=0.1$. The change in optimal value, $0.01$, is smaller than the certified bound $0.2$. For the vertical translation $h(x)=f(x)+0.2$, the bound is exact: its [supremum error](supremum-error.md) and optimal-value change are both $0.2$.

<a id="image-uniform-error-controls-the-optimal-value-maximizing-inputs-require-additional-control"></a>
![](supremum-uniform-perturbations-and-maximizers.png)

**[Figure 6](#image-uniform-error-controls-the-optimal-value-maximizing-inputs-require-additional-control). Uniform error controls the optimal value; maximizing inputs require additional control**. Original [polynomial](polynomial-split.md) examples on $[-1,1]$. Left: $-x^2$ and $-x^2+0.2x$ lie within a vertical error band of $0.2$, while their [maxima](maximum-of-a-subset-of-a-total-order.md) differ by $0.01$. Right: the small tilts $\varepsilon x$ and $-\varepsilon x$ have maximizing inputs $1$ and $-1$ for every $\varepsilon>0$; solid lines use $\varepsilon=0.1$ and dashed lines use $0.02$. These chosen examples are not measured errors or claims about an arbitrary optimizer.

A stable optimal value does not guarantee a stable maximizing input. On $[-1,1]$, the two [linear functions](linear-function.md) $f_\varepsilon(x)=\varepsilon x$ and $g_\varepsilon(x)=-\varepsilon x$ satisfy

$$
\|f_\varepsilon-g_\varepsilon\|_\infty=2\varepsilon\longrightarrow0,
\qquad\sup f_\varepsilon=\sup g_\varepsilon=\varepsilon.
$$

For every positive $\varepsilon$, their unique maximizing inputs remain two units apart, at $1$ and $-1$. Both [functions](function-split.md) approach the flat zero [function](function-split.md), which has many maximizing inputs. Consequently an accurate [objective function](objective-function.md) value is not by itself a certificate that the optimizing decision is accurate.

The estimate also gives a convenient consequence of [uniform convergence](uniform-convergence.md). If $f_n$ converges uniformly to a [bounded function](bounded-function.md) $f$ on a nonempty $X$, then $\sup_X f_n\to\sup_X f$ for the bounded tail of the [sequence](sequence.md). Uniform control handles the changing input that defines the best value. [Pointwise convergence](pointwise-convergence.md) alone supplies no such control; the existing examples under [uniform convergence](uniform-convergence.md) illustrate that distinction.

## ↑ Ancestors (7)

1. [Supremum](supremum.md)
2. [Infimum and supremum](infimum-and-supremum.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
