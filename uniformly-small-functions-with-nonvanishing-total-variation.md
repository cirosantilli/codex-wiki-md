# Uniformly small functions with nonvanishing total variation

↑ **Parent:** [Total variation of a function](total-variation-of-a-function.md)

For each positive [integer](integer-split.md) $n$, put $f_n(t)=\sin(2\pi nt)/n$ on $[0,1]$. Its [supremum norm](supremum-norm.md) is exactly $1/n$, so this [sequence of functions](sequence-of-functions.md) converges to zero by [uniform convergence](uniform-convergence.md). Nevertheless,

$$
\boxed{V_0^1(f_n)=4\quad\text{for every }n\geq1.}
$$

Each of its $n$ complete [sine](sine.md) oscillations contributes $4/n$: rise from zero to $1/n$, fall through zero to $-1/n$, then return to zero. Taking a [partition of an interval](partition-of-an-interval.md) through all extrema attains $4$. Every further [partition refinement](partition-refinement.md) merely subdivides [monotone function](monotonic-function.md) segments, so the same reasoning as in [partition example of total variation](partition-example-of-total-variation.md) proves the upper bound too.

<a id="image-the-functions-sin-2-pi-nt-n-converge-uniformly-to-zero-while-their-total-variation-remains-4-all-three-function-plots-use-the-same-vertical-scale"></a>
![](total-variation-small-amplitude-oscillations.png)

**[Figure 23](#image-the-functions-sin-2-pi-nt-n-converge-uniformly-to-zero-while-their-total-variation-remains-4-all-three-function-plots-use-the-same-vertical-scale). The functions sin(2πnt)/n converge uniformly to zero while their total variation remains 4; all three function plots use the same vertical scale**.

For a [continuously differentiable function](continuously-differentiable-function.md) on a closed bounded [interval](interval-mathematics.md), total variation also satisfies

$$
V_a^b(f)=\int_a^b|f'(t)|\,dt.
$$

Applied here, the [derivative](derivative.md) is $2\pi\cos(2\pi nt)$, and integrating its [absolute value](absolute-value.md) over $n$ periods gives $4$. The differentiability hypothesis matters: the partition definition applies much more widely than this derivative formula.[NIST Digital Library of Mathematical Functions; §1.4(v), equations 1.4.33–1.4.34, Functions of Bounded Variation](nist-digital-library-of-mathematical-functions/1-algebraic-and-analytic-methods.md) Small pointwise size and small accumulated movement are different approximation goals.

## ↑ Ancestors (7)

1. [Total variation of a function](total-variation-of-a-function.md)
2. [Riemann integration](riemann-integration.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
