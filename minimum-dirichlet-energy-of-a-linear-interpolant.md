# Minimum Dirichlet energy of a linear interpolant

↑ **Parent:** [Linear spline](linear-spline.md)

For nodes $a=x_0<\cdots<x_n=b$ and prescribed real node values, let $s$ be the [linear spline](linear-spline.md) joining them. Among all absolutely continuous [functions](function-split.md) $u$ with the same node values and square-integrable derivative, $s$ uniquely minimizes the [Dirichlet energy](dirichlet-energy.md) $\int_a^b|u'|^2$.

On each node interval, $s'$ is constant and $u-s$ vanishes at both endpoints. The [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) therefore gives $\int s'(u'-s')=s'[(u-s)(x_{i+1})-(u-s)(x_i)]=0$. Expanding the square and summing proves the displayed energy decomposition. Its final term is nonnegative; equality forces $u'=s'$ almost everywhere and the endpoint values fix the additive constant, proving uniqueness. In particular, the minimum is $\sum_i (u(x_{i+1})-u(x_i))^2/(x_{i+1}-x_i)$. If all interior node values are zero and there is at least one interior node, only the two endpoint intervals contribute to this minimum.

## ↑ Ancestors (7)

1. [Linear spline](linear-spline.md)
2. [Spline (mathematics)](spline-mathematics.md)
3. [Uniform approximation](uniform-approximation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2004/p/p3/solution.md)
