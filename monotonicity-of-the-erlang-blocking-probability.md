# Monotonicity of the Erlang blocking probability

↑ **Parent:** [Erlang loss formula](erlang-loss-formula.md)

For positive integer capacity $C$ and [offered load](offered-traffic.md) $a>0$, let $m_C(a)$ be the [carried load of an Erlang loss resource](carried-load-of-an-erlang-loss-resource.md). Differentiating the [upper-truncated Poisson distribution](upper-truncated-poisson-distribution.md) gives $m_C'(a)=\operatorname{Var}(N)/a>0$. Differentiating its probability at $C$ gives the displayed [derivative](derivative.md) of the [Erlang loss formula](erlang-loss-formula.md); it is positive because $m_C(a)<C$. Thus blocking increases continuously from zero to one, and the carried load increases from zero to $C$. These properties justify the inverse blocking coordinates in the [convex potential for the Erlang fixed point](convex-potential-for-the-erlang-fixed-point.md).

## ↑ Ancestors (9)

1. [Erlang loss formula](erlang-loss-formula.md)
2. [Loss network](loss-network.md)
3. [Stochastic network](stochastic-network.md)
4. [Queueing theory](queueing-theory-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34/2/ii/solution.md)
