<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

There are two positive roots for $u>1$: the [derivative](../../../../../../derivative.md) of $xe^{1/x}$ is $e^{1/x}(1-1/x)$, so the function decreases to its minimum $e$ at $x=1$ and then increases. Negative $x$ cannot solve the equation. For the larger root, expansion of the [exponential function](../../../../../../exponential-function.md) in $1/x$ gives

$$
xe^{1/x}=x+1+\frac1{2x}+O(x^{-2}),
$$

so [series reversion](../../../../../../series-reversion.md) yields

$$
\boxed{x_{\rm large}=e^u-1+O(e^{-u}).}
$$

For the smaller root, set $y=1/x$ and take a [logarithm](../../../../../../logarithm.md). Then $y-\log y=u$, so successive substitution gives $y=u+\log u+O(\log u/u)$ and

$$
\boxed{x_{\rm small}=\frac1u-\frac{\log u}{u^2}+O\left(\frac{(\log u)^2}{u^3}\right).}
$$

These are the first two nonzero terms of the two [asymptotic expansions](../../../../../../asymptotic-expansion.md). Equivalently, the roots are $-1/W_0(-e^{-u})$ and $-1/W_{-1}(-e^{-u})$, from the [real branches of Lambert W](../../../../../../real-branches-of-lambert-w.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
