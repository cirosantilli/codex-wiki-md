# Supremum of a sum

↑ **Parent:** [Supremum](supremum.md)

Let $A,B$ be nonempty [sets](set-split.md) of [real numbers](real-number.md) bounded above. Their [Minkowski sum](minkowski-addition.md) is $A+B=\{a+b:a\in A,\ b\in B\}$, allowing every pair from the [Cartesian product](cartesian-product.md) $A\times B$. Then

$$
\boxed{\sup(A+B)=\sup A+\sup B.}
$$

The sum of the two [suprema](supremum.md) is an [upper bound](upper-bound-in-a-partially-ordered-set.md) for every permitted sum. For the reverse bound, use the [approximation property of a supremum](approximation-property-of-a-supremum.md) to choose $a>\sup A-\varepsilon/2$ and $b>\sup B-\varepsilon/2$. Their sum is within $\varepsilon$ of the claimed value. This reasoning does not require either [supremum](supremum.md) to be a [maximum](maximum-of-a-subset-of-a-total-order.md).

Separate choices matter. On $X=[0,1]$, choose the [functions](function-split.md) $f(x)=x$ and $g(x)=1-x$. Each has [supremum](supremum.md) one, but their sum at a shared input is always one:

$$
\sup_{x\in X}(f(x)+g(x))=1<2=\sup_{x\in X}f(x)+\sup_{x\in X}g(x).
$$

The [maximum](maximum-of-a-subset-of-a-total-order.md) of $f$ occurs at $x=1$, while that of $g$ occurs at $x=0$. A common input cannot realize both choices. With separate inputs, choosing $x=1$ and $y=0$ gives $f(x)+g(y)=2$. The allowed pairs of output values are the entire [unit square](unit-square.md) for separate inputs, but only the [line segment](line-segment.md) $a+b=1$ for the shared input.

<a id="image-separate-input-choices-fill-a-square-one-shared-input-restricts-the-attainable-sums"></a>
![](supremum-sums-separate-and-shared-inputs.png)

**[Figure 5](#image-separate-input-choices-fill-a-square-one-shared-input-restricts-the-attainable-sums). Separate input choices fill a square; one shared input restricts the attainable sums**. Original example $f(x)=x$, $g(x)=1-x$ on $[0,1]$. Left: every pair $(f(x),g(y))$ is permitted for separate inputs, including $(1,1)$ with sum two. Right: the shared-input pairs $(f(x),g(x))$ lie on $a+b=1$, with sum one. The colours encode $a+b$; this is a deterministic constraint on choices, not probabilistic [independence](independent-random-variables.md).

For any two [bounded functions](bounded-function.md) on the same nonempty [domain of a function](domain-of-a-function.md), the useful general estimate is

$$
\sup_x(f(x)+g(x))\leq\sup_x f(x)+\sup_x g(x).
$$

The [inequality](inequality-mathematics.md) can be strict, as the example shows. Equality does not require attained [maxima](maximum-of-a-subset-of-a-total-order.md), but it does require that the two large values can be approached at compatible inputs. For example, $f(x)=g(x)=x$ on $(0,1)$ gives equality with value two, although neither [function](function-split.md) reaches its [supremum](supremum.md). This distinction is useful when an [objective function](objective-function.md) combines terms sharing a decision variable: adding the best possible termwise scores gives an [upper bound](upper-bound-in-a-partially-ordered-set.md), not necessarily a feasible combined score.

## ↑ Ancestors (7)

1. [Supremum](supremum.md)
2. [Infimum and supremum](infimum-and-supremum.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
