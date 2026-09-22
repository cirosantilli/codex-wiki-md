# Completeness of a graph norm from a bounded right inverse

↑ **Parent:** [Graph norm](graph-norm.md)

Let $X$ be a [normed space](normed-vector-space-split.md), $Y$ a [Banach space](banach-space-split.md), and $T:X\to Y$ a [linear map](linear-map.md). If its [kernel](kernel-of-a-linear-map-split.md) is [complete](completeness.md) in the original [norm](norm.md) and $S:Y\to X$ is a bounded [right inverse](right-inverse.md), then the [graph norm](graph-norm.md) $\|x\|_T=\|x\|_X+\|Tx\|_Y$ is [complete](completeness.md), even if $X$ with its original [norm](norm.md) is incomplete or $T$ is unbounded.

For a [Cauchy sequence](cauchy-sequence.md) $(x_n)$ in the [graph norm](graph-norm.md), $y_n=Tx_n$ converges to $y\in Y$. The elements $w_n=x_n-Sy_n$ lie in the [kernel](kernel-of-a-linear-map-split.md) and satisfy $\|w_n-w_m\|_X\leq(1+\|S\|)\|x_n-x_m\|_T$. Hence $w_n\to w\in\ker T$. The element $x=w+Sy$ satisfies $Tx=y$ and

$$
\|x_n-x\|_T\leq\|w_n-w\|_X+(1+\|S\|)\|y_n-y\|_Y\longrightarrow0.
$$

## ↑ Ancestors (8)

1. [Graph norm](graph-norm.md)
2. [Closed linear operator](closed-linear-operator.md)
3. [Graph of a linear operator](graph-of-a-linear-operator.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Differentiation operator](differentiation-operator.md)
- [Solution](past-exam-of-the-functional-analysis-i-course-of-the-university-of-oxford/2023/1/c/solution.md)
