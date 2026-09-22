# Derivative seminorms on a compact interval

↑ **Parent:** [Fréchet space](frechet-space.md)

Here $C^\infty([0,1])$ means the real- or complex-valued [functions](function-split.md) [continuous](continuous-function.md) on $[0,1]$, [smooth](smooth-function.md) on $(0,1)$, with every interior [derivative](derivative.md) having a [continuous](continuous-function.md) extension to the endpoints; endpoint values of [derivatives](derivative.md) are these extensions. On this [space of smooth functions on a compact interval](space-of-smooth-functions-on-a-compact-interval.md), define

$$
p_k(f)=\max_{0\leq j\leq k}\sup_{t\in[0,1]}|f^{(j)}(t)|,
\qquad k=0,1,2,\ldots,\qquad f^{(0)}=f.
$$

These finite-valued [seminorms](seminorm.md) increase with $k$ and separate points. In fact every $p_k$ is a [norm](norm.md), since it includes $p_0(f)=\|f\|_\infty$. The terminology [seminorm](seminorm.md) includes [norms](norm.md); it does not assert that every measurement has a nontrivial [kernel of a seminorm](kernel-of-a-seminorm.md). [Smooth convergence](smooth-convergence-on-a-compact-interval.md) means $p_k(f_n-f)\to0$ for every fixed $k$, equivalently [uniform convergence](uniform-convergence.md) of every [derivative](derivative.md) separately. It does not demand one tolerance or one convergence index that works for all orders simultaneously. The maximum convention is equivalent to the [derivative supremum norm](derivative-supremum-norm.md) convention using a finite sum, since $p_k(f)\leq\sum_{j=0}^k\|f^{(j)}\|_\infty\leq(k+1)p_k(f)$.

For a worked example, $f(t)=t^3$ gives $p_0(f)=1$, $p_1(f)=3$, $p_2(f)=6$, and $p_k(f)=6$ for $k\geq3$. The [linear functional](linear-functional.md) $\ell(f)=f''(1/2)$ obeys $|\ell(f)|\leq p_2(f)$ and is [continuous](continuous-function.md). Similarly, [differentiation](differentiation.md) is a [continuous linear operator](continuous-linear-operator.md) $D:f\mapsto f'$ for [smooth convergence](smooth-convergence-on-a-compact-interval.md), because $p_k(Df)\leq p_{k+1}(f)$.

The [space of smooth functions on a compact interval](space-of-smooth-functions-on-a-compact-interval.md) is complete for this [seminorm topology](seminorm-topology.md). A [Cauchy sequence](cauchy-sequence.md) has [uniform limits](uniform-limit.md) $g_j$ for its [derivatives](derivative.md) of each order. Passing to the limit in the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) identity

$$
f_n^{(j)}(t)-f_n^{(j)}(0)=\int_0^t f_n^{(j+1)}(s)\,ds
$$

gives $g_j(t)-g_j(0)=\int_0^t g_{j+1}(s)\,ds$, so $g_j'=g_{j+1}$ and $g_0$ belongs to the same space. This is the [completeness of the smooth-function metric](completeness-of-the-smooth-function-metric.md) argument; the [metric](metric.md) there and the increasing-$p_k$ [metric](metric.md) above induce the same smooth [topology](topology-split.md) and the same [Cauchy sequences](cauchy-sequence.md).

**Table of contents**

- [Smooth convergence on a compact interval](smooth-convergence-on-a-compact-interval.md)

## ↑ Ancestors (8)

1. [Fréchet space](frechet-space.md)
2. [Locally convex space](locally-convex-space.md)
3. [Topological vector space](topological-vector-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
