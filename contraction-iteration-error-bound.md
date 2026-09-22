# Contraction iteration error bound

↑ **Parent:** [Contraction mapping theorem](contraction-mapping-theorem.md)

Successive steps satisfy $d(x_{n+1},x_n)\leq L^n d(x_1,x_0)$. Summing the remaining steps with the [triangle inequality](triangle-inequality.md) gives a bound available before the iteration starts:

$$
d(x_n,x_*)\leq\frac{L^n}{1-L}\,d(x_1,x_0)\qquad(n\geq0).
$$

After computing a new step, the [contraction mapping](contraction-mapping.md) gives the often sharper bound

$$
d(x_n,x_*)\leq\frac{L}{1-L}\,d(x_n,x_{n-1})\qquad(n\geq1).
$$

Equivalently, the residual at any $z\in X$ satisfies $d(z,x_*)\leq d(z,Tz)/(1-L)$. These estimates convert visible step sizes into guaranteed distances to an unknown [fixed point](fixed-point.md). When $L$ is close to one, the factor $1/(1-L)$ can be large: a small step alone needs interpretation through the contraction constant.

## ↑ Ancestors (6)

1. [Contraction mapping theorem](contraction-mapping-theorem.md)
2. [Fixed-point theorem](fixed-point-theorem.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cosine fixed-point iteration](cosine-fixed-point-iteration.md)
