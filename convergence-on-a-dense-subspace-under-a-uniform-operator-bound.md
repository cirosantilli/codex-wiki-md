# Convergence on a dense subspace under a uniform operator bound

↑ **Parent:** [Continuous linear operator](continuous-linear-operator.md)

Let $A_h:X\to Z$, $0<h<1$, be [bounded linear operators](continuous-linear-operator.md) from a [normed space](normed-vector-space-split.md) into a [Banach space](banach-space-split.md), with $M=\sup_h\|A_h\|<\infty$. If $A_hd$ converges as $h\to0^+$ for each element of a [dense subspace](dense-subspace.md) $D$, then $A_hx$ converges for every $x\in X$. The limit defines a [bounded linear operator](continuous-linear-operator.md) $A$ with $\|A\|\leq M$.

For $d\in D$, the [triangle inequality](triangle-inequality.md) gives

$$
\|A_hx-A_kx\|\leq2M\|x-d\|+\|A_hd-A_kd\|.
$$

Approximate $x$ by $d$ and use the [Cauchy criterion for a function limit](cauchy-criterion-for-a-function-limit.md) on $D$. The [completeness](completeness.md) of $Z$ supplies the limit; passing to the limit preserves [linearity](linearity.md) and the bound. When every limit on $D$ is zero, the inequality $\|A_hx\|\leq M\|x-d\|+\|A_hd\|$ shows $A=0$.

## ↑ Ancestors (7)

1. [Continuous linear operator](continuous-linear-operator.md)
2. [Topological vector space](topological-vector-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analysis-i-course-of-the-university-of-oxford/2023/2/d/i/solution.md)
