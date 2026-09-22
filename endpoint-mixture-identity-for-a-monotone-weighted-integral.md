# Endpoint mixture identity for a monotone weighted integral

↑ **Parent:** [Weighted mean value theorem for integrals](weighted-mean-value-theorem-for-integrals.md)

If $f,g:[a,b]\to\mathbb R$ are [continuous functions](continuous-function.md), $g\geq0$, and $f$ is a nondecreasing [monotonic function](monotonic-function.md), there is $d\in[a,b]$ satisfying the identity in the title. It expresses the weighted [integral](integral-split.md) as a mixture of the two endpoint values of $f$, with the split occurring in the accumulated weight.

Put $G=\int_a^bg$ and $I=\int_a^bfg$. The [monotonicity of the Riemann integral](monotonicity-of-the-riemann-integral.md) gives $f(a)G\leq I\leq f(b)G$. The [function](function-split.md) $H(x)=\int_a^xg$ is [continuous](continuous-function.md); indeed, $|H(y)-H(x)|\leq\max_{[a,b]}|g|\,|y-x|$ by the [extreme value theorem](extreme-value-theorem.md) and the [triangle inequality](triangle-inequality.md) for the [Riemann integral](riemann-integral.md). Therefore

$$
K(x)=f(a)H(x)+f(b)(G-H(x))
$$

is [continuous](continuous-function.md), with $K(a)=f(b)G$ and $K(b)=f(a)G$. The [intermediate value theorem](intermediate-value-theorem.md) gives $K(d)=I$. If the endpoint values coincide, the bounds force $I$ to have that common value and an endpoint works. The proof covers zero total weight and a degenerate [interval](interval-mathematics.md) without division.

## ↑ Ancestors (8)

1. [Weighted mean value theorem for integrals](weighted-mean-value-theorem-for-integrals.md)
2. [Riemann integral](riemann-integral.md)
3. [Riemann integration](riemann-integration.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
